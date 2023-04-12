# Comparing `tmp/monai-1.2.0rc3-202303310920-py3-none-any.whl.zip` & `tmp/monai-1.2.0rc4-202304121831-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,372 +1,366 @@
-Zip file size: 1246217 bytes, number of entries: 370
--rw-r--r--  2.0 unx     2276 b- defN 23-Mar-31 09:20 monai/__init__.py
--rw-r--r--  2.0 unx      500 b- defN 23-Mar-31 09:23 monai/_version.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 09:20 monai/py.typed
--rw-r--r--  2.0 unx      642 b- defN 23-Mar-31 09:20 monai/_extensions/__init__.py
--rw-r--r--  2.0 unx     3643 b- defN 23-Mar-31 09:20 monai/_extensions/loader.py
--rw-r--r--  2.0 unx     2931 b- defN 23-Mar-31 09:20 monai/_extensions/gmm/gmm.cpp
--rw-r--r--  2.0 unx     1760 b- defN 23-Mar-31 09:20 monai/_extensions/gmm/gmm.h
--rw-r--r--  2.0 unx     1118 b- defN 23-Mar-31 09:20 monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--  2.0 unx    16213 b- defN 23-Mar-31 09:20 monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--  2.0 unx     3520 b- defN 23-Mar-31 09:20 monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--  2.0 unx      908 b- defN 23-Mar-31 09:20 monai/apps/__init__.py
--rw-r--r--  2.0 unx    34560 b- defN 23-Mar-31 09:20 monai/apps/datasets.py
--rw-r--r--  2.0 unx    13505 b- defN 23-Mar-31 09:20 monai/apps/utils.py
--rw-r--r--  2.0 unx      952 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/__init__.py
--rw-r--r--  2.0 unx     1349 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/__main__.py
--rw-r--r--  2.0 unx    35021 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/auto_runner.py
--rw-r--r--  2.0 unx    22395 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--  2.0 unx    13587 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--  2.0 unx    11371 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--  2.0 unx    17378 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--  2.0 unx     3733 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/transforms.py
--rw-r--r--  2.0 unx     2481 b- defN 23-Mar-31 09:20 monai/apps/auto3dseg/utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/deepedit/__init__.py
--rw-r--r--  2.0 unx     4501 b- defN 23-Mar-31 09:20 monai/apps/deepedit/interaction.py
--rw-r--r--  2.0 unx    37435 b- defN 23-Mar-31 09:20 monai/apps/deepedit/transforms.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/deepgrow/__init__.py
--rw-r--r--  2.0 unx    10054 b- defN 23-Mar-31 09:20 monai/apps/deepgrow/dataset.py
--rw-r--r--  2.0 unx     3739 b- defN 23-Mar-31 09:20 monai/apps/deepgrow/interaction.py
--rw-r--r--  2.0 unx    42011 b- defN 23-Mar-31 09:20 monai/apps/deepgrow/transforms.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/detection/__init__.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/detection/metrics/__init__.py
--rw-r--r--  2.0 unx    26617 b- defN 23-Mar-31 09:20 monai/apps/detection/metrics/coco.py
--rw-r--r--  2.0 unx    17161 b- defN 23-Mar-31 09:20 monai/apps/detection/metrics/matching.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/detection/networks/__init__.py
--rw-r--r--  2.0 unx    51663 b- defN 23-Mar-31 09:20 monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--  2.0 unx    17604 b- defN 23-Mar-31 09:20 monai/apps/detection/networks/retinanet_network.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/detection/transforms/__init__.py
--rw-r--r--  2.0 unx    24519 b- defN 23-Mar-31 09:20 monai/apps/detection/transforms/array.py
--rw-r--r--  2.0 unx    17970 b- defN 23-Mar-31 09:20 monai/apps/detection/transforms/box_ops.py
--rw-r--r--  2.0 unx    68979 b- defN 23-Mar-31 09:20 monai/apps/detection/transforms/dictionary.py
--rw-r--r--  2.0 unx    13531 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/__init__.py
--rw-r--r--  2.0 unx    18681 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/anchor_utils.py
--rw-r--r--  2.0 unx    11120 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/box_coder.py
--rw-r--r--  2.0 unx     9031 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/box_selector.py
--rw-r--r--  2.0 unx    10306 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/detector_utils.py
--rw-r--r--  2.0 unx    13890 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--  2.0 unx     5627 b- defN 23-Mar-31 09:20 monai/apps/detection/utils/predict_utils.py
--rw-r--r--  2.0 unx      726 b- defN 23-Mar-31 09:20 monai/apps/mmars/__init__.py
--rw-r--r--  2.0 unx    13115 b- defN 23-Mar-31 09:20 monai/apps/mmars/mmars.py
--rw-r--r--  2.0 unx     9996 b- defN 23-Mar-31 09:20 monai/apps/mmars/model_desc.py
--rw-r--r--  2.0 unx      745 b- defN 23-Mar-31 09:20 monai/apps/nnunet/__init__.py
--rw-r--r--  2.0 unx     2975 b- defN 23-Mar-31 09:20 monai/apps/nnunet/__main__.py
--rw-r--r--  2.0 unx    38587 b- defN 23-Mar-31 09:20 monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--  2.0 unx     6791 b- defN 23-Mar-31 09:20 monai/apps/nnunet/utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/nuclick/__init__.py
--rw-r--r--  2.0 unx    24948 b- defN 23-Mar-31 09:20 monai/apps/nuclick/transforms.py
--rw-r--r--  2.0 unx     1156 b- defN 23-Mar-31 09:20 monai/apps/pathology/__init__.py
--rw-r--r--  2.0 unx     2860 b- defN 23-Mar-31 09:20 monai/apps/pathology/utils.py
--rw-r--r--  2.0 unx      702 b- defN 23-Mar-31 09:20 monai/apps/pathology/data/__init__.py
--rw-r--r--  2.0 unx    15184 b- defN 23-Mar-31 09:20 monai/apps/pathology/data/datasets.py
--rw-r--r--  2.0 unx      650 b- defN 23-Mar-31 09:20 monai/apps/pathology/engines/__init__.py
--rw-r--r--  2.0 unx     2397 b- defN 23-Mar-31 09:20 monai/apps/pathology/engines/utils.py
--rw-r--r--  2.0 unx      657 b- defN 23-Mar-31 09:20 monai/apps/pathology/handlers/__init__.py
--rw-r--r--  2.0 unx     4851 b- defN 23-Mar-31 09:20 monai/apps/pathology/handlers/prob_map_producer.py
--rw-r--r--  2.0 unx     2315 b- defN 23-Mar-31 09:20 monai/apps/pathology/handlers/utils.py
--rw-r--r--  2.0 unx      660 b- defN 23-Mar-31 09:20 monai/apps/pathology/inferers/__init__.py
--rw-r--r--  2.0 unx     9088 b- defN 23-Mar-31 09:20 monai/apps/pathology/inferers/inferer.py
--rw-r--r--  2.0 unx      650 b- defN 23-Mar-31 09:20 monai/apps/pathology/losses/__init__.py
--rw-r--r--  2.0 unx     7293 b- defN 23-Mar-31 09:20 monai/apps/pathology/losses/hovernet_loss.py
--rw-r--r--  2.0 unx      646 b- defN 23-Mar-31 09:20 monai/apps/pathology/metrics/__init__.py
--rw-r--r--  2.0 unx     7227 b- defN 23-Mar-31 09:20 monai/apps/pathology/metrics/lesion_froc.py
--rw-r--r--  2.0 unx     2412 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/__init__.py
--rw-r--r--  2.0 unx     1995 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--  2.0 unx    36850 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/post/array.py
--rw-r--r--  2.0 unx    25716 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/post/dictionary.py
--rw-r--r--  2.0 unx      763 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/spatial/__init__.py
--rw-r--r--  2.0 unx    10919 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/spatial/array.py
--rw-r--r--  2.0 unx     5442 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/spatial/dictionary.py
--rw-r--r--  2.0 unx      836 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--  2.0 unx     8366 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/stain/array.py
--rw-r--r--  2.0 unx     4761 b- defN 23-Mar-31 09:20 monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/__init__.py
--rw-r--r--  2.0 unx     8393 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/complex_utils.py
--rw-r--r--  2.0 unx     3644 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--  2.0 unx     2000 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/mri_utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/__init__.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--  2.0 unx     4183 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/blocks/varnetblock.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--  2.0 unx     6215 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--  2.0 unx     4775 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--  2.0 unx    11377 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--  2.0 unx     3831 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/networks/nets/varnet.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/transforms/array.py
--rw-r--r--  2.0 unx    15844 b- defN 23-Mar-31 09:20 monai/apps/reconstruction/transforms/dictionary.py
--rw-r--r--  2.0 unx      765 b- defN 23-Mar-31 09:20 monai/apps/tcia/__init__.py
--rw-r--r--  2.0 unx     1582 b- defN 23-Mar-31 09:20 monai/apps/tcia/label_desc.py
--rw-r--r--  2.0 unx     6152 b- defN 23-Mar-31 09:20 monai/apps/tcia/utils.py
--rw-r--r--  2.0 unx     1164 b- defN 23-Mar-31 09:20 monai/auto3dseg/__init__.py
--rw-r--r--  2.0 unx     4209 b- defN 23-Mar-31 09:20 monai/auto3dseg/algo_gen.py
--rw-r--r--  2.0 unx    41223 b- defN 23-Mar-31 09:20 monai/auto3dseg/analyzer.py
--rw-r--r--  2.0 unx     5110 b- defN 23-Mar-31 09:20 monai/auto3dseg/operations.py
--rw-r--r--  2.0 unx     8725 b- defN 23-Mar-31 09:20 monai/auto3dseg/seg_summarizer.py
--rw-r--r--  2.0 unx    12193 b- defN 23-Mar-31 09:20 monai/auto3dseg/utils.py
--rw-r--r--  2.0 unx     1306 b- defN 23-Mar-31 09:20 monai/bundle/__init__.py
--rw-r--r--  2.0 unx      858 b- defN 23-Mar-31 09:20 monai/bundle/__main__.py
--rw-r--r--  2.0 unx    16035 b- defN 23-Mar-31 09:20 monai/bundle/config_item.py
--rw-r--r--  2.0 unx    22410 b- defN 23-Mar-31 09:20 monai/bundle/config_parser.py
--rw-r--r--  2.0 unx     8628 b- defN 23-Mar-31 09:20 monai/bundle/properties.py
--rw-r--r--  2.0 unx    14353 b- defN 23-Mar-31 09:20 monai/bundle/reference_resolver.py
--rw-r--r--  2.0 unx    53473 b- defN 23-Mar-31 09:20 monai/bundle/scripts.py
--rw-r--r--  2.0 unx     8911 b- defN 23-Mar-31 09:20 monai/bundle/utils.py
--rw-r--r--  2.0 unx    16484 b- defN 23-Mar-31 09:20 monai/bundle/workflows.py
--rw-r--r--  2.0 unx     1048 b- defN 23-Mar-31 09:20 monai/config/__init__.py
--rw-r--r--  2.0 unx     9913 b- defN 23-Mar-31 09:20 monai/config/deviceconfig.py
--rw-r--r--  2.0 unx     3485 b- defN 23-Mar-31 09:20 monai/config/type_definitions.py
--rw-r--r--  2.0 unx     5087 b- defN 23-Mar-31 09:20 monai/data/__init__.py
--rw-r--r--  2.0 unx    50102 b- defN 23-Mar-31 09:20 monai/data/box_utils.py
--rw-r--r--  2.0 unx     4952 b- defN 23-Mar-31 09:20 monai/data/csv_saver.py
--rw-r--r--  2.0 unx     3835 b- defN 23-Mar-31 09:20 monai/data/dataloader.py
--rw-r--r--  2.0 unx    68927 b- defN 23-Mar-31 09:20 monai/data/dataset.py
--rw-r--r--  2.0 unx    10216 b- defN 23-Mar-31 09:20 monai/data/dataset_summary.py
--rw-r--r--  2.0 unx    10318 b- defN 23-Mar-31 09:20 monai/data/decathlon_datalist.py
--rw-r--r--  2.0 unx     4448 b- defN 23-Mar-31 09:20 monai/data/fft_utils.py
--rw-r--r--  2.0 unx     6344 b- defN 23-Mar-31 09:20 monai/data/folder_layout.py
--rw-r--r--  2.0 unx    12484 b- defN 23-Mar-31 09:20 monai/data/grid_dataset.py
--rw-r--r--  2.0 unx     7008 b- defN 23-Mar-31 09:20 monai/data/image_dataset.py
--rw-r--r--  2.0 unx    71785 b- defN 23-Mar-31 09:20 monai/data/image_reader.py
--rw-r--r--  2.0 unx    39872 b- defN 23-Mar-31 09:20 monai/data/image_writer.py
--rw-r--r--  2.0 unx    13309 b- defN 23-Mar-31 09:20 monai/data/iterable_dataset.py
--rw-r--r--  2.0 unx    14097 b- defN 23-Mar-31 09:20 monai/data/itk_torch_bridge.py
--rw-r--r--  2.0 unx     8800 b- defN 23-Mar-31 09:20 monai/data/meta_obj.py
--rw-r--r--  2.0 unx    27125 b- defN 23-Mar-31 09:20 monai/data/meta_tensor.py
--rw-r--r--  2.0 unx     5268 b- defN 23-Mar-31 09:20 monai/data/samplers.py
--rw-r--r--  2.0 unx     7375 b- defN 23-Mar-31 09:20 monai/data/synthetic.py
--rw-r--r--  2.0 unx     9780 b- defN 23-Mar-31 09:20 monai/data/test_time_augmentation.py
--rw-r--r--  2.0 unx     8840 b- defN 23-Mar-31 09:20 monai/data/thread_buffer.py
--rw-r--r--  2.0 unx     5500 b- defN 23-Mar-31 09:20 monai/data/torchscript_utils.py
--rw-r--r--  2.0 unx    64334 b- defN 23-Mar-31 09:20 monai/data/utils.py
--rw-r--r--  2.0 unx     9059 b- defN 23-Mar-31 09:20 monai/data/video_dataset.py
--rw-r--r--  2.0 unx    18631 b- defN 23-Mar-31 09:20 monai/data/wsi_datasets.py
--rw-r--r--  2.0 unx    38749 b- defN 23-Mar-31 09:20 monai/data/wsi_reader.py
--rw-r--r--  2.0 unx     1133 b- defN 23-Mar-31 09:20 monai/engines/__init__.py
--rw-r--r--  2.0 unx    24568 b- defN 23-Mar-31 09:20 monai/engines/evaluator.py
--rw-r--r--  2.0 unx     7278 b- defN 23-Mar-31 09:20 monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--  2.0 unx    21347 b- defN 23-Mar-31 09:20 monai/engines/trainer.py
--rw-r--r--  2.0 unx    11631 b- defN 23-Mar-31 09:20 monai/engines/utils.py
--rw-r--r--  2.0 unx    15250 b- defN 23-Mar-31 09:20 monai/engines/workflow.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/fl/__init__.py
--rw-r--r--  2.0 unx      725 b- defN 23-Mar-31 09:20 monai/fl/client/__init__.py
--rw-r--r--  2.0 unx     5097 b- defN 23-Mar-31 09:20 monai/fl/client/client_algo.py
--rw-r--r--  2.0 unx    32635 b- defN 23-Mar-31 09:20 monai/fl/client/monai_algo.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/fl/utils/__init__.py
--rw-r--r--  2.0 unx     2091 b- defN 23-Mar-31 09:20 monai/fl/utils/constants.py
--rw-r--r--  2.0 unx     3527 b- defN 23-Mar-31 09:20 monai/fl/utils/exchange_object.py
--rw-r--r--  2.0 unx     1628 b- defN 23-Mar-31 09:20 monai/fl/utils/filters.py
--rw-r--r--  2.0 unx     2351 b- defN 23-Mar-31 09:20 monai/handlers/__init__.py
--rw-r--r--  2.0 unx     6798 b- defN 23-Mar-31 09:20 monai/handlers/checkpoint_loader.py
--rw-r--r--  2.0 unx    16071 b- defN 23-Mar-31 09:20 monai/handlers/checkpoint_saver.py
--rw-r--r--  2.0 unx     7606 b- defN 23-Mar-31 09:20 monai/handlers/classification_saver.py
--rw-r--r--  2.0 unx     7506 b- defN 23-Mar-31 09:20 monai/handlers/clearml_handlers.py
--rw-r--r--  2.0 unx     3989 b- defN 23-Mar-31 09:20 monai/handlers/confusion_matrix.py
--rw-r--r--  2.0 unx     4425 b- defN 23-Mar-31 09:20 monai/handlers/decollate_batch.py
--rw-r--r--  2.0 unx     4381 b- defN 23-Mar-31 09:20 monai/handlers/earlystop_handler.py
--rw-r--r--  2.0 unx     3338 b- defN 23-Mar-31 09:20 monai/handlers/garbage_collector.py
--rw-r--r--  2.0 unx     3580 b- defN 23-Mar-31 09:20 monai/handlers/hausdorff_distance.py
--rw-r--r--  2.0 unx     5578 b- defN 23-Mar-31 09:20 monai/handlers/ignite_metric.py
--rw-r--r--  2.0 unx     3931 b- defN 23-Mar-31 09:20 monai/handlers/logfile_handler.py
--rw-r--r--  2.0 unx     3575 b- defN 23-Mar-31 09:20 monai/handlers/lr_schedule_handler.py
--rw-r--r--  2.0 unx     2832 b- defN 23-Mar-31 09:20 monai/handlers/mean_dice.py
--rw-r--r--  2.0 unx     2831 b- defN 23-Mar-31 09:20 monai/handlers/mean_iou.py
--rw-r--r--  2.0 unx     5477 b- defN 23-Mar-31 09:20 monai/handlers/metric_logger.py
--rw-r--r--  2.0 unx     6168 b- defN 23-Mar-31 09:20 monai/handlers/metrics_reloaded_handler.py
--rw-r--r--  2.0 unx     8560 b- defN 23-Mar-31 09:20 monai/handlers/metrics_saver.py
--rw-r--r--  2.0 unx    16326 b- defN 23-Mar-31 09:20 monai/handlers/mlflow_handler.py
--rw-r--r--  2.0 unx     6819 b- defN 23-Mar-31 09:20 monai/handlers/nvtx_handlers.py
--rw-r--r--  2.0 unx     3637 b- defN 23-Mar-31 09:20 monai/handlers/panoptic_quality.py
--rw-r--r--  2.0 unx     7119 b- defN 23-Mar-31 09:20 monai/handlers/parameter_scheduler.py
--rw-r--r--  2.0 unx     3285 b- defN 23-Mar-31 09:20 monai/handlers/postprocessing.py
--rw-r--r--  2.0 unx     5336 b- defN 23-Mar-31 09:20 monai/handlers/probability_maps.py
--rw-r--r--  2.0 unx     8422 b- defN 23-Mar-31 09:20 monai/handlers/regression_metrics.py
--rw-r--r--  2.0 unx     2730 b- defN 23-Mar-31 09:20 monai/handlers/roc_auc.py
--rw-r--r--  2.0 unx     3051 b- defN 23-Mar-31 09:20 monai/handlers/smartcache_handler.py
--rw-r--r--  2.0 unx    14251 b- defN 23-Mar-31 09:20 monai/handlers/stats_handler.py
--rw-r--r--  2.0 unx     3313 b- defN 23-Mar-31 09:20 monai/handlers/surface_distance.py
--rw-r--r--  2.0 unx    23325 b- defN 23-Mar-31 09:20 monai/handlers/tensorboard_handlers.py
--rw-r--r--  2.0 unx     9855 b- defN 23-Mar-31 09:20 monai/handlers/utils.py
--rw-r--r--  2.0 unx     3269 b- defN 23-Mar-31 09:20 monai/handlers/validation_handler.py
--rw-r--r--  2.0 unx      857 b- defN 23-Mar-31 09:20 monai/inferers/__init__.py
--rw-r--r--  2.0 unx    26855 b- defN 23-Mar-31 09:20 monai/inferers/inferer.py
--rw-r--r--  2.0 unx     6393 b- defN 23-Mar-31 09:20 monai/inferers/merger.py
--rw-r--r--  2.0 unx     9397 b- defN 23-Mar-31 09:20 monai/inferers/splitter.py
--rw-r--r--  2.0 unx    16770 b- defN 23-Mar-31 09:20 monai/inferers/utils.py
--rw-r--r--  2.0 unx     1409 b- defN 23-Mar-31 09:20 monai/losses/__init__.py
--rw-r--r--  2.0 unx     3430 b- defN 23-Mar-31 09:20 monai/losses/contrastive.py
--rw-r--r--  2.0 unx     4979 b- defN 23-Mar-31 09:20 monai/losses/deform.py
--rw-r--r--  2.0 unx    46326 b- defN 23-Mar-31 09:20 monai/losses/dice.py
--rw-r--r--  2.0 unx     3733 b- defN 23-Mar-31 09:20 monai/losses/ds_loss.py
--rw-r--r--  2.0 unx     9490 b- defN 23-Mar-31 09:20 monai/losses/focal_loss.py
--rw-r--r--  2.0 unx     2795 b- defN 23-Mar-31 09:20 monai/losses/giou_loss.py
--rw-r--r--  2.0 unx    15492 b- defN 23-Mar-31 09:20 monai/losses/image_dissimilarity.py
--rw-r--r--  2.0 unx     3636 b- defN 23-Mar-31 09:20 monai/losses/multi_scale.py
--rw-r--r--  2.0 unx     2942 b- defN 23-Mar-31 09:20 monai/losses/spatial_mask.py
--rw-r--r--  2.0 unx     4292 b- defN 23-Mar-31 09:20 monai/losses/ssim_loss.py
--rw-r--r--  2.0 unx     6645 b- defN 23-Mar-31 09:20 monai/losses/tversky.py
--rw-r--r--  2.0 unx    10224 b- defN 23-Mar-31 09:20 monai/losses/unified_focal_loss.py
--rw-r--r--  2.0 unx     1977 b- defN 23-Mar-31 09:20 monai/metrics/__init__.py
--rw-r--r--  2.0 unx     8211 b- defN 23-Mar-31 09:20 monai/metrics/active_learning_metrics.py
--rw-r--r--  2.0 unx    15101 b- defN 23-Mar-31 09:20 monai/metrics/confusion_matrix.py
--rw-r--r--  2.0 unx     5578 b- defN 23-Mar-31 09:20 monai/metrics/cumulative_average.py
--rw-r--r--  2.0 unx     4026 b- defN 23-Mar-31 09:20 monai/metrics/f_beta_score.py
--rw-r--r--  2.0 unx     6157 b- defN 23-Mar-31 09:20 monai/metrics/froc.py
--rw-r--r--  2.0 unx     8262 b- defN 23-Mar-31 09:20 monai/metrics/generalized_dice.py
--rw-r--r--  2.0 unx     9120 b- defN 23-Mar-31 09:20 monai/metrics/hausdorff_distance.py
--rw-r--r--  2.0 unx     4868 b- defN 23-Mar-31 09:20 monai/metrics/loss_metric.py
--rw-r--r--  2.0 unx    10937 b- defN 23-Mar-31 09:20 monai/metrics/meandice.py
--rw-r--r--  2.0 unx     7209 b- defN 23-Mar-31 09:20 monai/metrics/meaniou.py
--rw-r--r--  2.0 unx    14720 b- defN 23-Mar-31 09:20 monai/metrics/metric.py
--rw-r--r--  2.0 unx    13679 b- defN 23-Mar-31 09:20 monai/metrics/panoptic_quality.py
--rw-r--r--  2.0 unx    18235 b- defN 23-Mar-31 09:20 monai/metrics/regression.py
--rw-r--r--  2.0 unx     8038 b- defN 23-Mar-31 09:20 monai/metrics/rocauc.py
--rw-r--r--  2.0 unx    12166 b- defN 23-Mar-31 09:20 monai/metrics/surface_dice.py
--rw-r--r--  2.0 unx     7928 b- defN 23-Mar-31 09:20 monai/metrics/surface_distance.py
--rw-r--r--  2.0 unx    11172 b- defN 23-Mar-31 09:20 monai/metrics/utils.py
--rw-r--r--  2.0 unx    11772 b- defN 23-Mar-31 09:20 monai/metrics/wrapper.py
--rw-r--r--  2.0 unx      999 b- defN 23-Mar-31 09:20 monai/networks/__init__.py
--rw-r--r--  2.0 unx    34353 b- defN 23-Mar-31 09:20 monai/networks/utils.py
--rw-r--r--  2.0 unx     2134 b- defN 23-Mar-31 09:20 monai/networks/blocks/__init__.py
--rw-r--r--  2.0 unx     4275 b- defN 23-Mar-31 09:20 monai/networks/blocks/acti_norm.py
--rw-r--r--  2.0 unx     5839 b- defN 23-Mar-31 09:20 monai/networks/blocks/activation.py
--rw-r--r--  2.0 unx     4380 b- defN 23-Mar-31 09:20 monai/networks/blocks/aspp.py
--rw-r--r--  2.0 unx     7490 b- defN 23-Mar-31 09:20 monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--  2.0 unx    11686 b- defN 23-Mar-31 09:20 monai/networks/blocks/convolutions.py
--rw-r--r--  2.0 unx     5009 b- defN 23-Mar-31 09:20 monai/networks/blocks/crf.py
--rw-r--r--  2.0 unx     4740 b- defN 23-Mar-31 09:20 monai/networks/blocks/denseblock.py
--rw-r--r--  2.0 unx     9255 b- defN 23-Mar-31 09:20 monai/networks/blocks/dints_block.py
--rw-r--r--  2.0 unx     2413 b- defN 23-Mar-31 09:20 monai/networks/blocks/downsample.py
--rw-r--r--  2.0 unx    11062 b- defN 23-Mar-31 09:20 monai/networks/blocks/dynunet_block.py
--rw-r--r--  2.0 unx     3669 b- defN 23-Mar-31 09:20 monai/networks/blocks/encoder.py
--rw-r--r--  2.0 unx     9024 b- defN 23-Mar-31 09:20 monai/networks/blocks/fcn.py
--rw-r--r--  2.0 unx    10586 b- defN 23-Mar-31 09:20 monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--  2.0 unx     8263 b- defN 23-Mar-31 09:20 monai/networks/blocks/fft_utils_t.py
--rw-r--r--  2.0 unx    11454 b- defN 23-Mar-31 09:20 monai/networks/blocks/localnet_block.py
--rw-r--r--  2.0 unx     2813 b- defN 23-Mar-31 09:20 monai/networks/blocks/mlp.py
--rw-r--r--  2.0 unx     7987 b- defN 23-Mar-31 09:20 monai/networks/blocks/patchembedding.py
--rw-r--r--  2.0 unx     8825 b- defN 23-Mar-31 09:20 monai/networks/blocks/regunet_block.py
--rw-r--r--  2.0 unx     3245 b- defN 23-Mar-31 09:20 monai/networks/blocks/segresnet_block.py
--rw-r--r--  2.0 unx     2567 b- defN 23-Mar-31 09:20 monai/networks/blocks/selfattention.py
--rw-r--r--  2.0 unx    12752 b- defN 23-Mar-31 09:20 monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--  2.0 unx     2047 b- defN 23-Mar-31 09:20 monai/networks/blocks/transformerblock.py
--rw-r--r--  2.0 unx     9049 b- defN 23-Mar-31 09:20 monai/networks/blocks/unetr_block.py
--rw-r--r--  2.0 unx    13312 b- defN 23-Mar-31 09:20 monai/networks/blocks/upsample.py
--rw-r--r--  2.0 unx     6656 b- defN 23-Mar-31 09:20 monai/networks/blocks/warp.py
--rw-r--r--  2.0 unx     1562 b- defN 23-Mar-31 09:20 monai/networks/layers/__init__.py
--rw-r--r--  2.0 unx     8288 b- defN 23-Mar-31 09:20 monai/networks/layers/convutils.py
--rw-r--r--  2.0 unx     1802 b- defN 23-Mar-31 09:20 monai/networks/layers/drop_path.py
--rw-r--r--  2.0 unx    13058 b- defN 23-Mar-31 09:20 monai/networks/layers/factories.py
--rw-r--r--  2.0 unx    17992 b- defN 23-Mar-31 09:20 monai/networks/layers/filtering.py
--rw-r--r--  2.0 unx     3324 b- defN 23-Mar-31 09:20 monai/networks/layers/gmm.py
--rw-r--r--  2.0 unx    28470 b- defN 23-Mar-31 09:20 monai/networks/layers/simplelayers.py
--rw-r--r--  2.0 unx    25576 b- defN 23-Mar-31 09:20 monai/networks/layers/spatial_transforms.py
--rw-r--r--  2.0 unx     4296 b- defN 23-Mar-31 09:20 monai/networks/layers/utils.py
--rw-r--r--  2.0 unx     2253 b- defN 23-Mar-31 09:20 monai/networks/layers/weight_init.py
--rw-r--r--  2.0 unx     3141 b- defN 23-Mar-31 09:20 monai/networks/nets/__init__.py
--rw-r--r--  2.0 unx    21533 b- defN 23-Mar-31 09:20 monai/networks/nets/ahnet.py
--rw-r--r--  2.0 unx     9202 b- defN 23-Mar-31 09:20 monai/networks/nets/attentionunet.py
--rw-r--r--  2.0 unx    12089 b- defN 23-Mar-31 09:20 monai/networks/nets/autoencoder.py
--rw-r--r--  2.0 unx    10950 b- defN 23-Mar-31 09:20 monai/networks/nets/basic_unet.py
--rw-r--r--  2.0 unx     7960 b- defN 23-Mar-31 09:20 monai/networks/nets/basic_unetplusplus.py
--rw-r--r--  2.0 unx     6293 b- defN 23-Mar-31 09:20 monai/networks/nets/classifier.py
--rw-r--r--  2.0 unx    15820 b- defN 23-Mar-31 09:20 monai/networks/nets/densenet.py
--rw-r--r--  2.0 unx    44771 b- defN 23-Mar-31 09:20 monai/networks/nets/dints.py
--rw-r--r--  2.0 unx    18210 b- defN 23-Mar-31 09:20 monai/networks/nets/dynunet.py
--rw-r--r--  2.0 unx    40643 b- defN 23-Mar-31 09:20 monai/networks/nets/efficientnet.py
--rw-r--r--  2.0 unx    14147 b- defN 23-Mar-31 09:20 monai/networks/nets/flexible_unet.py
--rw-r--r--  2.0 unx     7212 b- defN 23-Mar-31 09:20 monai/networks/nets/fullyconnectednet.py
--rw-r--r--  2.0 unx     6581 b- defN 23-Mar-31 09:20 monai/networks/nets/generator.py
--rw-r--r--  2.0 unx     8882 b- defN 23-Mar-31 09:20 monai/networks/nets/highresnet.py
--rw-r--r--  2.0 unx    27864 b- defN 23-Mar-31 09:20 monai/networks/nets/hovernet.py
--rw-r--r--  2.0 unx     9812 b- defN 23-Mar-31 09:20 monai/networks/nets/milmodel.py
--rw-r--r--  2.0 unx     6102 b- defN 23-Mar-31 09:20 monai/networks/nets/netadapter.py
--rw-r--r--  2.0 unx     6488 b- defN 23-Mar-31 09:20 monai/networks/nets/regressor.py
--rw-r--r--  2.0 unx    17189 b- defN 23-Mar-31 09:20 monai/networks/nets/regunet.py
--rw-r--r--  2.0 unx    16785 b- defN 23-Mar-31 09:20 monai/networks/nets/resnet.py
--rw-r--r--  2.0 unx    13994 b- defN 23-Mar-31 09:20 monai/networks/nets/segresnet.py
--rw-r--r--  2.0 unx    15667 b- defN 23-Mar-31 09:20 monai/networks/nets/segresnet_ds.py
--rw-r--r--  2.0 unx    19289 b- defN 23-Mar-31 09:20 monai/networks/nets/senet.py
--rw-r--r--  2.0 unx    42000 b- defN 23-Mar-31 09:20 monai/networks/nets/swin_unetr.py
--rw-r--r--  2.0 unx     6248 b- defN 23-Mar-31 09:20 monai/networks/nets/torchvision_fc.py
--rw-r--r--  2.0 unx    16626 b- defN 23-Mar-31 09:20 monai/networks/nets/transchex.py
--rw-r--r--  2.0 unx    13722 b- defN 23-Mar-31 09:20 monai/networks/nets/unet.py
--rw-r--r--  2.0 unx     7943 b- defN 23-Mar-31 09:20 monai/networks/nets/unetr.py
--rw-r--r--  2.0 unx     6285 b- defN 23-Mar-31 09:20 monai/networks/nets/varautoencoder.py
--rw-r--r--  2.0 unx     5017 b- defN 23-Mar-31 09:20 monai/networks/nets/vit.py
--rw-r--r--  2.0 unx     4817 b- defN 23-Mar-31 09:20 monai/networks/nets/vitautoenc.py
--rw-r--r--  2.0 unx    10011 b- defN 23-Mar-31 09:20 monai/networks/nets/vnet.py
--rw-r--r--  2.0 unx      796 b- defN 23-Mar-31 09:20 monai/optimizers/__init__.py
--rw-r--r--  2.0 unx    21948 b- defN 23-Mar-31 09:20 monai/optimizers/lr_finder.py
--rw-r--r--  2.0 unx     3652 b- defN 23-Mar-31 09:20 monai/optimizers/lr_scheduler.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Mar-31 09:20 monai/optimizers/novograd.py
--rw-r--r--  2.0 unx     4131 b- defN 23-Mar-31 09:20 monai/optimizers/utils.py
--rw-r--r--  2.0 unx    15216 b- defN 23-Mar-31 09:20 monai/transforms/__init__.py
--rw-r--r--  2.0 unx     8946 b- defN 23-Mar-31 09:20 monai/transforms/adaptors.py
--rw-r--r--  2.0 unx    40548 b- defN 23-Mar-31 09:20 monai/transforms/compose.py
--rw-r--r--  2.0 unx    17160 b- defN 23-Mar-31 09:20 monai/transforms/inverse.py
--rw-r--r--  2.0 unx     7054 b- defN 23-Mar-31 09:20 monai/transforms/inverse_batch_transform.py
--rw-r--r--  2.0 unx     3386 b- defN 23-Mar-31 09:20 monai/transforms/nvtx.py
--rw-r--r--  2.0 unx     2885 b- defN 23-Mar-31 09:20 monai/transforms/traits.py
--rw-r--r--  2.0 unx    18234 b- defN 23-Mar-31 09:20 monai/transforms/transform.py
--rw-r--r--  2.0 unx    70604 b- defN 23-Mar-31 09:20 monai/transforms/utils.py
--rw-r--r--  2.0 unx    31081 b- defN 23-Mar-31 09:20 monai/transforms/utils_create_transform_ims.py
--rw-r--r--  2.0 unx    18397 b- defN 23-Mar-31 09:20 monai/transforms/utils_pytorch_numpy_unification.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/croppad/__init__.py
--rw-r--r--  2.0 unx    68405 b- defN 23-Mar-31 09:20 monai/transforms/croppad/array.py
--rw-r--r--  2.0 unx     6194 b- defN 23-Mar-31 09:20 monai/transforms/croppad/batch.py
--rw-r--r--  2.0 unx    53819 b- defN 23-Mar-31 09:20 monai/transforms/croppad/dictionary.py
--rw-r--r--  2.0 unx    12673 b- defN 23-Mar-31 09:20 monai/transforms/croppad/functional.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/intensity/__init__.py
--rw-r--r--  2.0 unx    98613 b- defN 23-Mar-31 09:20 monai/transforms/intensity/array.py
--rw-r--r--  2.0 unx    76501 b- defN 23-Mar-31 09:20 monai/transforms/intensity/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/io/__init__.py
--rw-r--r--  2.0 unx    25430 b- defN 23-Mar-31 09:20 monai/transforms/io/array.py
--rw-r--r--  2.0 unx    17821 b- defN 23-Mar-31 09:20 monai/transforms/io/dictionary.py
--rw-r--r--  2.0 unx      699 b- defN 23-Mar-31 09:20 monai/transforms/lazy/__init__.py
--rw-r--r--  2.0 unx     5552 b- defN 23-Mar-31 09:20 monai/transforms/lazy/functional.py
--rw-r--r--  2.0 unx     9551 b- defN 23-Mar-31 09:20 monai/transforms/lazy/utils.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/meta_utility/__init__.py
--rw-r--r--  2.0 unx     4896 b- defN 23-Mar-31 09:20 monai/transforms/meta_utility/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/post/__init__.py
--rw-r--r--  2.0 unx    40858 b- defN 23-Mar-31 09:20 monai/transforms/post/array.py
--rw-r--r--  2.0 unx    39905 b- defN 23-Mar-31 09:20 monai/transforms/post/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/signal/__init__.py
--rw-r--r--  2.0 unx    16378 b- defN 23-Mar-31 09:20 monai/transforms/signal/array.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/smooth_field/__init__.py
--rw-r--r--  2.0 unx    17833 b- defN 23-Mar-31 09:20 monai/transforms/smooth_field/array.py
--rw-r--r--  2.0 unx    11194 b- defN 23-Mar-31 09:20 monai/transforms/smooth_field/dictionary.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/spatial/__init__.py
--rw-r--r--  2.0 unx   168592 b- defN 23-Mar-31 09:20 monai/transforms/spatial/array.py
--rw-r--r--  2.0 unx   107151 b- defN 23-Mar-31 09:20 monai/transforms/spatial/dictionary.py
--rw-r--r--  2.0 unx    31494 b- defN 23-Mar-31 09:20 monai/transforms/spatial/functional.py
--rw-r--r--  2.0 unx      573 b- defN 23-Mar-31 09:20 monai/transforms/utility/__init__.py
--rw-r--r--  2.0 unx    69977 b- defN 23-Mar-31 09:20 monai/transforms/utility/array.py
--rw-r--r--  2.0 unx    75587 b- defN 23-Mar-31 09:20 monai/transforms/utility/dictionary.py
--rw-r--r--  2.0 unx     3366 b- defN 23-Mar-31 09:20 monai/utils/__init__.py
--rw-r--r--  2.0 unx     4099 b- defN 23-Mar-31 09:20 monai/utils/aliases.py
--rw-r--r--  2.0 unx     3129 b- defN 23-Mar-31 09:20 monai/utils/decorators.py
--rw-r--r--  2.0 unx    14759 b- defN 23-Mar-31 09:20 monai/utils/deprecate_utils.py
--rw-r--r--  2.0 unx     8526 b- defN 23-Mar-31 09:20 monai/utils/dist.py
--rw-r--r--  2.0 unx    16215 b- defN 23-Mar-31 09:20 monai/utils/enums.py
--rw-r--r--  2.0 unx    15637 b- defN 23-Mar-31 09:20 monai/utils/jupyter_utils.py
--rw-r--r--  2.0 unx    24927 b- defN 23-Mar-31 09:20 monai/utils/misc.py
--rw-r--r--  2.0 unx    23560 b- defN 23-Mar-31 09:20 monai/utils/module.py
--rw-r--r--  2.0 unx     6876 b- defN 23-Mar-31 09:20 monai/utils/nvtx.py
--rw-r--r--  2.0 unx    15936 b- defN 23-Mar-31 09:20 monai/utils/profiling.py
--rw-r--r--  2.0 unx     5955 b- defN 23-Mar-31 09:20 monai/utils/state_cacher.py
--rw-r--r--  2.0 unx    21127 b- defN 23-Mar-31 09:20 monai/utils/type_conversion.py
--rw-r--r--  2.0 unx     1038 b- defN 23-Mar-31 09:20 monai/visualize/__init__.py
--rw-r--r--  2.0 unx    16156 b- defN 23-Mar-31 09:20 monai/visualize/class_activation_maps.py
--rw-r--r--  2.0 unx     6277 b- defN 23-Mar-31 09:20 monai/visualize/gradient_based.py
--rw-r--r--  2.0 unx     9200 b- defN 23-Mar-31 09:20 monai/visualize/img2tensorboard.py
--rw-r--r--  2.0 unx    18816 b- defN 23-Mar-31 09:20 monai/visualize/occlusion_sensitivity.py
--rw-r--r--  2.0 unx     9966 b- defN 23-Mar-31 09:20 monai/visualize/utils.py
--rw-r--r--  2.0 unx     1377 b- defN 23-Mar-31 09:20 monai/visualize/visualizer.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-31 09:23 monai-1.2.0rc3.dist-info/LICENSE
--rw-r--r--  2.0 unx     9782 b- defN 23-Mar-31 09:23 monai-1.2.0rc3.dist-info/METADATA
--rw-r--r--  2.0 unx      112 b- defN 23-Mar-31 09:23 monai-1.2.0rc3.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-31 09:23 monai-1.2.0rc3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    33217 b- defN 23-Mar-31 09:23 monai-1.2.0rc3.dist-info/RECORD
-370 files, 4694589 bytes uncompressed, 1193891 bytes compressed:  74.6%
+Zip file size: 1243555 bytes, number of entries: 364
+-rw-r--r--  2.0 unx     2276 b- defN 23-Apr-12 18:31 monai/__init__.py
+-rw-r--r--  2.0 unx      500 b- defN 23-Apr-12 18:33 monai/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 18:31 monai/py.typed
+-rw-r--r--  2.0 unx      642 b- defN 23-Apr-12 18:31 monai/_extensions/__init__.py
+-rw-r--r--  2.0 unx     3643 b- defN 23-Apr-12 18:31 monai/_extensions/loader.py
+-rw-r--r--  2.0 unx     2931 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm.cpp
+-rw-r--r--  2.0 unx     1760 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm.h
+-rw-r--r--  2.0 unx     1118 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--  2.0 unx    16213 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--  2.0 unx     3520 b- defN 23-Apr-12 18:31 monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--  2.0 unx      908 b- defN 23-Apr-12 18:31 monai/apps/__init__.py
+-rw-r--r--  2.0 unx    34560 b- defN 23-Apr-12 18:31 monai/apps/datasets.py
+-rw-r--r--  2.0 unx    13505 b- defN 23-Apr-12 18:31 monai/apps/utils.py
+-rw-r--r--  2.0 unx      952 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/__init__.py
+-rw-r--r--  2.0 unx     1349 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/__main__.py
+-rw-r--r--  2.0 unx    36092 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--  2.0 unx    23164 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--  2.0 unx    17319 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--  2.0 unx    11249 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--  2.0 unx    17523 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/transforms.py
+-rw-r--r--  2.0 unx     2765 b- defN 23-Apr-12 18:31 monai/apps/auto3dseg/utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/deepedit/__init__.py
+-rw-r--r--  2.0 unx     4501 b- defN 23-Apr-12 18:31 monai/apps/deepedit/interaction.py
+-rw-r--r--  2.0 unx    37435 b- defN 23-Apr-12 18:31 monai/apps/deepedit/transforms.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/__init__.py
+-rw-r--r--  2.0 unx    10054 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/dataset.py
+-rw-r--r--  2.0 unx     3739 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/interaction.py
+-rw-r--r--  2.0 unx    42011 b- defN 23-Apr-12 18:31 monai/apps/deepgrow/transforms.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/__init__.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/metrics/__init__.py
+-rw-r--r--  2.0 unx    26617 b- defN 23-Apr-12 18:31 monai/apps/detection/metrics/coco.py
+-rw-r--r--  2.0 unx    17161 b- defN 23-Apr-12 18:31 monai/apps/detection/metrics/matching.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/networks/__init__.py
+-rw-r--r--  2.0 unx    51663 b- defN 23-Apr-12 18:31 monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--  2.0 unx    17604 b- defN 23-Apr-12 18:31 monai/apps/detection/networks/retinanet_network.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/__init__.py
+-rw-r--r--  2.0 unx    24519 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/array.py
+-rw-r--r--  2.0 unx    17970 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/box_ops.py
+-rw-r--r--  2.0 unx    68979 b- defN 23-Apr-12 18:31 monai/apps/detection/transforms/dictionary.py
+-rw-r--r--  2.0 unx    13531 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/__init__.py
+-rw-r--r--  2.0 unx    18681 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--  2.0 unx    11120 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/box_coder.py
+-rw-r--r--  2.0 unx     9031 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/box_selector.py
+-rw-r--r--  2.0 unx    10306 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/detector_utils.py
+-rw-r--r--  2.0 unx    13890 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--  2.0 unx     5627 b- defN 23-Apr-12 18:31 monai/apps/detection/utils/predict_utils.py
+-rw-r--r--  2.0 unx      726 b- defN 23-Apr-12 18:31 monai/apps/mmars/__init__.py
+-rw-r--r--  2.0 unx    13115 b- defN 23-Apr-12 18:31 monai/apps/mmars/mmars.py
+-rw-r--r--  2.0 unx     9996 b- defN 23-Apr-12 18:31 monai/apps/mmars/model_desc.py
+-rw-r--r--  2.0 unx      745 b- defN 23-Apr-12 18:31 monai/apps/nnunet/__init__.py
+-rw-r--r--  2.0 unx     2975 b- defN 23-Apr-12 18:31 monai/apps/nnunet/__main__.py
+-rw-r--r--  2.0 unx    38587 b- defN 23-Apr-12 18:31 monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--  2.0 unx     6791 b- defN 23-Apr-12 18:31 monai/apps/nnunet/utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/nuclick/__init__.py
+-rw-r--r--  2.0 unx    24948 b- defN 23-Apr-12 18:31 monai/apps/nuclick/transforms.py
+-rw-r--r--  2.0 unx     1030 b- defN 23-Apr-12 18:31 monai/apps/pathology/__init__.py
+-rw-r--r--  2.0 unx     2860 b- defN 23-Apr-12 18:31 monai/apps/pathology/utils.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Apr-12 18:31 monai/apps/pathology/engines/__init__.py
+-rw-r--r--  2.0 unx     2397 b- defN 23-Apr-12 18:31 monai/apps/pathology/engines/utils.py
+-rw-r--r--  2.0 unx      609 b- defN 23-Apr-12 18:31 monai/apps/pathology/handlers/__init__.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-Apr-12 18:31 monai/apps/pathology/handlers/utils.py
+-rw-r--r--  2.0 unx      660 b- defN 23-Apr-12 18:31 monai/apps/pathology/inferers/__init__.py
+-rw-r--r--  2.0 unx     9148 b- defN 23-Apr-12 18:31 monai/apps/pathology/inferers/inferer.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Apr-12 18:31 monai/apps/pathology/losses/__init__.py
+-rw-r--r--  2.0 unx     7293 b- defN 23-Apr-12 18:31 monai/apps/pathology/losses/hovernet_loss.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Apr-12 18:31 monai/apps/pathology/metrics/__init__.py
+-rw-r--r--  2.0 unx     7225 b- defN 23-Apr-12 18:31 monai/apps/pathology/metrics/lesion_froc.py
+-rw-r--r--  2.0 unx     2243 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/__init__.py
+-rw-r--r--  2.0 unx     1995 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--  2.0 unx    37322 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/post/array.py
+-rw-r--r--  2.0 unx    25992 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/post/dictionary.py
+-rw-r--r--  2.0 unx      836 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--  2.0 unx     8366 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--  2.0 unx     4761 b- defN 23-Apr-12 18:31 monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/__init__.py
+-rw-r--r--  2.0 unx     8393 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/complex_utils.py
+-rw-r--r--  2.0 unx     3644 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--  2.0 unx     2000 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/mri_utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/__init__.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--  2.0 unx     4183 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/blocks/varnetblock.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--  2.0 unx     6215 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--  2.0 unx     4775 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--  2.0 unx    11377 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--  2.0 unx     3831 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/networks/nets/varnet.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/transforms/array.py
+-rw-r--r--  2.0 unx    15844 b- defN 23-Apr-12 18:31 monai/apps/reconstruction/transforms/dictionary.py
+-rw-r--r--  2.0 unx      765 b- defN 23-Apr-12 18:31 monai/apps/tcia/__init__.py
+-rw-r--r--  2.0 unx     1582 b- defN 23-Apr-12 18:31 monai/apps/tcia/label_desc.py
+-rw-r--r--  2.0 unx     6152 b- defN 23-Apr-12 18:31 monai/apps/tcia/utils.py
+-rw-r--r--  2.0 unx     1164 b- defN 23-Apr-12 18:31 monai/auto3dseg/__init__.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Apr-12 18:31 monai/auto3dseg/algo_gen.py
+-rw-r--r--  2.0 unx    41223 b- defN 23-Apr-12 18:31 monai/auto3dseg/analyzer.py
+-rw-r--r--  2.0 unx     5110 b- defN 23-Apr-12 18:31 monai/auto3dseg/operations.py
+-rw-r--r--  2.0 unx     8725 b- defN 23-Apr-12 18:31 monai/auto3dseg/seg_summarizer.py
+-rw-r--r--  2.0 unx    12193 b- defN 23-Apr-12 18:31 monai/auto3dseg/utils.py
+-rw-r--r--  2.0 unx     1341 b- defN 23-Apr-12 18:31 monai/bundle/__init__.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Apr-12 18:31 monai/bundle/__main__.py
+-rw-r--r--  2.0 unx    16035 b- defN 23-Apr-12 18:31 monai/bundle/config_item.py
+-rw-r--r--  2.0 unx    22410 b- defN 23-Apr-12 18:31 monai/bundle/config_parser.py
+-rw-r--r--  2.0 unx     8628 b- defN 23-Apr-12 18:31 monai/bundle/properties.py
+-rw-r--r--  2.0 unx    14353 b- defN 23-Apr-12 18:31 monai/bundle/reference_resolver.py
+-rw-r--r--  2.0 unx    63733 b- defN 23-Apr-12 18:31 monai/bundle/scripts.py
+-rw-r--r--  2.0 unx     8911 b- defN 23-Apr-12 18:31 monai/bundle/utils.py
+-rw-r--r--  2.0 unx    16520 b- defN 23-Apr-12 18:31 monai/bundle/workflows.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-Apr-12 18:31 monai/config/__init__.py
+-rw-r--r--  2.0 unx     9913 b- defN 23-Apr-12 18:31 monai/config/deviceconfig.py
+-rw-r--r--  2.0 unx     3485 b- defN 23-Apr-12 18:31 monai/config/type_definitions.py
+-rw-r--r--  2.0 unx     5087 b- defN 23-Apr-12 18:31 monai/data/__init__.py
+-rw-r--r--  2.0 unx    50102 b- defN 23-Apr-12 18:31 monai/data/box_utils.py
+-rw-r--r--  2.0 unx     4952 b- defN 23-Apr-12 18:31 monai/data/csv_saver.py
+-rw-r--r--  2.0 unx     3835 b- defN 23-Apr-12 18:31 monai/data/dataloader.py
+-rw-r--r--  2.0 unx    68927 b- defN 23-Apr-12 18:31 monai/data/dataset.py
+-rw-r--r--  2.0 unx    10216 b- defN 23-Apr-12 18:31 monai/data/dataset_summary.py
+-rw-r--r--  2.0 unx    10318 b- defN 23-Apr-12 18:31 monai/data/decathlon_datalist.py
+-rw-r--r--  2.0 unx     4448 b- defN 23-Apr-12 18:31 monai/data/fft_utils.py
+-rw-r--r--  2.0 unx     6344 b- defN 23-Apr-12 18:31 monai/data/folder_layout.py
+-rw-r--r--  2.0 unx    12484 b- defN 23-Apr-12 18:31 monai/data/grid_dataset.py
+-rw-r--r--  2.0 unx     7008 b- defN 23-Apr-12 18:31 monai/data/image_dataset.py
+-rw-r--r--  2.0 unx    60619 b- defN 23-Apr-12 18:31 monai/data/image_reader.py
+-rw-r--r--  2.0 unx    39872 b- defN 23-Apr-12 18:31 monai/data/image_writer.py
+-rw-r--r--  2.0 unx    13309 b- defN 23-Apr-12 18:31 monai/data/iterable_dataset.py
+-rw-r--r--  2.0 unx    14097 b- defN 23-Apr-12 18:31 monai/data/itk_torch_bridge.py
+-rw-r--r--  2.0 unx     8800 b- defN 23-Apr-12 18:31 monai/data/meta_obj.py
+-rw-r--r--  2.0 unx    27321 b- defN 23-Apr-12 18:31 monai/data/meta_tensor.py
+-rw-r--r--  2.0 unx     5268 b- defN 23-Apr-12 18:31 monai/data/samplers.py
+-rw-r--r--  2.0 unx     7375 b- defN 23-Apr-12 18:31 monai/data/synthetic.py
+-rw-r--r--  2.0 unx     9780 b- defN 23-Apr-12 18:31 monai/data/test_time_augmentation.py
+-rw-r--r--  2.0 unx     8840 b- defN 23-Apr-12 18:31 monai/data/thread_buffer.py
+-rw-r--r--  2.0 unx     5500 b- defN 23-Apr-12 18:31 monai/data/torchscript_utils.py
+-rw-r--r--  2.0 unx    64795 b- defN 23-Apr-12 18:31 monai/data/utils.py
+-rw-r--r--  2.0 unx     9059 b- defN 23-Apr-12 18:31 monai/data/video_dataset.py
+-rw-r--r--  2.0 unx    18631 b- defN 23-Apr-12 18:31 monai/data/wsi_datasets.py
+-rw-r--r--  2.0 unx    49442 b- defN 23-Apr-12 18:31 monai/data/wsi_reader.py
+-rw-r--r--  2.0 unx     1133 b- defN 23-Apr-12 18:31 monai/engines/__init__.py
+-rw-r--r--  2.0 unx    24568 b- defN 23-Apr-12 18:31 monai/engines/evaluator.py
+-rw-r--r--  2.0 unx     7278 b- defN 23-Apr-12 18:31 monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--  2.0 unx    21347 b- defN 23-Apr-12 18:31 monai/engines/trainer.py
+-rw-r--r--  2.0 unx    11631 b- defN 23-Apr-12 18:31 monai/engines/utils.py
+-rw-r--r--  2.0 unx    15250 b- defN 23-Apr-12 18:31 monai/engines/workflow.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/fl/__init__.py
+-rw-r--r--  2.0 unx      725 b- defN 23-Apr-12 18:31 monai/fl/client/__init__.py
+-rw-r--r--  2.0 unx     5097 b- defN 23-Apr-12 18:31 monai/fl/client/client_algo.py
+-rw-r--r--  2.0 unx    32635 b- defN 23-Apr-12 18:31 monai/fl/client/monai_algo.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/fl/utils/__init__.py
+-rw-r--r--  2.0 unx     2091 b- defN 23-Apr-12 18:31 monai/fl/utils/constants.py
+-rw-r--r--  2.0 unx     3527 b- defN 23-Apr-12 18:31 monai/fl/utils/exchange_object.py
+-rw-r--r--  2.0 unx     1628 b- defN 23-Apr-12 18:31 monai/fl/utils/filters.py
+-rw-r--r--  2.0 unx     2351 b- defN 23-Apr-12 18:31 monai/handlers/__init__.py
+-rw-r--r--  2.0 unx     6798 b- defN 23-Apr-12 18:31 monai/handlers/checkpoint_loader.py
+-rw-r--r--  2.0 unx    16071 b- defN 23-Apr-12 18:31 monai/handlers/checkpoint_saver.py
+-rw-r--r--  2.0 unx     7606 b- defN 23-Apr-12 18:31 monai/handlers/classification_saver.py
+-rw-r--r--  2.0 unx     7506 b- defN 23-Apr-12 18:31 monai/handlers/clearml_handlers.py
+-rw-r--r--  2.0 unx     3989 b- defN 23-Apr-12 18:31 monai/handlers/confusion_matrix.py
+-rw-r--r--  2.0 unx     4425 b- defN 23-Apr-12 18:31 monai/handlers/decollate_batch.py
+-rw-r--r--  2.0 unx     4381 b- defN 23-Apr-12 18:31 monai/handlers/earlystop_handler.py
+-rw-r--r--  2.0 unx     3338 b- defN 23-Apr-12 18:31 monai/handlers/garbage_collector.py
+-rw-r--r--  2.0 unx     3580 b- defN 23-Apr-12 18:31 monai/handlers/hausdorff_distance.py
+-rw-r--r--  2.0 unx     5578 b- defN 23-Apr-12 18:31 monai/handlers/ignite_metric.py
+-rw-r--r--  2.0 unx     3931 b- defN 23-Apr-12 18:31 monai/handlers/logfile_handler.py
+-rw-r--r--  2.0 unx     3575 b- defN 23-Apr-12 18:31 monai/handlers/lr_schedule_handler.py
+-rw-r--r--  2.0 unx     2832 b- defN 23-Apr-12 18:31 monai/handlers/mean_dice.py
+-rw-r--r--  2.0 unx     2831 b- defN 23-Apr-12 18:31 monai/handlers/mean_iou.py
+-rw-r--r--  2.0 unx     5477 b- defN 23-Apr-12 18:31 monai/handlers/metric_logger.py
+-rw-r--r--  2.0 unx     6168 b- defN 23-Apr-12 18:31 monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--  2.0 unx     8560 b- defN 23-Apr-12 18:31 monai/handlers/metrics_saver.py
+-rw-r--r--  2.0 unx    16326 b- defN 23-Apr-12 18:31 monai/handlers/mlflow_handler.py
+-rw-r--r--  2.0 unx     6819 b- defN 23-Apr-12 18:31 monai/handlers/nvtx_handlers.py
+-rw-r--r--  2.0 unx     3637 b- defN 23-Apr-12 18:31 monai/handlers/panoptic_quality.py
+-rw-r--r--  2.0 unx     7119 b- defN 23-Apr-12 18:31 monai/handlers/parameter_scheduler.py
+-rw-r--r--  2.0 unx     3285 b- defN 23-Apr-12 18:31 monai/handlers/postprocessing.py
+-rw-r--r--  2.0 unx     5336 b- defN 23-Apr-12 18:31 monai/handlers/probability_maps.py
+-rw-r--r--  2.0 unx     8422 b- defN 23-Apr-12 18:31 monai/handlers/regression_metrics.py
+-rw-r--r--  2.0 unx     2730 b- defN 23-Apr-12 18:31 monai/handlers/roc_auc.py
+-rw-r--r--  2.0 unx     3051 b- defN 23-Apr-12 18:31 monai/handlers/smartcache_handler.py
+-rw-r--r--  2.0 unx    14251 b- defN 23-Apr-12 18:31 monai/handlers/stats_handler.py
+-rw-r--r--  2.0 unx     3313 b- defN 23-Apr-12 18:31 monai/handlers/surface_distance.py
+-rw-r--r--  2.0 unx    23325 b- defN 23-Apr-12 18:31 monai/handlers/tensorboard_handlers.py
+-rw-r--r--  2.0 unx     9855 b- defN 23-Apr-12 18:31 monai/handlers/utils.py
+-rw-r--r--  2.0 unx     3269 b- defN 23-Apr-12 18:31 monai/handlers/validation_handler.py
+-rw-r--r--  2.0 unx      857 b- defN 23-Apr-12 18:31 monai/inferers/__init__.py
+-rw-r--r--  2.0 unx    27881 b- defN 23-Apr-12 18:31 monai/inferers/inferer.py
+-rw-r--r--  2.0 unx     6393 b- defN 23-Apr-12 18:31 monai/inferers/merger.py
+-rw-r--r--  2.0 unx     9397 b- defN 23-Apr-12 18:31 monai/inferers/splitter.py
+-rw-r--r--  2.0 unx    20036 b- defN 23-Apr-12 18:31 monai/inferers/utils.py
+-rw-r--r--  2.0 unx     1409 b- defN 23-Apr-12 18:31 monai/losses/__init__.py
+-rw-r--r--  2.0 unx     3430 b- defN 23-Apr-12 18:31 monai/losses/contrastive.py
+-rw-r--r--  2.0 unx     4979 b- defN 23-Apr-12 18:31 monai/losses/deform.py
+-rw-r--r--  2.0 unx    46326 b- defN 23-Apr-12 18:31 monai/losses/dice.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-Apr-12 18:31 monai/losses/ds_loss.py
+-rw-r--r--  2.0 unx     9490 b- defN 23-Apr-12 18:31 monai/losses/focal_loss.py
+-rw-r--r--  2.0 unx     2795 b- defN 23-Apr-12 18:31 monai/losses/giou_loss.py
+-rw-r--r--  2.0 unx    15492 b- defN 23-Apr-12 18:31 monai/losses/image_dissimilarity.py
+-rw-r--r--  2.0 unx     3636 b- defN 23-Apr-12 18:31 monai/losses/multi_scale.py
+-rw-r--r--  2.0 unx     2942 b- defN 23-Apr-12 18:31 monai/losses/spatial_mask.py
+-rw-r--r--  2.0 unx     4292 b- defN 23-Apr-12 18:31 monai/losses/ssim_loss.py
+-rw-r--r--  2.0 unx     6645 b- defN 23-Apr-12 18:31 monai/losses/tversky.py
+-rw-r--r--  2.0 unx    10224 b- defN 23-Apr-12 18:31 monai/losses/unified_focal_loss.py
+-rw-r--r--  2.0 unx     1977 b- defN 23-Apr-12 18:31 monai/metrics/__init__.py
+-rw-r--r--  2.0 unx     8211 b- defN 23-Apr-12 18:31 monai/metrics/active_learning_metrics.py
+-rw-r--r--  2.0 unx    15101 b- defN 23-Apr-12 18:31 monai/metrics/confusion_matrix.py
+-rw-r--r--  2.0 unx     5578 b- defN 23-Apr-12 18:31 monai/metrics/cumulative_average.py
+-rw-r--r--  2.0 unx     4026 b- defN 23-Apr-12 18:31 monai/metrics/f_beta_score.py
+-rw-r--r--  2.0 unx     6157 b- defN 23-Apr-12 18:31 monai/metrics/froc.py
+-rw-r--r--  2.0 unx     8262 b- defN 23-Apr-12 18:31 monai/metrics/generalized_dice.py
+-rw-r--r--  2.0 unx    11470 b- defN 23-Apr-12 18:31 monai/metrics/hausdorff_distance.py
+-rw-r--r--  2.0 unx     4907 b- defN 23-Apr-12 18:31 monai/metrics/loss_metric.py
+-rw-r--r--  2.0 unx    10937 b- defN 23-Apr-12 18:31 monai/metrics/meandice.py
+-rw-r--r--  2.0 unx     7209 b- defN 23-Apr-12 18:31 monai/metrics/meaniou.py
+-rw-r--r--  2.0 unx    15140 b- defN 23-Apr-12 18:31 monai/metrics/metric.py
+-rw-r--r--  2.0 unx    13679 b- defN 23-Apr-12 18:31 monai/metrics/panoptic_quality.py
+-rw-r--r--  2.0 unx    18235 b- defN 23-Apr-12 18:31 monai/metrics/regression.py
+-rw-r--r--  2.0 unx     8038 b- defN 23-Apr-12 18:31 monai/metrics/rocauc.py
+-rw-r--r--  2.0 unx    14415 b- defN 23-Apr-12 18:31 monai/metrics/surface_dice.py
+-rw-r--r--  2.0 unx    10186 b- defN 23-Apr-12 18:31 monai/metrics/surface_distance.py
+-rw-r--r--  2.0 unx    15100 b- defN 23-Apr-12 18:31 monai/metrics/utils.py
+-rw-r--r--  2.0 unx    11772 b- defN 23-Apr-12 18:31 monai/metrics/wrapper.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-Apr-12 18:31 monai/networks/__init__.py
+-rw-r--r--  2.0 unx    46286 b- defN 23-Apr-12 18:31 monai/networks/utils.py
+-rw-r--r--  2.0 unx     2134 b- defN 23-Apr-12 18:31 monai/networks/blocks/__init__.py
+-rw-r--r--  2.0 unx     4275 b- defN 23-Apr-12 18:31 monai/networks/blocks/acti_norm.py
+-rw-r--r--  2.0 unx     5839 b- defN 23-Apr-12 18:31 monai/networks/blocks/activation.py
+-rw-r--r--  2.0 unx     4380 b- defN 23-Apr-12 18:31 monai/networks/blocks/aspp.py
+-rw-r--r--  2.0 unx     7490 b- defN 23-Apr-12 18:31 monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--  2.0 unx    11686 b- defN 23-Apr-12 18:31 monai/networks/blocks/convolutions.py
+-rw-r--r--  2.0 unx     5009 b- defN 23-Apr-12 18:31 monai/networks/blocks/crf.py
+-rw-r--r--  2.0 unx     4740 b- defN 23-Apr-12 18:31 monai/networks/blocks/denseblock.py
+-rw-r--r--  2.0 unx     9255 b- defN 23-Apr-12 18:31 monai/networks/blocks/dints_block.py
+-rw-r--r--  2.0 unx     2413 b- defN 23-Apr-12 18:31 monai/networks/blocks/downsample.py
+-rw-r--r--  2.0 unx    11062 b- defN 23-Apr-12 18:31 monai/networks/blocks/dynunet_block.py
+-rw-r--r--  2.0 unx     3669 b- defN 23-Apr-12 18:31 monai/networks/blocks/encoder.py
+-rw-r--r--  2.0 unx     9024 b- defN 23-Apr-12 18:31 monai/networks/blocks/fcn.py
+-rw-r--r--  2.0 unx    10586 b- defN 23-Apr-12 18:31 monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--  2.0 unx     8263 b- defN 23-Apr-12 18:31 monai/networks/blocks/fft_utils_t.py
+-rw-r--r--  2.0 unx    11454 b- defN 23-Apr-12 18:31 monai/networks/blocks/localnet_block.py
+-rw-r--r--  2.0 unx     2813 b- defN 23-Apr-12 18:31 monai/networks/blocks/mlp.py
+-rw-r--r--  2.0 unx     7987 b- defN 23-Apr-12 18:31 monai/networks/blocks/patchembedding.py
+-rw-r--r--  2.0 unx     8825 b- defN 23-Apr-12 18:31 monai/networks/blocks/regunet_block.py
+-rw-r--r--  2.0 unx     3245 b- defN 23-Apr-12 18:31 monai/networks/blocks/segresnet_block.py
+-rw-r--r--  2.0 unx     3099 b- defN 23-Apr-12 18:31 monai/networks/blocks/selfattention.py
+-rw-r--r--  2.0 unx    12752 b- defN 23-Apr-12 18:31 monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--  2.0 unx     2322 b- defN 23-Apr-12 18:31 monai/networks/blocks/transformerblock.py
+-rw-r--r--  2.0 unx     9049 b- defN 23-Apr-12 18:31 monai/networks/blocks/unetr_block.py
+-rw-r--r--  2.0 unx    13312 b- defN 23-Apr-12 18:31 monai/networks/blocks/upsample.py
+-rw-r--r--  2.0 unx     6656 b- defN 23-Apr-12 18:31 monai/networks/blocks/warp.py
+-rw-r--r--  2.0 unx     1562 b- defN 23-Apr-12 18:31 monai/networks/layers/__init__.py
+-rw-r--r--  2.0 unx     8288 b- defN 23-Apr-12 18:31 monai/networks/layers/convutils.py
+-rw-r--r--  2.0 unx     1802 b- defN 23-Apr-12 18:31 monai/networks/layers/drop_path.py
+-rw-r--r--  2.0 unx    12620 b- defN 23-Apr-12 18:31 monai/networks/layers/factories.py
+-rw-r--r--  2.0 unx    17992 b- defN 23-Apr-12 18:31 monai/networks/layers/filtering.py
+-rw-r--r--  2.0 unx     3324 b- defN 23-Apr-12 18:31 monai/networks/layers/gmm.py
+-rw-r--r--  2.0 unx    28470 b- defN 23-Apr-12 18:31 monai/networks/layers/simplelayers.py
+-rw-r--r--  2.0 unx    25576 b- defN 23-Apr-12 18:31 monai/networks/layers/spatial_transforms.py
+-rw-r--r--  2.0 unx     4296 b- defN 23-Apr-12 18:31 monai/networks/layers/utils.py
+-rw-r--r--  2.0 unx     2253 b- defN 23-Apr-12 18:31 monai/networks/layers/weight_init.py
+-rw-r--r--  2.0 unx     3141 b- defN 23-Apr-12 18:31 monai/networks/nets/__init__.py
+-rw-r--r--  2.0 unx    21533 b- defN 23-Apr-12 18:31 monai/networks/nets/ahnet.py
+-rw-r--r--  2.0 unx     9202 b- defN 23-Apr-12 18:31 monai/networks/nets/attentionunet.py
+-rw-r--r--  2.0 unx    12089 b- defN 23-Apr-12 18:31 monai/networks/nets/autoencoder.py
+-rw-r--r--  2.0 unx    10950 b- defN 23-Apr-12 18:31 monai/networks/nets/basic_unet.py
+-rw-r--r--  2.0 unx     7960 b- defN 23-Apr-12 18:31 monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--  2.0 unx     6293 b- defN 23-Apr-12 18:31 monai/networks/nets/classifier.py
+-rw-r--r--  2.0 unx    15820 b- defN 23-Apr-12 18:31 monai/networks/nets/densenet.py
+-rw-r--r--  2.0 unx    44771 b- defN 23-Apr-12 18:31 monai/networks/nets/dints.py
+-rw-r--r--  2.0 unx    18210 b- defN 23-Apr-12 18:31 monai/networks/nets/dynunet.py
+-rw-r--r--  2.0 unx    40643 b- defN 23-Apr-12 18:31 monai/networks/nets/efficientnet.py
+-rw-r--r--  2.0 unx    14147 b- defN 23-Apr-12 18:31 monai/networks/nets/flexible_unet.py
+-rw-r--r--  2.0 unx     7212 b- defN 23-Apr-12 18:31 monai/networks/nets/fullyconnectednet.py
+-rw-r--r--  2.0 unx     6581 b- defN 23-Apr-12 18:31 monai/networks/nets/generator.py
+-rw-r--r--  2.0 unx     8882 b- defN 23-Apr-12 18:31 monai/networks/nets/highresnet.py
+-rw-r--r--  2.0 unx    28678 b- defN 23-Apr-12 18:31 monai/networks/nets/hovernet.py
+-rw-r--r--  2.0 unx     9812 b- defN 23-Apr-12 18:31 monai/networks/nets/milmodel.py
+-rw-r--r--  2.0 unx     6102 b- defN 23-Apr-12 18:31 monai/networks/nets/netadapter.py
+-rw-r--r--  2.0 unx     6488 b- defN 23-Apr-12 18:31 monai/networks/nets/regressor.py
+-rw-r--r--  2.0 unx    17189 b- defN 23-Apr-12 18:31 monai/networks/nets/regunet.py
+-rw-r--r--  2.0 unx    16785 b- defN 23-Apr-12 18:31 monai/networks/nets/resnet.py
+-rw-r--r--  2.0 unx    13994 b- defN 23-Apr-12 18:31 monai/networks/nets/segresnet.py
+-rw-r--r--  2.0 unx    15667 b- defN 23-Apr-12 18:31 monai/networks/nets/segresnet_ds.py
+-rw-r--r--  2.0 unx    19289 b- defN 23-Apr-12 18:31 monai/networks/nets/senet.py
+-rw-r--r--  2.0 unx    42000 b- defN 23-Apr-12 18:31 monai/networks/nets/swin_unetr.py
+-rw-r--r--  2.0 unx     6248 b- defN 23-Apr-12 18:31 monai/networks/nets/torchvision_fc.py
+-rw-r--r--  2.0 unx    16626 b- defN 23-Apr-12 18:31 monai/networks/nets/transchex.py
+-rw-r--r--  2.0 unx    13722 b- defN 23-Apr-12 18:31 monai/networks/nets/unet.py
+-rw-r--r--  2.0 unx     7943 b- defN 23-Apr-12 18:31 monai/networks/nets/unetr.py
+-rw-r--r--  2.0 unx     6285 b- defN 23-Apr-12 18:31 monai/networks/nets/varautoencoder.py
+-rw-r--r--  2.0 unx     5655 b- defN 23-Apr-12 18:31 monai/networks/nets/vit.py
+-rw-r--r--  2.0 unx     4817 b- defN 23-Apr-12 18:31 monai/networks/nets/vitautoenc.py
+-rw-r--r--  2.0 unx    10011 b- defN 23-Apr-12 18:31 monai/networks/nets/vnet.py
+-rw-r--r--  2.0 unx      796 b- defN 23-Apr-12 18:31 monai/optimizers/__init__.py
+-rw-r--r--  2.0 unx    21948 b- defN 23-Apr-12 18:31 monai/optimizers/lr_finder.py
+-rw-r--r--  2.0 unx     3652 b- defN 23-Apr-12 18:31 monai/optimizers/lr_scheduler.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Apr-12 18:31 monai/optimizers/novograd.py
+-rw-r--r--  2.0 unx     4131 b- defN 23-Apr-12 18:31 monai/optimizers/utils.py
+-rw-r--r--  2.0 unx    15216 b- defN 23-Apr-12 18:31 monai/transforms/__init__.py
+-rw-r--r--  2.0 unx     8946 b- defN 23-Apr-12 18:31 monai/transforms/adaptors.py
+-rw-r--r--  2.0 unx    40532 b- defN 23-Apr-12 18:31 monai/transforms/compose.py
+-rw-r--r--  2.0 unx    17160 b- defN 23-Apr-12 18:31 monai/transforms/inverse.py
+-rw-r--r--  2.0 unx     7054 b- defN 23-Apr-12 18:31 monai/transforms/inverse_batch_transform.py
+-rw-r--r--  2.0 unx     3386 b- defN 23-Apr-12 18:31 monai/transforms/nvtx.py
+-rw-r--r--  2.0 unx     2885 b- defN 23-Apr-12 18:31 monai/transforms/traits.py
+-rw-r--r--  2.0 unx    18234 b- defN 23-Apr-12 18:31 monai/transforms/transform.py
+-rw-r--r--  2.0 unx    71153 b- defN 23-Apr-12 18:31 monai/transforms/utils.py
+-rw-r--r--  2.0 unx    31081 b- defN 23-Apr-12 18:31 monai/transforms/utils_create_transform_ims.py
+-rw-r--r--  2.0 unx    18397 b- defN 23-Apr-12 18:31 monai/transforms/utils_pytorch_numpy_unification.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/croppad/__init__.py
+-rw-r--r--  2.0 unx    68728 b- defN 23-Apr-12 18:31 monai/transforms/croppad/array.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-Apr-12 18:31 monai/transforms/croppad/batch.py
+-rw-r--r--  2.0 unx    54071 b- defN 23-Apr-12 18:31 monai/transforms/croppad/dictionary.py
+-rw-r--r--  2.0 unx    12673 b- defN 23-Apr-12 18:31 monai/transforms/croppad/functional.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/intensity/__init__.py
+-rw-r--r--  2.0 unx    98613 b- defN 23-Apr-12 18:31 monai/transforms/intensity/array.py
+-rw-r--r--  2.0 unx    76501 b- defN 23-Apr-12 18:31 monai/transforms/intensity/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/io/__init__.py
+-rw-r--r--  2.0 unx    25430 b- defN 23-Apr-12 18:31 monai/transforms/io/array.py
+-rw-r--r--  2.0 unx    17821 b- defN 23-Apr-12 18:31 monai/transforms/io/dictionary.py
+-rw-r--r--  2.0 unx      699 b- defN 23-Apr-12 18:31 monai/transforms/lazy/__init__.py
+-rw-r--r--  2.0 unx     5552 b- defN 23-Apr-12 18:31 monai/transforms/lazy/functional.py
+-rw-r--r--  2.0 unx     9739 b- defN 23-Apr-12 18:31 monai/transforms/lazy/utils.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/meta_utility/__init__.py
+-rw-r--r--  2.0 unx     4896 b- defN 23-Apr-12 18:31 monai/transforms/meta_utility/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/post/__init__.py
+-rw-r--r--  2.0 unx    40858 b- defN 23-Apr-12 18:31 monai/transforms/post/array.py
+-rw-r--r--  2.0 unx    39905 b- defN 23-Apr-12 18:31 monai/transforms/post/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/signal/__init__.py
+-rw-r--r--  2.0 unx    16378 b- defN 23-Apr-12 18:31 monai/transforms/signal/array.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/smooth_field/__init__.py
+-rw-r--r--  2.0 unx    17833 b- defN 23-Apr-12 18:31 monai/transforms/smooth_field/array.py
+-rw-r--r--  2.0 unx    11194 b- defN 23-Apr-12 18:31 monai/transforms/smooth_field/dictionary.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/spatial/__init__.py
+-rw-r--r--  2.0 unx   168618 b- defN 23-Apr-12 18:31 monai/transforms/spatial/array.py
+-rw-r--r--  2.0 unx   107151 b- defN 23-Apr-12 18:31 monai/transforms/spatial/dictionary.py
+-rw-r--r--  2.0 unx    31494 b- defN 23-Apr-12 18:31 monai/transforms/spatial/functional.py
+-rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 18:31 monai/transforms/utility/__init__.py
+-rw-r--r--  2.0 unx    70325 b- defN 23-Apr-12 18:31 monai/transforms/utility/array.py
+-rw-r--r--  2.0 unx    75816 b- defN 23-Apr-12 18:31 monai/transforms/utility/dictionary.py
+-rw-r--r--  2.0 unx     3366 b- defN 23-Apr-12 18:31 monai/utils/__init__.py
+-rw-r--r--  2.0 unx     4099 b- defN 23-Apr-12 18:31 monai/utils/aliases.py
+-rw-r--r--  2.0 unx     3129 b- defN 23-Apr-12 18:31 monai/utils/decorators.py
+-rw-r--r--  2.0 unx    14759 b- defN 23-Apr-12 18:31 monai/utils/deprecate_utils.py
+-rw-r--r--  2.0 unx     8526 b- defN 23-Apr-12 18:31 monai/utils/dist.py
+-rw-r--r--  2.0 unx    16807 b- defN 23-Apr-12 18:31 monai/utils/enums.py
+-rw-r--r--  2.0 unx    15637 b- defN 23-Apr-12 18:31 monai/utils/jupyter_utils.py
+-rw-r--r--  2.0 unx    27512 b- defN 23-Apr-12 18:31 monai/utils/misc.py
+-rw-r--r--  2.0 unx    23631 b- defN 23-Apr-12 18:31 monai/utils/module.py
+-rw-r--r--  2.0 unx     6876 b- defN 23-Apr-12 18:31 monai/utils/nvtx.py
+-rw-r--r--  2.0 unx    15936 b- defN 23-Apr-12 18:31 monai/utils/profiling.py
+-rw-r--r--  2.0 unx     5955 b- defN 23-Apr-12 18:31 monai/utils/state_cacher.py
+-rw-r--r--  2.0 unx    21147 b- defN 23-Apr-12 18:31 monai/utils/type_conversion.py
+-rw-r--r--  2.0 unx     1038 b- defN 23-Apr-12 18:31 monai/visualize/__init__.py
+-rw-r--r--  2.0 unx    16156 b- defN 23-Apr-12 18:31 monai/visualize/class_activation_maps.py
+-rw-r--r--  2.0 unx     6277 b- defN 23-Apr-12 18:31 monai/visualize/gradient_based.py
+-rw-r--r--  2.0 unx     9200 b- defN 23-Apr-12 18:31 monai/visualize/img2tensorboard.py
+-rw-r--r--  2.0 unx    18816 b- defN 23-Apr-12 18:31 monai/visualize/occlusion_sensitivity.py
+-rw-r--r--  2.0 unx     9966 b- defN 23-Apr-12 18:31 monai/visualize/utils.py
+-rw-r--r--  2.0 unx     1377 b- defN 23-Apr-12 18:31 monai/visualize/visualizer.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10172 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    32603 b- defN 23-Apr-12 18:33 monai-1.2.0rc4.dist-info/RECORD
+364 files, 4707907 bytes uncompressed, 1192237 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -171,32 +171,23 @@
 
 Filename: monai/apps/pathology/__init__.py
 Comment: 
 
 Filename: monai/apps/pathology/utils.py
 Comment: 
 
-Filename: monai/apps/pathology/data/__init__.py
-Comment: 
-
-Filename: monai/apps/pathology/data/datasets.py
-Comment: 
-
 Filename: monai/apps/pathology/engines/__init__.py
 Comment: 
 
 Filename: monai/apps/pathology/engines/utils.py
 Comment: 
 
 Filename: monai/apps/pathology/handlers/__init__.py
 Comment: 
 
-Filename: monai/apps/pathology/handlers/prob_map_producer.py
-Comment: 
-
 Filename: monai/apps/pathology/handlers/utils.py
 Comment: 
 
 Filename: monai/apps/pathology/inferers/__init__.py
 Comment: 
 
 Filename: monai/apps/pathology/inferers/inferer.py
@@ -222,23 +213,14 @@
 
 Filename: monai/apps/pathology/transforms/post/array.py
 Comment: 
 
 Filename: monai/apps/pathology/transforms/post/dictionary.py
 Comment: 
 
-Filename: monai/apps/pathology/transforms/spatial/__init__.py
-Comment: 
-
-Filename: monai/apps/pathology/transforms/spatial/array.py
-Comment: 
-
-Filename: monai/apps/pathology/transforms/spatial/dictionary.py
-Comment: 
-
 Filename: monai/apps/pathology/transforms/stain/__init__.py
 Comment: 
 
 Filename: monai/apps/pathology/transforms/stain/array.py
 Comment: 
 
 Filename: monai/apps/pathology/transforms/stain/dictionary.py
@@ -1089,23 +1071,23 @@
 
 Filename: monai/visualize/utils.py
 Comment: 
 
 Filename: monai/visualize/visualizer.py
 Comment: 
 
-Filename: monai-1.2.0rc3.dist-info/LICENSE
+Filename: monai-1.2.0rc4.dist-info/LICENSE
 Comment: 
 
-Filename: monai-1.2.0rc3.dist-info/METADATA
+Filename: monai-1.2.0rc4.dist-info/METADATA
 Comment: 
 
-Filename: monai-1.2.0rc3.dist-info/WHEEL
+Filename: monai-1.2.0rc4.dist-info/WHEEL
 Comment: 
 
-Filename: monai-1.2.0rc3.dist-info/top_level.txt
+Filename: monai-1.2.0rc4.dist-info/top_level.txt
 Comment: 
 
-Filename: monai-1.2.0rc3.dist-info/RECORD
+Filename: monai-1.2.0rc4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-03-31T10:19:39+0100",
+ "date": "2023-04-12T19:27:56+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "8470454e294f1838635ccf733c6e8ec74aa77568",
- "version": "1.2.0rc3"
+ "full-revisionid": "1a55ba5423d04d2ef7ac19356ccabc4c7906f577",
+ "version": "1.2.0rc4"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## monai/apps/auto3dseg/auto_runner.py

```diff
@@ -32,15 +32,15 @@
 )
 from monai.apps.auto3dseg.hpo_gen import NNIGen
 from monai.apps.auto3dseg.utils import export_bundle_algo_history, import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle import ConfigParser
 from monai.transforms import SaveImage
-from monai.utils.enums import AlgoEnsembleKeys
+from monai.utils.enums import AlgoKeys
 from monai.utils.module import look_up_option, optional_import
 
 logger = get_logger(module_name=__name__)
 
 nni, has_nni = optional_import("nni")
 
 
@@ -277,15 +277,15 @@
         self.cache_filename = os.path.join(self.work_dir, "cache.yaml")
         self.cache = self.read_cache()
         self.export_cache()
 
         # determine if we need to analyze, algo_gen or train from cache, unless manually provided
         self.analyze = not self.cache["analyze"] if analyze is None else analyze
         self.algo_gen = not self.cache["algo_gen"] if algo_gen is None else algo_gen
-        self.train = not self.cache["train"] if train is None else train
+        self.train = train
         self.ensemble = ensemble  # last step, no need to check
 
         self.set_training_params()
         self.set_prediction_params()
         self.set_analyze_params()
 
         self.save_image = self.set_image_save_transform(kwargs)
@@ -631,21 +631,23 @@
                 After the training, the algo object with the ``best_metric`` will be saved as a pickle file.
 
         Note:
             The final results of the model training will be written to all the generated algorithm's output
             folders under the working directory. The results include the model checkpoints, a
             progress.yaml, accuracies in CSV and a pickle file of the Algo object.
         """
-        for task in history:
-            for _, algo in task.items():
-                algo.train(self.train_params)
-                acc = algo.get_score()
-                algo_to_pickle(algo, template_path=algo.template_path, best_metrics=acc)
+        for algo_dict in history:
+            algo = algo_dict[AlgoKeys.ALGO]
+            algo.train(self.train_params)
+            acc = algo.get_score()
 
-    def _train_algo_in_nni(self, history):
+            algo_meta_data = {str(AlgoKeys.SCORE): acc}
+            algo_to_pickle(algo, template_path=algo.template_path, **algo_meta_data)
+
+    def _train_algo_in_nni(self, history: list[dict[str, Any]]) -> None:
         """
         Train the Algos using HPO.
 
         Args:
             history: the history of generated Algos. It is a list of dicts. Each element has the task name
                 (e.g. "dints_0" for dints network in fold 0) as the key and the algo object as the value.
                 After the training, the algo object with the ``best_metric`` will be saved as a pickle file.
@@ -668,60 +670,65 @@
             "maxExperimentDuration": "1h",
             "tuner": {"name": "GridSearch"},
             "trainingService": {"platform": "local", "useActiveGpu": True},
         }
 
         last_total_tasks = len(import_bundle_algo_history(self.work_dir, only_trained=True))
         mode_dry_run = self.hpo_params.pop("nni_dry_run", False)
-        for task in history:
-            for name, algo in task.items():
-                nni_gen = NNIGen(algo=algo, params=self.hpo_params)
-                obj_filename = nni_gen.get_obj_filename()
-                nni_config = deepcopy(default_nni_config)
-                # override the default nni config with the same key in hpo_params
-                for key in self.hpo_params:
-                    if key in nni_config:
-                        nni_config[key] = self.hpo_params[key]
-                nni_config.update({"experimentName": name})
-                nni_config.update({"search_space": self.search_space})
-                trial_cmd = "python -m monai.apps.auto3dseg NNIGen run_algo " + obj_filename + " " + self.work_dir
-                nni_config.update({"trialCommand": trial_cmd})
-                nni_config_filename = os.path.abspath(os.path.join(self.work_dir, f"{name}_nni_config.yaml"))
-                ConfigParser.export_config_file(nni_config, nni_config_filename, fmt="yaml", default_flow_style=None)
-
-                max_trial = min(self.hpo_tasks, cast(int, default_nni_config["maxTrialNumber"]))
-                cmd = "nnictl create --config " + nni_config_filename + " --port 8088"
-
-                if mode_dry_run:
-                    logger.info(f"AutoRunner HPO is in dry-run mode. Please manually launch: {cmd}")
-                    continue
-
-                subprocess.run(cmd.split(), check=True)
-
+        for algo_dict in history:
+            name = algo_dict[AlgoKeys.ID]
+            algo = algo_dict[AlgoKeys.ALGO]
+            nni_gen = NNIGen(algo=algo, params=self.hpo_params)
+            obj_filename = nni_gen.get_obj_filename()
+            nni_config = deepcopy(default_nni_config)
+            # override the default nni config with the same key in hpo_params
+            for key in self.hpo_params:
+                if key in nni_config:
+                    nni_config[key] = self.hpo_params[key]
+            nni_config.update({"experimentName": name})
+            nni_config.update({"search_space": self.search_space})
+            trial_cmd = "python -m monai.apps.auto3dseg NNIGen run_algo " + obj_filename + " " + self.work_dir
+            nni_config.update({"trialCommand": trial_cmd})
+            nni_config_filename = os.path.abspath(os.path.join(self.work_dir, f"{name}_nni_config.yaml"))
+            ConfigParser.export_config_file(nni_config, nni_config_filename, fmt="yaml", default_flow_style=None)
+
+            max_trial = min(self.hpo_tasks, cast(int, default_nni_config["maxTrialNumber"]))
+            cmd = "nnictl create --config " + nni_config_filename + " --port 8088"
+
+            if mode_dry_run:
+                logger.info(f"AutoRunner HPO is in dry-run mode. Please manually launch: {cmd}")
+                continue
+
+            subprocess.run(cmd.split(), check=True)
+
+            n_trainings = len(import_bundle_algo_history(self.work_dir, only_trained=True))
+            while n_trainings - last_total_tasks < max_trial:
+                sleep(1)
                 n_trainings = len(import_bundle_algo_history(self.work_dir, only_trained=True))
-                while n_trainings - last_total_tasks < max_trial:
-                    sleep(1)
-                    n_trainings = len(import_bundle_algo_history(self.work_dir, only_trained=True))
-
-                cmd = "nnictl stop --all"
-                subprocess.run(cmd.split(), check=True)
-                logger.info(f"NNI completes HPO on {name}")
-                last_total_tasks = n_trainings
+
+            cmd = "nnictl stop --all"
+            subprocess.run(cmd.split(), check=True)
+            logger.info(f"NNI completes HPO on {name}")
+            last_total_tasks = n_trainings
 
     def run(self):
         """
         Run the AutoRunner pipeline
         """
         # step 1: data analysis
         if self.analyze and self.analyze_params is not None:
             logger.info("Running data analysis...")
             da = DataAnalyzer(
                 self.datalist_filename, self.dataroot, output_path=self.datastats_filename, **self.analyze_params
             )
             da.get_all_case_stats()
+
+            da = None  # type: ignore
+            torch.cuda.empty_cache()
+
             self.export_cache(analyze=True, datastats=self.datastats_filename)
         else:
             logger.info("Skipping data analysis...")
 
         # step 2: algorithm generation
         if self.algo_gen:
             if not os.path.isfile(self.datastats_filename):
@@ -750,48 +757,69 @@
             history = bundle_generator.get_history()
             export_bundle_algo_history(history)
             self.export_cache(algo_gen=True)
         else:
             logger.info("Skipping algorithm generation...")
 
         # step 3: algo training
-        if self.train:
+        auto_train_choice = self.train is None
+        if self.train or (auto_train_choice and not self.cache["train"]):
             history = import_bundle_algo_history(self.work_dir, only_trained=False)
 
             if len(history) == 0:
                 raise ValueError(
                     f"Could not find training scripts in {self.work_dir}. "
                     "Possibly the required algorithms generation step was not completed."
                 )
 
-            if not self.hpo:
-                self._train_algo_in_sequence(history)
-            else:
-                self._train_algo_in_nni(history)
+            if auto_train_choice:
+                skip_algos = [h[AlgoKeys.ID] for h in history if h[AlgoKeys.IS_TRAINED]]
+                if len(skip_algos) > 0:
+                    logger.info(
+                        f"Skipping already trained algos {skip_algos}."
+                        "Set option train=True to always retrain all algos."
+                    )
+                    history = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
+
+            if len(history) > 0:
+                if not self.hpo:
+                    self._train_algo_in_sequence(history)
+                else:
+                    self._train_algo_in_nni(history)
+
             self.export_cache(train=True)
         else:
             logger.info("Skipping algorithm training...")
 
         # step 4: model ensemble and write the prediction to disks.
         if self.ensemble:
-            history = import_bundle_algo_history(self.work_dir, only_trained=True)
+            history = import_bundle_algo_history(self.work_dir, only_trained=False)
+
+            history_untrained = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
+            if len(history_untrained) > 0:
+                warnings.warn(
+                    f"Ensembling step will skip {[h['name'] for h in history_untrained]} untrained algos."
+                    "Generally it means these algos did not complete training."
+                )
+                history = [h for h in history if h[AlgoKeys.IS_TRAINED]]
+
             if len(history) == 0:
                 raise ValueError(
-                    f"Could not find the trained results in {self.work_dir}. "
+                    f"Could not find any trained algos in {self.work_dir}. "
                     "Possibly the required training step was not completed."
                 )
 
             builder = AlgoEnsembleBuilder(history, self.data_src_cfg_name)
             builder.set_ensemble_method(self.ensemble_method)
 
             ensembler = builder.get_ensemble()
             preds = ensembler(pred_param=self.pred_params)
             if len(preds) > 0:
                 logger.info("Auto3Dseg picked the following networks to ensemble:")
                 for algo in ensembler.get_algo_ensemble():
-                    logger.info(algo[AlgoEnsembleKeys.ID])
+                    logger.info(algo[AlgoKeys.ID])
 
                 for pred in preds:
                     self.save_image(pred)
                 logger.info(f"Auto3Dseg ensemble prediction outputs are saved in {self.output_dir}.")
 
-        logger.info("Auto3Dseg pipeline is complete successfully.")
+        logger.info("Auto3Dseg pipeline is completed successfully.")
```

## monai/apps/auto3dseg/bundle_gen.py

```diff
@@ -29,17 +29,18 @@
 
 from monai.apps import download_and_extract
 from monai.apps.utils import get_logger
 from monai.auto3dseg.algo_gen import Algo, AlgoGen
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
 from monai.utils import ensure_tuple
+from monai.utils.enums import AlgoKeys
 
 logger = get_logger(module_name=__name__)
-ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "4af80e1")
+ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "b37ed82")
 
 __all__ = ["BundleAlgo", "BundleGen"]
 
 
 class BundleAlgo(Algo):
     """
     An algorithm represented by a set of bundle configurations and scripts.
@@ -76,14 +77,24 @@
         self.data_list_file = ""
         self.output_path = ""
         self.name = ""
         self.best_metric = None
         # track records when filling template config: {"<config name>": {"<placeholder key>": value, ...}, ...}
         self.fill_records: dict = {}
 
+    def pre_check_skip_algo(self, skip_bundlegen: bool = False, skip_info: str = "") -> tuple[bool, str]:
+        """
+        Analyse the data analysis report and check if the algorithm needs to be skipped.
+        This function is overriden within algo.
+        Args:
+            skip_bundlegen: skip generating bundles for this algo if true.
+            skip_info: info to print when skipped.
+        """
+        return skip_bundlegen, skip_info
+
     def set_data_stats(self, data_stats_files: str) -> None:
         """
         Set the data analysis report (generated by DataAnalyzer).
 
         Args:
             data_stats_files: path to the datastats yaml file
         """
@@ -402,15 +413,15 @@
                 if len(algos) == 0:
                     raise ValueError(f"Unable to find provided algos in {algos_all}")
             else:
                 algos = algos_all
 
         self.algos: Any = []
         if isinstance(algos, dict):
-            for algo_name, algo_params in algos.items():
+            for algo_name, algo_params in sorted(algos.items()):
                 template_path = os.path.dirname(algo_params.get("template_path", "."))
                 if len(template_path) > 0 and template_path not in sys.path:
                     sys.path.append(template_path)
 
                 try:
                     onealgo = ConfigParser(algo_params).get_parsed_content()
                     onealgo.name = algo_name
@@ -456,15 +467,15 @@
         self.data_src_cfg_filename = data_src_cfg_filename
 
     def get_data_src(self):
         """Get the data source filename"""
         return self.data_src_cfg_filename
 
     def get_history(self) -> list:
-        """get the history of the bundleAlgo object with their names/identifiers"""
+        """Get the history of the bundleAlgo object with their names/identifiers"""
         return self.history
 
     def generate(
         self,
         output_folder: str = ".",
         num_fold: int = 5,
         gpu_customization: bool = False,
@@ -507,19 +518,26 @@
             for f_id in ensure_tuple(fold_idx):
                 data_stats = self.get_data_stats()
                 data_src_cfg = self.get_data_src()
                 gen_algo = deepcopy(algo)
                 gen_algo.set_data_stats(data_stats)
                 gen_algo.set_data_source(data_src_cfg)
                 name = f"{gen_algo.name}_{f_id}"
+                skip_bundlegen, skip_info = gen_algo.pre_check_skip_algo()
+                if skip_bundlegen:
+                    logger.info(f"{name} is skipped! {skip_info}")
+                    continue
                 if gpu_customization:
                     gen_algo.export_to_disk(
                         output_folder,
                         name,
                         fold=f_id,
                         gpu_customization=True,
                         gpu_customization_specs=gpu_customization_specs,
                     )
                 else:
                     gen_algo.export_to_disk(output_folder, name, fold=f_id)
+
                 algo_to_pickle(gen_algo, template_path=algo.template_path)
-                self.history.append({name: gen_algo})  # track the previous, may create a persistent history
+                self.history.append(
+                    {AlgoKeys.ID: name, AlgoKeys.ALGO: gen_algo}
+                )  # track the previous, may create a persistent history
```

## monai/apps/auto3dseg/data_analyzer.py

```diff
@@ -13,22 +13,23 @@
 
 import warnings
 from os import path
 from typing import Any, cast
 
 import numpy as np
 import torch
+from torch.multiprocessing import get_context
 
 from monai.apps.auto3dseg.transforms import EnsureSameShaped
 from monai.apps.utils import get_logger
 from monai.auto3dseg import SegSummarizer
 from monai.auto3dseg.utils import datafold_read
 from monai.bundle import config_parser
 from monai.bundle.config_parser import ConfigParser
-from monai.data import DataLoader, Dataset
+from monai.data import DataLoader, Dataset, partition_dataset
 from monai.data.utils import no_collation
 from monai.transforms import Compose, EnsureTyped, LoadImaged, Orientationd
 from monai.utils import StrEnum, min_version, optional_import
 from monai.utils.enums import DataStatsKeys, ImageStatsKeys
 
 
 def strenum_representer(dumper, data):
@@ -57,16 +58,15 @@
         datalist: a Python dictionary storing group, fold, and other information of the medical
             image dataset, or a string to the JSON file storing the dictionary.
         dataroot: user's local directory containing the datasets.
         output_path: path to save the analysis result.
         average: whether to average the statistical value across different image modalities.
         do_ccp: apply the connected component algorithm to process the labels/images
         device: a string specifying hardware (CUDA/CPU) utilized for the operations.
-        worker: number of workers to use for parallel processing. If device is cuda/GPU, worker has
-            to be 0.
+        worker: number of workers to use for loading datasets in each GPU/CPU sub-process.
         image_key: a string that user specify for the image. The DataAnalyzer will look it up in the
             datalist to locate the image files of the dataset.
         label_key: a string that user specify for the label. The DataAnalyzer will look it up in the
             datalist to locate the label files of the dataset. If label_key is NoneType or "None",
             the DataAnalyzer will skip looking for labels and all label-related operations.
         hist_bins: bins to compute histogram for each image channel.
         hist_range: ranges to compute histogram for each image channel.
@@ -114,15 +114,15 @@
     def __init__(
         self,
         datalist: str | dict,
         dataroot: str = "",
         output_path: str = "./datastats.yaml",
         average: bool = True,
         do_ccp: bool = False,
-        device: str | torch.device = "cpu",
+        device: str | torch.device = "cuda",
         worker: int = 4,
         image_key: str = "image",
         label_key: str | None = "label",
         hist_bins: list | int | None = 0,
         hist_range: list | None = None,
         fmt: str = "yaml",
         histogram_only: bool = False,
@@ -166,16 +166,17 @@
             if "stdev" in prop and np.any(prop["stdev"]):
                 return False
 
         return True
 
     def get_all_case_stats(self, key="training", transform_list=None):
         """
-        Get all case stats. Caller of the DataAnalyser class. The function iterates datalist and
-        call get_case_stats to generate stats. Then get_case_summary is called to combine results.
+        Get all case stats. Caller of the DataAnalyser class. The function initiates multiple GPU or CPU processes of the internal
+        _get_all_case_stats functions, which iterates datalist and call SegSummarizer to generate stats for each case.
+        After all case stats are generated, SegSummarizer is called to combine results.
 
         Args:
             key: dataset key
             transform_list: option list of transforms before SegSummarizer
 
         Returns:
             A data statistics dictionary containing
@@ -193,14 +194,94 @@
 
         Notes:
             Since the backend of the statistics computation are torch/numpy, nan/inf value
             may be generated and carried over in the computation. In such cases, the output
             dictionary will include .nan/.inf in the statistics.
 
         """
+        result: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
+        result_bycase: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
+        if self.device.type == "cpu":
+            nprocs = 1
+            logger.info("Using CPU for data analyzing!")
+        else:
+            nprocs = torch.cuda.device_count()
+            logger.info(f"Found {nprocs} GPUs for data analyzing!")
+        if nprocs > 1:
+            tmp_ctx = get_context("forkserver")
+            with tmp_ctx.Manager() as manager:
+                manager_list = manager.list()
+                processes = []
+                for rank in range(nprocs):
+                    p = tmp_ctx.Process(
+                        target=self._get_all_case_stats, args=(rank, nprocs, manager_list, key, transform_list)
+                    )
+                    processes.append(p)
+                for p in processes:
+                    p.start()
+                for p in processes:
+                    p.join()
+                # merge DataStatsKeys.BY_CASE
+                for _ in manager_list:
+                    result_bycase[DataStatsKeys.BY_CASE].extend(_[DataStatsKeys.BY_CASE])
+        else:
+            result_bycase = self._get_all_case_stats(0, 1, None, key, transform_list)
+
+        summarizer = SegSummarizer(
+            self.image_key,
+            self.label_key,
+            average=self.average,
+            do_ccp=self.do_ccp,
+            hist_bins=self.hist_bins,
+            hist_range=self.hist_range,
+            histogram_only=self.histogram_only,
+        )
+        n_cases = len(result_bycase[DataStatsKeys.BY_CASE])
+        result[DataStatsKeys.SUMMARY] = summarizer.summarize(cast(list, result_bycase[DataStatsKeys.BY_CASE]))
+        result[DataStatsKeys.SUMMARY]["n_cases"] = n_cases
+        result[DataStatsKeys.BY_CASE] = [None] * n_cases
+        result_bycase[DataStatsKeys.SUMMARY] = result[DataStatsKeys.SUMMARY]
+        if not self._check_data_uniformity([ImageStatsKeys.SPACING], result):
+            logger.info("Data spacing is not completely uniform. MONAI transforms may provide unexpected result")
+        if self.output_path:
+            ConfigParser.export_config_file(
+                result, self.output_path, fmt=self.fmt, default_flow_style=None, sort_keys=False
+            )
+            ConfigParser.export_config_file(
+                result_bycase,
+                self.output_path.replace(".yaml", "_by_case.yaml"),
+                fmt=self.fmt,
+                default_flow_style=None,
+                sort_keys=False,
+            )
+        # release memory
+        if self.device.type == "cuda":
+            # release unreferenced tensors to mitigate OOM
+            # limitation: https://github.com/pytorch/pytorch/issues/12873#issuecomment-482916237
+            torch.cuda.empty_cache()
+        result[DataStatsKeys.BY_CASE] = result_bycase[DataStatsKeys.BY_CASE]
+        return result
+
+    def _get_all_case_stats(
+        self,
+        rank: int = 0,
+        world_size: int = 1,
+        manager_list: list | None = None,
+        key: str = "training",
+        transform_list: list | None = None,
+    ) -> Any:
+        """
+        Get all case stats from a partitioned datalist. The function can only be called internally by get_all_case_stats.
+        Args:
+            rank: GPU process rank, 0 for CPU process
+            world_size: total number of GPUs, 1 for CPU process
+            manager_list: multiprocessing manager list object, if using multi-GPU.
+            key: dataset key
+            transform_list: option list of transforms before SegSummarizer
+        """
         summarizer = SegSummarizer(
             self.image_key,
             self.label_key,
             average=self.average,
             do_ccp=self.do_ccp,
             hist_bins=self.hist_bins,
             hist_range=self.hist_range,
@@ -220,41 +301,56 @@
                         keys=self.label_key,
                         source_key=self.image_key,
                         allowed_shape_difference=allowed_shape_difference,
                     )
                 )
 
         transform = Compose(transform_list)
-
         files, _ = datafold_read(datalist=self.datalist, basedir=self.dataroot, fold=-1, key=key)
+        if world_size <= len(files):
+            files = partition_dataset(data=files, num_partitions=world_size)[rank]
+        else:
+            files = partition_dataset(data=files, num_partitions=len(files))[rank] if rank < len(files) else []
         dataset = Dataset(data=files, transform=transform)
         dataloader = DataLoader(
             dataset,
             batch_size=1,
             shuffle=False,
             num_workers=self.worker,
             collate_fn=no_collation,
             pin_memory=self.device.type == "cuda",
         )
-        result: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
         result_bycase: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
-
+        device = self.device if self.device.type == "cpu" else torch.device("cuda", rank)
         if not has_tqdm:
             warnings.warn("tqdm is not installed. not displaying the caching progress.")
 
-        for batch_data in tqdm(dataloader) if has_tqdm else dataloader:
+        for batch_data in tqdm(dataloader) if (has_tqdm and rank == 0) else dataloader:
             batch_data = batch_data[0]
-            batch_data[self.image_key] = batch_data[self.image_key].to(self.device)
-
-            if self.label_key is not None:
-                label = batch_data[self.label_key]
-                label = torch.argmax(label, dim=0) if label.shape[0] > 1 else label[0]
-                batch_data[self.label_key] = label.to(self.device)
-
-            d = summarizer(batch_data)
+            try:
+                batch_data[self.image_key] = batch_data[self.image_key].to(device)
+                if self.label_key is not None:
+                    label = batch_data[self.label_key]
+                    label = torch.argmax(label, dim=0) if label.shape[0] > 1 else label[0]
+                    batch_data[self.label_key] = label.to(device)
+                d = summarizer(batch_data)
+            except BaseException:
+                if "image_meta_dict" in batch_data.keys():
+                    filename = batch_data["image_meta_dict"]["filename_or_obj"]
+                else:
+                    filename = batch_data[self.image_key].meta["filename_or_obj"]
+                logger.info(f"Unable to process data {filename} on {device}.")
+                if self.device.type == "cuda":
+                    logger.info("DataAnalyzer `device` set to GPU execution hit an exception. Falling back to `cpu`.")
+                    batch_data[self.image_key] = batch_data[self.image_key].to("cpu")
+                    if self.label_key is not None:
+                        label = batch_data[self.label_key]
+                        label = torch.argmax(label, dim=0) if label.shape[0] > 1 else label[0]
+                        batch_data[self.label_key] = label.to("cpu")
+                    d = summarizer(batch_data)
 
             stats_by_cases = {
                 DataStatsKeys.BY_CASE_IMAGE_PATH: d[DataStatsKeys.BY_CASE_IMAGE_PATH],
                 DataStatsKeys.BY_CASE_LABEL_PATH: d[DataStatsKeys.BY_CASE_LABEL_PATH],
                 DataStatsKeys.IMAGE_STATS: d[DataStatsKeys.IMAGE_STATS],
             }
             if self.hist_bins != 0:
@@ -264,40 +360,11 @@
                 stats_by_cases.update(
                     {
                         DataStatsKeys.FG_IMAGE_STATS: d[DataStatsKeys.FG_IMAGE_STATS],
                         DataStatsKeys.LABEL_STATS: d[DataStatsKeys.LABEL_STATS],
                     }
                 )
             result_bycase[DataStatsKeys.BY_CASE].append(stats_by_cases)
-
-        n_cases = len(result_bycase[DataStatsKeys.BY_CASE])
-
-        result[DataStatsKeys.SUMMARY] = summarizer.summarize(cast(list, result_bycase[DataStatsKeys.BY_CASE]))
-        result[DataStatsKeys.SUMMARY]["n_cases"] = n_cases
-        result[DataStatsKeys.BY_CASE] = [None] * n_cases
-
-        if not self._check_data_uniformity([ImageStatsKeys.SPACING], result):
-            print("Data spacing is not completely uniform. MONAI transforms may provide unexpected result")
-
-        if self.output_path:
-            # saving summary and by_case as 2 files, to minimize loading time when only the summary is necessary
-            ConfigParser.export_config_file(
-                result, self.output_path, fmt=self.fmt, default_flow_style=None, sort_keys=False
-            )
-            ConfigParser.export_config_file(
-                result_bycase,
-                self.output_path.replace(".yaml", "_by_case.yaml"),
-                fmt=self.fmt,
-                default_flow_style=None,
-                sort_keys=False,
-            )
-
-        # release memory
-        d = None
-        if self.device.type == "cuda":
-            # release unreferenced tensors to mitigate OOM
-            # limitation: https://github.com/pytorch/pytorch/issues/12873#issuecomment-482916237
-            torch.cuda.empty_cache()
-
-        # return combined
-        result[DataStatsKeys.BY_CASE] = result_bycase[DataStatsKeys.BY_CASE]
-        return result
+        if manager_list is None:
+            return result_bycase
+        else:
+            manager_list.append(result_bycase)
```

## monai/apps/auto3dseg/ensemble_builder.py

```diff
@@ -23,15 +23,15 @@
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.apps.utils import get_logger
 from monai.auto3dseg import concat_val_to_np
 from monai.auto3dseg.utils import datafold_read
 from monai.bundle import ConfigParser
 from monai.transforms import MeanEnsemble, VoteEnsemble
-from monai.utils.enums import AlgoEnsembleKeys
+from monai.utils.enums import AlgoKeys
 from monai.utils.misc import prob2class
 from monai.utils.module import look_up_option
 
 logger = get_logger(module_name=__name__)
 
 
 class AlgoEnsemble(ABC):
@@ -55,15 +55,15 @@
         """
         Get a model by identifier.
 
         Args:
             identifier: the name of the bundleAlgo
         """
         for algo in self.algos:
-            if identifier == algo[AlgoEnsembleKeys.ID]:
+            if identifier == algo[AlgoKeys.ID]:
                 return algo
 
     def get_algo_ensemble(self):
         """
         Get the algo ensemble after ranking or a empty list if ranking was not started.
 
         Returns:
@@ -156,15 +156,15 @@
         sigmoid = param.pop("sigmoid", False)
 
         outputs = []
         for i, file in enumerate(files):
             print(i)
             preds = []
             for algo in self.algo_ensemble:
-                infer_instance = algo[AlgoEnsembleKeys.ALGO]
+                infer_instance = algo[AlgoKeys.ALGO]
                 pred = infer_instance.predict(predict_files=[file], predict_params=param)
                 preds.append(pred[0])
             outputs.append(self.ensemble_pred(preds, sigmoid=sigmoid))
         return outputs
 
     @abstractmethod
     def collect_algos(self, *args, **kwargs):
@@ -183,15 +183,15 @@
         super().__init__()
         self.n_best = n_best
 
     def sort_score(self):
         """
         Sort the best_metrics
         """
-        scores = concat_val_to_np(self.algos, [AlgoEnsembleKeys.SCORE])
+        scores = concat_val_to_np(self.algos, [AlgoKeys.SCORE])
         return np.argsort(scores).tolist()
 
     def collect_algos(self, n_best: int = -1) -> None:
         """
         Rank the algos by finding the top N (n_best) validation scores.
         """
 
@@ -199,16 +199,16 @@
             n_best = self.n_best
 
         ranks = self.sort_score()
         if len(ranks) < n_best:
             warn(f"Found {len(ranks)} available algos (pre-defined n_best={n_best}). All {len(ranks)} will be used.")
             n_best = len(ranks)
 
-        # get the indices that the rank is larger than N
-        indices = [i for (i, r) in enumerate(ranks) if r >= n_best]
+        # get the ranks for which the indices are lower than N-n_best
+        indices = [r for (i, r) in enumerate(ranks) if i < (len(ranks) - n_best)]
 
         # remove the found indices
         indices = sorted(indices, reverse=True)
 
         self.algo_ensemble = deepcopy(self.algos)
         for idx in indices:
             if idx < len(self.algo_ensemble):
@@ -234,21 +234,22 @@
 
         self.algo_ensemble = []
         for f_idx in range(self.n_fold):
             best_score = -1.0
             best_model: BundleAlgo | None = None
             for algo in self.algos:
                 # algorithm folder: {net}_{fold_index}_{other}
-                identifier = algo[AlgoEnsembleKeys.ID].split("_")[1]
+                identifier = algo[AlgoKeys.ID].split("_")[1]
                 try:
                     algo_id = int(identifier)
                 except ValueError as err:
                     raise ValueError(f"model identifier {identifier} is not number.") from err
-                if algo_id == f_idx and algo[AlgoEnsembleKeys.SCORE] > best_score:
+                if algo_id == f_idx and algo[AlgoKeys.SCORE] > best_score:
                     best_model = algo
+                    best_score = algo[AlgoKeys.SCORE]
             self.algo_ensemble.append(best_model)
 
 
 class AlgoEnsembleBuilder:
     """
     Build ensemble workflow from configs and arguments.
 
@@ -262,30 +263,28 @@
 
             builder = AlgoEnsembleBuilder(history, data_src_cfg)
             builder.set_ensemble_method(BundleAlgoEnsembleBestN(3))
             ensemble = builder.get_ensemble()
 
     """
 
-    def __init__(self, history: Sequence[dict], data_src_cfg_filename: str | None = None):
-        self.infer_algos: list[dict[AlgoEnsembleKeys, Any]] = []
+    def __init__(self, history: Sequence[dict[str, Any]], data_src_cfg_filename: str | None = None):
+        self.infer_algos: list[dict[AlgoKeys, Any]] = []
         self.ensemble: AlgoEnsemble
         self.data_src_cfg = ConfigParser(globals=False)
 
         if data_src_cfg_filename is not None and os.path.exists(str(data_src_cfg_filename)):
             self.data_src_cfg.read_config(data_src_cfg_filename)
 
-        for h in history:
+        for algo_dict in history:
             # load inference_config_paths
-            # raise warning/error if not found
-            if len(h) > 1:
-                raise ValueError(f"{h} should only contain one set of genAlgo key-value")
 
-            name = list(h.keys())[0]
-            gen_algo = h[name]
+            name = algo_dict[AlgoKeys.ID]
+            gen_algo = algo_dict[AlgoKeys.ALGO]
+
             best_metric = gen_algo.get_score()
             algo_path = gen_algo.output_path
             infer_path = os.path.join(algo_path, "scripts", "infer.py")
 
             if not os.path.isdir(algo_path):
                 warn(f"{gen_algo.output_path} is not a directory. Please check the path.")
 
@@ -303,15 +302,15 @@
             gen_algo: a trained BundleAlgo model object.
             best_metric: the best metric in validation of the trained model.
         """
 
         if best_metric is None:
             raise ValueError("Feature to re-validate is to be implemented")
 
-        algo = {AlgoEnsembleKeys.ID: identifier, AlgoEnsembleKeys.ALGO: gen_algo, AlgoEnsembleKeys.SCORE: best_metric}
+        algo = {AlgoKeys.ID: identifier, AlgoKeys.ALGO: gen_algo, AlgoKeys.SCORE: best_metric}
         self.infer_algos.append(algo)
 
     def set_ensemble_method(self, ensemble: AlgoEnsemble, *args: Any, **kwargs: Any) -> None:
         """
         Set the ensemble method.
 
         Args:
```

## monai/apps/auto3dseg/hpo_gen.py

```diff
@@ -19,14 +19,15 @@
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.apps.utils import get_logger
 from monai.auto3dseg import Algo, AlgoGen, algo_from_pickle, algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
 from monai.config import PathLike
 from monai.utils import optional_import
+from monai.utils.enums import AlgoKeys
 
 nni, has_nni = optional_import("nni")
 optuna, has_optuna = optional_import("optuna")
 logger = get_logger(module_name=__name__)
 
 __all__ = ["HPOGen", "NNIGen", "OptunaGen"]
 
@@ -94,16 +95,16 @@
             ├── model_fold0
             └── scripts
 
         .. code-block:: python
             # Bundle Algorithms are already generated by BundleGen in work_dir
             import_bundle_algo_history(work_dir, only_trained=False)
             algo_dict = self.history[0]  # pick the first algorithm
-            algo_name = list(algo_dict.keys())[0]
-            onealgo = algo_dict[algo_name]
+            algo_name = algo_dict[AlgoKeys.ID]
+            onealgo = algo_dict[AlgoKeys.ALGO]
             nni_gen = NNIGen(algo=onealgo)
             nni_gen.print_bundle_algo_instruction()
 
     Notes:
         The NNIGen will prepare the algorithms in a folder and suggest a command to replace trialCommand in the experiment
         config. However, NNIGen will not trigger NNI. User needs to write their NNI experiment configs, and then run the
         NNI command manually.
@@ -233,18 +234,20 @@
         # step 2 set the update params for the algo to run in the next trial
         self.update_params(params)
         # step 3 generate the folder to save checkpoints and train
         self.generate(output_folder)
         self.algo.train(self.params)
         # step 4 report validation acc to controller
         acc = self.algo.get_score()
+        algo_meta_data = {str(AlgoKeys.SCORE): acc}
+
         if isinstance(self.algo, BundleAlgo):
-            algo_to_pickle(self.algo, template_path=self.algo.template_path, best_metrics=acc)
+            algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
         else:
-            algo_to_pickle(self.algo, best_metrics=acc)
+            algo_to_pickle(self.algo, **algo_meta_data)
         self.set_score(acc)
 
 
 class OptunaGen(HPOGen):
     """
     Generate algorithms for the Optuna to automate hyperparameter tuning. Please refer to NNI and Optuna
     (https://optuna.readthedocs.io/en/stable/) for more information. Optuna has different running scheme
@@ -404,12 +407,13 @@
         # step 2 set the update params for the algo to run in the next trial
         self.update_params(params)
         # step 3 generate the folder to save checkpoints and train
         self.generate(output_folder)
         self.algo.train(self.params)
         # step 4 report validation acc to controller
         acc = self.algo.get_score()
+        algo_meta_data = {str(AlgoKeys.SCORE): acc}
         if isinstance(self.algo, BundleAlgo):
-            algo_to_pickle(self.algo, template_path=self.algo.template_path, best_metrics=acc)
+            algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
         else:
-            algo_to_pickle(self.algo, best_metrics=acc)
+            algo_to_pickle(self.algo, **algo_meta_data)
         self.set_score(acc)
```

## monai/apps/auto3dseg/utils.py

```diff
@@ -11,21 +11,23 @@
 
 from __future__ import annotations
 
 import os
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.auto3dseg import algo_from_pickle, algo_to_pickle
+from monai.utils.enums import AlgoKeys
 
 
 def import_bundle_algo_history(
     output_folder: str = ".", template_path: str | None = None, only_trained: bool = True
 ) -> list:
     """
-    import the history of the bundleAlgo object with their names/identifiers
+    import the history of the bundleAlgo objects as a list of algo dicts.
+    each algo_dict has keys name (folder name), algo (bundleAlgo), is_trained (bool),
 
     Args:
         output_folder: the root path of the algorithms templates.
         template_path: the algorithm_template. It must contain algo.py in the follow path:
             ``{algorithm_templates_dir}/{network}/scripts/algo.py``.
         only_trained: only read the algo history if the algo is trained.
     """
@@ -43,26 +45,28 @@
             continue
 
         algo, algo_meta_data = algo_from_pickle(obj_filename, template_path=template_path)
 
         if isinstance(algo, BundleAlgo):  # algo's template path needs override
             algo.template_path = algo_meta_data["template_path"]
 
-        if only_trained:
-            if "best_metrics" in algo_meta_data:
-                history.append({name: algo})
-        else:
-            history.append({name: algo})
+        best_metric = algo_meta_data.get(AlgoKeys.SCORE, None)
+        is_trained = best_metric is not None
+
+        if (only_trained and is_trained) or not only_trained:
+            history.append(
+                {AlgoKeys.ID: name, AlgoKeys.ALGO: algo, AlgoKeys.SCORE: best_metric, AlgoKeys.IS_TRAINED: is_trained}
+            )
 
     return history
 
 
 def export_bundle_algo_history(history: list[dict[str, BundleAlgo]]) -> None:
     """
     Save all the BundleAlgo in the history to algo_object.pkl in each individual folder
 
     Args:
         history: a List of Bundle. Typically, the history can be obtained from BundleGen get_history method
     """
-    for task in history:
-        for _, algo in task.items():
-            algo_to_pickle(algo, template_path=algo.template_path)
+    for algo_dict in history:
+        algo = algo_dict[AlgoKeys.ALGO]
+        algo_to_pickle(algo, template_path=algo.template_path)
```

## monai/apps/pathology/__init__.py

```diff
@@ -7,16 +7,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from .data import MaskedInferenceWSIDataset, PatchWSIDataset, SmartCachePatchWSIDataset
-from .handlers import ProbMapProducer
 from .losses import HoVerNetLoss
 from .metrics import LesionFROC
 from .transforms.stain.array import ExtractHEStains, NormalizeHEStains
 from .transforms.stain.dictionary import (
     ExtractHEStainsd,
     ExtractHEStainsD,
     ExtractHEStainsDict,
```

## monai/apps/pathology/handlers/__init__.py

```diff
@@ -6,9 +6,7 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
-
-from .prob_map_producer import ProbMapProducer
```

## monai/apps/pathology/inferers/inferer.py

```diff
@@ -172,14 +172,16 @@
             self.padding_mode,
             self.cval,
             self.sw_device,
             device,
             self.progress,
             self.roi_weight_map,
             self.process_output,
+            self.buffer_steps,
+            self.buffer_dim,
             *args,
             **kwargs,
         )
 
         if self.extra_input_padding:
             extra_slicing: list[slice] = []
             num_padded_dims = len(self.extra_input_padding) // 2
```

## monai/apps/pathology/metrics/lesion_froc.py

```diff
@@ -13,15 +13,15 @@
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from monai.apps.pathology.utils import PathologyProbNMS, compute_isolated_tumor_cells, compute_multi_instance_mask
 from monai.config import NdarrayOrTensor
-from monai.data.image_reader import WSIReader
+from monai.data.wsi_reader import WSIReader
 from monai.metrics import compute_fp_tp_probs, compute_froc_curve_data, compute_froc_score
 from monai.utils import min_version, optional_import
 
 if TYPE_CHECKING:
     from tqdm import tqdm
 
     has_tqdm = True
```

## monai/apps/pathology/transforms/__init__.py

```diff
@@ -55,16 +55,14 @@
     HoVerNetNuclearTypePostProcessingD,
     HoVerNetNuclearTypePostProcessingd,
     HoVerNetNuclearTypePostProcessingDict,
     WatershedD,
     Watershedd,
     WatershedDict,
 )
-from .spatial.array import SplitOnGrid, TileOnGrid
-from .spatial.dictionary import SplitOnGridd, SplitOnGridD, SplitOnGridDict, TileOnGridd, TileOnGridD, TileOnGridDict
 from .stain.array import ExtractHEStains, NormalizeHEStains
 from .stain.dictionary import (
     ExtractHEStainsd,
     ExtractHEStainsD,
     ExtractHEStainsDict,
     NormalizeHEStainsd,
     NormalizeHEStainsD,
```

## monai/apps/pathology/transforms/post/array.py

```diff
@@ -27,15 +27,15 @@
     RemoveSmallObjects,
     SobelGradients,
 )
 from monai.transforms.transform import Transform
 from monai.transforms.utils_pytorch_numpy_unification import max, maximum, min, sum, unique
 from monai.utils import TransformBackends, convert_to_numpy, optional_import
 from monai.utils.misc import ensure_tuple_rep
-from monai.utils.type_conversion import convert_to_dst_type
+from monai.utils.type_conversion import convert_to_dst_type, convert_to_tensor
 
 label, _ = optional_import("scipy.ndimage.measurements", name="label")
 disk, _ = optional_import("skimage.morphology", name="disk")
 opening, _ = optional_import("skimage.morphology", name="opening")
 watershed, _ = optional_import("skimage.segmentation", name="watershed")
 find_contours, _ = optional_import("skimage.measure", name="find_contours")
 centroid, _ = optional_import("skimage.measure", name="centroid")
@@ -667,14 +667,15 @@
         marker_radius: the radius of the disk-shaped footprint used in `opening` of markers. Defaults to 2.
         marker_postprocess_fn: post-process function for watershed markers.
             If not provided, :py:class:`monai.transforms.post.FillHoles()` will be used.
         watershed_connectivity: `connectivity` argument of `skimage.segmentation.watershed`.
         min_num_points: minimum number of points to be considered as a contour. Defaults to 3.
         contour_level: an optional value for `skimage.measure.find_contours` to find contours in the array.
             If not provided, the level is set to `(max(image) + min(image)) / 2`.
+        device: target device to put the output Tensor data.
     """
 
     def __init__(
         self,
         activation: str | Callable = "softmax",
         mask_threshold: float | None = None,
         min_object_size: int = 10,
@@ -682,17 +683,18 @@
         distance_smooth_fn: Callable | None = None,
         marker_threshold: float = 0.4,
         marker_radius: int = 2,
         marker_postprocess_fn: Callable | None = None,
         watershed_connectivity: int | None = 1,
         min_num_points: int = 3,
         contour_level: float | None = None,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
-
+        self.device = device
         self.generate_watershed_mask = GenerateWatershedMask(
             activation=activation, threshold=mask_threshold, min_object_size=min_object_size
         )
         self.generate_instance_border = GenerateInstanceBorder(kernel_size=sobel_kernel_size)
         self.generate_distance_map = GenerateDistanceMap(smooth_fn=distance_smooth_fn)
         self.generate_watershed_markers = GenerateWatershedMarkers(
             threshold=marker_threshold,
@@ -738,15 +740,15 @@
             if instance_contour is not None:
                 instance_centroid = self.generate_instance_centroid(instance_mask, offset)
                 instance_info[inst_id] = {
                     "bounding_box": instance_bbox,
                     "centroid": instance_centroid,
                     "contour": instance_contour,
                 }
-
+        instance_map = convert_to_tensor(instance_map, device=self.device)
         return instance_info, instance_map
 
 
 class HoVerNetNuclearTypePostProcessing(Transform):
     """
     The post-processing transform for HoVerNet model to generate nuclear type information.
     It updates the input instance info dictionary with information about types of the nuclei (value and probability).
@@ -754,21 +756,27 @@
 
     Args:
         activation: the activation layer to be applied on nuclear type branch. It can be "softmax" or "sigmoid" string,
             or any callable. Defaults to "softmax".
         threshold: an optional float value to threshold to binarize probability map.
             If not provided, defaults to 0.5 when activation is not "softmax", otherwise None.
         return_type_map: whether to calculate and return pixel-level type map.
+        device: target device to put the output Tensor data.
 
     """
 
     def __init__(
-        self, activation: str | Callable = "softmax", threshold: float | None = None, return_type_map: bool = True
+        self,
+        activation: str | Callable = "softmax",
+        threshold: float | None = None,
+        return_type_map: bool = True,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
+        self.device = device
         self.return_type_map = return_type_map
         self.generate_instance_type = GenerateInstanceType()
 
         # set activation layer
         use_softmax = False
         use_sigmoid = False
         activation_fn = None
@@ -820,9 +828,10 @@
             # update instance info dict with type data
             instance_info[inst_id]["type_prob"] = instance_type_prob
             instance_info[inst_id]["type"] = instance_type
 
             # update instance type map
             if type_map is not None:
                 type_map[instance_map == inst_id] = instance_type
+                type_map = convert_to_tensor(type_map, device=self.device)
 
         return instance_info, type_map
```

## monai/apps/pathology/transforms/post/dictionary.py

```diff
@@ -10,14 +10,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections.abc import Callable, Hashable, Mapping
 
 import numpy as np
+import torch
 
 from monai.apps.pathology.transforms.post.array import (
     GenerateDistanceMap,
     GenerateInstanceBorder,
     GenerateInstanceCentroid,
     GenerateInstanceContour,
     GenerateInstanceType,
@@ -484,14 +485,15 @@
         marker_radius: the radius of the disk-shaped footprint used in `opening` of markers. Defaults to 2.
         marker_postprocess_fn: post-process function for watershed markers.
             If not provided, :py:class:`monai.transforms.post.FillHoles()` will be used.
         watershed_connectivity: `connectivity` argument of `skimage.segmentation.watershed`.
         min_num_points: minimum number of points to be considered as a contour. Defaults to 3.
         contour_level: an optional value for `skimage.measure.find_contours` to find contours in the array.
             If not provided, the level is set to `(max(image) + min(image)) / 2`.
+        device: target device to put the output Tensor data.
     """
 
     def __init__(
         self,
         nuclear_prediction_key: str = HoVerNetBranch.NP.value,
         hover_map_key: str = HoVerNetBranch.HV.value,
         instance_info_key: str = "instance_info",
@@ -503,28 +505,30 @@
         distance_smooth_fn: Callable | None = None,
         marker_threshold: float = 0.4,
         marker_radius: int = 2,
         marker_postprocess_fn: Callable | None = None,
         watershed_connectivity: int | None = 1,
         min_num_points: int = 3,
         contour_level: float | None = None,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
         self.instance_map_post_process = HoVerNetInstanceMapPostProcessing(
             activation=activation,
             mask_threshold=mask_threshold,
             min_object_size=min_object_size,
             sobel_kernel_size=sobel_kernel_size,
             distance_smooth_fn=distance_smooth_fn,
             marker_threshold=marker_threshold,
             marker_radius=marker_radius,
             marker_postprocess_fn=marker_postprocess_fn,
             watershed_connectivity=watershed_connectivity,
             min_num_points=min_num_points,
             contour_level=contour_level,
+            device=device,
         )
         self.nuclear_prediction_key = nuclear_prediction_key
         self.hover_map_key = hover_map_key
         self.instance_info_key = instance_info_key
         self.instance_map_key = instance_map_key
 
     def __call__(self, data):
@@ -549,31 +553,32 @@
 
     Args:
         type_prediction_key: the key for HoVerNet NC (type prediction) branch. Defaults to `HoVerNetBranch.NC`.
         instance_info_key: the key where instance information (contour, bounding boxes, and centroids) is stored.
             Defaults to `"instance_info"`.
         instance_map_key: the key where instance map is stored. Defaults to `"instance_map"`.
         type_map_key: the output key where type map is written. Defaults to `"type_map"`.
-
+        device: target device to put the output Tensor data.
 
     """
 
     def __init__(
         self,
         type_prediction_key: str = HoVerNetBranch.NC.value,
         instance_info_key: str = "instance_info",
         instance_map_key: str = "instance_map",
         type_map_key: str = "type_map",
         activation: str | Callable = "softmax",
         threshold: float | None = None,
         return_type_map: bool = True,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
         self.type_post_process = HoVerNetNuclearTypePostProcessing(
-            activation=activation, threshold=threshold, return_type_map=return_type_map
+            activation=activation, threshold=threshold, return_type_map=return_type_map, device=device
         )
         self.type_prediction_key = type_prediction_key
         self.instance_info_key = instance_info_key
         self.instance_map_key = instance_map_key
         self.type_map_key = type_map_key
         self.return_type_map = return_type_map
```

## monai/bundle/__init__.py

```diff
@@ -19,15 +19,17 @@
     ckpt_export,
     download,
     get_all_bundles_list,
     get_bundle_info,
     get_bundle_versions,
     init_bundle,
     load,
+    onnx_export,
     run,
+    run_workflow,
     trt_export,
     verify_metadata,
     verify_net_in_out,
 )
 from .utils import (
     DEFAULT_EXP_MGMT_SETTINGS,
     DEFAULT_MLFLOW_SETTINGS,
```

## monai/bundle/__main__.py

```diff
@@ -7,14 +7,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from monai.bundle.scripts import ckpt_export, download, init_bundle, run, trt_export, verify_metadata, verify_net_in_out
+from monai.bundle.scripts import (
+    ckpt_export,
+    download,
+    init_bundle,
+    onnx_export,
+    run,
+    run_workflow,
+    trt_export,
+    verify_metadata,
+    verify_net_in_out,
+)
 
 if __name__ == "__main__":
     from monai.utils import optional_import
 
     fire, _ = optional_import("fire")
     fire.Fire()
```

## monai/bundle/scripts.py

```diff
@@ -14,44 +14,53 @@
 import ast
 import json
 import os
 import re
 import warnings
 from collections.abc import Mapping, Sequence
 from pathlib import Path
+from pydoc import locate
 from shutil import copyfile
 from textwrap import dedent
 from typing import Any, Callable
 
 import torch
 from torch.cuda import is_available
 
 from monai.apps.mmars.mmars import _get_all_ngc_models
 from monai.apps.utils import _basename, download_url, extractall, get_logger
 from monai.bundle.config_item import ConfigComponent
 from monai.bundle.config_parser import ConfigParser
 from monai.bundle.utils import DEFAULT_INFERENCE, DEFAULT_METADATA
-from monai.bundle.workflows import ConfigWorkflow
+from monai.bundle.workflows import BundleWorkflow, ConfigWorkflow
 from monai.config import IgniteInfo, PathLike
 from monai.data import load_net_with_metadata, save_net_with_metadata
-from monai.networks import convert_to_torchscript, convert_to_trt, copy_model_state, get_state_dict, save_state
+from monai.networks import (
+    convert_to_onnx,
+    convert_to_torchscript,
+    convert_to_trt,
+    copy_model_state,
+    get_state_dict,
+    save_state,
+)
 from monai.utils import (
     check_parent_dir,
     deprecated_arg,
     ensure_tuple,
     get_equivalent_dtype,
     min_version,
     optional_import,
     pprint_edges,
 )
 
 validate, _ = optional_import("jsonschema", name="validate")
 ValidationError, _ = optional_import("jsonschema.exceptions", name="ValidationError")
 Checkpoint, has_ignite = optional_import("ignite.handlers", IgniteInfo.OPT_IMPORT_VERSION, min_version, "Checkpoint")
 requests_get, has_requests = optional_import("requests", name="get")
+onnx, _ = optional_import("onnx")
 
 logger = get_logger(module_name=__name__)
 
 # set BUNDLE_DOWNLOAD_SRC="ngc" to use NGC source in default for bundle download
 download_source = os.environ.get("BUNDLE_DOWNLOAD_SRC", "github")
 PPRINT_CONFIG_N = 5
 
@@ -631,15 +640,15 @@
             if `dict`, treat it as tracking settings.
             will patch the target config content with `tracking handlers` and the top-level items of `configs`.
             for detailed usage examples, plesae check the tutorial:
             https://github.com/Project-MONAI/tutorials/blob/main/experiment_management/bundle_integrate_mlflow.ipynb.
         args_file: a JSON or YAML file to provide default values for `runner_id`, `meta_file`,
             `config_file`, `logging`, and override pairs. so that the command line inputs can be simplified.
         override: id-value pairs to override or add the corresponding config content.
-            e.g. ``--net#input_chns 42``.
+            e.g. ``--net#input_chns 42``, ``--net %/data/other.json#net_arg``.
 
     """
 
     _args = _update_args(
         args=args_file,
         run_id=run_id,
         init_id=init_id,
@@ -674,14 +683,61 @@
         **_args,
     )
     workflow.initialize()
     workflow.run()
     workflow.finalize()
 
 
+def run_workflow(workflow: str | BundleWorkflow | None = None, args_file: str | None = None, **kwargs: Any) -> None:
+    """
+    Specify `bundle workflow` to run monai bundle components and workflows.
+    The workflow should be suclass of `BundleWorkflow` and be available to import.
+    It can be MONAI existing bundle workflows or user customized workflows.
+
+    Typical usage examples:
+
+    .. code-block:: bash
+
+        # Execute this module as a CLI entry with default ConfigWorkflow:
+        python -m monai.bundle run_workflow --meta_file <meta path> --config_file <config path>
+
+        # Set the workflow to other customized BundleWorkflow subclass:
+        python -m monai.bundle run_workflow --workflow CustomizedWorkflow ...
+
+    Args:
+        workflow: specified bundle workflow name, should be a string or class, default to "ConfigWorkflow".
+        args_file: a JSON or YAML file to provide default values for this API.
+            so that the command line inputs can be simplified.
+        kwargs: arguments to instantiate the workflow class.
+
+    """
+
+    _args = _update_args(args=args_file, workflow=workflow, **kwargs)
+    _log_input_summary(tag="run", args=_args)
+    (workflow_name,) = _pop_args(_args, workflow=ConfigWorkflow)  # the default workflow name is "ConfigWorkflow"
+    if isinstance(workflow_name, str):
+        workflow_class, has_built_in = optional_import("monai.bundle", name=str(workflow_name))  # search built-in
+        if not has_built_in:
+            workflow_class = locate(str(workflow_name))  # search dotted path
+        if workflow_class is None:
+            raise ValueError(f"cannot locate specified workflow class: {workflow_name}.")
+    elif issubclass(workflow_name, BundleWorkflow):
+        workflow_class = workflow_name
+    else:
+        raise ValueError(
+            "Argument `workflow` must be a bundle workflow class name"
+            f"or subclass of BundleWorkflow, got: {workflow_name}."
+        )
+
+    workflow_ = workflow_class(**_args)
+    workflow_.initialize()
+    workflow_.run()
+    workflow_.finalize()
+
+
 def verify_metadata(
     meta_file: str | Sequence[str] | None = None,
     filepath: PathLike | None = None,
     create_dir: bool | None = None,
     hash_val: str | None = None,
     hash_type: str | None = None,
     args_file: str | None = None,
@@ -772,14 +828,27 @@
     output_channels = parser.get(key)
     key = f"{prefix_key}#pred#dtype"
     output_dtype = get_equivalent_dtype(parser.get(key), torch.Tensor)
 
     return input_channels, input_spatial_shape, input_dtype, output_channels, output_dtype
 
 
+def _get_fake_input_shape(parser: ConfigParser) -> tuple:
+    """
+    Get a fake input shape e.g. [N, C, H, W] or [N, C, H, W, D], whose batch size is 1, from the given parser.
+
+    Args:
+        parser: a ConfigParser which contains the i/o information of a bundle.
+    """
+    input_channels, input_spatial_shape, _, _, _ = _get_net_io_info(parser=parser)
+    spatial_shape = _get_fake_spatial_shape(input_spatial_shape)
+    input_shape = (1, input_channels, *spatial_shape)
+    return input_shape
+
+
 def verify_net_in_out(
     net_id: str | None = None,
     meta_file: str | Sequence[str] | None = None,
     config_file: str | Sequence[str] | None = None,
     device: str | None = None,
     p: int | None = None,
     n: int | None = None,
@@ -928,24 +997,133 @@
         append_timestamp=False,
         meta_values=parser.get().pop("_meta_", None),
         more_extra_files=extra_files,
     )
     logger.info(f"exported to file: {filepath}.")
 
 
+def onnx_export(
+    net_id: str | None = None,
+    filepath: PathLike | None = None,
+    ckpt_file: str | None = None,
+    meta_file: str | Sequence[str] | None = None,
+    config_file: str | Sequence[str] | None = None,
+    key_in_ckpt: str | None = None,
+    use_trace: bool | None = None,
+    input_shape: Sequence[int] | None = None,
+    args_file: str | None = None,
+    converter_kwargs: Mapping | None = None,
+    **override: Any,
+) -> None:
+    """
+    Export the model checkpoint to an onnx model.
+
+    Typical usage examples:
+
+    .. code-block:: bash
+
+        python -m monai.bundle onnx_export network --filepath <export path> --ckpt_file <checkpoint path> ...
+
+    Args:
+        net_id: ID name of the network component in the config, it must be `torch.nn.Module`.
+        filepath: filepath where the onnx model is saved to.
+        ckpt_file: filepath of the model checkpoint to load.
+        meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
+        config_file: filepath of the config file that contains extract network information,
+        key_in_ckpt: for nested checkpoint like `{"model": XXX, "optimizer": XXX, ...}`, specify the key of model
+            weights. if not nested checkpoint, no need to set.
+        use_trace: whether using `torch.jit.trace` to convert the pytorch model to torchscript model.
+        input_shape: a shape used to generate the random input of the network, when converting the model to an
+            onnx model. Should be a list like [N, C, H, W] or [N, C, H, W, D]. If not given, will try to parse from
+            the `metadata` config.
+        args_file: a JSON or YAML file to provide default values for all the parameters of this function, so that
+            the command line inputs can be simplified.
+        converter_kwargs: extra arguments that are needed by `convert_to_onnx`, except ones that already exist in the
+            input parameters.
+        override: id-value pairs to override or add the corresponding config content.
+            e.g. ``--_meta#network_data_format#inputs#image#num_channels 3``.
+
+    """
+    _args = _update_args(
+        args=args_file,
+        net_id=net_id,
+        filepath=filepath,
+        meta_file=meta_file,
+        config_file=config_file,
+        ckpt_file=ckpt_file,
+        key_in_ckpt=key_in_ckpt,
+        use_trace=use_trace,
+        input_shape=input_shape,
+        converter_kwargs=converter_kwargs,
+        **override,
+    )
+    _log_input_summary(tag="onnx_export", args=_args)
+    (
+        filepath_,
+        ckpt_file_,
+        config_file_,
+        net_id_,
+        meta_file_,
+        key_in_ckpt_,
+        use_trace_,
+        input_shape_,
+        converter_kwargs_,
+    ) = _pop_args(
+        _args,
+        "filepath",
+        "ckpt_file",
+        "config_file",
+        net_id="",
+        meta_file=None,
+        key_in_ckpt="",
+        use_trace=False,
+        input_shape=None,
+        converter_kwargs={},
+    )
+
+    parser = ConfigParser()
+
+    parser.read_config(f=config_file_)
+    if meta_file_ is not None:
+        parser.read_meta(f=meta_file_)
+
+    # the rest key-values in the _args are to override config content
+    for k, v in _args.items():
+        parser[k] = v
+
+    # The convert_to_onnx must have an `inputs` as input, no matter what the `use_trace` is.
+    # If the `input_shape` is not provided, will try to parse it from the parser to generate a random `inputs`.
+    if not input_shape_:
+        input_shape_ = _get_fake_input_shape(parser=parser)
+
+    inputs_ = [torch.rand(input_shape_)]
+    net = parser.get_parsed_content(net_id_)
+    if has_ignite:
+        # here we use ignite Checkpoint to support nested weights and be compatible with MONAI CheckpointSaver
+        Checkpoint.load_objects(to_load={key_in_ckpt_: net}, checkpoint=ckpt_file_)
+    else:
+        ckpt = torch.load(ckpt_file_)
+        copy_model_state(dst=net, src=ckpt if key_in_ckpt_ == "" else ckpt[key_in_ckpt_])
+
+    converter_kwargs_.update({"inputs": inputs_, "use_trace": use_trace_})
+    onnx_model = convert_to_onnx(model=net, **converter_kwargs_)
+    onnx.save(onnx_model, filepath_)
+
+
 def ckpt_export(
     net_id: str | None = None,
     filepath: PathLike | None = None,
     ckpt_file: str | None = None,
     meta_file: str | Sequence[str] | None = None,
     config_file: str | Sequence[str] | None = None,
     key_in_ckpt: str | None = None,
     use_trace: bool | None = None,
     input_shape: Sequence[int] | None = None,
     args_file: str | None = None,
+    converter_kwargs: Mapping | None = None,
     **override: Any,
 ) -> None:
     """
     Export the model checkpoint to the given filepath with metadata and config included as JSON files.
 
     Typical usage examples:
 
@@ -960,70 +1138,90 @@
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
         config_file: filepath of the config file to save in TorchScript model and extract network information,
             the saved key in the TorchScript model is the config filename without extension, and the saved config
             value is always serialized in JSON format no matter the original file format is JSON or YAML.
             it can be a single file or a list of files. if `None`, must be provided in `args_file`.
         key_in_ckpt: for nested checkpoint like `{"model": XXX, "optimizer": XXX, ...}`, specify the key of model
             weights. if not nested checkpoint, no need to set.
-        use_trace: whether using `torch.jit.trace` to convert the pytorch model to torchscript model.
-        input_shape: must specify the `input_shape` of the network to convert the model when `use_trace` is True.
-            Should be a list like [N, C, H, W] or [N, C, H, W, D].
-        args_file: a JSON or YAML file to provide default values for `meta_file`, `config_file`,
-            `net_id` and override pairs. so that the command line inputs can be simplified.
+        use_trace: whether using `torch.jit.trace` to convert the PyTorch model to TorchScript model.
+        input_shape: a shape used to generate the random input of the network, when converting the model to a
+            TorchScript model. Should be a list like [N, C, H, W] or [N, C, H, W, D]. If not given, will try to
+            parse from the `metadata` config.
+        args_file: a JSON or YAML file to provide default values for all the parameters of this function, so that
+            the command line inputs can be simplified.
+        converter_kwargs: extra arguments that are needed by `convert_to_torchscript`, except ones that already exist
+            in the input parameters.
         override: id-value pairs to override or add the corresponding config content.
             e.g. ``--_meta#network_data_format#inputs#image#num_channels 3``.
 
     """
     _args = _update_args(
         args=args_file,
         net_id=net_id,
         filepath=filepath,
         meta_file=meta_file,
         config_file=config_file,
         ckpt_file=ckpt_file,
         key_in_ckpt=key_in_ckpt,
         use_trace=use_trace,
         input_shape=input_shape,
+        converter_kwargs=converter_kwargs,
         **override,
     )
     _log_input_summary(tag="ckpt_export", args=_args)
-    filepath_, ckpt_file_, config_file_, net_id_, meta_file_, key_in_ckpt_, use_trace_, input_shape_ = _pop_args(
+    (
+        filepath_,
+        ckpt_file_,
+        config_file_,
+        net_id_,
+        meta_file_,
+        key_in_ckpt_,
+        use_trace_,
+        input_shape_,
+        converter_kwargs_,
+    ) = _pop_args(
         _args,
         "filepath",
         "ckpt_file",
         "config_file",
         net_id="",
         meta_file=None,
         key_in_ckpt="",
         use_trace=False,
         input_shape=None,
+        converter_kwargs={},
     )
 
     parser = ConfigParser()
 
     parser.read_config(f=config_file_)
     if meta_file_ is not None:
         parser.read_meta(f=meta_file_)
 
     # the rest key-values in the _args are to override config content
     for k, v in _args.items():
         parser[k] = v
 
+    # When export through torch.jit.trace without providing input_shape, will try to parse one from the parser.
+    if (not input_shape_) and use_trace:
+        input_shape_ = _get_fake_input_shape(parser=parser)
+
     inputs_: Sequence[Any] | None = [torch.rand(input_shape_)] if input_shape_ else None
 
+    converter_kwargs_.update({"inputs": inputs_, "use_trace": use_trace_})
+    # Use the given converter to convert a model and save with metadata, config content
     _export(
         convert_to_torchscript,
         parser,
         net_id=net_id_,
         filepath=filepath_,
         ckpt_file=ckpt_file_,
         config_file=config_file_,
         key_in_ckpt=key_in_ckpt_,
-        use_trace=use_trace_,
-        inputs=inputs_,
+        **converter_kwargs_,
     )
 
 
 def trt_export(
     net_id: str | None = None,
     filepath: PathLike | None = None,
     ckpt_file: str | None = None,
@@ -1031,51 +1229,75 @@
     config_file: str | Sequence[str] | None = None,
     key_in_ckpt: str | None = None,
     precision: str | None = None,
     input_shape: Sequence[int] | None = None,
     use_trace: bool | None = None,
     dynamic_batchsize: Sequence[int] | None = None,
     device: int | None = None,
+    use_onnx: bool | None = None,
+    onnx_input_names: Sequence[str] | None = None,
+    onnx_output_names: Sequence[str] | None = None,
     args_file: str | None = None,
+    converter_kwargs: Mapping | None = None,
     **override: Any,
 ) -> None:
     """
-    Export the model checkpoint to the given filepath as a TensorRT engine based torchscript.
-    Currently, this API only supports to convert models whose inputs are all tensors.
+    Export the model checkpoint to the given filepath as a TensorRT engine-based TorchScript.
+    Currently, this API only supports converting models whose inputs are all tensors.
+
+    There are two ways to export a model:
+    1, Torch-TensorRT way: PyTorch module ---> TorchScript module ---> TensorRT engine-based TorchScript.
+    2, ONNX-TensorRT way: PyTorch module ---> TorchScript module ---> ONNX model ---> TensorRT engine --->
+    TensorRT engine-based TorchScript.
+
+    When exporting through the first way, some models suffer from the slowdown problem, since Torch-TensorRT
+    may only convert a little part of the PyTorch model to the TensorRT engine. However when exporting through
+    the second way, some Python data structures like `dict` are not supported. And some TorchScript models are
+    not supported by the ONNX if exported through `torch.jit.script`.
 
     Typical usage examples:
 
     .. code-block:: bash
 
         python -m monai.bundle trt_export --net_id <network definition> --filepath <export path> \
             --ckpt_file <checkpoint path> --input_shape <input shape> --dynamic_batchsize <batch range> ...
 
     Args:
         net_id: ID name of the network component in the config, it must be `torch.nn.Module`.
-        filepath: filepath to export, if filename has no extension it becomes `.ts`.
+        filepath: filepath to export, if filename has no extension, it becomes `.ts`.
         ckpt_file: filepath of the model checkpoint to load.
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
-        config_file: filepath of the config file to save in the TensorRT based torchscript model and extract network
+        config_file: filepath of the config file to save in the TensorRT based TorchScript model and extract network
             information, the saved key in the model is the config filename without extension, and the saved config
             value is always serialized in JSON format no matter the original file format is JSON or YAML.
             it can be a single file or a list of files. if `None`, must be provided in `args_file`.
         key_in_ckpt: for nested checkpoint like `{"model": XXX, "optimizer": XXX, ...}`, specify the key of model
             weights. if not nested checkpoint, no need to set.
-        precision: the weight precision of the converted TensorRT engine based torchscript models. Should be 'fp32' or 'fp16'.
+        precision: the weight precision of the converted TensorRT engine based TorchScript models. Should be 'fp32' or 'fp16'.
         input_shape: the input shape that is used to convert the model. Should be a list like [N, C, H, W] or
-            [N, C, H, W, D].
-        use_trace: whether using `torch.jit.trace` to convert the pytorch model to torchscript model and then convert to
-            a TensorRT engine based torchscript model.
-        dynamic_batchsize: a sequence with three elements to define the batch size range of the input for the model to be converted.
-            Should be a sequence like [MIN_BATCH, OPT_BATCH, MAX_BATCH]. After converted, the batchsize of model input should
-            between `MIN_BATCH` and `MAX_BATCH` and the `OPT_BATCH` is the best peformance batchsize that the TensorRT trys to fit.
-            We suggest the `OPT_BATCH` to be the most frequently used input batchsize in your application.
+            [N, C, H, W, D]. If not given, will try to parse from the `metadata` config.
+        use_trace: whether using `torch.jit.trace` to convert the PyTorch model to a TorchScript model and then convert to
+            a TensorRT engine based TorchScript model or an ONNX model (if `use_onnx` is True).
+        dynamic_batchsize: a sequence with three elements to define the batch size range of the input for the model to be
+            converted. Should be a sequence like [MIN_BATCH, OPT_BATCH, MAX_BATCH]. After converted, the batchsize of
+            model input should between `MIN_BATCH` and `MAX_BATCH` and the `OPT_BATCH` is the best performance batchsize
+            that the TensorRT tries to fit. The `OPT_BATCH` should be the most frequently used input batchsize in
+            the application.
         device: the target GPU index to convert and verify the model.
-        args_file: a JSON or YAML file to provide default values for `meta_file`, `config_file`,
-            `net_id` and override pairs. so that the command line inputs can be simplified.
+        use_onnx: whether using the ONNX-TensorRT way to export the TensorRT engine-based TorchScript model.
+        onnx_input_names: optional input names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `['input_0', 'input_1', ..., 'input_N']` where N equals to the number of the model inputs. If not
+            given, will use `['input_0']`, which supposes the model only has one input.
+        onnx_output_names: optional output names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `['output_0', 'output_1', ..., 'output_N']` where N equals to the number of the model outputs. If
+            not given, will use `['output_0']`, which supposes the model only has one output.
+        args_file: a JSON or YAML file to provide default values for all the parameters of this function, so that
+            the command line inputs can be simplified.
+        converter_kwargs: extra arguments that are needed by `convert_to_trt`, except ones that already exist in the
+            input parameters.
         override: id-value pairs to override or add the corresponding config content.
             e.g. ``--_meta#network_data_format#inputs#image#num_channels 3``.
 
     """
     _args = _update_args(
         args=args_file,
         net_id=net_id,
@@ -1085,14 +1307,18 @@
         ckpt_file=ckpt_file,
         key_in_ckpt=key_in_ckpt,
         precision=precision,
         input_shape=input_shape,
         use_trace=use_trace,
         dynamic_batchsize=dynamic_batchsize,
         device=device,
+        use_onnx=use_onnx,
+        onnx_input_names=onnx_input_names,
+        onnx_output_names=onnx_output_names,
+        converter_kwargs=converter_kwargs,
         **override,
     )
     _log_input_summary(tag="trt_export", args=_args)
     (
         filepath_,
         ckpt_file_,
         config_file_,
@@ -1100,57 +1326,73 @@
         meta_file_,
         key_in_ckpt_,
         precision_,
         input_shape_,
         use_trace_,
         dynamic_batchsize_,
         device_,
+        use_onnx_,
+        onnx_input_names_,
+        onnx_output_names_,
+        converter_kwargs_,
     ) = _pop_args(
         _args,
         "filepath",
         "ckpt_file",
         "config_file",
         net_id="",
         meta_file=None,
         key_in_ckpt="",
         precision="fp32",
         input_shape=[],
         use_trace=False,
         dynamic_batchsize=None,
         device=None,
+        use_onnx=False,
+        onnx_input_names=["input_0"],
+        onnx_output_names=["output_0"],
+        converter_kwargs={},
     )
 
     parser = ConfigParser()
 
     parser.read_config(f=config_file_)
     if meta_file_ is not None:
         parser.read_meta(f=meta_file_)
 
     # the rest key-values in the _args are to override config content
     for k, v in _args.items():
         parser[k] = v
 
+    # The convert_to_trt must have an `input_shape_` as input, no matter what the `use_trace` is.
+    # If the `input_shape` is not provided, will try to parse it from the parser`.
     if not input_shape_:
-        input_channels, input_spatial_shape, _, _, _ = _get_net_io_info(parser=parser)
-        spatial_shape = _get_fake_spatial_shape(input_spatial_shape, p=1, n=1, any=1)
-        input_shape_ = (1, input_channels, *spatial_shape)
+        input_shape_ = _get_fake_input_shape(parser=parser)
+
+    trt_api_parameters = {
+        "precision": precision_,
+        "input_shape": input_shape_,
+        "dynamic_batchsize": dynamic_batchsize_,
+        "use_trace": use_trace_,
+        "device": device_,
+        "use_onnx": use_onnx_,
+        "onnx_input_names": onnx_input_names_,
+        "onnx_output_names": onnx_output_names_,
+    }
+    converter_kwargs_.update(trt_api_parameters)
 
     _export(
         convert_to_trt,
         parser,
         net_id=net_id_,
         filepath=filepath_,
         ckpt_file=ckpt_file_,
         config_file=config_file_,
         key_in_ckpt=key_in_ckpt_,
-        precision=precision_,
-        input_shape=input_shape_,
-        dynamic_batchsize=dynamic_batchsize_,
-        use_trace=use_trace_,
-        device=device_,
+        **converter_kwargs_,
     )
 
 
 def init_bundle(
     bundle_dir: PathLike,
     ckpt_file: PathLike | None = None,
     network: torch.nn.Module | None = None,
```

## monai/bundle/workflows.py

```diff
@@ -161,15 +161,15 @@
             for detailed usage examples, plesae check the tutorial:
             https://github.com/Project-MONAI/tutorials/blob/main/experiment_management/bundle_integrate_mlflow.ipynb.
         workflow: specifies the workflow type: "train" or "training" for a training workflow,
             or "infer", "inference", "eval", "evaluation" for a inference workflow,
             other unsupported string will raise a ValueError.
             default to `None` for common workflow.
         override: id-value pairs to override or add the corresponding config content.
-            e.g. ``--net#input_chns 42``.
+            e.g. ``--net#input_chns 42``, ``--net %/data/other.json#net_arg``
 
     """
 
     def __init__(
         self,
         config_file: str | Sequence[str],
         meta_file: str | Sequence[str] | None = "configs/metadata.json",
```

## monai/data/image_reader.py

```diff
@@ -67,4421 +67,3723 @@
 00000420: 2063 6f72 7265 6374 5f6e 6966 7469 5f68   correct_nifti_h
 00000430: 6561 6465 725f 6966 5f6e 6563 6573 7361  eader_if_necessa
 00000440: 7279 2c0a 2020 2020 6973 5f6e 6f5f 6368  ry,.    is_no_ch
 00000450: 616e 6e65 6c2c 0a20 2020 2069 735f 7375  annel,.    is_su
 00000460: 7070 6f72 7465 645f 666f 726d 6174 2c0a  pported_format,.
 00000470: 2020 2020 6f72 6965 6e74 6174 696f 6e5f      orientation_
 00000480: 7261 735f 6c70 732c 0a29 0a66 726f 6d20  ras_lps,.).from 
-00000490: 6d6f 6e61 692e 7472 616e 7366 6f72 6d73  monai.transforms
-000004a0: 2e75 7469 6c69 7479 2e61 7272 6179 2069  .utility.array i
-000004b0: 6d70 6f72 7420 456e 7375 7265 4368 616e  mport EnsureChan
-000004c0: 6e65 6c46 6972 7374 0a66 726f 6d20 6d6f  nelFirst.from mo
-000004d0: 6e61 692e 7574 696c 7320 696d 706f 7274  nai.utils import
-000004e0: 2028 0a20 2020 204d 6574 614b 6579 732c   (.    MetaKeys,
-000004f0: 0a20 2020 2053 7061 6365 4b65 7973 2c0a  .    SpaceKeys,.
-00000500: 2020 2020 5472 6163 654b 6579 732c 0a20      TraceKeys,. 
-00000510: 2020 2064 6570 7265 6361 7465 642c 0a20     deprecated,. 
-00000520: 2020 2064 6570 7265 6361 7465 645f 6172     deprecated_ar
-00000530: 672c 0a20 2020 2065 6e73 7572 655f 7475  g,.    ensure_tu
-00000540: 706c 652c 0a20 2020 2065 6e73 7572 655f  ple,.    ensure_
-00000550: 7475 706c 655f 7265 702c 0a20 2020 206f  tuple_rep,.    o
-00000560: 7074 696f 6e61 6c5f 696d 706f 7274 2c0a  ptional_import,.
-00000570: 2020 2020 7265 7175 6972 655f 706b 672c      require_pkg,
-00000580: 0a29 0a0a 6966 2054 5950 455f 4348 4543  .)..if TYPE_CHEC
-00000590: 4b49 4e47 3a0a 2020 2020 696d 706f 7274  KING:.    import
-000005a0: 2069 746b 0a20 2020 2069 6d70 6f72 7420   itk.    import 
-000005b0: 6e69 6261 6265 6c20 6173 206e 6962 0a20  nibabel as nib. 
-000005c0: 2020 2069 6d70 6f72 7420 6e72 7264 0a20     import nrrd. 
-000005d0: 2020 2069 6d70 6f72 7420 7079 6469 636f     import pydico
-000005e0: 6d0a 2020 2020 6672 6f6d 206e 6962 6162  m.    from nibab
-000005f0: 656c 2e6e 6966 7469 3120 696d 706f 7274  el.nifti1 import
-00000600: 204e 6966 7469 3149 6d61 6765 0a20 2020   Nifti1Image.   
-00000610: 2066 726f 6d20 5049 4c20 696d 706f 7274   from PIL import
-00000620: 2049 6d61 6765 2061 7320 5049 4c49 6d61   Image as PILIma
-00000630: 6765 0a0a 2020 2020 6861 735f 6e72 7264  ge..    has_nrrd
-00000640: 203d 2068 6173 5f69 746b 203d 2068 6173   = has_itk = has
-00000650: 5f6e 6962 203d 2068 6173 5f70 696c 203d  _nib = has_pil =
-00000660: 2068 6173 5f70 7964 6963 6f6d 203d 2054   has_pydicom = T
-00000670: 7275 650a 656c 7365 3a0a 2020 2020 6974  rue.else:.    it
-00000680: 6b2c 2068 6173 5f69 746b 203d 206f 7074  k, has_itk = opt
-00000690: 696f 6e61 6c5f 696d 706f 7274 2822 6974  ional_import("it
-000006a0: 6b22 2c20 616c 6c6f 775f 6e61 6d65 7370  k", allow_namesp
-000006b0: 6163 655f 706b 673d 5472 7565 290a 2020  ace_pkg=True).  
-000006c0: 2020 6e69 622c 2068 6173 5f6e 6962 203d    nib, has_nib =
-000006d0: 206f 7074 696f 6e61 6c5f 696d 706f 7274   optional_import
-000006e0: 2822 6e69 6261 6265 6c22 290a 2020 2020  ("nibabel").    
-000006f0: 4e69 6674 6931 496d 6167 652c 205f 203d  Nifti1Image, _ =
-00000700: 206f 7074 696f 6e61 6c5f 696d 706f 7274   optional_import
-00000710: 2822 6e69 6261 6265 6c2e 6e69 6674 6931  ("nibabel.nifti1
-00000720: 222c 206e 616d 653d 224e 6966 7469 3149  ", name="Nifti1I
-00000730: 6d61 6765 2229 0a20 2020 2050 494c 496d  mage").    PILIm
-00000740: 6167 652c 2068 6173 5f70 696c 203d 206f  age, has_pil = o
-00000750: 7074 696f 6e61 6c5f 696d 706f 7274 2822  ptional_import("
-00000760: 5049 4c2e 496d 6167 6522 290a 2020 2020  PIL.Image").    
-00000770: 7079 6469 636f 6d2c 2068 6173 5f70 7964  pydicom, has_pyd
-00000780: 6963 6f6d 203d 206f 7074 696f 6e61 6c5f  icom = optional_
-00000790: 696d 706f 7274 2822 7079 6469 636f 6d22  import("pydicom"
-000007a0: 290a 2020 2020 6e72 7264 2c20 6861 735f  ).    nrrd, has_
-000007b0: 6e72 7264 203d 206f 7074 696f 6e61 6c5f  nrrd = optional_
-000007c0: 696d 706f 7274 2822 6e72 7264 222c 2061  import("nrrd", a
-000007d0: 6c6c 6f77 5f6e 616d 6573 7061 6365 5f70  llow_namespace_p
-000007e0: 6b67 3d54 7275 6529 0a0a 4f70 656e 536c  kg=True)..OpenSl
-000007f0: 6964 652c 205f 203d 206f 7074 696f 6e61  ide, _ = optiona
-00000800: 6c5f 696d 706f 7274 2822 6f70 656e 736c  l_import("opensl
-00000810: 6964 6522 2c20 6e61 6d65 3d22 4f70 656e  ide", name="Open
-00000820: 536c 6964 6522 290a 5469 6666 4669 6c65  Slide").TiffFile
-00000830: 2c20 5f20 3d20 6f70 7469 6f6e 616c 5f69  , _ = optional_i
-00000840: 6d70 6f72 7428 2274 6966 6666 696c 6522  mport("tifffile"
-00000850: 2c20 6e61 6d65 3d22 5469 6666 4669 6c65  , name="TiffFile
-00000860: 2229 0a0a 5f5f 616c 6c5f 5f20 3d20 5b0a  ")..__all__ = [.
-00000870: 2020 2020 2249 6d61 6765 5265 6164 6572      "ImageReader
-00000880: 222c 0a20 2020 2022 4954 4b52 6561 6465  ",.    "ITKReade
-00000890: 7222 2c0a 2020 2020 224e 6962 6162 656c  r",.    "Nibabel
-000008a0: 5265 6164 6572 222c 0a20 2020 2022 4e75  Reader",.    "Nu
-000008b0: 6d70 7952 6561 6465 7222 2c0a 2020 2020  mpyReader",.    
-000008c0: 2250 494c 5265 6164 6572 222c 0a20 2020  "PILReader",.   
-000008d0: 2022 5079 6469 636f 6d52 6561 6465 7222   "PydicomReader"
-000008e0: 2c0a 2020 2020 2257 5349 5265 6164 6572  ,.    "WSIReader
-000008f0: 222c 0a20 2020 2022 4e72 7264 5265 6164  ",.    "NrrdRead
-00000900: 6572 222c 0a5d 0a0a 0a63 6c61 7373 2049  er",.]...class I
-00000910: 6d61 6765 5265 6164 6572 2841 4243 293a  mageReader(ABC):
-00000920: 0a20 2020 2022 2222 0a20 2020 2041 6e20  .    """.    An 
-00000930: 6162 7374 7261 6374 2063 6c61 7373 2064  abstract class d
-00000940: 6566 696e 6573 2041 5049 7320 746f 206c  efines APIs to l
-00000950: 6f61 6420 696d 6167 6520 6669 6c65 732e  oad image files.
-00000960: 0a0a 2020 2020 5479 7069 6361 6c20 7573  ..    Typical us
-00000970: 6167 6520 6f66 2061 6e20 696d 706c 656d  age of an implem
-00000980: 656e 7461 7469 6f6e 206f 6620 7468 6973  entation of this
-00000990: 2063 6c61 7373 2069 733a 0a0a 2020 2020   class is:..    
-000009a0: 2e2e 2063 6f64 652d 626c 6f63 6b3a 3a20  .. code-block:: 
-000009b0: 7079 7468 6f6e 0a0a 2020 2020 2020 2020  python..        
-000009c0: 696d 6167 655f 7265 6164 6572 203d 204d  image_reader = M
-000009d0: 7949 6d61 6765 5265 6164 6572 2829 0a20  yImageReader(). 
-000009e0: 2020 2020 2020 2069 6d67 5f6f 626a 203d         img_obj =
-000009f0: 2069 6d61 6765 5f72 6561 6465 722e 7265   image_reader.re
-00000a00: 6164 2870 6174 685f 746f 5f69 6d61 6765  ad(path_to_image
-00000a10: 290a 2020 2020 2020 2020 696d 675f 6461  ).        img_da
-00000a20: 7461 2c20 6d65 7461 5f64 6174 6120 3d20  ta, meta_data = 
-00000a30: 696d 6167 655f 7265 6164 6572 2e67 6574  image_reader.get
-00000a40: 5f64 6174 6128 696d 675f 6f62 6a29 0a0a  _data(img_obj)..
-00000a50: 2020 2020 2d20 5468 6520 6072 6561 6460      - The `read`
-00000a60: 2063 616c 6c20 636f 6e76 6572 7473 2069   call converts i
-00000a70: 6d61 6765 2066 696c 656e 616d 6573 2069  mage filenames i
-00000a80: 6e74 6f20 696d 6167 6520 6f62 6a65 6374  nto image object
-00000a90: 732c 0a20 2020 202d 2054 6865 2060 6765  s,.    - The `ge
-00000aa0: 745f 6461 7461 6020 6361 6c6c 2066 6574  t_data` call fet
-00000ab0: 6368 6573 2074 6865 2069 6d61 6765 2064  ches the image d
-00000ac0: 6174 612c 2061 7320 7765 6c6c 2061 7320  ata, as well as 
-00000ad0: 6d65 7461 6461 7461 2e0a 2020 2020 2d20  metadata..    - 
-00000ae0: 4120 7265 6164 6572 2073 686f 756c 6420  A reader should 
-00000af0: 696d 706c 656d 656e 7420 6076 6572 6966  implement `verif
-00000b00: 795f 7375 6666 6978 6020 7769 7468 2074  y_suffix` with t
-00000b10: 6865 206c 6f67 6963 206f 6620 6368 6563  he logic of chec
-00000b20: 6b69 6e67 2074 6865 2069 6e70 7574 2066  king the input f
-00000b30: 696c 656e 616d 650a 2020 2020 2020 6279  ilename.      by
-00000b40: 2074 6865 2066 696c 656e 616d 6520 6578   the filename ex
-00000b50: 7465 6e73 696f 6e73 2e0a 0a20 2020 2022  tensions...    "
-00000b60: 2222 0a0a 2020 2020 4061 6273 7472 6163  ""..    @abstrac
-00000b70: 746d 6574 686f 640a 2020 2020 6465 6620  tmethod.    def 
-00000b80: 7665 7269 6679 5f73 7566 6669 7828 7365  verify_suffix(se
-00000b90: 6c66 2c20 6669 6c65 6e61 6d65 3a20 5365  lf, filename: Se
-00000ba0: 7175 656e 6365 5b50 6174 684c 696b 655d  quence[PathLike]
-00000bb0: 207c 2050 6174 684c 696b 6529 202d 3e20   | PathLike) -> 
-00000bc0: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00000bd0: 220a 2020 2020 2020 2020 5665 7269 6679  ".        Verify
-00000be0: 2077 6865 7468 6572 2074 6865 2073 7065   whether the spe
-00000bf0: 6369 6669 6564 2060 6669 6c65 6e61 6d65  cified `filename
-00000c00: 6020 6973 2073 7570 706f 7274 6564 2062  ` is supported b
-00000c10: 7920 7468 6520 6375 7272 656e 7420 7265  y the current re
-00000c20: 6164 6572 2e0a 2020 2020 2020 2020 5468  ader..        Th
-00000c30: 6973 206d 6574 686f 6420 7368 6f75 6c64  is method should
-00000c40: 2072 6574 7572 6e20 5472 7565 2069 6620   return True if 
-00000c50: 7468 6520 7265 6164 6572 2069 7320 6162  the reader is ab
-00000c60: 6c65 2074 6f20 7265 6164 2074 6865 2066  le to read the f
-00000c70: 6f72 6d61 7420 7375 6767 6573 7465 6420  ormat suggested 
-00000c80: 6279 2074 6865 0a20 2020 2020 2020 2060  by the.        `
-00000c90: 6669 6c65 6e61 6d65 602e 0a0a 2020 2020  filename`...    
-00000ca0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00000cb0: 2020 2020 2020 6669 6c65 6e61 6d65 3a20        filename: 
-00000cc0: 6669 6c65 206e 616d 6520 6f72 2061 206c  file name or a l
-00000cd0: 6973 7420 6f66 2066 696c 6520 6e61 6d65  ist of file name
-00000ce0: 7320 746f 2072 6561 642e 0a20 2020 2020  s to read..     
-00000cf0: 2020 2020 2020 2020 2020 2069 6620 6120             if a 
-00000d00: 6c69 7374 206f 6620 6669 6c65 732c 2076  list of files, v
-00000d10: 6572 6966 7920 616c 6c20 7468 6520 7375  erify all the su
-00000d20: 6666 6978 6573 2e0a 0a20 2020 2020 2020  ffixes...       
-00000d30: 2022 2222 0a20 2020 2020 2020 2072 6169   """.        rai
-00000d40: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-00000d50: 6445 7272 6f72 2866 2253 7562 636c 6173  dError(f"Subclas
-00000d60: 7320 7b73 656c 662e 5f5f 636c 6173 735f  s {self.__class_
-00000d70: 5f2e 5f5f 6e61 6d65 5f5f 7d20 6d75 7374  _.__name__} must
-00000d80: 2069 6d70 6c65 6d65 6e74 2074 6869 7320   implement this 
-00000d90: 6d65 7468 6f64 2e22 290a 0a20 2020 2040  method.")..    @
-00000da0: 6162 7374 7261 6374 6d65 7468 6f64 0a20  abstractmethod. 
-00000db0: 2020 2064 6566 2072 6561 6428 7365 6c66     def read(self
-00000dc0: 2c20 6461 7461 3a20 5365 7175 656e 6365  , data: Sequence
-00000dd0: 5b50 6174 684c 696b 655d 207c 2050 6174  [PathLike] | Pat
-00000de0: 684c 696b 652c 202a 2a6b 7761 7267 7329  hLike, **kwargs)
-00000df0: 202d 3e20 5365 7175 656e 6365 5b41 6e79   -> Sequence[Any
-00000e00: 5d20 7c20 416e 793a 0a20 2020 2020 2020  ] | Any:.       
-00000e10: 2022 2222 0a20 2020 2020 2020 2052 6561   """.        Rea
-00000e20: 6420 696d 6167 6520 6461 7461 2066 726f  d image data fro
-00000e30: 6d20 7370 6563 6966 6965 6420 6669 6c65  m specified file
-00000e40: 206f 7220 6669 6c65 732e 0a20 2020 2020   or files..     
-00000e50: 2020 204e 6f74 6520 7468 6174 2069 7420     Note that it 
-00000e60: 7265 7475 726e 7320 6120 6461 7461 206f  returns a data o
-00000e70: 626a 6563 7420 6f72 2061 2073 6571 7565  bject or a seque
-00000e80: 6e63 6520 6f66 2064 6174 6120 6f62 6a65  nce of data obje
-00000e90: 6374 732e 0a0a 2020 2020 2020 2020 4172  cts...        Ar
-00000ea0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00000eb0: 6461 7461 3a20 6669 6c65 206e 616d 6520  data: file name 
-00000ec0: 6f72 2061 206c 6973 7420 6f66 2066 696c  or a list of fil
-00000ed0: 6520 6e61 6d65 7320 746f 2072 6561 642e  e names to read.
-00000ee0: 0a20 2020 2020 2020 2020 2020 206b 7761  .            kwa
-00000ef0: 7267 733a 2061 6464 6974 696f 6e61 6c20  rgs: additional 
-00000f00: 6172 6773 2066 6f72 2061 6374 7561 6c20  args for actual 
-00000f10: 6072 6561 6460 2041 5049 206f 6620 3372  `read` API of 3r
-00000f20: 6420 7061 7274 7920 6c69 6273 2e0a 0a20  d party libs... 
-00000f30: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00000f40: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
-00000f50: 656d 656e 7465 6445 7272 6f72 2866 2253  ementedError(f"S
-00000f60: 7562 636c 6173 7320 7b73 656c 662e 5f5f  ubclass {self.__
-00000f70: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-00000f80: 7d20 6d75 7374 2069 6d70 6c65 6d65 6e74  } must implement
-00000f90: 2074 6869 7320 6d65 7468 6f64 2e22 290a   this method.").
-00000fa0: 0a20 2020 2040 6162 7374 7261 6374 6d65  .    @abstractme
-00000fb0: 7468 6f64 0a20 2020 2064 6566 2067 6574  thod.    def get
-00000fc0: 5f64 6174 6128 7365 6c66 2c20 696d 6729  _data(self, img)
-00000fd0: 202d 3e20 7475 706c 655b 6e70 2e6e 6461   -> tuple[np.nda
-00000fe0: 7272 6179 2c20 6469 6374 5d3a 0a20 2020  rray, dict]:.   
-00000ff0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00001000: 2045 7874 7261 6374 2064 6174 6120 6172   Extract data ar
-00001010: 7261 7920 616e 6420 6d65 7461 6461 7461  ray and metadata
-00001020: 2066 726f 6d20 6c6f 6164 6564 2069 6d61   from loaded ima
-00001030: 6765 2061 6e64 2072 6574 7572 6e20 7468  ge and return th
-00001040: 656d 2e0a 2020 2020 2020 2020 5468 6973  em..        This
-00001050: 2066 756e 6374 696f 6e20 6d75 7374 2072   function must r
-00001060: 6574 7572 6e20 7477 6f20 6f62 6a65 6374  eturn two object
-00001070: 732c 2074 6865 2066 6972 7374 2069 7320  s, the first is 
-00001080: 6120 6e75 6d70 7920 6172 7261 7920 6f66  a numpy array of
-00001090: 2069 6d61 6765 2064 6174 612c 0a20 2020   image data,.   
-000010a0: 2020 2020 2074 6865 2073 6563 6f6e 6420       the second 
-000010b0: 6973 2061 2064 6963 7469 6f6e 6172 7920  is a dictionary 
-000010c0: 6f66 206d 6574 6164 6174 612e 0a0a 2020  of metadata...  
-000010d0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-000010e0: 2020 2020 2020 2020 696d 673a 2061 6e20          img: an 
-000010f0: 696d 6167 6520 6f62 6a65 6374 206c 6f61  image object loa
-00001100: 6465 6420 6672 6f6d 2061 6e20 696d 6167  ded from an imag
-00001110: 6520 6669 6c65 206f 7220 6120 6c69 7374  e file or a list
-00001120: 206f 6620 696d 6167 6520 6f62 6a65 6374   of image object
-00001130: 732e 0a0a 2020 2020 2020 2020 2222 220a  s...        """.
-00001140: 2020 2020 2020 2020 7261 6973 6520 4e6f          raise No
-00001150: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-00001160: 7228 6622 5375 6263 6c61 7373 207b 7365  r(f"Subclass {se
-00001170: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
-00001180: 616d 655f 5f7d 206d 7573 7420 696d 706c  ame__} must impl
-00001190: 656d 656e 7420 7468 6973 206d 6574 686f  ement this metho
-000011a0: 642e 2229 0a0a 0a64 6566 205f 636f 7079  d.")...def _copy
-000011b0: 5f63 6f6d 7061 7469 626c 655f 6469 6374  _compatible_dict
-000011c0: 2866 726f 6d5f 6469 6374 3a20 6469 6374  (from_dict: dict
-000011d0: 2c20 746f 5f64 6963 743a 2064 6963 7429  , to_dict: dict)
-000011e0: 3a0a 2020 2020 6966 206e 6f74 2069 7369  :.    if not isi
-000011f0: 6e73 7461 6e63 6528 746f 5f64 6963 742c  nstance(to_dict,
-00001200: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
-00001210: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00001220: 2866 2274 6f5f 6469 6374 206d 7573 7420  (f"to_dict must 
-00001230: 6265 2061 2044 6963 742c 2067 6f74 207b  be a Dict, got {
-00001240: 7479 7065 2874 6f5f 6469 6374 297d 2e22  type(to_dict)}."
-00001250: 290a 2020 2020 6966 206e 6f74 2074 6f5f  ).    if not to_
-00001260: 6469 6374 3a0a 2020 2020 2020 2020 666f  dict:.        fo
-00001270: 7220 6b65 7920 696e 2066 726f 6d5f 6469  r key in from_di
-00001280: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
-00001290: 6461 7475 6d20 3d20 6672 6f6d 5f64 6963  datum = from_dic
-000012a0: 745b 6b65 795d 0a20 2020 2020 2020 2020  t[key].         
-000012b0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-000012c0: 2864 6174 756d 2c20 6e70 2e6e 6461 7272  (datum, np.ndarr
-000012d0: 6179 2920 616e 6420 6e70 5f73 7472 5f6f  ay) and np_str_o
-000012e0: 626a 5f61 7272 6179 5f70 6174 7465 726e  bj_array_pattern
-000012f0: 2e73 6561 7263 6828 6461 7475 6d2e 6474  .search(datum.dt
-00001300: 7970 652e 7374 7229 2069 7320 6e6f 7420  ype.str) is not 
-00001310: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00001320: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-00001330: 2020 2020 2020 2020 2020 2074 6f5f 6469             to_di
-00001340: 6374 5b6b 6579 5d20 3d20 7374 7228 5472  ct[key] = str(Tr
-00001350: 6163 654b 6579 732e 4e4f 4e45 2920 6966  aceKeys.NONE) if
-00001360: 2064 6174 756d 2069 7320 4e6f 6e65 2065   datum is None e
-00001370: 6c73 6520 6461 7475 6d20 2023 204e 6f6e  lse datum  # Non
-00001380: 6554 7970 6520 746f 2073 7472 696e 6720  eType to string 
-00001390: 666f 7220 6465 6661 756c 745f 636f 6c6c  for default_coll
-000013a0: 6174 650a 2020 2020 656c 7365 3a0a 2020  ate.    else:.  
-000013b0: 2020 2020 2020 6166 6669 6e65 5f6b 6579        affine_key
-000013c0: 2c20 7368 6170 655f 6b65 7920 3d20 4d65  , shape_key = Me
-000013d0: 7461 4b65 7973 2e41 4646 494e 452c 204d  taKeys.AFFINE, M
-000013e0: 6574 614b 6579 732e 5350 4154 4941 4c5f  etaKeys.SPATIAL_
-000013f0: 5348 4150 450a 2020 2020 2020 2020 6966  SHAPE.        if
-00001400: 2061 6666 696e 655f 6b65 7920 696e 2066   affine_key in f
-00001410: 726f 6d5f 6469 6374 2061 6e64 206e 6f74  rom_dict and not
-00001420: 206e 702e 616c 6c63 6c6f 7365 2866 726f   np.allclose(fro
-00001430: 6d5f 6469 6374 5b61 6666 696e 655f 6b65  m_dict[affine_ke
-00001440: 795d 2c20 746f 5f64 6963 745b 6166 6669  y], to_dict[affi
-00001450: 6e65 5f6b 6579 5d29 3a0a 2020 2020 2020  ne_key]):.      
-00001460: 2020 2020 2020 7261 6973 6520 5275 6e74        raise Runt
-00001470: 696d 6545 7272 6f72 280a 2020 2020 2020  imeError(.      
-00001480: 2020 2020 2020 2020 2020 2261 6666 696e            "affin
-00001490: 6520 6d61 7472 6978 206f 6620 616c 6c20  e matrix of all 
-000014a0: 696d 6167 6573 2073 686f 756c 6420 6265  images should be
-000014b0: 2074 6865 2073 616d 6520 666f 7220 6368   the same for ch
-000014c0: 616e 6e65 6c2d 7769 7365 2063 6f6e 6361  annel-wise conca
-000014d0: 7465 6e61 7469 6f6e 2e20 220a 2020 2020  tenation. ".    
-000014e0: 2020 2020 2020 2020 2020 2020 6622 476f              f"Go
-000014f0: 7420 7b66 726f 6d5f 6469 6374 5b61 6666  t {from_dict[aff
-00001500: 696e 655f 6b65 795d 7d20 616e 6420 7b74  ine_key]} and {t
-00001510: 6f5f 6469 6374 5b61 6666 696e 655f 6b65  o_dict[affine_ke
-00001520: 795d 7d2e 220a 2020 2020 2020 2020 2020  y]}.".          
-00001530: 2020 290a 2020 2020 2020 2020 6966 2073    ).        if s
-00001540: 6861 7065 5f6b 6579 2069 6e20 6672 6f6d  hape_key in from
-00001550: 5f64 6963 7420 616e 6420 6e6f 7420 6e70  _dict and not np
-00001560: 2e61 6c6c 636c 6f73 6528 6672 6f6d 5f64  .allclose(from_d
-00001570: 6963 745b 7368 6170 655f 6b65 795d 2c20  ict[shape_key], 
-00001580: 746f 5f64 6963 745b 7368 6170 655f 6b65  to_dict[shape_ke
-00001590: 795d 293a 0a20 2020 2020 2020 2020 2020  y]):.           
-000015a0: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
-000015b0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-000015c0: 2020 2020 2022 7370 6174 6961 6c5f 7368       "spatial_sh
-000015d0: 6170 6520 6f66 2061 6c6c 2069 6d61 6765  ape of all image
-000015e0: 7320 7368 6f75 6c64 2062 6520 7468 6520  s should be the 
-000015f0: 7361 6d65 2066 6f72 2063 6861 6e6e 656c  same for channel
-00001600: 2d77 6973 6520 636f 6e63 6174 656e 6174  -wise concatenat
-00001610: 696f 6e2e 2022 0a20 2020 2020 2020 2020  ion. ".         
-00001620: 2020 2020 2020 2066 2247 6f74 207b 6672         f"Got {fr
-00001630: 6f6d 5f64 6963 745b 7368 6170 655f 6b65  om_dict[shape_ke
-00001640: 795d 7d20 616e 6420 7b74 6f5f 6469 6374  y]} and {to_dict
-00001650: 5b73 6861 7065 5f6b 6579 5d7d 2e22 0a20  [shape_key]}.". 
-00001660: 2020 2020 2020 2020 2020 2029 0a0a 0a64             )...d
-00001670: 6566 205f 7374 6163 6b5f 696d 6167 6573  ef _stack_images
-00001680: 2869 6d61 6765 5f6c 6973 743a 206c 6973  (image_list: lis
-00001690: 742c 206d 6574 615f 6469 6374 3a20 6469  t, meta_dict: di
-000016a0: 6374 293a 0a20 2020 2069 6620 6c65 6e28  ct):.    if len(
-000016b0: 696d 6167 655f 6c69 7374 2920 3c3d 2031  image_list) <= 1
-000016c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000016d0: 2069 6d61 6765 5f6c 6973 745b 305d 0a20   image_list[0]. 
-000016e0: 2020 2069 6620 6e6f 7420 6973 5f6e 6f5f     if not is_no_
-000016f0: 6368 616e 6e65 6c28 6d65 7461 5f64 6963  channel(meta_dic
-00001700: 742e 6765 7428 4d65 7461 4b65 7973 2e4f  t.get(MetaKeys.O
-00001710: 5249 4749 4e41 4c5f 4348 414e 4e45 4c5f  RIGINAL_CHANNEL_
-00001720: 4449 4d2c 204e 6f6e 6529 293a 0a20 2020  DIM, None)):.   
-00001730: 2020 2020 2063 6861 6e6e 656c 5f64 696d       channel_dim
-00001740: 203d 2069 6e74 286d 6574 615f 6469 6374   = int(meta_dict
-00001750: 5b4d 6574 614b 6579 732e 4f52 4947 494e  [MetaKeys.ORIGIN
-00001760: 414c 5f43 4841 4e4e 454c 5f44 494d 5d29  AL_CHANNEL_DIM])
-00001770: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001780: 6e70 2e63 6f6e 6361 7465 6e61 7465 2869  np.concatenate(i
-00001790: 6d61 6765 5f6c 6973 742c 2061 7869 733d  mage_list, axis=
-000017a0: 6368 616e 6e65 6c5f 6469 6d29 0a20 2020  channel_dim).   
-000017b0: 2023 2073 7461 636b 2061 7420 6120 6e65   # stack at a ne
-000017c0: 7720 6669 7273 7420 6469 6d20 6173 2074  w first dim as t
-000017d0: 6865 2063 6861 6e6e 656c 2064 696d 2c20  he channel dim, 
-000017e0: 6966 2060 276f 7269 6769 6e61 6c5f 6368  if `'original_ch
-000017f0: 616e 6e65 6c5f 6469 6d27 6020 6973 2075  annel_dim'` is u
-00001800: 6e73 7065 6369 6669 6564 0a20 2020 206d  nspecified.    m
-00001810: 6574 615f 6469 6374 5b4d 6574 614b 6579  eta_dict[MetaKey
-00001820: 732e 4f52 4947 494e 414c 5f43 4841 4e4e  s.ORIGINAL_CHANN
-00001830: 454c 5f44 494d 5d20 3d20 300a 2020 2020  EL_DIM] = 0.    
-00001840: 7265 7475 726e 206e 702e 7374 6163 6b28  return np.stack(
-00001850: 696d 6167 655f 6c69 7374 2c20 6178 6973  image_list, axis
-00001860: 3d30 290a 0a0a 4072 6571 7569 7265 5f70  =0)...@require_p
-00001870: 6b67 2870 6b67 5f6e 616d 653d 2269 746b  kg(pkg_name="itk
-00001880: 2229 0a63 6c61 7373 2049 544b 5265 6164  ").class ITKRead
-00001890: 6572 2849 6d61 6765 5265 6164 6572 293a  er(ImageReader):
-000018a0: 0a20 2020 2022 2222 0a20 2020 204c 6f61  .    """.    Loa
-000018b0: 6420 6d65 6469 6361 6c20 696d 6167 6573  d medical images
-000018c0: 2062 6173 6564 206f 6e20 4954 4b20 6c69   based on ITK li
-000018d0: 6272 6172 792e 0a20 2020 2041 6c6c 2074  brary..    All t
-000018e0: 6865 2073 7570 706f 7274 6564 2069 6d61  he supported ima
-000018f0: 6765 2066 6f72 6d61 7473 2063 616e 2062  ge formats can b
-00001900: 6520 666f 756e 6420 6174 3a0a 2020 2020  e found at:.    
-00001910: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001920: 6f6d 2f49 6e73 6967 6874 536f 6674 7761  om/InsightSoftwa
-00001930: 7265 436f 6e73 6f72 7469 756d 2f49 544b  reConsortium/ITK
-00001940: 2f74 7265 652f 6d61 7374 6572 2f4d 6f64  /tree/master/Mod
-00001950: 756c 6573 2f49 4f0a 2020 2020 5468 6520  ules/IO.    The 
-00001960: 6c6f 6164 6564 2064 6174 6120 6172 7261  loaded data arra
-00001970: 7920 7769 6c6c 2062 6520 696e 2043 206f  y will be in C o
-00001980: 7264 6572 2c20 666f 7220 6578 616d 706c  rder, for exampl
-00001990: 652c 2061 2033 4420 696d 6167 6520 4e75  e, a 3D image Nu
-000019a0: 6d50 790a 2020 2020 6172 7261 7920 696e  mPy.    array in
-000019b0: 6465 7820 6f72 6465 7220 7769 6c6c 2062  dex order will b
-000019c0: 6520 6043 4457 4860 2e0a 0a20 2020 2041  e `CDWH`...    A
-000019d0: 7267 733a 0a20 2020 2020 2020 2063 6861  rgs:.        cha
-000019e0: 6e6e 656c 5f64 696d 3a20 7468 6520 6368  nnel_dim: the ch
-000019f0: 616e 6e65 6c20 6469 6d65 6e73 696f 6e20  annel dimension 
-00001a00: 6f66 2074 6865 2069 6e70 7574 2069 6d61  of the input ima
-00001a10: 6765 2c20 6465 6661 756c 7420 6973 204e  ge, default is N
-00001a20: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-00001a30: 2054 6869 7320 6973 2075 7365 6420 746f   This is used to
-00001a40: 2073 6574 206f 7269 6769 6e61 6c5f 6368   set original_ch
-00001a50: 616e 6e65 6c5f 6469 6d20 696e 2074 6865  annel_dim in the
-00001a60: 206d 6574 6164 6174 612c 2045 6e73 7572   metadata, Ensur
-00001a70: 6543 6861 6e6e 656c 4669 7273 7444 2072  eChannelFirstD r
-00001a80: 6561 6473 2074 6869 7320 6669 656c 642e  eads this field.
-00001a90: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-00001aa0: 4e6f 6e65 2c20 606f 7269 6769 6e61 6c5f  None, `original_
-00001ab0: 6368 616e 6e65 6c5f 6469 6d60 2077 696c  channel_dim` wil
-00001ac0: 6c20 6265 2065 6974 6865 7220 606e 6f5f  l be either `no_
-00001ad0: 6368 616e 6e65 6c60 206f 7220 602d 3160  channel` or `-1`
-00001ae0: 2e0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-00001af0: 2020 202d 204e 6966 7469 2066 696c 6520     - Nifti file 
-00001b00: 6973 2075 7375 616c 6c79 2022 6368 616e  is usually "chan
-00001b10: 6e65 6c20 6c61 7374 222c 2073 6f20 7468  nel last", so th
-00001b20: 6572 6520 6973 206e 6f20 6e65 6564 2074  ere is no need t
-00001b30: 6f20 7370 6563 6966 7920 7468 6973 2061  o specify this a
-00001b40: 7267 756d 656e 742e 0a20 2020 2020 2020  rgument..       
-00001b50: 2020 2020 2020 2020 202d 2050 4e47 2066           - PNG f
-00001b60: 696c 6520 7573 7561 6c6c 7920 6861 7320  ile usually has 
-00001b70: 6047 6574 4e75 6d62 6572 4f66 436f 6d70  `GetNumberOfComp
-00001b80: 6f6e 656e 7473 5065 7250 6978 656c 2829  onentsPerPixel()
-00001b90: 3d3d 3360 2c20 736f 2074 6865 7265 2069  ==3`, so there i
-00001ba0: 7320 6e6f 206e 6565 6420 746f 2073 7065  s no need to spe
-00001bb0: 6369 6679 2074 6869 7320 6172 6775 6d65  cify this argume
-00001bc0: 6e74 2e0a 0a20 2020 2020 2020 2073 6572  nt...        ser
-00001bd0: 6965 735f 6e61 6d65 3a20 7468 6520 6e61  ies_name: the na
-00001be0: 6d65 206f 6620 7468 6520 4449 434f 4d20  me of the DICOM 
-00001bf0: 7365 7269 6573 2069 6620 7468 6572 6520  series if there 
-00001c00: 6172 6520 6d75 6c74 6970 6c65 206f 6e65  are multiple one
-00001c10: 732e 0a20 2020 2020 2020 2020 2020 2075  s..            u
-00001c20: 7365 6420 7768 656e 206c 6f61 6469 6e67  sed when loading
-00001c30: 2044 4943 4f4d 2073 6572 6965 732e 0a20   DICOM series.. 
-00001c40: 2020 2020 2020 2072 6576 6572 7365 5f69         reverse_i
-00001c50: 6e64 6578 696e 673a 2077 6865 7468 6572  ndexing: whether
-00001c60: 2074 6f20 7573 6520 6120 7265 7665 7273   to use a revers
-00001c70: 6564 2073 7061 7469 616c 2069 6e64 6578  ed spatial index
-00001c80: 696e 6720 636f 6e76 656e 7469 6f6e 2066  ing convention f
-00001c90: 6f72 2074 6865 2072 6574 7572 6e65 6420  or the returned 
-00001ca0: 6461 7461 2061 7272 6179 2e0a 2020 2020  data array..    
-00001cb0: 2020 2020 2020 2020 4966 2060 6046 616c          If ``Fal
-00001cc0: 7365 6060 2c20 7468 6520 7370 6174 6961  se``, the spatia
-00001cd0: 6c20 696e 6465 7869 6e67 2066 6f6c 6c6f  l indexing follo
-00001ce0: 7773 2074 6865 206e 756d 7079 2063 6f6e  ws the numpy con
-00001cf0: 7665 6e74 696f 6e3b 0a20 2020 2020 2020  vention;.       
-00001d00: 2020 2020 206f 7468 6572 7769 7365 2c20       otherwise, 
-00001d10: 7468 6520 7370 6174 6961 6c20 696e 6465  the spatial inde
-00001d20: 7869 6e67 2063 6f6e 7665 6e74 696f 6e20  xing convention 
-00001d30: 6973 2072 6576 6572 7365 6420 746f 2062  is reversed to b
-00001d40: 6520 636f 6d70 6174 6962 6c65 2077 6974  e compatible wit
-00001d50: 6820 4954 4b2e 2044 6566 6175 6c74 2069  h ITK. Default i
-00001d60: 7320 6060 4661 6c73 6560 602e 0a20 2020  s ``False``..   
-00001d70: 2020 2020 2020 2020 2054 6869 7320 6f70           This op
-00001d80: 7469 6f6e 2064 6f65 7320 6e6f 7420 6166  tion does not af
-00001d90: 6665 6374 2074 6865 206d 6574 6164 6174  fect the metadat
-00001da0: 612e 0a20 2020 2020 2020 2073 6572 6965  a..        serie
-00001db0: 735f 6d65 7461 3a20 7768 6574 6865 7220  s_meta: whether 
-00001dc0: 746f 206c 6f61 6420 7468 6520 6d65 7461  to load the meta
-00001dd0: 6461 7461 206f 6620 7468 6520 4449 434f  data of the DICO
-00001de0: 4d20 7365 7269 6573 2028 7573 696e 6720  M series (using 
-00001df0: 7468 6520 6d65 7461 6461 7461 2066 726f  the metadata fro
-00001e00: 6d20 7468 6520 6669 7273 7420 736c 6963  m the first slic
-00001e10: 6529 2e0a 2020 2020 2020 2020 2020 2020  e)..            
-00001e20: 5468 6973 2066 6c61 6720 6973 2063 6865  This flag is che
-00001e30: 636b 6564 206f 6e6c 7920 7768 656e 206c  cked only when l
-00001e40: 6f61 6469 6e67 2044 4943 4f4d 2073 6572  oading DICOM ser
-00001e50: 6965 732e 2044 6566 6175 6c74 2069 7320  ies. Default is 
-00001e60: 6060 4661 6c73 6560 602e 0a20 2020 2020  ``False``..     
-00001e70: 2020 2061 6666 696e 655f 6c70 735f 746f     affine_lps_to
-00001e80: 5f72 6173 3a20 7768 6574 6865 7220 746f  _ras: whether to
-00001e90: 2063 6f6e 7665 7274 2074 6865 2061 6666   convert the aff
-00001ea0: 696e 6520 6d61 7472 6978 2066 726f 6d20  ine matrix from 
-00001eb0: 224c 5053 2220 746f 2022 5241 5322 2e20  "LPS" to "RAS". 
-00001ec0: 4465 6661 756c 7473 2074 6f20 6060 5472  Defaults to ``Tr
-00001ed0: 7565 6060 2e0a 2020 2020 2020 2020 2020  ue``..          
-00001ee0: 2020 5365 7420 746f 2060 6054 7275 6560    Set to ``True`
-00001ef0: 6020 746f 2062 6520 636f 6e73 6973 7465  ` to be consiste
-00001f00: 6e74 2077 6974 6820 6060 4e69 6261 6265  nt with ``Nibabe
-00001f10: 6c52 6561 6465 7260 602c 206f 7468 6572  lReader``, other
-00001f20: 7769 7365 2074 6865 2061 6666 696e 6520  wise the affine 
-00001f30: 6d61 7472 6978 2072 656d 6169 6e73 2069  matrix remains i
-00001f40: 6e20 7468 6520 4954 4b20 636f 6e76 656e  n the ITK conven
-00001f50: 7469 6f6e 2e0a 2020 2020 2020 2020 6b77  tion..        kw
-00001f60: 6172 6773 3a20 6164 6469 7469 6f6e 616c  args: additional
-00001f70: 2061 7267 7320 666f 7220 6069 746b 2e69   args for `itk.i
-00001f80: 6d72 6561 6460 2041 5049 2e20 6d6f 7265  mread` API. more
-00001f90: 2064 6574 6169 6c73 2061 626f 7574 2061   details about a
-00001fa0: 7661 696c 6162 6c65 2061 7267 733a 0a20  vailable args:. 
-00001fb0: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00001fc0: 3a2f 2f67 6974 6875 622e 636f 6d2f 496e  ://github.com/In
-00001fd0: 7369 6768 7453 6f66 7477 6172 6543 6f6e  sightSoftwareCon
-00001fe0: 736f 7274 6975 6d2f 4954 4b2f 626c 6f62  sortium/ITK/blob
-00001ff0: 2f6d 6173 7465 722f 5772 6170 7069 6e67  /master/Wrapping
-00002000: 2f47 656e 6572 6174 6f72 732f 5079 7468  /Generators/Pyth
-00002010: 6f6e 2f69 746b 2f73 7570 706f 7274 2f65  on/itk/support/e
-00002020: 7874 7261 732e 7079 0a0a 2020 2020 2222  xtras.py..    ""
-00002030: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-00002040: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-00002050: 662c 0a20 2020 2020 2020 2063 6861 6e6e  f,.        chann
-00002060: 656c 5f64 696d 3a20 7374 7220 7c20 696e  el_dim: str | in
-00002070: 7420 7c20 4e6f 6e65 203d 204e 6f6e 652c  t | None = None,
-00002080: 0a20 2020 2020 2020 2073 6572 6965 735f  .        series_
-00002090: 6e61 6d65 3a20 7374 7220 3d20 2222 2c0a  name: str = "",.
-000020a0: 2020 2020 2020 2020 7265 7665 7273 655f          reverse_
-000020b0: 696e 6465 7869 6e67 3a20 626f 6f6c 203d  indexing: bool =
-000020c0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-000020d0: 7365 7269 6573 5f6d 6574 613a 2062 6f6f  series_meta: boo
-000020e0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-000020f0: 2020 2061 6666 696e 655f 6c70 735f 746f     affine_lps_to
-00002100: 5f72 6173 3a20 626f 6f6c 203d 2054 7275  _ras: bool = Tru
-00002110: 652c 0a20 2020 2020 2020 202a 2a6b 7761  e,.        **kwa
-00002120: 7267 732c 0a20 2020 2029 3a0a 2020 2020  rgs,.    ):.    
-00002130: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00002140: 6974 5f5f 2829 0a20 2020 2020 2020 2073  it__().        s
-00002150: 656c 662e 6b77 6172 6773 203d 206b 7761  elf.kwargs = kwa
-00002160: 7267 730a 2020 2020 2020 2020 7365 6c66  rgs.        self
-00002170: 2e63 6861 6e6e 656c 5f64 696d 203d 2066  .channel_dim = f
-00002180: 6c6f 6174 2822 6e61 6e22 2920 6966 2063  loat("nan") if c
-00002190: 6861 6e6e 656c 5f64 696d 203d 3d20 226e  hannel_dim == "n
-000021a0: 6f5f 6368 616e 6e65 6c22 2065 6c73 6520  o_channel" else 
-000021b0: 6368 616e 6e65 6c5f 6469 6d0a 2020 2020  channel_dim.    
-000021c0: 2020 2020 7365 6c66 2e73 6572 6965 735f      self.series_
-000021d0: 6e61 6d65 203d 2073 6572 6965 735f 6e61  name = series_na
-000021e0: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
-000021f0: 7265 7665 7273 655f 696e 6465 7869 6e67  reverse_indexing
-00002200: 203d 2072 6576 6572 7365 5f69 6e64 6578   = reverse_index
-00002210: 696e 670a 2020 2020 2020 2020 7365 6c66  ing.        self
-00002220: 2e73 6572 6965 735f 6d65 7461 203d 2073  .series_meta = s
-00002230: 6572 6965 735f 6d65 7461 0a20 2020 2020  eries_meta.     
-00002240: 2020 2073 656c 662e 6166 6669 6e65 5f6c     self.affine_l
-00002250: 7073 5f74 6f5f 7261 7320 3d20 6166 6669  ps_to_ras = affi
-00002260: 6e65 5f6c 7073 5f74 6f5f 7261 730a 0a20  ne_lps_to_ras.. 
-00002270: 2020 2064 6566 2076 6572 6966 795f 7375     def verify_su
-00002280: 6666 6978 2873 656c 662c 2066 696c 656e  ffix(self, filen
-00002290: 616d 653a 2053 6571 7565 6e63 655b 5061  ame: Sequence[Pa
-000022a0: 7468 4c69 6b65 5d20 7c20 5061 7468 4c69  thLike] | PathLi
-000022b0: 6b65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ke) -> bool:.   
-000022c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000022d0: 2056 6572 6966 7920 7768 6574 6865 7220   Verify whether 
-000022e0: 7468 6520 7370 6563 6966 6965 6420 6669  the specified fi
-000022f0: 6c65 206f 7220 6669 6c65 7320 666f 726d  le or files form
-00002300: 6174 2069 7320 7375 7070 6f72 7465 6420  at is supported 
-00002310: 6279 2049 544b 2072 6561 6465 722e 0a0a  by ITK reader...
-00002320: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00002330: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
-00002340: 6d65 3a20 6669 6c65 206e 616d 6520 6f72  me: file name or
-00002350: 2061 206c 6973 7420 6f66 2066 696c 6520   a list of file 
-00002360: 6e61 6d65 7320 746f 2072 6561 642e 0a20  names to read.. 
-00002370: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00002380: 6620 6120 6c69 7374 206f 6620 6669 6c65  f a list of file
-00002390: 732c 2076 6572 6966 7920 616c 6c20 7468  s, verify all th
-000023a0: 6520 7375 6666 6978 6573 2e0a 0a20 2020  e suffixes...   
-000023b0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000023c0: 2072 6574 7572 6e20 6861 735f 6974 6b0a   return has_itk.
-000023d0: 0a20 2020 2064 6566 2072 6561 6428 7365  .    def read(se
-000023e0: 6c66 2c20 6461 7461 3a20 5365 7175 656e  lf, data: Sequen
-000023f0: 6365 5b50 6174 684c 696b 655d 207c 2050  ce[PathLike] | P
-00002400: 6174 684c 696b 652c 202a 2a6b 7761 7267  athLike, **kwarg
-00002410: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
-00002420: 2020 2020 2020 2020 5265 6164 2069 6d61          Read ima
-00002430: 6765 2064 6174 6120 6672 6f6d 2073 7065  ge data from spe
-00002440: 6369 6669 6564 2066 696c 6520 6f72 2066  cified file or f
-00002450: 696c 6573 2c20 6974 2063 616e 2072 6561  iles, it can rea
-00002460: 6420 6120 6c69 7374 206f 6620 696d 6167  d a list of imag
-00002470: 6573 0a20 2020 2020 2020 2061 6e64 2073  es.        and s
-00002480: 7461 636b 2074 6865 6d20 746f 6765 7468  tack them togeth
-00002490: 6572 2061 7320 6d75 6c74 692d 6368 616e  er as multi-chan
-000024a0: 6e65 6c20 6461 7461 2069 6e20 6067 6574  nel data in `get
-000024b0: 5f64 6174 6128 2960 2e0a 2020 2020 2020  _data()`..      
-000024c0: 2020 4966 2070 6173 7369 6e67 2064 6972    If passing dir
-000024d0: 6563 746f 7279 2070 6174 6820 696e 7374  ectory path inst
-000024e0: 6561 6420 6f66 2066 696c 6520 7061 7468  ead of file path
-000024f0: 2c20 7769 6c6c 2074 7265 6174 2069 7420  , will treat it 
-00002500: 6173 2044 4943 4f4d 2069 6d61 6765 7320  as DICOM images 
-00002510: 7365 7269 6573 2061 6e64 2072 6561 642e  series and read.
-00002520: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
-00002530: 6174 2074 6865 2072 6574 7572 6e65 6420  at the returned 
-00002540: 6f62 6a65 6374 2069 7320 4954 4b20 696d  object is ITK im
-00002550: 6167 6520 6f62 6a65 6374 206f 7220 6c69  age object or li
-00002560: 7374 206f 6620 4954 4b20 696d 6167 6520  st of ITK image 
-00002570: 6f62 6a65 6374 732e 0a0a 2020 2020 2020  objects...      
-00002580: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00002590: 2020 2020 6461 7461 3a20 6669 6c65 206e      data: file n
-000025a0: 616d 6520 6f72 2061 206c 6973 7420 6f66  ame or a list of
-000025b0: 2066 696c 6520 6e61 6d65 7320 746f 2072   file names to r
-000025c0: 6561 642c 0a20 2020 2020 2020 2020 2020  ead,.           
-000025d0: 206b 7761 7267 733a 2061 6464 6974 696f   kwargs: additio
-000025e0: 6e61 6c20 6172 6773 2066 6f72 2060 6974  nal args for `it
-000025f0: 6b2e 696d 7265 6164 6020 4150 492c 2077  k.imread` API, w
-00002600: 696c 6c20 6f76 6572 7269 6465 2060 7365  ill override `se
-00002610: 6c66 2e6b 7761 7267 7360 2066 6f72 2065  lf.kwargs` for e
-00002620: 7869 7374 696e 6720 6b65 7973 2e0a 2020  xisting keys..  
-00002630: 2020 2020 2020 2020 2020 2020 2020 4d6f                Mo
-00002640: 7265 2064 6574 6169 6c73 2061 626f 7574  re details about
-00002650: 2061 7661 696c 6162 6c65 2061 7267 733a   available args:
-00002660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002670: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00002680: 636f 6d2f 496e 7369 6768 7453 6f66 7477  com/InsightSoftw
-00002690: 6172 6543 6f6e 736f 7274 6975 6d2f 4954  areConsortium/IT
-000026a0: 4b2f 626c 6f62 2f6d 6173 7465 722f 5772  K/blob/master/Wr
-000026b0: 6170 7069 6e67 2f47 656e 6572 6174 6f72  apping/Generator
-000026c0: 732f 5079 7468 6f6e 2f69 746b 4578 7472  s/Python/itkExtr
-000026d0: 6173 2e70 790a 0a20 2020 2020 2020 2022  as.py..        "
-000026e0: 2222 0a20 2020 2020 2020 2069 6d67 5f20  "".        img_ 
-000026f0: 3d20 5b5d 0a0a 2020 2020 2020 2020 6669  = []..        fi
-00002700: 6c65 6e61 6d65 733a 2053 6571 7565 6e63  lenames: Sequenc
-00002710: 655b 5061 7468 4c69 6b65 5d20 3d20 656e  e[PathLike] = en
-00002720: 7375 7265 5f74 7570 6c65 2864 6174 6129  sure_tuple(data)
-00002730: 0a20 2020 2020 2020 206b 7761 7267 735f  .        kwargs_
-00002740: 203d 2073 656c 662e 6b77 6172 6773 2e63   = self.kwargs.c
-00002750: 6f70 7928 290a 2020 2020 2020 2020 6b77  opy().        kw
-00002760: 6172 6773 5f2e 7570 6461 7465 286b 7761  args_.update(kwa
-00002770: 7267 7329 0a20 2020 2020 2020 2066 6f72  rgs).        for
-00002780: 206e 616d 6520 696e 2066 696c 656e 616d   name in filenam
-00002790: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-000027a0: 6e61 6d65 203d 2066 227b 6e61 6d65 7d22  name = f"{name}"
-000027b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000027c0: 5061 7468 286e 616d 6529 2e69 735f 6469  Path(name).is_di
-000027d0: 7228 293a 0a20 2020 2020 2020 2020 2020  r():.           
-000027e0: 2020 2020 2023 2072 6561 6420 4449 434f       # read DICO
-000027f0: 4d20 7365 7269 6573 0a20 2020 2020 2020  M series.       
-00002800: 2020 2020 2020 2020 2023 2068 7474 7073           # https
-00002810: 3a2f 2f69 746b 2e6f 7267 2f49 544b 4578  ://itk.org/ITKEx
-00002820: 616d 706c 6573 2f73 7263 2f49 4f2f 4744  amples/src/IO/GD
-00002830: 434d 2f52 6561 6444 4943 4f4d 5365 7269  CM/ReadDICOMSeri
-00002840: 6573 416e 6457 7269 7465 3344 496d 6167  esAndWrite3DImag
-00002850: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00002860: 2020 6e61 6d65 735f 6765 6e65 7261 746f    names_generato
-00002870: 7220 3d20 6974 6b2e 4744 434d 5365 7269  r = itk.GDCMSeri
-00002880: 6573 4669 6c65 4e61 6d65 732e 4e65 7728  esFileNames.New(
-00002890: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000028a0: 2020 6e61 6d65 735f 6765 6e65 7261 746f    names_generato
-000028b0: 722e 5365 7455 7365 5365 7269 6573 4465  r.SetUseSeriesDe
-000028c0: 7461 696c 7328 5472 7565 290a 2020 2020  tails(True).    
-000028d0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-000028e0: 735f 6765 6e65 7261 746f 722e 4164 6453  s_generator.AddS
-000028f0: 6572 6965 7352 6573 7472 6963 7469 6f6e  eriesRestriction
-00002900: 2822 3030 3038 7c30 3032 3122 2920 2023  ("0008|0021")  #
-00002910: 2053 6572 6965 7320 4461 7465 0a20 2020   Series Date.   
-00002920: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00002930: 6573 5f67 656e 6572 6174 6f72 2e53 6574  es_generator.Set
-00002940: 4469 7265 6374 6f72 7928 6e61 6d65 290a  Directory(name).
-00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002960: 7365 7269 6573 5f75 6964 203d 206e 616d  series_uid = nam
-00002970: 6573 5f67 656e 6572 6174 6f72 2e47 6574  es_generator.Get
-00002980: 5365 7269 6573 5549 4473 2829 0a0a 2020  SeriesUIDs()..  
-00002990: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000029a0: 206c 656e 2873 6572 6965 735f 7569 6429   len(series_uid)
-000029b0: 203c 2031 3a0a 2020 2020 2020 2020 2020   < 1:.          
-000029c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000029d0: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
-000029e0: 7228 6622 6e6f 2044 4943 4f4d 7320 696e  r(f"no DICOMs in
-000029f0: 3a20 7b6e 616d 657d 2e22 290a 2020 2020  : {name}.").    
-00002a00: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00002a10: 656e 2873 6572 6965 735f 7569 6429 203e  en(series_uid) >
-00002a20: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00002a30: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
-00002a40: 2e77 6172 6e28 6622 7468 6520 6469 7265  .warn(f"the dire
-00002a50: 6374 6f72 793a 207b 6e61 6d65 7d20 636f  ctory: {name} co
-00002a60: 6e74 6169 6e73 206d 6f72 6520 7468 616e  ntains more than
-00002a70: 206f 6e65 2044 4943 4f4d 2073 6572 6965   one DICOM serie
-00002a80: 732e 2229 0a20 2020 2020 2020 2020 2020  s.").           
-00002a90: 2020 2020 2073 6572 6965 735f 6964 656e       series_iden
-00002aa0: 7469 6669 6572 203d 2073 6572 6965 735f  tifier = series_
-00002ab0: 7569 645b 305d 2069 6620 6e6f 7420 7365  uid[0] if not se
-00002ac0: 6c66 2e73 6572 6965 735f 6e61 6d65 2065  lf.series_name e
-00002ad0: 6c73 6520 7365 6c66 2e73 6572 6965 735f  lse self.series_
-00002ae0: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-00002af0: 2020 2020 206e 616d 6520 3d20 6e61 6d65       name = name
-00002b00: 735f 6765 6e65 7261 746f 722e 4765 7446  s_generator.GetF
-00002b10: 696c 654e 616d 6573 2873 6572 6965 735f  ileNames(series_
-00002b20: 6964 656e 7469 6669 6572 290a 0a20 2020  identifier)..   
-00002b30: 2020 2020 2020 2020 2020 2020 205f 6f62               _ob
-00002b40: 6a20 3d20 6974 6b2e 696d 7265 6164 286e  j = itk.imread(n
-00002b50: 616d 652c 202a 2a6b 7761 7267 735f 290a  ame, **kwargs_).
-00002b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b70: 6966 2073 656c 662e 7365 7269 6573 5f6d  if self.series_m
-00002b80: 6574 613a 0a20 2020 2020 2020 2020 2020  eta:.           
-00002b90: 2020 2020 2020 2020 205f 7265 6164 6572           _reader
-00002ba0: 203d 2069 746b 2e49 6d61 6765 5365 7269   = itk.ImageSeri
-00002bb0: 6573 5265 6164 6572 2e4e 6577 2846 696c  esReader.New(Fil
-00002bc0: 654e 616d 6573 3d6e 616d 6529 0a20 2020  eNames=name).   
-00002bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002be0: 205f 7265 6164 6572 2e55 7064 6174 6528   _reader.Update(
-00002bf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00002c00: 2020 2020 2020 5f6d 6574 6120 3d20 5f72        _meta = _r
-00002c10: 6561 6465 722e 4765 744d 6574 6144 6174  eader.GetMetaDat
-00002c20: 6144 6963 7469 6f6e 6172 7941 7272 6179  aDictionaryArray
-00002c30: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00002c40: 2020 2020 2020 2069 6620 6c65 6e28 5f6d         if len(_m
-00002c50: 6574 6129 203e 2030 3a0a 2020 2020 2020  eta) > 0:.      
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2320 544f 444f 3a20 7573 696e 6720    # TODO: using 
-00002c80: 7468 6520 6669 7273 7420 736c 6963 6527  the first slice'
-00002c90: 7320 6d65 7461 2e20 7468 6973 2063 6f75  s meta. this cou
-00002ca0: 6c64 2062 6520 696d 7072 6f76 6564 2074  ld be improved t
-00002cb0: 6f20 6669 6c74 6572 2075 6e6e 6563 6573  o filter unneces
-00002cc0: 7361 7279 2074 6167 732e 0a20 2020 2020  sary tags..     
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ce0: 2020 205f 6f62 6a2e 5365 744d 6574 6144     _obj.SetMetaD
-00002cf0: 6174 6144 6963 7469 6f6e 6172 7928 5f6d  ataDictionary(_m
-00002d00: 6574 615b 305d 290a 2020 2020 2020 2020  eta[0]).        
-00002d10: 2020 2020 2020 2020 696d 675f 2e61 7070          img_.app
-00002d20: 656e 6428 5f6f 626a 290a 2020 2020 2020  end(_obj).      
-00002d30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00002d40: 2020 2020 2020 2020 2020 2020 696d 675f              img_
-00002d50: 2e61 7070 656e 6428 6974 6b2e 696d 7265  .append(itk.imre
-00002d60: 6164 286e 616d 652c 202a 2a6b 7761 7267  ad(name, **kwarg
-00002d70: 735f 2929 0a20 2020 2020 2020 2072 6574  s_)).        ret
-00002d80: 7572 6e20 696d 675f 2069 6620 6c65 6e28  urn img_ if len(
-00002d90: 6669 6c65 6e61 6d65 7329 203e 2031 2065  filenames) > 1 e
-00002da0: 6c73 6520 696d 675f 5b30 5d0a 0a20 2020  lse img_[0]..   
-00002db0: 2064 6566 2067 6574 5f64 6174 6128 7365   def get_data(se
-00002dc0: 6c66 2c20 696d 6729 202d 3e20 7475 706c  lf, img) -> tupl
-00002dd0: 655b 6e70 2e6e 6461 7272 6179 2c20 6469  e[np.ndarray, di
-00002de0: 6374 5d3a 0a20 2020 2020 2020 2022 2222  ct]:.        """
-00002df0: 0a20 2020 2020 2020 2045 7874 7261 6374  .        Extract
-00002e00: 2064 6174 6120 6172 7261 7920 616e 6420   data array and 
-00002e10: 6d65 7461 6461 7461 2066 726f 6d20 6c6f  metadata from lo
-00002e20: 6164 6564 2069 6d61 6765 2061 6e64 2072  aded image and r
-00002e30: 6574 7572 6e20 7468 656d 2e0a 2020 2020  eturn them..    
-00002e40: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-00002e50: 6e20 7265 7475 726e 7320 7477 6f20 6f62  n returns two ob
-00002e60: 6a65 6374 732c 2066 6972 7374 2069 7320  jects, first is 
-00002e70: 6e75 6d70 7920 6172 7261 7920 6f66 2069  numpy array of i
-00002e80: 6d61 6765 2064 6174 612c 2073 6563 6f6e  mage data, secon
-00002e90: 6420 6973 2064 6963 7420 6f66 206d 6574  d is dict of met
-00002ea0: 6164 6174 612e 0a20 2020 2020 2020 2049  adata..        I
-00002eb0: 7420 636f 6e73 7472 7563 7473 2060 6166  t constructs `af
-00002ec0: 6669 6e65 602c 2060 6f72 6967 696e 616c  fine`, `original
-00002ed0: 5f61 6666 696e 6560 2c20 616e 6420 6073  _affine`, and `s
-00002ee0: 7061 7469 616c 5f73 6861 7065 6020 616e  patial_shape` an
-00002ef0: 6420 7374 6f72 6573 2074 6865 6d20 696e  d stores them in
-00002f00: 206d 6574 6120 6469 6374 2e0a 2020 2020   meta dict..    
-00002f10: 2020 2020 5768 656e 206c 6f61 6469 6e67      When loading
-00002f20: 2061 206c 6973 7420 6f66 2066 696c 6573   a list of files
-00002f30: 2c20 7468 6579 2061 7265 2073 7461 636b  , they are stack
-00002f40: 6564 2074 6f67 6574 6865 7220 6174 2061  ed together at a
-00002f50: 206e 6577 2064 696d 656e 7369 6f6e 2061   new dimension a
-00002f60: 7320 7468 6520 6669 7273 7420 6469 6d65  s the first dime
-00002f70: 6e73 696f 6e2c 0a20 2020 2020 2020 2061  nsion,.        a
-00002f80: 6e64 2074 6865 206d 6574 6164 6174 6120  nd the metadata 
-00002f90: 6f66 2074 6865 2066 6972 7374 2069 6d61  of the first ima
-00002fa0: 6765 2069 7320 7573 6564 2074 6f20 7265  ge is used to re
-00002fb0: 7072 6573 656e 7420 7468 6520 6f75 7470  present the outp
-00002fc0: 7574 206d 6574 6164 6174 612e 0a0a 2020  ut metadata...  
-00002fd0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00002fe0: 2020 2020 2020 2020 696d 673a 2061 6e20          img: an 
-00002ff0: 4954 4b20 696d 6167 6520 6f62 6a65 6374  ITK image object
-00003000: 206c 6f61 6465 6420 6672 6f6d 2061 6e20   loaded from an 
-00003010: 696d 6167 6520 6669 6c65 206f 7220 6120  image file or a 
-00003020: 6c69 7374 206f 6620 4954 4b20 696d 6167  list of ITK imag
-00003030: 6520 6f62 6a65 6374 732e 0a0a 2020 2020  e objects...    
-00003040: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003050: 696d 675f 6172 7261 793a 206c 6973 745b  img_array: list[
-00003060: 6e70 2e6e 6461 7272 6179 5d20 3d20 5b5d  np.ndarray] = []
-00003070: 0a20 2020 2020 2020 2063 6f6d 7061 7469  .        compati
-00003080: 626c 655f 6d65 7461 3a20 6469 6374 203d  ble_meta: dict =
-00003090: 207b 7d0a 0a20 2020 2020 2020 2066 6f72   {}..        for
-000030a0: 2069 2069 6e20 656e 7375 7265 5f74 7570   i in ensure_tup
-000030b0: 6c65 2869 6d67 293a 0a20 2020 2020 2020  le(img):.       
-000030c0: 2020 2020 2064 6174 6120 3d20 7365 6c66       data = self
-000030d0: 2e5f 6765 745f 6172 7261 795f 6461 7461  ._get_array_data
-000030e0: 2869 290a 2020 2020 2020 2020 2020 2020  (i).            
-000030f0: 696d 675f 6172 7261 792e 6170 7065 6e64  img_array.append
-00003100: 2864 6174 6129 0a20 2020 2020 2020 2020  (data).         
-00003110: 2020 2068 6561 6465 7220 3d20 7365 6c66     header = self
-00003120: 2e5f 6765 745f 6d65 7461 5f64 6963 7428  ._get_meta_dict(
-00003130: 6929 0a20 2020 2020 2020 2020 2020 2068  i).            h
-00003140: 6561 6465 725b 4d65 7461 4b65 7973 2e4f  eader[MetaKeys.O
-00003150: 5249 4749 4e41 4c5f 4146 4649 4e45 5d20  RIGINAL_AFFINE] 
-00003160: 3d20 7365 6c66 2e5f 6765 745f 6166 6669  = self._get_affi
-00003170: 6e65 2869 2c20 7365 6c66 2e61 6666 696e  ne(i, self.affin
-00003180: 655f 6c70 735f 746f 5f72 6173 290a 2020  e_lps_to_ras).  
-00003190: 2020 2020 2020 2020 2020 6865 6164 6572            header
-000031a0: 5b4d 6574 614b 6579 732e 5350 4143 455d  [MetaKeys.SPACE]
-000031b0: 203d 2053 7061 6365 4b65 7973 2e52 4153   = SpaceKeys.RAS
-000031c0: 2069 6620 7365 6c66 2e61 6666 696e 655f   if self.affine_
-000031d0: 6c70 735f 746f 5f72 6173 2065 6c73 6520  lps_to_ras else 
-000031e0: 5370 6163 654b 6579 732e 4c50 530a 2020  SpaceKeys.LPS.  
-000031f0: 2020 2020 2020 2020 2020 6865 6164 6572            header
-00003200: 5b4d 6574 614b 6579 732e 4146 4649 4e45  [MetaKeys.AFFINE
-00003210: 5d20 3d20 6865 6164 6572 5b4d 6574 614b  ] = header[MetaK
-00003220: 6579 732e 4f52 4947 494e 414c 5f41 4646  eys.ORIGINAL_AFF
-00003230: 494e 455d 2e63 6f70 7928 290a 2020 2020  INE].copy().    
-00003240: 2020 2020 2020 2020 6865 6164 6572 5b4d          header[M
-00003250: 6574 614b 6579 732e 5350 4154 4941 4c5f  etaKeys.SPATIAL_
-00003260: 5348 4150 455d 203d 2073 656c 662e 5f67  SHAPE] = self._g
-00003270: 6574 5f73 7061 7469 616c 5f73 6861 7065  et_spatial_shape
-00003280: 2869 290a 2020 2020 2020 2020 2020 2020  (i).            
-00003290: 6966 2073 656c 662e 6368 616e 6e65 6c5f  if self.channel_
-000032a0: 6469 6d20 6973 204e 6f6e 653a 2020 2320  dim is None:  # 
-000032b0: 6465 6661 756c 7420 746f 2022 6e6f 5f63  default to "no_c
-000032c0: 6861 6e6e 656c 2220 6f72 202d 310a 2020  hannel" or -1.  
-000032d0: 2020 2020 2020 2020 2020 2020 2020 6865                he
-000032e0: 6164 6572 5b4d 6574 614b 6579 732e 4f52  ader[MetaKeys.OR
-000032f0: 4947 494e 414c 5f43 4841 4e4e 454c 5f44  IGINAL_CHANNEL_D
-00003300: 494d 5d20 3d20 280a 2020 2020 2020 2020  IM] = (.        
-00003310: 2020 2020 2020 2020 2020 2020 666c 6f61              floa
-00003320: 7428 226e 616e 2229 2069 6620 6c65 6e28  t("nan") if len(
-00003330: 6461 7461 2e73 6861 7065 2920 3d3d 206c  data.shape) == l
-00003340: 656e 2868 6561 6465 725b 4d65 7461 4b65  en(header[MetaKe
-00003350: 7973 2e53 5041 5449 414c 5f53 4841 5045  ys.SPATIAL_SHAPE
-00003360: 5d29 2065 6c73 6520 2d31 0a20 2020 2020  ]) else -1.     
-00003370: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00003380: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00003390: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-000033a0: 6561 6465 725b 4d65 7461 4b65 7973 2e4f  eader[MetaKeys.O
-000033b0: 5249 4749 4e41 4c5f 4348 414e 4e45 4c5f  RIGINAL_CHANNEL_
-000033c0: 4449 4d5d 203d 2073 656c 662e 6368 616e  DIM] = self.chan
-000033d0: 6e65 6c5f 6469 6d0a 2020 2020 2020 2020  nel_dim.        
-000033e0: 2020 2020 5f63 6f70 795f 636f 6d70 6174      _copy_compat
-000033f0: 6962 6c65 5f64 6963 7428 6865 6164 6572  ible_dict(header
-00003400: 2c20 636f 6d70 6174 6962 6c65 5f6d 6574  , compatible_met
-00003410: 6129 0a0a 2020 2020 2020 2020 7265 7475  a)..        retu
-00003420: 726e 205f 7374 6163 6b5f 696d 6167 6573  rn _stack_images
-00003430: 2869 6d67 5f61 7272 6179 2c20 636f 6d70  (img_array, comp
-00003440: 6174 6962 6c65 5f6d 6574 6129 2c20 636f  atible_meta), co
-00003450: 6d70 6174 6962 6c65 5f6d 6574 610a 0a20  mpatible_meta.. 
-00003460: 2020 2064 6566 205f 6765 745f 6d65 7461     def _get_meta
-00003470: 5f64 6963 7428 7365 6c66 2c20 696d 6729  _dict(self, img)
-00003480: 202d 3e20 6469 6374 3a0a 2020 2020 2020   -> dict:.      
-00003490: 2020 2222 220a 2020 2020 2020 2020 4765    """.        Ge
-000034a0: 7420 616c 6c20 7468 6520 6d65 7461 6461  t all the metada
-000034b0: 7461 206f 6620 7468 6520 696d 6167 6520  ta of the image 
-000034c0: 616e 6420 636f 6e76 6572 7420 746f 2064  and convert to d
-000034d0: 6963 7420 7479 7065 2e0a 0a20 2020 2020  ict type...     
-000034e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-000034f0: 2020 2020 2069 6d67 3a20 616e 2049 544b       img: an ITK
-00003500: 2069 6d61 6765 206f 626a 6563 7420 6c6f   image object lo
-00003510: 6164 6564 2066 726f 6d20 616e 2069 6d61  aded from an ima
-00003520: 6765 2066 696c 652e 0a0a 2020 2020 2020  ge file...      
-00003530: 2020 2222 220a 2020 2020 2020 2020 696d    """.        im
-00003540: 675f 6d65 7461 5f64 6963 7420 3d20 696d  g_meta_dict = im
-00003550: 672e 4765 744d 6574 6144 6174 6144 6963  g.GetMetaDataDic
-00003560: 7469 6f6e 6172 7928 290a 2020 2020 2020  tionary().      
-00003570: 2020 6d65 7461 5f64 6963 7420 3d20 7b7d    meta_dict = {}
-00003580: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
-00003590: 2069 6e20 696d 675f 6d65 7461 5f64 6963   in img_meta_dic
-000035a0: 742e 4765 744b 6579 7328 293a 0a20 2020  t.GetKeys():.   
-000035b0: 2020 2020 2020 2020 2069 6620 6b65 792e           if key.
-000035c0: 7374 6172 7473 7769 7468 2822 4954 4b5f  startswith("ITK_
-000035d0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000035e0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-000035f0: 2020 2020 2020 2020 2076 616c 203d 2069           val = i
-00003600: 6d67 5f6d 6574 615f 6469 6374 5b6b 6579  mg_meta_dict[key
-00003610: 5d0a 2020 2020 2020 2020 2020 2020 6d65  ].            me
-00003620: 7461 5f64 6963 745b 6b65 795d 203d 206e  ta_dict[key] = n
-00003630: 702e 6173 6172 7261 7928 7661 6c29 2069  p.asarray(val) i
-00003640: 6620 7479 7065 2876 616c 292e 5f5f 6e61  f type(val).__na
-00003650: 6d65 5f5f 2e73 7461 7274 7377 6974 6828  me__.startswith(
-00003660: 2269 746b 2229 2065 6c73 6520 7661 6c0a  "itk") else val.
-00003670: 0a20 2020 2020 2020 206d 6574 615f 6469  .        meta_di
-00003680: 6374 5b22 7370 6163 696e 6722 5d20 3d20  ct["spacing"] = 
-00003690: 6e70 2e61 7361 7272 6179 2869 6d67 2e47  np.asarray(img.G
-000036a0: 6574 5370 6163 696e 6728 2929 0a20 2020  etSpacing()).   
-000036b0: 2020 2020 2072 6574 7572 6e20 6d65 7461       return meta
-000036c0: 5f64 6963 740a 0a20 2020 2064 6566 205f  _dict..    def _
-000036d0: 6765 745f 6166 6669 6e65 2873 656c 662c  get_affine(self,
-000036e0: 2069 6d67 2c20 6c70 735f 746f 5f72 6173   img, lps_to_ras
-000036f0: 3a20 626f 6f6c 203d 2054 7275 6529 3a0a  : bool = True):.
-00003700: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003710: 2020 2020 4765 7420 6f72 2063 6f6e 7374      Get or const
-00003720: 7275 6374 2074 6865 2061 6666 696e 6520  ruct the affine 
-00003730: 6d61 7472 6978 206f 6620 7468 6520 696d  matrix of the im
-00003740: 6167 652c 2069 7420 6361 6e20 6265 2075  age, it can be u
-00003750: 7365 6420 746f 2063 6f72 7265 6374 0a20  sed to correct. 
-00003760: 2020 2020 2020 2073 7061 6369 6e67 2c20         spacing, 
-00003770: 6f72 6965 6e74 6174 696f 6e20 6f72 2065  orientation or e
-00003780: 7865 6375 7465 2073 7061 7469 616c 2074  xecute spatial t
-00003790: 7261 6e73 666f 726d 732e 0a0a 2020 2020  ransforms...    
-000037a0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000037b0: 2020 2020 2020 696d 673a 2061 6e20 4954        img: an IT
-000037c0: 4b20 696d 6167 6520 6f62 6a65 6374 206c  K image object l
-000037d0: 6f61 6465 6420 6672 6f6d 2061 6e20 696d  oaded from an im
-000037e0: 6167 6520 6669 6c65 2e0a 2020 2020 2020  age file..      
-000037f0: 2020 2020 2020 6c70 735f 746f 5f72 6173        lps_to_ras
-00003800: 3a20 7768 6574 6865 7220 746f 2063 6f6e  : whether to con
-00003810: 7665 7274 2074 6865 2061 6666 696e 6520  vert the affine 
-00003820: 6d61 7472 6978 2066 726f 6d20 224c 5053  matrix from "LPS
-00003830: 2220 746f 2022 5241 5322 2e20 4465 6661  " to "RAS". Defa
-00003840: 756c 7473 2074 6f20 5472 7565 2e0a 0a20  ults to True... 
-00003850: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00003860: 2020 2064 6972 6563 7469 6f6e 203d 2069     direction = i
-00003870: 746b 2e61 7272 6179 5f66 726f 6d5f 6d61  tk.array_from_ma
-00003880: 7472 6978 2869 6d67 2e47 6574 4469 7265  trix(img.GetDire
-00003890: 6374 696f 6e28 2929 0a20 2020 2020 2020  ction()).       
-000038a0: 2073 7061 6369 6e67 203d 206e 702e 6173   spacing = np.as
-000038b0: 6172 7261 7928 696d 672e 4765 7453 7061  array(img.GetSpa
-000038c0: 6369 6e67 2829 290a 2020 2020 2020 2020  cing()).        
-000038d0: 6f72 6967 696e 203d 206e 702e 6173 6172  origin = np.asar
-000038e0: 7261 7928 696d 672e 4765 744f 7269 6769  ray(img.GetOrigi
-000038f0: 6e28 2929 0a0a 2020 2020 2020 2020 6469  n())..        di
-00003900: 7265 6374 696f 6e20 3d20 6e70 2e61 7361  rection = np.asa
-00003910: 7272 6179 2864 6972 6563 7469 6f6e 290a  rray(direction).
-00003920: 2020 2020 2020 2020 7372 203d 206d 696e          sr = min
-00003930: 286d 6178 2864 6972 6563 7469 6f6e 2e73  (max(direction.s
-00003940: 6861 7065 5b30 5d2c 2031 292c 2033 290a  hape[0], 1), 3).
-00003950: 2020 2020 2020 2020 6166 6669 6e65 3a20          affine: 
-00003960: 6e70 2e6e 6461 7272 6179 203d 206e 702e  np.ndarray = np.
-00003970: 6579 6528 7372 202b 2031 290a 2020 2020  eye(sr + 1).    
-00003980: 2020 2020 6166 6669 6e65 5b3a 7372 2c20      affine[:sr, 
-00003990: 3a73 725d 203d 2064 6972 6563 7469 6f6e  :sr] = direction
-000039a0: 5b3a 7372 2c20 3a73 725d 2040 206e 702e  [:sr, :sr] @ np.
-000039b0: 6469 6167 2873 7061 6369 6e67 5b3a 7372  diag(spacing[:sr
-000039c0: 5d29 0a20 2020 2020 2020 2061 6666 696e  ]).        affin
-000039d0: 655b 3a73 722c 202d 315d 203d 206f 7269  e[:sr, -1] = ori
-000039e0: 6769 6e5b 3a73 725d 0a20 2020 2020 2020  gin[:sr].       
-000039f0: 2069 6620 6c70 735f 746f 5f72 6173 3a0a   if lps_to_ras:.
-00003a00: 2020 2020 2020 2020 2020 2020 6166 6669              affi
-00003a10: 6e65 203d 206f 7269 656e 7461 7469 6f6e  ne = orientation
-00003a20: 5f72 6173 5f6c 7073 2861 6666 696e 6529  _ras_lps(affine)
-00003a30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003a40: 6166 6669 6e65 0a0a 2020 2020 6465 6620  affine..    def 
-00003a50: 5f67 6574 5f73 7061 7469 616c 5f73 6861  _get_spatial_sha
-00003a60: 7065 2873 656c 662c 2069 6d67 293a 0a20  pe(self, img):. 
-00003a70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00003a80: 2020 2047 6574 2074 6865 2073 7061 7469     Get the spati
-00003a90: 616c 2073 6861 7065 206f 6620 6069 6d67  al shape of `img
-00003aa0: 602e 0a0a 2020 2020 2020 2020 4172 6773  `...        Args
-00003ab0: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
-00003ac0: 673a 2061 6e20 4954 4b20 696d 6167 6520  g: an ITK image 
-00003ad0: 6f62 6a65 6374 206c 6f61 6465 6420 6672  object loaded fr
-00003ae0: 6f6d 2061 6e20 696d 6167 6520 6669 6c65  om an image file
-00003af0: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
-00003b00: 2020 2020 2020 2073 7220 3d20 6974 6b2e         sr = itk.
-00003b10: 6172 7261 795f 6672 6f6d 5f6d 6174 7269  array_from_matri
-00003b20: 7828 696d 672e 4765 7444 6972 6563 7469  x(img.GetDirecti
-00003b30: 6f6e 2829 292e 7368 6170 655b 305d 0a20  on()).shape[0]. 
-00003b40: 2020 2020 2020 2073 7220 3d20 6d61 7828         sr = max(
-00003b50: 6d69 6e28 7372 2c20 3329 2c20 3129 0a20  min(sr, 3), 1). 
-00003b60: 2020 2020 2020 205f 7369 7a65 203d 206c         _size = l
-00003b70: 6973 7428 6974 6b2e 7369 7a65 2869 6d67  ist(itk.size(img
-00003b80: 2929 0a20 2020 2020 2020 2069 6620 6973  )).        if is
-00003b90: 696e 7374 616e 6365 2873 656c 662e 6368  instance(self.ch
-00003ba0: 616e 6e65 6c5f 6469 6d2c 2069 6e74 293a  annel_dim, int):
-00003bb0: 0a20 2020 2020 2020 2020 2020 205f 7369  .            _si
-00003bc0: 7a65 2e70 6f70 2873 656c 662e 6368 616e  ze.pop(self.chan
-00003bd0: 6e65 6c5f 6469 6d29 0a20 2020 2020 2020  nel_dim).       
-00003be0: 2072 6574 7572 6e20 6e70 2e61 7361 7272   return np.asarr
-00003bf0: 6179 285f 7369 7a65 5b3a 7372 5d29 0a0a  ay(_size[:sr])..
-00003c00: 2020 2020 6465 6620 5f67 6574 5f61 7272      def _get_arr
-00003c10: 6179 5f64 6174 6128 7365 6c66 2c20 696d  ay_data(self, im
-00003c20: 6729 3a0a 2020 2020 2020 2020 2222 220a  g):.        """.
-00003c30: 2020 2020 2020 2020 4765 7420 7468 6520          Get the 
-00003c40: 7261 7720 6172 7261 7920 6461 7461 206f  raw array data o
-00003c50: 6620 7468 6520 696d 6167 652c 2063 6f6e  f the image, con
-00003c60: 7665 7274 6564 2074 6f20 4e75 6d70 7920  verted to Numpy 
-00003c70: 6172 7261 792e 0a0a 2020 2020 2020 2020  array...        
-00003c80: 466f 6c6c 6f77 696e 6720 5079 546f 7263  Following PyTorc
-00003c90: 6820 636f 6e76 656e 7469 6f6e 732c 2074  h conventions, t
-00003ca0: 6865 2072 6574 7572 6e65 6420 6172 7261  he returned arra
-00003cb0: 7920 6461 7461 2068 6173 2063 6f6e 7469  y data has conti
-00003cc0: 6775 6f75 7320 6368 616e 6e65 6c73 2c0a  guous channels,.
-00003cd0: 2020 2020 2020 2020 652e 672e 2066 6f72          e.g. for
-00003ce0: 2061 6e20 5247 4220 696d 6167 652c 2061   an RGB image, a
-00003cf0: 6c6c 2072 6564 2063 6861 6e6e 656c 2069  ll red channel i
-00003d00: 6d61 6765 2070 6978 656c 7320 6172 6520  mage pixels are 
-00003d10: 636f 6e74 6967 756f 7573 2069 6e20 6d65  contiguous in me
-00003d20: 6d6f 7279 2e0a 2020 2020 2020 2020 5468  mory..        Th
-00003d30: 6520 6c61 7374 2061 7869 7320 6f66 2074  e last axis of t
-00003d40: 6865 2072 6574 7572 6e65 6420 6172 7261  he returned arra
-00003d50: 7920 6973 2074 6865 2063 6861 6e6e 656c  y is the channel
-00003d60: 2061 7869 732e 0a0a 2020 2020 2020 2020   axis...        
-00003d70: 5365 6520 616c 736f 3a0a 0a20 2020 2020  See also:..     
-00003d80: 2020 2020 2020 202d 2068 7474 7073 3a2f         - https:/
-00003d90: 2f67 6974 6875 622e 636f 6d2f 496e 7369  /github.com/Insi
-00003da0: 6768 7453 6f66 7477 6172 6543 6f6e 736f  ghtSoftwareConso
-00003db0: 7274 6975 6d2f 4954 4b2f 626c 6f62 2f76  rtium/ITK/blob/v
-00003dc0: 352e 322e 312f 4d6f 6475 6c65 732f 4272  5.2.1/Modules/Br
-00003dd0: 6964 6765 2f4e 756d 5079 2f77 7261 7070  idge/NumPy/wrapp
-00003de0: 696e 672f 5079 4275 6666 6572 2e69 2e69  ing/PyBuffer.i.i
-00003df0: 6e0a 0a20 2020 2020 2020 2041 7267 733a  n..        Args:
-00003e00: 0a20 2020 2020 2020 2020 2020 2069 6d67  .            img
-00003e10: 3a20 616e 2049 544b 2069 6d61 6765 206f  : an ITK image o
-00003e20: 626a 6563 7420 6c6f 6164 6564 2066 726f  bject loaded fro
-00003e30: 6d20 616e 2069 6d61 6765 2066 696c 652e  m an image file.
-00003e40: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00003e50: 2020 2020 2020 6e70 5f69 6d67 203d 2069        np_img = i
-00003e60: 746b 2e61 7272 6179 5f76 6965 775f 6672  tk.array_view_fr
-00003e70: 6f6d 5f69 6d61 6765 2869 6d67 2c20 6b65  om_image(img, ke
-00003e80: 6570 5f61 7865 733d 4661 6c73 6529 0a20  ep_axes=False). 
-00003e90: 2020 2020 2020 2069 6620 696d 672e 4765         if img.Ge
-00003ea0: 744e 756d 6265 724f 6643 6f6d 706f 6e65  tNumberOfCompone
-00003eb0: 6e74 7350 6572 5069 7865 6c28 2920 3d3d  ntsPerPixel() ==
-00003ec0: 2031 3a20 2023 2068 616e 646c 696e 6720   1:  # handling 
-00003ed0: 7370 6174 6961 6c20 696d 6167 6573 0a20  spatial images. 
-00003ee0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003ef0: 6e20 6e70 5f69 6d67 2069 6620 7365 6c66  n np_img if self
-00003f00: 2e72 6576 6572 7365 5f69 6e64 6578 696e  .reverse_indexin
-00003f10: 6720 656c 7365 206e 705f 696d 672e 540a  g else np_img.T.
-00003f20: 2020 2020 2020 2020 2320 6861 6e64 6c69          # handli
-00003f30: 6e67 206d 756c 7469 2d63 6861 6e6e 656c  ng multi-channel
-00003f40: 2069 6d61 6765 730a 2020 2020 2020 2020   images.        
-00003f50: 7265 7475 726e 206e 705f 696d 6720 6966  return np_img if
-00003f60: 2073 656c 662e 7265 7665 7273 655f 696e   self.reverse_in
-00003f70: 6465 7869 6e67 2065 6c73 6520 6e70 2e6d  dexing else np.m
-00003f80: 6f76 6561 7869 7328 6e70 5f69 6d67 2e54  oveaxis(np_img.T
-00003f90: 2c20 302c 202d 3129 0a0a 0a40 7265 7175  , 0, -1)...@requ
-00003fa0: 6972 655f 706b 6728 706b 675f 6e61 6d65  ire_pkg(pkg_name
-00003fb0: 3d22 7079 6469 636f 6d22 290a 636c 6173  ="pydicom").clas
-00003fc0: 7320 5079 6469 636f 6d52 6561 6465 7228  s PydicomReader(
-00003fd0: 496d 6167 6552 6561 6465 7229 3a0a 2020  ImageReader):.  
-00003fe0: 2020 2222 220a 2020 2020 4c6f 6164 206d    """.    Load m
-00003ff0: 6564 6963 616c 2069 6d61 6765 7320 6261  edical images ba
-00004000: 7365 6420 6f6e 2050 7964 6963 6f6d 206c  sed on Pydicom l
-00004010: 6962 7261 7279 2e0a 2020 2020 416c 6c20  ibrary..    All 
-00004020: 7468 6520 7375 7070 6f72 7465 6420 696d  the supported im
-00004030: 6167 6520 666f 726d 6174 7320 6361 6e20  age formats can 
-00004040: 6265 2066 6f75 6e64 2061 743a 0a20 2020  be found at:.   
-00004050: 2068 7474 7073 3a2f 2f64 6963 6f6d 2e6e   https://dicom.n
-00004060: 656d 612e 6f72 672f 6d65 6469 6361 6c2f  ema.org/medical/
-00004070: 6469 636f 6d2f 6375 7272 656e 742f 6f75  dicom/current/ou
-00004080: 7470 7574 2f63 6874 6d6c 2f70 6172 7431  tput/chtml/part1
-00004090: 302f 6368 6170 7465 725f 372e 6874 6d6c  0/chapter_7.html
-000040a0: 0a0a 2020 2020 5079 6469 636f 6d52 6561  ..    PydicomRea
-000040b0: 6465 7220 6973 2061 6c73 6f20 6162 6c65  der is also able
-000040c0: 2074 6f20 6c6f 6164 2073 6567 6d65 6e74   to load segment
-000040d0: 6174 696f 6e73 2c20 6966 2061 2064 6963  ations, if a dic
-000040e0: 6f6d 2066 696c 6520 636f 6e74 6169 6e73  om file contains
-000040f0: 2074 6167 3a20 6053 6567 6d65 6e74 5365   tag: `SegmentSe
-00004100: 7175 656e 6365 602c 2074 6865 2072 6561  quence`, the rea
-00004110: 6465 720a 2020 2020 7769 6c6c 2063 6f6e  der.    will con
-00004120: 7369 6465 7220 6974 2061 7320 7365 676d  sider it as segm
-00004130: 656e 7461 7469 6f6e 2064 6174 612c 2061  entation data, a
-00004140: 6e64 2074 6f20 6c6f 6164 2069 7420 7375  nd to load it su
-00004150: 6363 6573 7366 756c 6c79 2c20 6050 6572  ccessfully, `Per
-00004160: 4672 616d 6546 756e 6374 696f 6e61 6c47  FrameFunctionalG
-00004170: 726f 7570 7353 6571 7565 6e63 6560 2069  roupsSequence` i
-00004180: 7320 7265 7175 6972 6564 0a20 2020 2066  s required.    f
-00004190: 6f72 2064 6963 6f6d 2066 696c 652c 2061  or dicom file, a
-000041a0: 6e64 2066 6f72 2065 6163 6820 6672 616d  nd for each fram
-000041b0: 6520 6f66 2064 6963 6f6d 2066 696c 652c  e of dicom file,
-000041c0: 2060 5365 676d 656e 7449 6465 6e74 6966   `SegmentIdentif
-000041d0: 6963 6174 696f 6e53 6571 7565 6e63 6560  icationSequence`
-000041e0: 2069 7320 7265 7175 6972 6564 2e0a 2020   is required..  
-000041f0: 2020 5468 6973 206d 6574 686f 6420 7265    This method re
-00004200: 6665 7273 2074 6f20 7468 6520 4869 6768  fers to the High
-00004210: 6469 636f 6d20 6c69 6272 6172 792e 0a0a  dicom library...
-00004220: 2020 2020 5468 6973 2063 6c61 7373 2072      This class r
-00004230: 6566 6572 7320 746f 3a0a 2020 2020 6874  efers to:.    ht
-00004240: 7470 733a 2f2f 6e69 7079 2e6f 7267 2f6e  tps://nipy.org/n
-00004250: 6962 6162 656c 2f64 6963 6f6d 2f64 6963  ibabel/dicom/dic
-00004260: 6f6d 5f6f 7269 656e 7461 7469 6f6e 2e68  om_orientation.h
-00004270: 746d 6c23 6469 636f 6d2d 6166 6669 6e65  tml#dicom-affine
-00004280: 2d66 6f72 6d75 6c61 0a20 2020 2068 7474  -formula.    htt
-00004290: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000042a0: 7079 6469 636f 6d2f 636f 6e74 7269 622d  pydicom/contrib-
-000042b0: 7079 6469 636f 6d2f 626c 6f62 2f6d 6173  pydicom/blob/mas
-000042c0: 7465 722f 696e 7075 742d 6f75 7470 7574  ter/input-output
-000042d0: 2f70 7964 6963 6f6d 5f73 6572 6965 732e  /pydicom_series.
-000042e0: 7079 0a20 2020 2068 7474 7073 3a2f 2f68  py.    https://h
-000042f0: 6967 6864 6963 6f6d 2e72 6561 6474 6865  ighdicom.readthe
-00004300: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00004310: 742f 7573 6167 652e 6874 6d6c 2370 6172  t/usage.html#par
-00004320: 7369 6e67 2d73 6567 6d65 6e74 6174 696f  sing-segmentatio
-00004330: 6e2d 7365 672d 696d 6167 6573 0a0a 2020  n-seg-images..  
-00004340: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00004350: 6368 616e 6e65 6c5f 6469 6d3a 2074 6865  channel_dim: the
-00004360: 2063 6861 6e6e 656c 2064 696d 656e 7369   channel dimensi
-00004370: 6f6e 206f 6620 7468 6520 696e 7075 7420  on of the input 
-00004380: 696d 6167 652c 2064 6566 6175 6c74 2069  image, default i
-00004390: 7320 4e6f 6e65 2e0a 2020 2020 2020 2020  s None..        
-000043a0: 2020 2020 5468 6973 2069 7320 7573 6564      This is used
-000043b0: 2074 6f20 7365 7420 6f72 6967 696e 616c   to set original
-000043c0: 5f63 6861 6e6e 656c 5f64 696d 2069 6e20  _channel_dim in 
-000043d0: 7468 6520 6d65 7461 6461 7461 2c20 456e  the metadata, En
-000043e0: 7375 7265 4368 616e 6e65 6c46 6972 7374  sureChannelFirst
-000043f0: 4420 7265 6164 7320 7468 6973 2066 6965  D reads this fie
-00004400: 6c64 2e0a 2020 2020 2020 2020 2020 2020  ld..            
-00004410: 4966 204e 6f6e 652c 2060 6f72 6967 696e  If None, `origin
-00004420: 616c 5f63 6861 6e6e 656c 5f64 696d 6020  al_channel_dim` 
-00004430: 7769 6c6c 2062 6520 6569 7468 6572 2060  will be either `
-00004440: 6e6f 5f63 6861 6e6e 656c 6020 6f72 2060  no_channel` or `
-00004450: 2d31 602e 0a20 2020 2020 2020 2061 6666  -1`..        aff
-00004460: 696e 655f 6c70 735f 746f 5f72 6173 3a20  ine_lps_to_ras: 
-00004470: 7768 6574 6865 7220 746f 2063 6f6e 7665  whether to conve
-00004480: 7274 2074 6865 2061 6666 696e 6520 6d61  rt the affine ma
-00004490: 7472 6978 2066 726f 6d20 224c 5053 2220  trix from "LPS" 
-000044a0: 746f 2022 5241 5322 2e20 4465 6661 756c  to "RAS". Defaul
-000044b0: 7473 2074 6f20 6060 5472 7565 6060 2e0a  ts to ``True``..
-000044c0: 2020 2020 2020 2020 2020 2020 5365 7420              Set 
-000044d0: 746f 2060 6054 7275 6560 6020 746f 2062  to ``True`` to b
-000044e0: 6520 636f 6e73 6973 7465 6e74 2077 6974  e consistent wit
-000044f0: 6820 6060 4e69 6261 6265 6c52 6561 6465  h ``NibabelReade
-00004500: 7260 602c 0a20 2020 2020 2020 2020 2020  r``,.           
-00004510: 206f 7468 6572 7769 7365 2074 6865 2061   otherwise the a
-00004520: 6666 696e 6520 6d61 7472 6978 2072 656d  ffine matrix rem
-00004530: 6169 6e73 2069 6e20 7468 6520 4469 636f  ains in the Dico
-00004540: 6d20 636f 6e76 656e 7469 6f6e 2e0a 2020  m convention..  
-00004550: 2020 2020 2020 7377 6170 5f69 6a3a 2077        swap_ij: w
-00004560: 6865 7468 6572 2074 6f20 7377 6170 2074  hether to swap t
-00004570: 6865 2066 6972 7374 2074 776f 2073 7061  he first two spa
-00004580: 7469 616c 2061 7865 732e 2044 6566 6175  tial axes. Defau
-00004590: 6c74 2074 6f20 6060 5472 7565 6060 2c20  lt to ``True``, 
-000045a0: 736f 2074 6861 7420 7468 6520 6f75 7470  so that the outp
-000045b0: 7574 730a 2020 2020 2020 2020 2020 2020  uts.            
-000045c0: 6172 6520 636f 6e73 6973 7465 6e74 2077  are consistent w
-000045d0: 6974 6820 7468 6520 6f74 6865 7220 7265  ith the other re
-000045e0: 6164 6572 732e 0a20 2020 2020 2020 2070  aders..        p
-000045f0: 7275 6e65 5f6d 6574 6164 6174 613a 2077  rune_metadata: w
-00004600: 6865 7468 6572 2074 6f20 7072 756e 6520  hether to prune 
-00004610: 7468 6520 7361 7665 6420 696e 666f 726d  the saved inform
-00004620: 6174 696f 6e20 696e 206d 6574 6164 6174  ation in metadat
-00004630: 612e 2054 6869 7320 6172 6775 6d65 6e74  a. This argument
-00004640: 2069 7320 7573 6564 2066 6f72 0a20 2020   is used for.   
-00004650: 2020 2020 2020 2020 2060 6765 745f 6461           `get_da
-00004660: 7461 6020 6675 6e63 7469 6f6e 2e20 4966  ta` function. If
-00004670: 2054 7275 652c 206f 6e6c 7920 6974 656d   True, only item
-00004680: 7320 7468 6174 2061 7265 2072 656c 6174  s that are relat
-00004690: 6564 2074 6f20 7468 6520 6166 6669 6e65  ed to the affine
-000046a0: 206d 6174 7269 7820 7769 6c6c 2062 6520   matrix will be 
-000046b0: 7361 7665 642e 0a20 2020 2020 2020 2020  saved..         
-000046c0: 2020 2044 6566 6175 6c74 2074 6f20 6060     Default to ``
-000046d0: 5472 7565 6060 2e0a 2020 2020 2020 2020  True``..        
-000046e0: 6c61 6265 6c5f 6469 6374 3a20 6c61 6265  label_dict: labe
-000046f0: 6c20 6f66 2074 6865 2064 6963 6f6d 2064  l of the dicom d
-00004700: 6174 612e 2049 6620 7072 6f76 6964 6564  ata. If provided
-00004710: 2c20 6974 2077 696c 6c20 6265 2075 7365  , it will be use
-00004720: 6420 7768 656e 206c 6f61 6469 6e67 2073  d when loading s
-00004730: 6567 6d65 6e74 6174 696f 6e20 6461 7461  egmentation data
-00004740: 2e0a 2020 2020 2020 2020 2020 2020 4b65  ..            Ke
-00004750: 7973 206f 6620 7468 6520 6469 6374 2061  ys of the dict a
-00004760: 7265 2074 6865 2063 6c61 7373 6573 2c20  re the classes, 
-00004770: 616e 6420 7661 6c75 6573 2061 7265 2074  and values are t
-00004780: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00004790: 2063 6c61 7373 206e 756d 6265 722e 2046   class number. F
-000047a0: 6f72 2065 7861 6d70 6c65 3a0a 2020 2020  or example:.    
-000047b0: 2020 2020 2020 2020 666f 7220 5443 4941          for TCIA
-000047c0: 2063 6f6c 6c65 6374 696f 6e20 2243 344b   collection "C4K
-000047d0: 432d 4b69 5453 222c 2069 7420 6361 6e20  C-KiTS", it can 
-000047e0: 6265 3a20 7b22 4b69 646e 6579 223a 2030  be: {"Kidney": 0
-000047f0: 2c20 2252 656e 616c 2054 756d 6f72 223a  , "Renal Tumor":
-00004800: 2031 7d2e 0a20 2020 2020 2020 206b 7761   1}..        kwa
-00004810: 7267 733a 2061 6464 6974 696f 6e61 6c20  rgs: additional 
-00004820: 6172 6773 2066 6f72 2060 7079 6469 636f  args for `pydico
-00004830: 6d2e 6463 6d72 6561 6460 2041 5049 2e20  m.dcmread` API. 
-00004840: 6d6f 7265 2064 6574 6169 6c73 2061 626f  more details abo
-00004850: 7574 2061 7661 696c 6162 6c65 2061 7267  ut available arg
-00004860: 733a 0a20 2020 2020 2020 2020 2020 2068  s:.            h
-00004870: 7474 7073 3a2f 2f70 7964 6963 6f6d 2e67  ttps://pydicom.g
-00004880: 6974 6875 622e 696f 2f70 7964 6963 6f6d  ithub.io/pydicom
-00004890: 2f73 7461 626c 652f 7265 6665 7265 6e63  /stable/referenc
-000048a0: 652f 6765 6e65 7261 7465 642f 7079 6469  e/generated/pydi
-000048b0: 636f 6d2e 6669 6c65 7265 6164 6572 2e64  com.filereader.d
-000048c0: 636d 7265 6164 2e68 746d 6c23 7079 6469  cmread.html#pydi
-000048d0: 636f 6d2e 6669 6c65 7265 6164 6572 2e64  com.filereader.d
-000048e0: 636d 7265 6164 0a20 2020 2020 2020 2020  cmread.         
-000048f0: 2020 2049 6620 7468 6520 6067 6574 5f64     If the `get_d
-00004900: 6174 6160 2066 756e 6374 696f 6e20 7769  ata` function wi
-00004910: 6c6c 2062 6520 6361 6c6c 6564 0a20 2020  ll be called.   
-00004920: 2020 2020 2020 2020 2028 666f 7220 6578           (for ex
-00004930: 616d 706c 652c 2077 6865 6e20 7573 696e  ample, when usin
-00004940: 6720 7468 6973 2072 6561 6465 7220 7769  g this reader wi
-00004950: 7468 2060 6d6f 6e61 692e 7472 616e 7366  th `monai.transf
-00004960: 6f72 6d73 2e4c 6f61 6449 6d61 6765 6029  orms.LoadImage`)
-00004970: 2c20 706c 6561 7365 2065 6e73 7572 6520  , please ensure 
-00004980: 7468 6174 2074 6865 2061 7267 756d 656e  that the argumen
-00004990: 740a 2020 2020 2020 2020 2020 2020 6073  t.            `s
-000049a0: 746f 705f 6265 666f 7265 5f70 6978 656c  top_before_pixel
-000049b0: 7360 2069 7320 6054 7275 6560 2c20 616e  s` is `True`, an
-000049c0: 6420 6073 7065 6369 6669 635f 7461 6773  d `specific_tags
-000049d0: 6020 636f 7665 7273 2061 6c6c 206e 6563  ` covers all nec
-000049e0: 6573 7361 7279 2074 6167 732c 2073 7563  essary tags, suc
-000049f0: 6820 6173 2060 5069 7865 6c53 7061 6369  h as `PixelSpaci
-00004a00: 6e67 602c 0a20 2020 2020 2020 2020 2020  ng`,.           
-00004a10: 2060 496d 6167 6550 6f73 6974 696f 6e50   `ImagePositionP
-00004a20: 6174 6965 6e74 602c 2060 496d 6167 654f  atient`, `ImageO
-00004a30: 7269 656e 7461 7469 6f6e 5061 7469 656e  rientationPatien
-00004a40: 7460 2061 6e64 2061 6c6c 2060 7069 7865  t` and all `pixe
-00004a50: 6c5f 6172 7261 7960 2072 656c 6174 6564  l_array` related
-00004a60: 2074 6167 732e 0a20 2020 2022 2222 0a0a   tags..    """..
-00004a70: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00004a80: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00004a90: 2020 2020 2020 2020 6368 616e 6e65 6c5f          channel_
-00004aa0: 6469 6d3a 2073 7472 207c 2069 6e74 207c  dim: str | int |
-00004ab0: 204e 6f6e 6520 3d20 4e6f 6e65 2c0a 2020   None = None,.  
-00004ac0: 2020 2020 2020 6166 6669 6e65 5f6c 7073        affine_lps
-00004ad0: 5f74 6f5f 7261 733a 2062 6f6f 6c20 3d20  _to_ras: bool = 
-00004ae0: 5472 7565 2c0a 2020 2020 2020 2020 7377  True,.        sw
-00004af0: 6170 5f69 6a3a 2062 6f6f 6c20 3d20 5472  ap_ij: bool = Tr
-00004b00: 7565 2c0a 2020 2020 2020 2020 7072 756e  ue,.        prun
-00004b10: 655f 6d65 7461 6461 7461 3a20 626f 6f6c  e_metadata: bool
-00004b20: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-00004b30: 206c 6162 656c 5f64 6963 743a 2064 6963   label_dict: dic
-00004b40: 7420 7c20 4e6f 6e65 203d 204e 6f6e 652c  t | None = None,
-00004b50: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
-00004b60: 732c 0a20 2020 2029 3a0a 2020 2020 2020  s,.    ):.      
-00004b70: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00004b80: 5f5f 2829 0a20 2020 2020 2020 2073 656c  __().        sel
-00004b90: 662e 6b77 6172 6773 203d 206b 7761 7267  f.kwargs = kwarg
-00004ba0: 730a 2020 2020 2020 2020 7365 6c66 2e63  s.        self.c
-00004bb0: 6861 6e6e 656c 5f64 696d 203d 2066 6c6f  hannel_dim = flo
-00004bc0: 6174 2822 6e61 6e22 2920 6966 2063 6861  at("nan") if cha
-00004bd0: 6e6e 656c 5f64 696d 203d 3d20 226e 6f5f  nnel_dim == "no_
-00004be0: 6368 616e 6e65 6c22 2065 6c73 6520 6368  channel" else ch
-00004bf0: 616e 6e65 6c5f 6469 6d0a 2020 2020 2020  annel_dim.      
-00004c00: 2020 7365 6c66 2e61 6666 696e 655f 6c70    self.affine_lp
-00004c10: 735f 746f 5f72 6173 203d 2061 6666 696e  s_to_ras = affin
-00004c20: 655f 6c70 735f 746f 5f72 6173 0a20 2020  e_lps_to_ras.   
-00004c30: 2020 2020 2073 656c 662e 7377 6170 5f69       self.swap_i
-00004c40: 6a20 3d20 7377 6170 5f69 6a0a 2020 2020  j = swap_ij.    
-00004c50: 2020 2020 7365 6c66 2e70 7275 6e65 5f6d      self.prune_m
-00004c60: 6574 6164 6174 6120 3d20 7072 756e 655f  etadata = prune_
-00004c70: 6d65 7461 6461 7461 0a20 2020 2020 2020  metadata.       
-00004c80: 2073 656c 662e 6c61 6265 6c5f 6469 6374   self.label_dict
-00004c90: 203d 206c 6162 656c 5f64 6963 740a 0a20   = label_dict.. 
-00004ca0: 2020 2064 6566 2076 6572 6966 795f 7375     def verify_su
-00004cb0: 6666 6978 2873 656c 662c 2066 696c 656e  ffix(self, filen
-00004cc0: 616d 653a 2053 6571 7565 6e63 655b 5061  ame: Sequence[Pa
-00004cd0: 7468 4c69 6b65 5d20 7c20 5061 7468 4c69  thLike] | PathLi
-00004ce0: 6b65 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ke) -> bool:.   
-00004cf0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004d00: 2056 6572 6966 7920 7768 6574 6865 7220   Verify whether 
-00004d10: 7468 6520 7370 6563 6966 6965 6420 6669  the specified fi
-00004d20: 6c65 206f 7220 6669 6c65 7320 666f 726d  le or files form
-00004d30: 6174 2069 7320 7375 7070 6f72 7465 6420  at is supported 
-00004d40: 6279 2050 7964 6963 6f6d 2072 6561 6465  by Pydicom reade
-00004d50: 722e 0a0a 2020 2020 2020 2020 4172 6773  r...        Args
-00004d60: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-00004d70: 6c65 6e61 6d65 3a20 6669 6c65 206e 616d  lename: file nam
-00004d80: 6520 6f72 2061 206c 6973 7420 6f66 2066  e or a list of f
-00004d90: 696c 6520 6e61 6d65 7320 746f 2072 6561  ile names to rea
-00004da0: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
-00004db0: 2020 2069 6620 6120 6c69 7374 206f 6620     if a list of 
-00004dc0: 6669 6c65 732c 2076 6572 6966 7920 616c  files, verify al
-00004dd0: 6c20 7468 6520 7375 6666 6978 6573 2e0a  l the suffixes..
-00004de0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00004df0: 2020 2020 2072 6574 7572 6e20 6861 735f       return has_
-00004e00: 7079 6469 636f 6d0a 0a20 2020 2064 6566  pydicom..    def
-00004e10: 2072 6561 6428 7365 6c66 2c20 6461 7461   read(self, data
-00004e20: 3a20 5365 7175 656e 6365 5b50 6174 684c  : Sequence[PathL
-00004e30: 696b 655d 207c 2050 6174 684c 696b 652c  ike] | PathLike,
-00004e40: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00004e50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00004e60: 5265 6164 2069 6d61 6765 2064 6174 6120  Read image data 
-00004e70: 6672 6f6d 2073 7065 6369 6669 6564 2066  from specified f
-00004e80: 696c 6520 6f72 2066 696c 6573 2c20 6974  ile or files, it
-00004e90: 2063 616e 2072 6561 6420 6120 6c69 7374   can read a list
-00004ea0: 206f 6620 696d 6167 6573 0a20 2020 2020   of images.     
-00004eb0: 2020 2061 6e64 2073 7461 636b 2074 6865     and stack the
-00004ec0: 6d20 746f 6765 7468 6572 2061 7320 6d75  m together as mu
-00004ed0: 6c74 692d 6368 616e 6e65 6c20 6461 7461  lti-channel data
-00004ee0: 2069 6e20 6067 6574 5f64 6174 6128 2960   in `get_data()`
-00004ef0: 2e0a 2020 2020 2020 2020 4966 2070 6173  ..        If pas
-00004f00: 7369 6e67 2064 6972 6563 746f 7279 2070  sing directory p
-00004f10: 6174 6820 696e 7374 6561 6420 6f66 2066  ath instead of f
-00004f20: 696c 6520 7061 7468 2c20 7769 6c6c 2074  ile path, will t
-00004f30: 7265 6174 2069 7420 6173 2044 4943 4f4d  reat it as DICOM
-00004f40: 2069 6d61 6765 7320 7365 7269 6573 2061   images series a
-00004f50: 6e64 2072 6561 642e 0a0a 2020 2020 2020  nd read...      
-00004f60: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00004f70: 2020 2020 6461 7461 3a20 6669 6c65 206e      data: file n
-00004f80: 616d 6520 6f72 2061 206c 6973 7420 6f66  ame or a list of
-00004f90: 2066 696c 6520 6e61 6d65 7320 746f 2072   file names to r
-00004fa0: 6561 642c 0a20 2020 2020 2020 2020 2020  ead,.           
-00004fb0: 206b 7761 7267 733a 2061 6464 6974 696f   kwargs: additio
-00004fc0: 6e61 6c20 6172 6773 2066 6f72 2060 7079  nal args for `py
-00004fd0: 6469 636f 6d2e 6463 6d72 6561 6460 2041  dicom.dcmread` A
-00004fe0: 5049 2c20 7769 6c6c 206f 7665 7272 6964  PI, will overrid
-00004ff0: 6520 6073 656c 662e 6b77 6172 6773 6020  e `self.kwargs` 
-00005000: 666f 7220 6578 6973 7469 6e67 206b 6579  for existing key
-00005010: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
-00005020: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00005030: 2049 6620 6064 6174 6160 2072 6570 7265   If `data` repre
-00005040: 7365 6e74 7320 6120 6669 6c65 6e61 6d65  sents a filename
-00005050: 3a20 7265 7475 726e 2061 2070 7964 6963  : return a pydic
-00005060: 6f6d 2064 6174 6173 6574 206f 626a 6563  om dataset objec
-00005070: 742e 0a20 2020 2020 2020 2020 2020 2049  t..            I
-00005080: 6620 6064 6174 6160 2072 6570 7265 7365  f `data` represe
-00005090: 6e74 7320 6120 6c69 7374 206f 6620 6669  nts a list of fi
-000050a0: 6c65 6e61 6d65 7320 6f72 2061 2064 6972  lenames or a dir
-000050b0: 6563 746f 7279 3a20 7265 7475 726e 2061  ectory: return a
-000050c0: 206c 6973 7420 6f66 2070 7964 6963 6f6d   list of pydicom
-000050d0: 2064 6174 6173 6574 206f 626a 6563 742e   dataset object.
-000050e0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-000050f0: 6064 6174 6160 2072 6570 7265 7365 6e74  `data` represent
-00005100: 7320 6120 6c69 7374 206f 6620 6469 7265  s a list of dire
-00005110: 6374 6f72 6965 733a 2072 6574 7572 6e20  ctories: return 
-00005120: 6120 6c69 7374 206f 6620 6c69 7374 206f  a list of list o
-00005130: 6620 7079 6469 636f 6d20 6461 7461 7365  f pydicom datase
-00005140: 7420 6f62 6a65 6374 2e0a 0a20 2020 2020  t object...     
-00005150: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00005160: 6d67 5f20 3d20 5b5d 0a0a 2020 2020 2020  mg_ = []..      
-00005170: 2020 6669 6c65 6e61 6d65 733a 2053 6571    filenames: Seq
-00005180: 7565 6e63 655b 5061 7468 4c69 6b65 5d20  uence[PathLike] 
-00005190: 3d20 656e 7375 7265 5f74 7570 6c65 2864  = ensure_tuple(d
-000051a0: 6174 6129 0a20 2020 2020 2020 206b 7761  ata).        kwa
-000051b0: 7267 735f 203d 2073 656c 662e 6b77 6172  rgs_ = self.kwar
-000051c0: 6773 2e63 6f70 7928 290a 2020 2020 2020  gs.copy().      
-000051d0: 2020 6b77 6172 6773 5f2e 7570 6461 7465    kwargs_.update
-000051e0: 286b 7761 7267 7329 0a0a 2020 2020 2020  (kwargs)..      
-000051f0: 2020 7365 6c66 2e68 6173 5f73 6572 6965    self.has_serie
-00005200: 7320 3d20 4661 6c73 650a 0a20 2020 2020  s = False..     
-00005210: 2020 2066 6f72 206e 616d 6520 696e 2066     for name in f
-00005220: 696c 656e 616d 6573 3a0a 2020 2020 2020  ilenames:.      
-00005230: 2020 2020 2020 6e61 6d65 203d 2066 227b        name = f"{
-00005240: 6e61 6d65 7d22 0a20 2020 2020 2020 2020  name}".         
-00005250: 2020 2069 6620 5061 7468 286e 616d 6529     if Path(name)
-00005260: 2e69 735f 6469 7228 293a 0a20 2020 2020  .is_dir():.     
-00005270: 2020 2020 2020 2020 2020 2023 2072 6561             # rea
-00005280: 6420 4449 434f 4d20 7365 7269 6573 0a20  d DICOM series. 
-00005290: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000052a0: 6572 6965 735f 736c 6373 203d 2067 6c6f  eries_slcs = glo
-000052b0: 622e 676c 6f62 286f 732e 7061 7468 2e6a  b.glob(os.path.j
-000052c0: 6f69 6e28 6e61 6d65 2c20 222a 2229 290a  oin(name, "*")).
-000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052e0: 7365 7269 6573 5f73 6c63 7320 3d20 5b73  series_slcs = [s
-000052f0: 6c63 2066 6f72 2073 6c63 2069 6e20 7365  lc for slc in se
-00005300: 7269 6573 5f73 6c63 7320 6966 2022 4c49  ries_slcs if "LI
-00005310: 4345 4e53 4522 206e 6f74 2069 6e20 736c  CENSE" not in sl
-00005320: 635d 0a20 2020 2020 2020 2020 2020 2020  c].             
-00005330: 2020 2073 6c69 6365 7320 3d20 5b70 7964     slices = [pyd
-00005340: 6963 6f6d 2e64 636d 7265 6164 2866 703d  icom.dcmread(fp=
-00005350: 736c 632c 202a 2a6b 7761 7267 735f 2920  slc, **kwargs_) 
-00005360: 666f 7220 736c 6320 696e 2073 6572 6965  for slc in serie
-00005370: 735f 736c 6373 5d0a 2020 2020 2020 2020  s_slcs].        
-00005380: 2020 2020 2020 2020 696d 675f 2e61 7070          img_.app
-00005390: 656e 6428 736c 6963 6573 2069 6620 6c65  end(slices if le
-000053a0: 6e28 736c 6963 6573 2920 3e20 3120 656c  n(slices) > 1 el
-000053b0: 7365 2073 6c69 6365 735b 305d 290a 2020  se slices[0]).  
-000053c0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000053d0: 206c 656e 2873 6c69 6365 7329 203e 2031   len(slices) > 1
-000053e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000053f0: 2020 2020 2020 7365 6c66 2e68 6173 5f73        self.has_s
-00005400: 6572 6965 7320 3d20 5472 7565 0a20 2020  eries = True.   
-00005410: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00005420: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00005430: 7320 3d20 7079 6469 636f 6d2e 6463 6d72  s = pydicom.dcmr
-00005440: 6561 6428 6670 3d6e 616d 652c 202a 2a6b  ead(fp=name, **k
-00005450: 7761 7267 735f 290a 2020 2020 2020 2020  wargs_).        
-00005460: 2020 2020 2020 2020 696d 675f 2e61 7070          img_.app
-00005470: 656e 6428 6473 290a 2020 2020 2020 2020  end(ds).        
-00005480: 7265 7475 726e 2069 6d67 5f20 6966 206c  return img_ if l
-00005490: 656e 2866 696c 656e 616d 6573 2920 3e20  en(filenames) > 
-000054a0: 3120 656c 7365 2069 6d67 5f5b 305d 0a0a  1 else img_[0]..
-000054b0: 2020 2020 6465 6620 5f63 6f6d 6269 6e65      def _combine
-000054c0: 5f64 6963 6f6d 5f73 6572 6965 7328 7365  _dicom_series(se
-000054d0: 6c66 2c20 6461 7461 3a20 4974 6572 6162  lf, data: Iterab
-000054e0: 6c65 293a 0a20 2020 2020 2020 2022 2222  le):.        """
-000054f0: 0a20 2020 2020 2020 2043 6f6d 6269 6e65  .        Combine
-00005500: 2064 6963 6f6d 2073 6572 6965 7320 2861   dicom series (a
-00005510: 206c 6973 7420 6f66 2070 7964 6963 6f6d   list of pydicom
-00005520: 2064 6174 6173 6574 206f 626a 6563 7473   dataset objects
-00005530: 292e 2054 6865 6972 2064 6174 6120 6172  ). Their data ar
-00005540: 7261 7973 2077 696c 6c20 6265 2073 7461  rays will be sta
-00005550: 636b 6564 2074 6f67 6574 6865 7220 6174  cked together at
-00005560: 2061 206e 6577 0a20 2020 2020 2020 2064   a new.        d
-00005570: 696d 656e 7369 6f6e 2061 7320 7468 6520  imension as the 
-00005580: 6c61 7374 2064 696d 656e 7369 6f6e 2e0a  last dimension..
-00005590: 0a20 2020 2020 2020 2054 6865 2073 7461  .        The sta
-000055a0: 636b 206f 7264 6572 2064 6570 656e 6473  ck order depends
-000055b0: 206f 6e20 496e 7374 616e 6365 204e 756d   on Instance Num
-000055c0: 6265 722e 2054 6865 206d 6574 6164 6174  ber. The metadat
-000055d0: 6120 7769 6c6c 2062 6520 6261 7365 6420  a will be based 
-000055e0: 6f6e 2074 6865 0a20 2020 2020 2020 2066  on the.        f
-000055f0: 6972 7374 2073 6c69 6365 2773 206d 6574  irst slice's met
-00005600: 6164 6174 612c 2061 6e64 2073 6f6d 6520  adata, and some 
-00005610: 6e65 7720 6974 656d 7320 7769 6c6c 2062  new items will b
-00005620: 6520 6164 6465 643a 0a0a 2020 2020 2020  e added:..      
-00005630: 2020 2273 7061 6369 6e67 223a 2074 6865    "spacing": the
-00005640: 206e 6577 2073 7061 6369 6e67 206f 6620   new spacing of 
-00005650: 7468 6520 7374 6163 6b65 6420 736c 6963  the stacked slic
-00005660: 6573 2e0a 2020 2020 2020 2020 226c 6173  es..        "las
-00005670: 7449 6d61 6765 506f 7369 7469 6f6e 5061  tImagePositionPa
-00005680: 7469 656e 7422 3a20 6049 6d61 6765 506f  tient": `ImagePo
-00005690: 7369 7469 6f6e 5061 7469 656e 7460 2066  sitionPatient` f
-000056a0: 6f72 2074 6865 206c 6173 7420 736c 6963  or the last slic
-000056b0: 652c 2069 7420 7769 6c6c 2062 6520 7573  e, it will be us
-000056c0: 6564 2074 6f20 6163 6869 6576 6520 7468  ed to achieve th
-000056d0: 6520 6166 6669 6e65 0a20 2020 2020 2020  e affine.       
-000056e0: 2020 2020 206d 6174 7269 782e 0a20 2020       matrix..   
-000056f0: 2020 2020 2022 7370 6174 6961 6c5f 7368       "spatial_sh
-00005700: 6170 6522 3a20 7468 6520 7370 6174 6961  ape": the spatia
-00005710: 6c20 7368 6170 6520 6f66 2074 6865 2073  l shape of the s
-00005720: 7461 636b 6564 2073 6c69 6365 732e 0a0a  tacked slices...
-00005730: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00005740: 2020 2020 2020 2020 2020 6461 7461 3a20            data: 
-00005750: 6120 6c69 7374 206f 6620 7079 6469 636f  a list of pydico
-00005760: 6d20 6461 7461 7365 7420 6f62 6a65 6374  m dataset object
-00005770: 732e 0a20 2020 2020 2020 2052 6574 7572  s..        Retur
-00005780: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00005790: 6120 7475 706c 6520 7468 6174 2063 6f6e  a tuple that con
-000057a0: 7369 7374 6564 2077 6974 6820 6461 7461  sisted with data
-000057b0: 2061 7272 6179 2061 6e64 206d 6574 6164   array and metad
-000057c0: 6174 612e 0a20 2020 2020 2020 2022 2222  ata..        """
-000057d0: 0a20 2020 2020 2020 2073 6c69 6365 733a  .        slices:
-000057e0: 206c 6973 7420 3d20 5b5d 0a20 2020 2020   list = [].     
-000057f0: 2020 2023 2066 6f72 2061 2064 6963 6f6d     # for a dicom
-00005800: 2073 6572 6965 730a 2020 2020 2020 2020   series.        
-00005810: 666f 7220 736c 635f 6473 2069 6e20 6461  for slc_ds in da
-00005820: 7461 3a0a 2020 2020 2020 2020 2020 2020  ta:.            
-00005830: 6966 2068 6173 6174 7472 2873 6c63 5f64  if hasattr(slc_d
-00005840: 732c 2022 496e 7374 616e 6365 4e75 6d62  s, "InstanceNumb
-00005850: 6572 2229 3a0a 2020 2020 2020 2020 2020  er"):.          
-00005860: 2020 2020 2020 736c 6963 6573 2e61 7070        slices.app
-00005870: 656e 6428 736c 635f 6473 290a 2020 2020  end(slc_ds).    
-00005880: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00005890: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-000058a0: 726e 696e 6773 2e77 6172 6e28 6622 736c  rnings.warn(f"sl
-000058b0: 6963 653a 207b 736c 635f 6473 2e66 696c  ice: {slc_ds.fil
-000058c0: 656e 616d 657d 2064 6f65 7320 6e6f 7420  ename} does not 
-000058d0: 6861 7665 2049 6e73 7461 6e63 654e 756d  have InstanceNum
-000058e0: 6265 7220 7461 672c 2073 6b69 7020 6974  ber tag, skip it
-000058f0: 2e22 290a 2020 2020 2020 2020 736c 6963  .").        slic
-00005900: 6573 203d 2073 6f72 7465 6428 736c 6963  es = sorted(slic
-00005910: 6573 2c20 6b65 793d 6c61 6d62 6461 2073  es, key=lambda s
-00005920: 3a20 732e 496e 7374 616e 6365 4e75 6d62  : s.InstanceNumb
-00005930: 6572 2920 2023 2074 7970 653a 2069 676e  er)  # type: ign
-00005940: 6f72 650a 0a20 2020 2020 2020 2069 6620  ore..        if 
-00005950: 6c65 6e28 736c 6963 6573 2920 3d3d 2030  len(slices) == 0
-00005960: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00005970: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00005980: 7468 6520 696e 7075 7420 646f 6573 206e  the input does n
-00005990: 6f74 2068 6176 6520 7661 6c69 6420 736c  ot have valid sl
-000059a0: 6963 6573 2e22 290a 0a20 2020 2020 2020  ices.")..       
-000059b0: 2066 6972 7374 5f73 6c69 6365 203d 2073   first_slice = s
-000059c0: 6c69 6365 735b 305d 0a20 2020 2020 2020  lices[0].       
-000059d0: 2061 7665 7261 6765 5f64 6973 7461 6e63   average_distanc
-000059e0: 6520 3d20 302e 300a 2020 2020 2020 2020  e = 0.0.        
-000059f0: 6669 7273 745f 6172 7261 7920 3d20 7365  first_array = se
-00005a00: 6c66 2e5f 6765 745f 6172 7261 795f 6461  lf._get_array_da
-00005a10: 7461 2866 6972 7374 5f73 6c69 6365 290a  ta(first_slice).
-00005a20: 2020 2020 2020 2020 7368 6170 6520 3d20          shape = 
-00005a30: 6669 7273 745f 6172 7261 792e 7368 6170  first_array.shap
-00005a40: 650a 2020 2020 2020 2020 7370 6163 696e  e.        spacin
-00005a50: 6720 3d20 6765 7461 7474 7228 6669 7273  g = getattr(firs
-00005a60: 745f 736c 6963 652c 2022 5069 7865 6c53  t_slice, "PixelS
-00005a70: 7061 6369 6e67 222c 205b 312e 302c 2031  pacing", [1.0, 1
-00005a80: 2e30 2c20 312e 305d 290a 2020 2020 2020  .0, 1.0]).      
-00005a90: 2020 706f 7320 3d20 6765 7461 7474 7228    pos = getattr(
-00005aa0: 6669 7273 745f 736c 6963 652c 2022 496d  first_slice, "Im
-00005ab0: 6167 6550 6f73 6974 696f 6e50 6174 6965  agePositionPatie
-00005ac0: 6e74 222c 2028 302e 302c 2030 2e30 2c20  nt", (0.0, 0.0, 
-00005ad0: 302e 3029 295b 325d 0a20 2020 2020 2020  0.0))[2].       
-00005ae0: 2073 7461 636b 5f61 7272 6179 203d 205b   stack_array = [
-00005af0: 6669 7273 745f 6172 7261 795d 0a20 2020  first_array].   
-00005b00: 2020 2020 2066 6f72 2069 6478 2069 6e20       for idx in 
-00005b10: 7261 6e67 6528 312c 206c 656e 2873 6c69  range(1, len(sli
-00005b20: 6365 7329 293a 0a20 2020 2020 2020 2020  ces)):.         
-00005b30: 2020 2073 6c63 5f61 7272 6179 203d 2073     slc_array = s
-00005b40: 656c 662e 5f67 6574 5f61 7272 6179 5f64  elf._get_array_d
-00005b50: 6174 6128 736c 6963 6573 5b69 6478 5d29  ata(slices[idx])
-00005b60: 0a20 2020 2020 2020 2020 2020 2073 6c63  .            slc
-00005b70: 5f73 6861 7065 203d 2073 6c63 5f61 7272  _shape = slc_arr
-00005b80: 6179 2e73 6861 7065 0a20 2020 2020 2020  ay.shape.       
-00005b90: 2020 2020 2073 6c63 5f73 7061 6369 6e67       slc_spacing
-00005ba0: 203d 2067 6574 6174 7472 2866 6972 7374   = getattr(first
-00005bb0: 5f73 6c69 6365 2c20 2250 6978 656c 5370  _slice, "PixelSp
-00005bc0: 6163 696e 6722 2c20 2831 2e30 2c20 312e  acing", (1.0, 1.
-00005bd0: 302c 2031 2e30 2929 0a20 2020 2020 2020  0, 1.0)).       
-00005be0: 2020 2020 2073 6c63 5f70 6f73 203d 2067       slc_pos = g
-00005bf0: 6574 6174 7472 2866 6972 7374 5f73 6c69  etattr(first_sli
-00005c00: 6365 2c20 2249 6d61 6765 506f 7369 7469  ce, "ImagePositi
-00005c10: 6f6e 5061 7469 656e 7422 2c20 2830 2e30  onPatient", (0.0
-00005c20: 2c20 302e 302c 2066 6c6f 6174 2869 6478  , 0.0, float(idx
-00005c30: 2929 295b 325d 0a20 2020 2020 2020 2020  )))[2].         
-00005c40: 2020 2069 6620 7370 6163 696e 6720 213d     if spacing !=
-00005c50: 2073 6c63 5f73 7061 6369 6e67 3a0a 2020   slc_spacing:.  
-00005c60: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-00005c70: 726e 696e 6773 2e77 6172 6e28 6622 7468  rnings.warn(f"th
-00005c80: 6520 6c69 7374 2063 6f6e 7461 696e 7320  e list contains 
-00005c90: 736c 6963 6573 2074 6861 7420 6861 7665  slices that have
-00005ca0: 2064 6966 6665 7265 6e74 2073 7061 6369   different spaci
-00005cb0: 6e67 7320 7b73 7061 6369 6e67 7d20 616e  ngs {spacing} an
-00005cc0: 6420 7b73 6c63 5f73 7061 6369 6e67 7d2e  d {slc_spacing}.
-00005cd0: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-00005ce0: 6620 7368 6170 6520 213d 2073 6c63 5f73  f shape != slc_s
-00005cf0: 6861 7065 3a0a 2020 2020 2020 2020 2020  hape:.          
-00005d00: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00005d10: 6172 6e28 6622 7468 6520 6c69 7374 2063  arn(f"the list c
-00005d20: 6f6e 7461 696e 7320 736c 6963 6573 2074  ontains slices t
-00005d30: 6861 7420 6861 7665 2064 6966 6665 7265  hat have differe
-00005d40: 6e74 2073 6861 7065 7320 7b73 6861 7065  nt shapes {shape
-00005d50: 7d20 616e 6420 7b73 6c63 5f73 6861 7065  } and {slc_shape
-00005d60: 7d2e 2229 0a20 2020 2020 2020 2020 2020  }.").           
-00005d70: 2061 7665 7261 6765 5f64 6973 7461 6e63   average_distanc
-00005d80: 6520 2b3d 2061 6273 2870 6f73 202d 2073  e += abs(pos - s
-00005d90: 6c63 5f70 6f73 290a 2020 2020 2020 2020  lc_pos).        
-00005da0: 2020 2020 706f 7320 3d20 736c 635f 706f      pos = slc_po
-00005db0: 730a 2020 2020 2020 2020 2020 2020 7374  s.            st
-00005dc0: 6163 6b5f 6172 7261 792e 6170 7065 6e64  ack_array.append
-00005dd0: 2873 6c63 5f61 7272 6179 290a 0a20 2020  (slc_array)..   
-00005de0: 2020 2020 2069 6620 6c65 6e28 736c 6963       if len(slic
-00005df0: 6573 2920 3e20 313a 0a20 2020 2020 2020  es) > 1:.       
-00005e00: 2020 2020 2061 7665 7261 6765 5f64 6973       average_dis
-00005e10: 7461 6e63 6520 2f3d 206c 656e 2873 6c69  tance /= len(sli
-00005e20: 6365 7329 202d 2031 0a20 2020 2020 2020  ces) - 1.       
-00005e30: 2020 2020 2073 7061 6369 6e67 2e61 7070       spacing.app
-00005e40: 656e 6428 6176 6572 6167 655f 6469 7374  end(average_dist
-00005e50: 616e 6365 290a 2020 2020 2020 2020 2020  ance).          
-00005e60: 2020 7374 6163 6b5f 6172 7261 7920 3d20    stack_array = 
-00005e70: 6e70 2e73 7461 636b 2873 7461 636b 5f61  np.stack(stack_a
-00005e80: 7272 6179 2c20 6178 6973 3d2d 3129 0a20  rray, axis=-1). 
-00005e90: 2020 2020 2020 2020 2020 2073 7461 636b             stack
-00005ea0: 5f6d 6574 6164 6174 6120 3d20 7365 6c66  _metadata = self
-00005eb0: 2e5f 6765 745f 6d65 7461 5f64 6963 7428  ._get_meta_dict(
-00005ec0: 6669 7273 745f 736c 6963 6529 0a20 2020  first_slice).   
-00005ed0: 2020 2020 2020 2020 2073 7461 636b 5f6d           stack_m
-00005ee0: 6574 6164 6174 615b 2273 7061 6369 6e67  etadata["spacing
-00005ef0: 225d 203d 206e 702e 6173 6172 7261 7928  "] = np.asarray(
-00005f00: 7370 6163 696e 6729 0a20 2020 2020 2020  spacing).       
-00005f10: 2020 2020 2069 6620 6861 7361 7474 7228       if hasattr(
-00005f20: 736c 6963 6573 5b2d 315d 2c20 2249 6d61  slices[-1], "Ima
-00005f30: 6765 506f 7369 7469 6f6e 5061 7469 656e  gePositionPatien
-00005f40: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
-00005f50: 2020 2020 2073 7461 636b 5f6d 6574 6164       stack_metad
-00005f60: 6174 615b 226c 6173 7449 6d61 6765 506f  ata["lastImagePo
-00005f70: 7369 7469 6f6e 5061 7469 656e 7422 5d20  sitionPatient"] 
-00005f80: 3d20 6e70 2e61 7361 7272 6179 2873 6c69  = np.asarray(sli
-00005f90: 6365 735b 2d31 5d2e 496d 6167 6550 6f73  ces[-1].ImagePos
-00005fa0: 6974 696f 6e50 6174 6965 6e74 290a 2020  itionPatient).  
-00005fb0: 2020 2020 2020 2020 2020 7374 6163 6b5f            stack_
-00005fc0: 6d65 7461 6461 7461 5b4d 6574 614b 6579  metadata[MetaKey
-00005fd0: 732e 5350 4154 4941 4c5f 5348 4150 455d  s.SPATIAL_SHAPE]
-00005fe0: 203d 2073 6861 7065 202b 2028 6c65 6e28   = shape + (len(
-00005ff0: 736c 6963 6573 292c 290a 2020 2020 2020  slices),).      
-00006000: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00006010: 2020 2020 7374 6163 6b5f 6172 7261 7920      stack_array 
-00006020: 3d20 7374 6163 6b5f 6172 7261 795b 305d  = stack_array[0]
-00006030: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-00006040: 636b 5f6d 6574 6164 6174 6120 3d20 7365  ck_metadata = se
-00006050: 6c66 2e5f 6765 745f 6d65 7461 5f64 6963  lf._get_meta_dic
-00006060: 7428 6669 7273 745f 736c 6963 6529 0a20  t(first_slice). 
-00006070: 2020 2020 2020 2020 2020 2073 7461 636b             stack
-00006080: 5f6d 6574 6164 6174 615b 2273 7061 6369  _metadata["spaci
-00006090: 6e67 225d 203d 206e 702e 6173 6172 7261  ng"] = np.asarra
-000060a0: 7928 7370 6163 696e 6729 0a20 2020 2020  y(spacing).     
-000060b0: 2020 2020 2020 2073 7461 636b 5f6d 6574         stack_met
-000060c0: 6164 6174 615b 4d65 7461 4b65 7973 2e53  adata[MetaKeys.S
-000060d0: 5041 5449 414c 5f53 4841 5045 5d20 3d20  PATIAL_SHAPE] = 
-000060e0: 7368 6170 650a 0a20 2020 2020 2020 2072  shape..        r
-000060f0: 6574 7572 6e20 7374 6163 6b5f 6172 7261  eturn stack_arra
-00006100: 792c 2073 7461 636b 5f6d 6574 6164 6174  y, stack_metadat
-00006110: 610a 0a20 2020 2064 6566 2067 6574 5f64  a..    def get_d
-00006120: 6174 6128 7365 6c66 2c20 6461 7461 2920  ata(self, data) 
-00006130: 2d3e 2074 7570 6c65 5b6e 702e 6e64 6172  -> tuple[np.ndar
-00006140: 7261 792c 2064 6963 745d 3a0a 2020 2020  ray, dict]:.    
-00006150: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006160: 4578 7472 6163 7420 6461 7461 2061 7272  Extract data arr
-00006170: 6179 2061 6e64 206d 6574 6164 6174 6120  ay and metadata 
-00006180: 6672 6f6d 206c 6f61 6465 6420 696d 6167  from loaded imag
-00006190: 6520 616e 6420 7265 7475 726e 2074 6865  e and return the
-000061a0: 6d2e 0a20 2020 2020 2020 2054 6869 7320  m..        This 
-000061b0: 6675 6e63 7469 6f6e 2072 6574 7572 6e73  function returns
-000061c0: 2074 776f 206f 626a 6563 7473 2c20 6669   two objects, fi
-000061d0: 7273 7420 6973 206e 756d 7079 2061 7272  rst is numpy arr
-000061e0: 6179 206f 6620 696d 6167 6520 6461 7461  ay of image data
-000061f0: 2c20 7365 636f 6e64 2069 7320 6469 6374  , second is dict
-00006200: 206f 6620 6d65 7461 6461 7461 2e0a 2020   of metadata..  
-00006210: 2020 2020 2020 4974 2063 6f6e 7374 7275        It constru
-00006220: 6374 7320 6061 6666 696e 6560 2c20 606f  cts `affine`, `o
-00006230: 7269 6769 6e61 6c5f 6166 6669 6e65 602c  riginal_affine`,
-00006240: 2061 6e64 2060 7370 6174 6961 6c5f 7368   and `spatial_sh
-00006250: 6170 6560 2061 6e64 2073 746f 7265 7320  ape` and stores 
-00006260: 7468 656d 2069 6e20 6d65 7461 2064 6963  them in meta dic
-00006270: 742e 0a20 2020 2020 2020 2046 6f72 2064  t..        For d
-00006280: 6963 6f6d 2073 6572 6965 7320 7769 7468  icom series with
-00006290: 696e 2074 6865 2069 6e70 7574 2c20 616c  in the input, al
-000062a0: 6c20 736c 6963 6573 2077 696c 6c20 6265  l slices will be
-000062b0: 2073 7461 636b 6564 2066 6972 7374 2c0a   stacked first,.
-000062c0: 2020 2020 2020 2020 5768 656e 206c 6f61          When loa
-000062d0: 6469 6e67 2061 206c 6973 7420 6f66 2066  ding a list of f
-000062e0: 696c 6573 2028 6469 636f 6d20 6669 6c65  iles (dicom file
-000062f0: 2c20 6f72 2073 7461 636b 6564 2064 6963  , or stacked dic
-00006300: 6f6d 2073 6572 6965 7329 2c20 7468 6579  om series), they
-00006310: 2061 7265 2073 7461 636b 6564 2074 6f67   are stacked tog
-00006320: 6574 6865 7220 6174 2061 206e 6577 0a20  ether at a new. 
-00006330: 2020 2020 2020 2064 696d 656e 7369 6f6e         dimension
-00006340: 2061 7320 7468 6520 6669 7273 7420 6469   as the first di
-00006350: 6d65 6e73 696f 6e2c 2061 6e64 2074 6865  mension, and the
-00006360: 206d 6574 6164 6174 6120 6f66 2074 6865   metadata of the
-00006370: 2066 6972 7374 2069 6d61 6765 2069 7320   first image is 
-00006380: 7573 6564 2074 6f20 7265 7072 6573 656e  used to represen
-00006390: 7420 7468 6520 6f75 7470 7574 206d 6574  t the output met
-000063a0: 6164 6174 612e 0a0a 2020 2020 2020 2020  adata...        
-000063b0: 546f 2075 7365 2074 6869 7320 6675 6e63  To use this func
-000063c0: 7469 6f6e 2c20 616c 6c20 7079 6469 636f  tion, all pydico
-000063d0: 6d20 6461 7461 7365 7420 6f62 6a65 6374  m dataset object
-000063e0: 7320 2869 6620 6e6f 7420 7365 676d 656e  s (if not segmen
-000063f0: 7461 7469 6f6e 2064 6174 6129 2073 686f  tation data) sho
-00006400: 756c 6420 636f 6e74 6169 6e3a 0a20 2020  uld contain:.   
-00006410: 2020 2020 2060 7069 7865 6c5f 6172 7261       `pixel_arra
-00006420: 7960 2c20 6050 6978 656c 5370 6163 696e  y`, `PixelSpacin
-00006430: 6760 2c20 6049 6d61 6765 506f 7369 7469  g`, `ImagePositi
-00006440: 6f6e 5061 7469 656e 7460 2061 6e64 2060  onPatient` and `
-00006450: 496d 6167 654f 7269 656e 7461 7469 6f6e  ImageOrientation
-00006460: 5061 7469 656e 7460 2e0a 0a20 2020 2020  Patient`...     
-00006470: 2020 2046 6f72 2073 6567 6d65 6e74 6174     For segmentat
-00006480: 696f 6e20 6461 7461 2c20 7765 2061 7373  ion data, we ass
-00006490: 756d 6520 7468 6174 2074 6865 2069 6e70  ume that the inp
-000064a0: 7574 2069 7320 6e6f 7420 6120 6469 636f  ut is not a dico
-000064b0: 6d20 7365 7269 6573 2c20 616e 6420 7468  m series, and th
-000064c0: 6520 6f62 6a65 6374 2073 686f 756c 6420  e object should 
-000064d0: 636f 6e74 6169 6e0a 2020 2020 2020 2020  contain.        
-000064e0: 6053 6567 6d65 6e74 5365 7175 656e 6365  `SegmentSequence
-000064f0: 6020 696e 206f 7264 6572 2074 6f20 6964  ` in order to id
-00006500: 656e 7469 6679 2069 742e 0a20 2020 2020  entify it..     
-00006510: 2020 2049 6e20 6164 6469 7469 6f6e 2c20     In addition, 
-00006520: 7461 6773 2028 3532 3030 2c20 3932 3239  tags (5200, 9229
-00006530: 2920 616e 6420 2835 3230 302c 2039 3233  ) and (5200, 923
-00006540: 3029 2061 7265 2072 6571 7569 7265 6420  0) are required 
-00006550: 746f 2061 6368 6965 7665 0a20 2020 2020  to achieve.     
-00006560: 2020 2060 5069 7865 6c53 7061 6369 6e67     `PixelSpacing
-00006570: 602c 2060 496d 6167 654f 7269 656e 7461  `, `ImageOrienta
-00006580: 7469 6f6e 5061 7469 656e 7460 2061 6e64  tionPatient` and
-00006590: 2060 496d 6167 6550 6f73 6974 696f 6e50   `ImagePositionP
-000065a0: 6174 6965 6e74 602e 0a0a 2020 2020 2020  atient`...      
-000065b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000065c0: 2020 2020 6461 7461 3a20 6120 7079 6469      data: a pydi
-000065d0: 636f 6d20 6461 7461 7365 7420 6f62 6a65  com dataset obje
-000065e0: 6374 2c20 6f72 2061 206c 6973 7420 6f66  ct, or a list of
-000065f0: 2070 7964 6963 6f6d 2064 6174 6173 6574   pydicom dataset
-00006600: 206f 626a 6563 7473 2c20 6f72 2061 206c   objects, or a l
-00006610: 6973 7420 6f66 206c 6973 7420 6f66 0a20  ist of list of. 
-00006620: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006630: 7964 6963 6f6d 2064 6174 6173 6574 206f  ydicom dataset o
-00006640: 626a 6563 7473 2e0a 0a20 2020 2020 2020  bjects...       
-00006650: 2022 2222 0a0a 2020 2020 2020 2020 6469   """..        di
-00006660: 636f 6d5f 6461 7461 203d 205b 5d0a 2020  com_data = [].  
-00006670: 2020 2020 2020 2320 636f 6d62 696e 6520        # combine 
-00006680: 6469 636f 6d20 7365 7269 6573 2069 6620  dicom series if 
-00006690: 6578 6973 7473 0a20 2020 2020 2020 2069  exists.        i
-000066a0: 6620 7365 6c66 2e68 6173 5f73 6572 6965  f self.has_serie
-000066b0: 7320 6973 2054 7275 653a 0a20 2020 2020  s is True:.     
-000066c0: 2020 2020 2020 2023 2061 206c 6973 742c         # a list,
-000066d0: 2061 6c6c 206f 626a 6563 7473 2077 6974   all objects wit
-000066e0: 6869 6e20 6120 6c69 7374 2062 656c 6f6e  hin a list belon
-000066f0: 6720 746f 206f 6e65 2064 6963 6f6d 2073  g to one dicom s
-00006700: 6572 6965 730a 2020 2020 2020 2020 2020  eries.          
-00006710: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-00006720: 6e63 6528 6461 7461 5b30 5d2c 206c 6973  nce(data[0], lis
-00006730: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-00006740: 2020 2020 6469 636f 6d5f 6461 7461 2e61      dicom_data.a
-00006750: 7070 656e 6428 7365 6c66 2e5f 636f 6d62  ppend(self._comb
-00006760: 696e 655f 6469 636f 6d5f 7365 7269 6573  ine_dicom_series
-00006770: 2864 6174 6129 290a 2020 2020 2020 2020  (data)).        
-00006780: 2020 2020 2320 6120 6c69 7374 206f 6620      # a list of 
-00006790: 6c69 7374 2c20 6561 6368 2069 6e6e 6572  list, each inner
-000067a0: 206c 6973 7420 7265 7072 6573 656e 7473   list represents
-000067b0: 2061 2064 6963 6f6d 2073 6572 6965 730a   a dicom series.
-000067c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000067d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000067e0: 2020 666f 7220 7365 7269 6573 2069 6e20    for series in 
-000067f0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-00006800: 2020 2020 2020 2020 2020 6469 636f 6d5f            dicom_
-00006810: 6461 7461 2e61 7070 656e 6428 7365 6c66  data.append(self
-00006820: 2e5f 636f 6d62 696e 655f 6469 636f 6d5f  ._combine_dicom_
-00006830: 7365 7269 6573 2873 6572 6965 7329 290a  series(series)).
-00006840: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006850: 2020 2020 2020 2020 2020 2320 6120 7369            # a si
-00006860: 6e67 6c65 2070 7964 6963 6f6d 2064 6174  ngle pydicom dat
-00006870: 6173 6574 206f 626a 6563 740a 2020 2020  aset object.    
-00006880: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00006890: 7369 6e73 7461 6e63 6528 6461 7461 2c20  sinstance(data, 
-000068a0: 6c69 7374 293a 0a20 2020 2020 2020 2020  list):.         
-000068b0: 2020 2020 2020 2064 6174 6120 3d20 5b64         data = [d
-000068c0: 6174 615d 0a20 2020 2020 2020 2020 2020  ata].           
-000068d0: 2066 6f72 2064 2069 6e20 6461 7461 3a0a   for d in data:.
-000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 6966 2068 6173 6174 7472 2864 2c20 2253  if hasattr(d, "S
-00006900: 6567 6d65 6e74 5365 7175 656e 6365 2229  egmentSequence")
-00006910: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006920: 2020 2020 2020 6461 7461 5f61 7272 6179        data_array
-00006930: 2c20 6d65 7461 6461 7461 203d 2073 656c  , metadata = sel
-00006940: 662e 5f67 6574 5f73 6567 5f64 6174 6128  f._get_seg_data(
-00006950: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
-00006960: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00006970: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00006980: 615f 6172 7261 7920 3d20 7365 6c66 2e5f  a_array = self._
-00006990: 6765 745f 6172 7261 795f 6461 7461 2864  get_array_data(d
-000069a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000069b0: 2020 2020 2020 6d65 7461 6461 7461 203d        metadata =
-000069c0: 2073 656c 662e 5f67 6574 5f6d 6574 615f   self._get_meta_
-000069d0: 6469 6374 2864 290a 2020 2020 2020 2020  dict(d).        
-000069e0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-000069f0: 6461 7461 5b4d 6574 614b 6579 732e 5350  data[MetaKeys.SP
-00006a00: 4154 4941 4c5f 5348 4150 455d 203d 2064  ATIAL_SHAPE] = d
-00006a10: 6174 615f 6172 7261 792e 7368 6170 650a  ata_array.shape.
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 6469 636f 6d5f 6461 7461 2e61 7070 656e  dicom_data.appen
-00006a40: 6428 2864 6174 615f 6172 7261 792c 206d  d((data_array, m
-00006a50: 6574 6164 6174 6129 290a 0a20 2020 2020  etadata))..     
-00006a60: 2020 2069 6d67 5f61 7272 6179 3a20 6c69     img_array: li
-00006a70: 7374 5b6e 702e 6e64 6172 7261 795d 203d  st[np.ndarray] =
-00006a80: 205b 5d0a 2020 2020 2020 2020 636f 6d70   [].        comp
-00006a90: 6174 6962 6c65 5f6d 6574 613a 2064 6963  atible_meta: dic
-00006aa0: 7420 3d20 7b7d 0a0a 2020 2020 2020 2020  t = {}..        
-00006ab0: 666f 7220 6461 7461 5f61 7272 6179 2c20  for data_array, 
-00006ac0: 6d65 7461 6461 7461 2069 6e20 656e 7375  metadata in ensu
-00006ad0: 7265 5f74 7570 6c65 2864 6963 6f6d 5f64  re_tuple(dicom_d
-00006ae0: 6174 6129 3a0a 2020 2020 2020 2020 2020  ata):.          
-00006af0: 2020 696d 675f 6172 7261 792e 6170 7065    img_array.appe
-00006b00: 6e64 286e 702e 6173 636f 6e74 6967 756f  nd(np.ascontiguo
-00006b10: 7573 6172 7261 7928 6e70 2e73 7761 7061  usarray(np.swapa
-00006b20: 7865 7328 6461 7461 5f61 7272 6179 2c20  xes(data_array, 
-00006b30: 302c 2031 2920 6966 2073 656c 662e 7377  0, 1) if self.sw
-00006b40: 6170 5f69 6a20 656c 7365 2064 6174 615f  ap_ij else data_
-00006b50: 6172 7261 7929 290a 2020 2020 2020 2020  array)).        
-00006b60: 2020 2020 6166 6669 6e65 203d 2073 656c      affine = sel
-00006b70: 662e 5f67 6574 5f61 6666 696e 6528 6d65  f._get_affine(me
-00006b80: 7461 6461 7461 2c20 7365 6c66 2e61 6666  tadata, self.aff
-00006b90: 696e 655f 6c70 735f 746f 5f72 6173 290a  ine_lps_to_ras).
-00006ba0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00006bb0: 6461 7461 5b4d 6574 614b 6579 732e 5350  data[MetaKeys.SP
-00006bc0: 4143 455d 203d 2053 7061 6365 4b65 7973  ACE] = SpaceKeys
-00006bd0: 2e52 4153 2069 6620 7365 6c66 2e61 6666  .RAS if self.aff
-00006be0: 696e 655f 6c70 735f 746f 5f72 6173 2065  ine_lps_to_ras e
-00006bf0: 6c73 6520 5370 6163 654b 6579 732e 4c50  lse SpaceKeys.LP
-00006c00: 530a 2020 2020 2020 2020 2020 2020 6966  S.            if
-00006c10: 2073 656c 662e 7377 6170 5f69 6a3a 0a20   self.swap_ij:. 
-00006c20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00006c30: 6666 696e 6520 3d20 6166 6669 6e65 2040  ffine = affine @
-00006c40: 206e 702e 6172 7261 7928 5b5b 302c 2031   np.array([[0, 1
-00006c50: 2c20 302c 2030 5d2c 205b 312c 2030 2c20  , 0, 0], [1, 0, 
-00006c60: 302c 2030 5d2c 205b 302c 2030 2c20 312c  0, 0], [0, 0, 1,
-00006c70: 2030 5d2c 205b 302c 2030 2c20 302c 2031   0], [0, 0, 0, 1
-00006c80: 5d5d 290a 2020 2020 2020 2020 2020 2020  ]]).            
-00006c90: 2020 2020 7370 5f73 697a 6520 3d20 6c69      sp_size = li
-00006ca0: 7374 286d 6574 6164 6174 615b 4d65 7461  st(metadata[Meta
-00006cb0: 4b65 7973 2e53 5041 5449 414c 5f53 4841  Keys.SPATIAL_SHA
-00006cc0: 5045 5d29 0a20 2020 2020 2020 2020 2020  PE]).           
-00006cd0: 2020 2020 2073 705f 7369 7a65 5b30 5d2c       sp_size[0],
-00006ce0: 2073 705f 7369 7a65 5b31 5d20 3d20 7370   sp_size[1] = sp
-00006cf0: 5f73 697a 655b 315d 2c20 7370 5f73 697a  _size[1], sp_siz
-00006d00: 655b 305d 0a20 2020 2020 2020 2020 2020  e[0].           
-00006d10: 2020 2020 206d 6574 6164 6174 615b 4d65       metadata[Me
-00006d20: 7461 4b65 7973 2e53 5041 5449 414c 5f53  taKeys.SPATIAL_S
-00006d30: 4841 5045 5d20 3d20 656e 7375 7265 5f74  HAPE] = ensure_t
-00006d40: 7570 6c65 2873 705f 7369 7a65 290a 2020  uple(sp_size).  
-00006d50: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
-00006d60: 7461 5b4d 6574 614b 6579 732e 4f52 4947  ta[MetaKeys.ORIG
-00006d70: 494e 414c 5f41 4646 494e 455d 203d 2061  INAL_AFFINE] = a
-00006d80: 6666 696e 650a 2020 2020 2020 2020 2020  ffine.          
-00006d90: 2020 6d65 7461 6461 7461 5b4d 6574 614b    metadata[MetaK
-00006da0: 6579 732e 4146 4649 4e45 5d20 3d20 6166  eys.AFFINE] = af
-00006db0: 6669 6e65 2e63 6f70 7928 290a 2020 2020  fine.copy().    
-00006dc0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00006dd0: 6368 616e 6e65 6c5f 6469 6d20 6973 204e  channel_dim is N
-00006de0: 6f6e 653a 2020 2320 6465 6661 756c 7420  one:  # default 
-00006df0: 746f 2022 6e6f 5f63 6861 6e6e 656c 2220  to "no_channel" 
-00006e00: 6f72 202d 310a 2020 2020 2020 2020 2020  or -1.          
-00006e10: 2020 2020 2020 6d65 7461 6461 7461 5b4d        metadata[M
-00006e20: 6574 614b 6579 732e 4f52 4947 494e 414c  etaKeys.ORIGINAL
-00006e30: 5f43 4841 4e4e 454c 5f44 494d 5d20 3d20  _CHANNEL_DIM] = 
-00006e40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00006e50: 2020 2020 2020 666c 6f61 7428 226e 616e        float("nan
-00006e60: 2229 2069 6620 6c65 6e28 6461 7461 5f61  ") if len(data_a
-00006e70: 7272 6179 2e73 6861 7065 2920 3d3d 206c  rray.shape) == l
-00006e80: 656e 286d 6574 6164 6174 615b 4d65 7461  en(metadata[Meta
-00006e90: 4b65 7973 2e53 5041 5449 414c 5f53 4841  Keys.SPATIAL_SHA
-00006ea0: 5045 5d29 2065 6c73 6520 2d31 0a20 2020  PE]) else -1.   
-00006eb0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00006ec0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00006ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006ee0: 206d 6574 6164 6174 615b 4d65 7461 4b65   metadata[MetaKe
-00006ef0: 7973 2e4f 5249 4749 4e41 4c5f 4348 414e  ys.ORIGINAL_CHAN
-00006f00: 4e45 4c5f 4449 4d5d 203d 2073 656c 662e  NEL_DIM] = self.
-00006f10: 6368 616e 6e65 6c5f 6469 6d0a 2020 2020  channel_dim.    
-00006f20: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
-00006f30: 5b22 7370 6163 696e 6722 5d20 3d20 6166  ["spacing"] = af
-00006f40: 6669 6e65 5f74 6f5f 7370 6163 696e 6728  fine_to_spacing(
-00006f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006f60: 206d 6574 6164 6174 615b 4d65 7461 4b65   metadata[MetaKe
-00006f70: 7973 2e4f 5249 4749 4e41 4c5f 4146 4649  ys.ORIGINAL_AFFI
-00006f80: 4e45 5d2c 2072 3d6c 656e 286d 6574 6164  NE], r=len(metad
-00006f90: 6174 615b 4d65 7461 4b65 7973 2e53 5041  ata[MetaKeys.SPA
-00006fa0: 5449 414c 5f53 4841 5045 5d29 0a20 2020  TIAL_SHAPE]).   
-00006fb0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00006fc0: 2020 2020 2020 2020 5f63 6f70 795f 636f          _copy_co
-00006fd0: 6d70 6174 6962 6c65 5f64 6963 7428 6d65  mpatible_dict(me
-00006fe0: 7461 6461 7461 2c20 636f 6d70 6174 6962  tadata, compatib
-00006ff0: 6c65 5f6d 6574 6129 0a0a 2020 2020 2020  le_meta)..      
-00007000: 2020 7265 7475 726e 205f 7374 6163 6b5f    return _stack_
-00007010: 696d 6167 6573 2869 6d67 5f61 7272 6179  images(img_array
-00007020: 2c20 636f 6d70 6174 6962 6c65 5f6d 6574  , compatible_met
-00007030: 6129 2c20 636f 6d70 6174 6962 6c65 5f6d  a), compatible_m
-00007040: 6574 610a 0a20 2020 2064 6566 205f 6765  eta..    def _ge
-00007050: 745f 6d65 7461 5f64 6963 7428 7365 6c66  t_meta_dict(self
-00007060: 2c20 696d 6729 202d 3e20 6469 6374 3a0a  , img) -> dict:.
-00007070: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00007080: 2020 2020 4765 7420 616c 6c20 7468 6520      Get all the 
-00007090: 6d65 7461 6461 7461 206f 6620 7468 6520  metadata of the 
-000070a0: 696d 6167 6520 616e 6420 636f 6e76 6572  image and conver
-000070b0: 7420 746f 2064 6963 7420 7479 7065 2e0a  t to dict type..
-000070c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-000070d0: 2020 2020 2020 2020 2020 2069 6d67 3a20             img: 
-000070e0: 6120 5079 6469 636f 6d20 6461 7461 7365  a Pydicom datase
-000070f0: 7420 6f62 6a65 6374 2e0a 0a20 2020 2020  t object...     
-00007100: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00007110: 6d65 7461 6461 7461 203d 2069 6d67 2e74  metadata = img.t
-00007120: 6f5f 6a73 6f6e 5f64 6963 7428 7375 7070  o_json_dict(supp
-00007130: 7265 7373 5f69 6e76 616c 6964 5f74 6167  ress_invalid_tag
-00007140: 733d 5472 7565 290a 0a20 2020 2020 2020  s=True)..       
-00007150: 2069 6620 7365 6c66 2e70 7275 6e65 5f6d   if self.prune_m
-00007160: 6574 6164 6174 613a 0a20 2020 2020 2020  etadata:.       
-00007170: 2020 2020 2070 7275 6e65 5f6d 6574 6164       prune_metad
-00007180: 6174 6120 3d20 7b7d 0a20 2020 2020 2020  ata = {}.       
-00007190: 2020 2020 2066 6f72 206b 6579 2069 6e20       for key in 
-000071a0: 5b22 3030 3230 3030 3337 222c 2022 3030  ["00200037", "00
-000071b0: 3230 3030 3332 222c 2022 3532 3030 3932  200032", "520092
-000071c0: 3239 222c 2022 3532 3030 3932 3330 225d  29", "52009230"]
-000071d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000071e0: 2020 6966 206b 6579 2069 6e20 6d65 7461    if key in meta
-000071f0: 6461 7461 2e6b 6579 7328 293a 0a20 2020  data.keys():.   
-00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007210: 2070 7275 6e65 5f6d 6574 6164 6174 615b   prune_metadata[
-00007220: 6b65 795d 203d 206d 6574 6164 6174 615b  key] = metadata[
-00007230: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
-00007240: 2072 6574 7572 6e20 7072 756e 655f 6d65   return prune_me
-00007250: 7461 6461 7461 0a0a 2020 2020 2020 2020  tadata..        
-00007260: 2320 616c 7761 7973 2072 656d 6f76 6520  # always remove 
-00007270: 5069 7865 6c20 4461 7461 2022 3746 4530  Pixel Data "7FE0
-00007280: 3030 3038 2220 6f72 2022 3746 4530 3030  0008" or "7FE000
-00007290: 3039 2220 6f72 2022 3746 4530 3030 3130  09" or "7FE00010
-000072a0: 220a 2020 2020 2020 2020 2320 616c 7761  ".        # alwa
-000072b0: 7973 2072 656d 6f76 6520 4461 7461 2053  ys remove Data S
-000072c0: 6574 2054 7261 696c 696e 6720 5061 6464  et Trailing Padd
-000072d0: 696e 6720 2246 4646 4346 4646 4322 0a20  ing "FFFCFFFC". 
-000072e0: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
-000072f0: 6e20 5b22 3746 4530 3030 3038 222c 2022  n ["7FE00008", "
-00007300: 3746 4530 3030 3039 222c 2022 3746 4530  7FE00009", "7FE0
-00007310: 3030 3130 222c 2022 4646 4643 4646 4643  0010", "FFFCFFFC
-00007320: 225d 3a0a 2020 2020 2020 2020 2020 2020  "]:.            
-00007330: 6966 206b 6579 2069 6e20 6d65 7461 6461  if key in metada
-00007340: 7461 2e6b 6579 7328 293a 0a20 2020 2020  ta.keys():.     
-00007350: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00007360: 6174 612e 706f 7028 6b65 7929 0a0a 2020  ata.pop(key)..  
-00007370: 2020 2020 2020 7265 7475 726e 206d 6574        return met
-00007380: 6164 6174 6120 2023 2074 7970 653a 2069  adata  # type: i
-00007390: 676e 6f72 650a 0a20 2020 2064 6566 205f  gnore..    def _
-000073a0: 6765 745f 6166 6669 6e65 2873 656c 662c  get_affine(self,
-000073b0: 206d 6574 6164 6174 613a 2064 6963 742c   metadata: dict,
-000073c0: 206c 7073 5f74 6f5f 7261 733a 2062 6f6f   lps_to_ras: boo
-000073d0: 6c20 3d20 5472 7565 293a 0a20 2020 2020  l = True):.     
-000073e0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-000073f0: 6574 206f 7220 636f 6e73 7472 7563 7420  et or construct 
-00007400: 7468 6520 6166 6669 6e65 206d 6174 7269  the affine matri
-00007410: 7820 6f66 2074 6865 2069 6d61 6765 2c20  x of the image, 
-00007420: 6974 2063 616e 2062 6520 7573 6564 2074  it can be used t
-00007430: 6f20 636f 7272 6563 740a 2020 2020 2020  o correct.      
-00007440: 2020 7370 6163 696e 672c 206f 7269 656e    spacing, orien
-00007450: 7461 7469 6f6e 206f 7220 6578 6563 7574  tation or execut
-00007460: 6520 7370 6174 6961 6c20 7472 616e 7366  e spatial transf
-00007470: 6f72 6d73 2e0a 0a20 2020 2020 2020 2041  orms...        A
-00007480: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00007490: 206d 6574 6164 6174 613a 206d 6574 6164   metadata: metad
-000074a0: 6174 6120 7769 7468 2064 6963 7420 7479  ata with dict ty
-000074b0: 7065 2e0a 2020 2020 2020 2020 2020 2020  pe..            
-000074c0: 6c70 735f 746f 5f72 6173 3a20 7768 6574  lps_to_ras: whet
-000074d0: 6865 7220 746f 2063 6f6e 7665 7274 2074  her to convert t
-000074e0: 6865 2061 6666 696e 6520 6d61 7472 6978  he affine matrix
-000074f0: 2066 726f 6d20 224c 5053 2220 746f 2022   from "LPS" to "
-00007500: 5241 5322 2e20 4465 6661 756c 7473 2074  RAS". Defaults t
-00007510: 6f20 5472 7565 2e0a 0a20 2020 2020 2020  o True...       
-00007520: 2022 2222 0a20 2020 2020 2020 2061 6666   """.        aff
-00007530: 696e 653a 206e 702e 6e64 6172 7261 7920  ine: np.ndarray 
-00007540: 3d20 6e70 2e65 7965 2834 290a 2020 2020  = np.eye(4).    
-00007550: 2020 2020 6966 206e 6f74 2028 2230 3032      if not ("002
-00007560: 3030 3033 3722 2069 6e20 6d65 7461 6461  00037" in metada
-00007570: 7461 2061 6e64 2022 3030 3230 3030 3332  ta and "00200032
-00007580: 2220 696e 206d 6574 6164 6174 6129 3a0a  " in metadata):.
-00007590: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000075a0: 726e 2061 6666 696e 650a 2020 2020 2020  rn affine.      
-000075b0: 2020 2320 2230 3032 3030 3033 3722 2069    # "00200037" i
-000075c0: 7320 7468 6520 7461 6720 6f66 2060 496d  s the tag of `Im
-000075d0: 6167 654f 7269 656e 7461 7469 6f6e 5061  ageOrientationPa
-000075e0: 7469 656e 7460 0a20 2020 2020 2020 2072  tient`.        r
-000075f0: 782c 2072 792c 2072 7a2c 2063 782c 2063  x, ry, rz, cx, c
-00007600: 792c 2063 7a20 3d20 6d65 7461 6461 7461  y, cz = metadata
-00007610: 5b22 3030 3230 3030 3337 225d 5b22 5661  ["00200037"]["Va
-00007620: 6c75 6522 5d0a 2020 2020 2020 2020 2320  lue"].        # 
-00007630: 2230 3032 3030 3033 3222 2069 7320 7468  "00200032" is th
-00007640: 6520 7461 6720 6f66 2060 496d 6167 6550  e tag of `ImageP
-00007650: 6f73 6974 696f 6e50 6174 6965 6e74 600a  ositionPatient`.
-00007660: 2020 2020 2020 2020 7378 2c20 7379 2c20          sx, sy, 
-00007670: 737a 203d 206d 6574 6164 6174 615b 2230  sz = metadata["0
-00007680: 3032 3030 3033 3222 5d5b 2256 616c 7565  0200032"]["Value
-00007690: 225d 0a20 2020 2020 2020 2064 722c 2064  "].        dr, d
-000076a0: 6320 3d20 6d65 7461 6461 7461 2e67 6574  c = metadata.get
-000076b0: 2822 7370 6163 696e 6722 2c20 2831 2e30  ("spacing", (1.0
-000076c0: 2c20 312e 3029 295b 3a32 5d0a 2020 2020  , 1.0))[:2].    
-000076d0: 2020 2020 6166 6669 6e65 5b30 2c20 305d      affine[0, 0]
-000076e0: 203d 2063 7820 2a20 6472 0a20 2020 2020   = cx * dr.     
-000076f0: 2020 2061 6666 696e 655b 302c 2031 5d20     affine[0, 1] 
-00007700: 3d20 7278 202a 2064 630a 2020 2020 2020  = rx * dc.      
-00007710: 2020 6166 6669 6e65 5b30 2c20 335d 203d    affine[0, 3] =
-00007720: 2073 780a 2020 2020 2020 2020 6166 6669   sx.        affi
-00007730: 6e65 5b31 2c20 305d 203d 2063 7920 2a20  ne[1, 0] = cy * 
-00007740: 6472 0a20 2020 2020 2020 2061 6666 696e  dr.        affin
-00007750: 655b 312c 2031 5d20 3d20 7279 202a 2064  e[1, 1] = ry * d
-00007760: 630a 2020 2020 2020 2020 6166 6669 6e65  c.        affine
-00007770: 5b31 2c20 335d 203d 2073 790a 2020 2020  [1, 3] = sy.    
-00007780: 2020 2020 6166 6669 6e65 5b32 2c20 305d      affine[2, 0]
-00007790: 203d 2063 7a20 2a20 6472 0a20 2020 2020   = cz * dr.     
-000077a0: 2020 2061 6666 696e 655b 322c 2031 5d20     affine[2, 1] 
-000077b0: 3d20 727a 202a 2064 630a 2020 2020 2020  = rz * dc.      
-000077c0: 2020 6166 6669 6e65 5b32 2c20 325d 203d    affine[2, 2] =
-000077d0: 2030 0a20 2020 2020 2020 2061 6666 696e   0.        affin
-000077e0: 655b 322c 2033 5d20 3d20 737a 0a0a 2020  e[2, 3] = sz..  
-000077f0: 2020 2020 2020 2320 3364 0a20 2020 2020        # 3d.     
-00007800: 2020 2069 6620 226c 6173 7449 6d61 6765     if "lastImage
-00007810: 506f 7369 7469 6f6e 5061 7469 656e 7422  PositionPatient"
-00007820: 2069 6e20 6d65 7461 6461 7461 3a0a 2020   in metadata:.  
-00007830: 2020 2020 2020 2020 2020 7431 6e2c 2074            t1n, t
-00007840: 326e 2c20 7433 6e20 3d20 6d65 7461 6461  2n, t3n = metada
-00007850: 7461 5b22 6c61 7374 496d 6167 6550 6f73  ta["lastImagePos
-00007860: 6974 696f 6e50 6174 6965 6e74 225d 0a20  itionPatient"]. 
-00007870: 2020 2020 2020 2020 2020 206e 203d 206d             n = m
-00007880: 6574 6164 6174 615b 4d65 7461 4b65 7973  etadata[MetaKeys
-00007890: 2e53 5041 5449 414c 5f53 4841 5045 5d5b  .SPATIAL_SHAPE][
-000078a0: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
-000078b0: 6b31 2c20 6b32 2c20 6b33 203d 2028 7431  k1, k2, k3 = (t1
-000078c0: 6e20 2d20 7378 2920 2f20 286e 202d 2031  n - sx) / (n - 1
-000078d0: 292c 2028 7432 6e20 2d20 7379 2920 2f20  ), (t2n - sy) / 
-000078e0: 286e 202d 2031 292c 2028 7433 6e20 2d20  (n - 1), (t3n - 
-000078f0: 737a 2920 2f20 286e 202d 2031 290a 2020  sz) / (n - 1).  
-00007900: 2020 2020 2020 2020 2020 6166 6669 6e65            affine
-00007910: 5b30 2c20 325d 203d 206b 310a 2020 2020  [0, 2] = k1.    
-00007920: 2020 2020 2020 2020 6166 6669 6e65 5b31          affine[1
-00007930: 2c20 325d 203d 206b 320a 2020 2020 2020  , 2] = k2.      
-00007940: 2020 2020 2020 6166 6669 6e65 5b32 2c20        affine[2, 
-00007950: 325d 203d 206b 330a 0a20 2020 2020 2020  2] = k3..       
-00007960: 2069 6620 6c70 735f 746f 5f72 6173 3a0a   if lps_to_ras:.
-00007970: 2020 2020 2020 2020 2020 2020 6166 6669              affi
-00007980: 6e65 203d 206f 7269 656e 7461 7469 6f6e  ne = orientation
-00007990: 5f72 6173 5f6c 7073 2861 6666 696e 6529  _ras_lps(affine)
-000079a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000079b0: 6166 6669 6e65 0a0a 2020 2020 6465 6620  affine..    def 
-000079c0: 5f67 6574 5f66 7261 6d65 5f64 6174 6128  _get_frame_data(
-000079d0: 7365 6c66 2c20 696d 6729 202d 3e20 4974  self, img) -> It
-000079e0: 6572 6174 6f72 3a0a 2020 2020 2020 2020  erator:.        
-000079f0: 2222 220a 2020 2020 2020 2020 7969 656c  """.        yiel
-00007a00: 6420 6672 616d 6573 2061 6e64 2064 6573  d frames and des
-00007a10: 6372 6970 7469 6f6e 2066 726f 6d20 7468  cription from th
-00007a20: 6520 7365 676d 656e 7461 7469 6f6e 2069  e segmentation i
-00007a30: 6d61 6765 2e0a 2020 2020 2020 2020 5468  mage..        Th
-00007a40: 6973 2066 756e 6374 696f 6e20 6973 2061  is function is a
-00007a50: 6461 7074 6564 2066 726f 6d20 4869 6768  dapted from High
-00007a60: 6469 636f 6d3a 0a20 2020 2020 2020 2068  dicom:.        h
-00007a70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00007a80: 6d2f 6865 7272 6d61 6e6e 6c61 622f 6869  m/herrmannlab/hi
-00007a90: 6768 6469 636f 6d2f 626c 6f62 2f76 302e  ghdicom/blob/v0.
-00007aa0: 3138 2e32 2f73 7263 2f68 6967 6864 6963  18.2/src/highdic
-00007ab0: 6f6d 2f73 6567 2f75 7469 6c73 2e70 790a  om/seg/utils.py.
-00007ac0: 0a20 2020 2020 2020 2077 6869 6368 2068  .        which h
-00007ad0: 6173 2074 6865 2066 6f6c 6c6f 7769 6e67  as the following
-00007ae0: 206c 6963 656e 7365 2e2e 2e0a 0a20 2020   license.....   
-00007af0: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
-00007b00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007b10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007b20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007b30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007b40: 0a20 2020 2020 2020 2023 2068 7474 7073  .        # https
-00007b50: 3a2f 2f67 6974 6875 622e 636f 6d2f 6865  ://github.com/he
-00007b60: 7272 6d61 6e6e 6c61 622f 6869 6768 6469  rrmannlab/highdi
-00007b70: 636f 6d2f 626c 6f62 2f76 302e 3138 2e32  com/blob/v0.18.2
-00007b80: 2f4c 4943 454e 5345 0a20 2020 2020 2020  /LICENSE.       
-00007b90: 2023 0a20 2020 2020 2020 2023 2043 6f70   #.        # Cop
-00007ba0: 7972 6967 6874 2032 3032 3020 4d47 4820  yright 2020 MGH 
-00007bb0: 436f 6d70 7574 6174 696f 6e61 6c20 5061  Computational Pa
-00007bc0: 7468 6f6c 6f67 790a 2020 2020 2020 2020  thology.        
-00007bd0: 2320 5065 726d 6973 7369 6f6e 2069 7320  # Permission is 
-00007be0: 6865 7265 6279 2067 7261 6e74 6564 2c20  hereby granted, 
-00007bf0: 6672 6565 206f 6620 6368 6172 6765 2c20  free of charge, 
-00007c00: 746f 2061 6e79 2070 6572 736f 6e20 6f62  to any person ob
-00007c10: 7461 696e 696e 6720 610a 2020 2020 2020  taining a.      
-00007c20: 2020 2320 636f 7079 206f 6620 7468 6973    # copy of this
-00007c30: 2073 6f66 7477 6172 6520 616e 6420 6173   software and as
-00007c40: 736f 6369 6174 6564 2064 6f63 756d 656e  sociated documen
-00007c50: 7461 7469 6f6e 2066 696c 6573 2028 7468  tation files (th
-00007c60: 650a 2020 2020 2020 2020 2320 2253 6f66  e.        # "Sof
-00007c70: 7477 6172 6522 292c 2074 6f20 6465 616c  tware"), to deal
-00007c80: 2069 6e20 7468 6520 536f 6674 7761 7265   in the Software
-00007c90: 2077 6974 686f 7574 2072 6573 7472 6963   without restric
-00007ca0: 7469 6f6e 2c20 696e 636c 7564 696e 670a  tion, including.
-00007cb0: 2020 2020 2020 2020 2320 7769 7468 6f75          # withou
-00007cc0: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
-00007cd0: 2072 6967 6874 7320 746f 2075 7365 2c20   rights to use, 
-00007ce0: 636f 7079 2c20 6d6f 6469 6679 2c20 6d65  copy, modify, me
-00007cf0: 7267 652c 2070 7562 6c69 7368 2c0a 2020  rge, publish,.  
-00007d00: 2020 2020 2020 2320 6469 7374 7269 6275        # distribu
-00007d10: 7465 2c20 7375 626c 6963 656e 7365 2c20  te, sublicense, 
-00007d20: 616e 642f 6f72 2073 656c 6c20 636f 7069  and/or sell copi
-00007d30: 6573 206f 6620 7468 6520 536f 6674 7761  es of the Softwa
-00007d40: 7265 2c20 616e 6420 746f 0a20 2020 2020  re, and to.     
-00007d50: 2020 2023 2070 6572 6d69 7420 7065 7273     # permit pers
-00007d60: 6f6e 7320 746f 2077 686f 6d20 7468 6520  ons to whom the 
-00007d70: 536f 6674 7761 7265 2069 7320 6675 726e  Software is furn
-00007d80: 6973 6865 6420 746f 2064 6f20 736f 2c20  ished to do so, 
-00007d90: 7375 626a 6563 7420 746f 0a20 2020 2020  subject to.     
-00007da0: 2020 2023 2074 6865 2066 6f6c 6c6f 7769     # the followi
-00007db0: 6e67 2063 6f6e 6469 7469 6f6e 733a 0a20  ng conditions:. 
-00007dc0: 2020 2020 2020 2023 2054 6865 2061 626f         # The abo
-00007dd0: 7665 2063 6f70 7972 6967 6874 206e 6f74  ve copyright not
-00007de0: 6963 6520 616e 6420 7468 6973 2070 6572  ice and this per
-00007df0: 6d69 7373 696f 6e20 6e6f 7469 6365 2073  mission notice s
-00007e00: 6861 6c6c 2062 6520 696e 636c 7564 6564  hall be included
-00007e10: 0a20 2020 2020 2020 2023 2069 6e20 616c  .        # in al
-00007e20: 6c20 636f 7069 6573 206f 7220 7375 6273  l copies or subs
-00007e30: 7461 6e74 6961 6c20 706f 7274 696f 6e73  tantial portions
-00007e40: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
-00007e50: 2e0a 2020 2020 2020 2020 2320 5448 4520  ..        # THE 
-00007e60: 534f 4654 5741 5245 2049 5320 5052 4f56  SOFTWARE IS PROV
-00007e70: 4944 4544 2022 4153 2049 5322 2c20 5749  IDED "AS IS", WI
-00007e80: 5448 4f55 5420 5741 5252 414e 5459 204f  THOUT WARRANTY O
-00007e90: 4620 414e 5920 4b49 4e44 2c20 4558 5052  F ANY KIND, EXPR
-00007ea0: 4553 530a 2020 2020 2020 2020 2320 4f52  ESS.        # OR
-00007eb0: 2049 4d50 4c49 4544 2c20 494e 434c 5544   IMPLIED, INCLUD
-00007ec0: 494e 4720 4255 5420 4e4f 5420 4c49 4d49  ING BUT NOT LIMI
-00007ed0: 5445 4420 544f 2054 4845 2057 4152 5241  TED TO THE WARRA
-00007ee0: 4e54 4945 5320 4f46 0a20 2020 2020 2020  NTIES OF.       
-00007ef0: 2023 204d 4552 4348 414e 5441 4249 4c49   # MERCHANTABILI
-00007f00: 5459 2c20 4649 544e 4553 5320 464f 5220  TY, FITNESS FOR 
-00007f10: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
-00007f20: 504f 5345 2041 4e44 204e 4f4e 494e 4652  POSE AND NONINFR
-00007f30: 494e 4745 4d45 4e54 2e0a 2020 2020 2020  INGEMENT..      
-00007f40: 2020 2320 494e 204e 4f20 4556 454e 5420    # IN NO EVENT 
-00007f50: 5348 414c 4c20 5448 4520 4155 5448 4f52  SHALL THE AUTHOR
-00007f60: 5320 4f52 2043 4f50 5952 4947 4854 2048  S OR COPYRIGHT H
-00007f70: 4f4c 4445 5253 2042 4520 4c49 4142 4c45  OLDERS BE LIABLE
-00007f80: 2046 4f52 2041 4e59 0a20 2020 2020 2020   FOR ANY.       
-00007f90: 2023 2043 4c41 494d 2c20 4441 4d41 4745   # CLAIM, DAMAGE
-00007fa0: 5320 4f52 204f 5448 4552 204c 4941 4249  S OR OTHER LIABI
-00007fb0: 4c49 5459 2c20 5748 4554 4845 5220 494e  LITY, WHETHER IN
-00007fc0: 2041 4e20 4143 5449 4f4e 204f 4620 434f   AN ACTION OF CO
-00007fd0: 4e54 5241 4354 2c0a 2020 2020 2020 2020  NTRACT,.        
-00007fe0: 2320 544f 5254 204f 5220 4f54 4845 5257  # TORT OR OTHERW
-00007ff0: 4953 452c 2041 5249 5349 4e47 2046 524f  ISE, ARISING FRO
-00008000: 4d2c 204f 5554 204f 4620 4f52 2049 4e20  M, OUT OF OR IN 
-00008010: 434f 4e4e 4543 5449 4f4e 2057 4954 4820  CONNECTION WITH 
-00008020: 5448 450a 2020 2020 2020 2020 2320 534f  THE.        # SO
-00008030: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
-00008040: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
-00008050: 4e47 5320 494e 2054 4845 2053 4f46 5457  NGS IN THE SOFTW
-00008060: 4152 452e 0a20 2020 2020 2020 2023 203d  ARE..        # =
-00008070: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00008090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000080a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000080b0: 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020 2020  ========..      
-000080c0: 2020 2868 7474 7073 3a2f 2f67 6974 6875    (https://githu
-000080d0: 622e 636f 6d2f 6865 7272 6d61 6e6e 6c61  b.com/herrmannla
-000080e0: 622f 6869 6768 6469 636f 6d2f 6973 7375  b/highdicom/issu
-000080f0: 6573 2f31 3838 290a 0a20 2020 2020 2020  es/188)..       
-00008100: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00008110: 2020 2069 6d67 3a20 6120 5079 6469 636f     img: a Pydico
-00008120: 6d20 6461 7461 7365 7420 6f62 6a65 6374  m dataset object
-00008130: 2074 6861 7420 6861 7320 6174 7472 6962   that has attrib
-00008140: 7574 6520 2253 6567 6d65 6e74 5365 7175  ute "SegmentSequ
-00008150: 656e 6365 222e 0a0a 2020 2020 2020 2020  ence"...        
-00008160: 2222 220a 0a20 2020 2020 2020 2069 6620  """..        if 
-00008170: 6e6f 7420 6861 7361 7474 7228 696d 672c  not hasattr(img,
-00008180: 2022 5065 7246 7261 6d65 4675 6e63 7469   "PerFrameFuncti
-00008190: 6f6e 616c 4772 6f75 7073 5365 7175 656e  onalGroupsSequen
+00000490: 6d6f 6e61 692e 7574 696c 7320 696d 706f  monai.utils impo
+000004a0: 7274 204d 6574 614b 6579 732c 2053 7061  rt MetaKeys, Spa
+000004b0: 6365 4b65 7973 2c20 5472 6163 654b 6579  ceKeys, TraceKey
+000004c0: 732c 2064 6570 7265 6361 7465 645f 6172  s, deprecated_ar
+000004d0: 672c 2065 6e73 7572 655f 7475 706c 652c  g, ensure_tuple,
+000004e0: 206f 7074 696f 6e61 6c5f 696d 706f 7274   optional_import
+000004f0: 2c20 7265 7175 6972 655f 706b 670a 0a69  , require_pkg..i
+00000500: 6620 5459 5045 5f43 4845 434b 494e 473a  f TYPE_CHECKING:
+00000510: 0a20 2020 2069 6d70 6f72 7420 6974 6b0a  .    import itk.
+00000520: 2020 2020 696d 706f 7274 206e 6962 6162      import nibab
+00000530: 656c 2061 7320 6e69 620a 2020 2020 696d  el as nib.    im
+00000540: 706f 7274 206e 7272 640a 2020 2020 696d  port nrrd.    im
+00000550: 706f 7274 2070 7964 6963 6f6d 0a20 2020  port pydicom.   
+00000560: 2066 726f 6d20 6e69 6261 6265 6c2e 6e69   from nibabel.ni
+00000570: 6674 6931 2069 6d70 6f72 7420 4e69 6674  fti1 import Nift
+00000580: 6931 496d 6167 650a 2020 2020 6672 6f6d  i1Image.    from
+00000590: 2050 494c 2069 6d70 6f72 7420 496d 6167   PIL import Imag
+000005a0: 6520 6173 2050 494c 496d 6167 650a 0a20  e as PILImage.. 
+000005b0: 2020 2068 6173 5f6e 7272 6420 3d20 6861     has_nrrd = ha
+000005c0: 735f 6974 6b20 3d20 6861 735f 6e69 6220  s_itk = has_nib 
+000005d0: 3d20 6861 735f 7069 6c20 3d20 6861 735f  = has_pil = has_
+000005e0: 7079 6469 636f 6d20 3d20 5472 7565 0a65  pydicom = True.e
+000005f0: 6c73 653a 0a20 2020 2069 746b 2c20 6861  lse:.    itk, ha
+00000600: 735f 6974 6b20 3d20 6f70 7469 6f6e 616c  s_itk = optional
+00000610: 5f69 6d70 6f72 7428 2269 746b 222c 2061  _import("itk", a
+00000620: 6c6c 6f77 5f6e 616d 6573 7061 6365 5f70  llow_namespace_p
+00000630: 6b67 3d54 7275 6529 0a20 2020 206e 6962  kg=True).    nib
+00000640: 2c20 6861 735f 6e69 6220 3d20 6f70 7469  , has_nib = opti
+00000650: 6f6e 616c 5f69 6d70 6f72 7428 226e 6962  onal_import("nib
+00000660: 6162 656c 2229 0a20 2020 204e 6966 7469  abel").    Nifti
+00000670: 3149 6d61 6765 2c20 5f20 3d20 6f70 7469  1Image, _ = opti
+00000680: 6f6e 616c 5f69 6d70 6f72 7428 226e 6962  onal_import("nib
+00000690: 6162 656c 2e6e 6966 7469 3122 2c20 6e61  abel.nifti1", na
+000006a0: 6d65 3d22 4e69 6674 6931 496d 6167 6522  me="Nifti1Image"
+000006b0: 290a 2020 2020 5049 4c49 6d61 6765 2c20  ).    PILImage, 
+000006c0: 6861 735f 7069 6c20 3d20 6f70 7469 6f6e  has_pil = option
+000006d0: 616c 5f69 6d70 6f72 7428 2250 494c 2e49  al_import("PIL.I
+000006e0: 6d61 6765 2229 0a20 2020 2070 7964 6963  mage").    pydic
+000006f0: 6f6d 2c20 6861 735f 7079 6469 636f 6d20  om, has_pydicom 
+00000700: 3d20 6f70 7469 6f6e 616c 5f69 6d70 6f72  = optional_impor
+00000710: 7428 2270 7964 6963 6f6d 2229 0a20 2020  t("pydicom").   
+00000720: 206e 7272 642c 2068 6173 5f6e 7272 6420   nrrd, has_nrrd 
+00000730: 3d20 6f70 7469 6f6e 616c 5f69 6d70 6f72  = optional_impor
+00000740: 7428 226e 7272 6422 2c20 616c 6c6f 775f  t("nrrd", allow_
+00000750: 6e61 6d65 7370 6163 655f 706b 673d 5472  namespace_pkg=Tr
+00000760: 7565 290a 0a5f 5f61 6c6c 5f5f 203d 205b  ue)..__all__ = [
+00000770: 2249 6d61 6765 5265 6164 6572 222c 2022  "ImageReader", "
+00000780: 4954 4b52 6561 6465 7222 2c20 224e 6962  ITKReader", "Nib
+00000790: 6162 656c 5265 6164 6572 222c 2022 4e75  abelReader", "Nu
+000007a0: 6d70 7952 6561 6465 7222 2c20 2250 494c  mpyReader", "PIL
+000007b0: 5265 6164 6572 222c 2022 5079 6469 636f  Reader", "Pydico
+000007c0: 6d52 6561 6465 7222 2c20 224e 7272 6452  mReader", "NrrdR
+000007d0: 6561 6465 7222 5d0a 0a0a 636c 6173 7320  eader"]...class 
+000007e0: 496d 6167 6552 6561 6465 7228 4142 4329  ImageReader(ABC)
+000007f0: 3a0a 2020 2020 2222 220a 2020 2020 416e  :.    """.    An
+00000800: 2061 6273 7472 6163 7420 636c 6173 7320   abstract class 
+00000810: 6465 6669 6e65 7320 4150 4973 2074 6f20  defines APIs to 
+00000820: 6c6f 6164 2069 6d61 6765 2066 696c 6573  load image files
+00000830: 2e0a 0a20 2020 2054 7970 6963 616c 2075  ...    Typical u
+00000840: 7361 6765 206f 6620 616e 2069 6d70 6c65  sage of an imple
+00000850: 6d65 6e74 6174 696f 6e20 6f66 2074 6869  mentation of thi
+00000860: 7320 636c 6173 7320 6973 3a0a 0a20 2020  s class is:..   
+00000870: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+00000880: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+00000890: 2069 6d61 6765 5f72 6561 6465 7220 3d20   image_reader = 
+000008a0: 4d79 496d 6167 6552 6561 6465 7228 290a  MyImageReader().
+000008b0: 2020 2020 2020 2020 696d 675f 6f62 6a20          img_obj 
+000008c0: 3d20 696d 6167 655f 7265 6164 6572 2e72  = image_reader.r
+000008d0: 6561 6428 7061 7468 5f74 6f5f 696d 6167  ead(path_to_imag
+000008e0: 6529 0a20 2020 2020 2020 2069 6d67 5f64  e).        img_d
+000008f0: 6174 612c 206d 6574 615f 6461 7461 203d  ata, meta_data =
+00000900: 2069 6d61 6765 5f72 6561 6465 722e 6765   image_reader.ge
+00000910: 745f 6461 7461 2869 6d67 5f6f 626a 290a  t_data(img_obj).
+00000920: 0a20 2020 202d 2054 6865 2060 7265 6164  .    - The `read
+00000930: 6020 6361 6c6c 2063 6f6e 7665 7274 7320  ` call converts 
+00000940: 696d 6167 6520 6669 6c65 6e61 6d65 7320  image filenames 
+00000950: 696e 746f 2069 6d61 6765 206f 626a 6563  into image objec
+00000960: 7473 2c0a 2020 2020 2d20 5468 6520 6067  ts,.    - The `g
+00000970: 6574 5f64 6174 6160 2063 616c 6c20 6665  et_data` call fe
+00000980: 7463 6865 7320 7468 6520 696d 6167 6520  tches the image 
+00000990: 6461 7461 2c20 6173 2077 656c 6c20 6173  data, as well as
+000009a0: 206d 6574 6164 6174 612e 0a20 2020 202d   metadata..    -
+000009b0: 2041 2072 6561 6465 7220 7368 6f75 6c64   A reader should
+000009c0: 2069 6d70 6c65 6d65 6e74 2060 7665 7269   implement `veri
+000009d0: 6679 5f73 7566 6669 7860 2077 6974 6820  fy_suffix` with 
+000009e0: 7468 6520 6c6f 6769 6320 6f66 2063 6865  the logic of che
+000009f0: 636b 696e 6720 7468 6520 696e 7075 7420  cking the input 
+00000a00: 6669 6c65 6e61 6d65 0a20 2020 2020 2062  filename.      b
+00000a10: 7920 7468 6520 6669 6c65 6e61 6d65 2065  y the filename e
+00000a20: 7874 656e 7369 6f6e 732e 0a0a 2020 2020  xtensions...    
+00000a30: 2222 220a 0a20 2020 2040 6162 7374 7261  """..    @abstra
+00000a40: 6374 6d65 7468 6f64 0a20 2020 2064 6566  ctmethod.    def
+00000a50: 2076 6572 6966 795f 7375 6666 6978 2873   verify_suffix(s
+00000a60: 656c 662c 2066 696c 656e 616d 653a 2053  elf, filename: S
+00000a70: 6571 7565 6e63 655b 5061 7468 4c69 6b65  equence[PathLike
+00000a80: 5d20 7c20 5061 7468 4c69 6b65 2920 2d3e  ] | PathLike) ->
+00000a90: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
+00000aa0: 2222 0a20 2020 2020 2020 2056 6572 6966  "".        Verif
+00000ab0: 7920 7768 6574 6865 7220 7468 6520 7370  y whether the sp
+00000ac0: 6563 6966 6965 6420 6066 696c 656e 616d  ecified `filenam
+00000ad0: 6560 2069 7320 7375 7070 6f72 7465 6420  e` is supported 
+00000ae0: 6279 2074 6865 2063 7572 7265 6e74 2072  by the current r
+00000af0: 6561 6465 722e 0a20 2020 2020 2020 2054  eader..        T
+00000b00: 6869 7320 6d65 7468 6f64 2073 686f 756c  his method shoul
+00000b10: 6420 7265 7475 726e 2054 7275 6520 6966  d return True if
+00000b20: 2074 6865 2072 6561 6465 7220 6973 2061   the reader is a
+00000b30: 626c 6520 746f 2072 6561 6420 7468 6520  ble to read the 
+00000b40: 666f 726d 6174 2073 7567 6765 7374 6564  format suggested
+00000b50: 2062 7920 7468 650a 2020 2020 2020 2020   by the.        
+00000b60: 6066 696c 656e 616d 6560 2e0a 0a20 2020  `filename`...   
+00000b70: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00000b80: 2020 2020 2020 2066 696c 656e 616d 653a         filename:
+00000b90: 2066 696c 6520 6e61 6d65 206f 7220 6120   file name or a 
+00000ba0: 6c69 7374 206f 6620 6669 6c65 206e 616d  list of file nam
+00000bb0: 6573 2074 6f20 7265 6164 2e0a 2020 2020  es to read..    
+00000bc0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00000bd0: 206c 6973 7420 6f66 2066 696c 6573 2c20   list of files, 
+00000be0: 7665 7269 6679 2061 6c6c 2074 6865 2073  verify all the s
+00000bf0: 7566 6669 7865 732e 0a0a 2020 2020 2020  uffixes...      
+00000c00: 2020 2222 220a 2020 2020 2020 2020 7261    """.        ra
+00000c10: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+00000c20: 6564 4572 726f 7228 6622 5375 6263 6c61  edError(f"Subcla
+00000c30: 7373 207b 7365 6c66 2e5f 5f63 6c61 7373  ss {self.__class
+00000c40: 5f5f 2e5f 5f6e 616d 655f 5f7d 206d 7573  __.__name__} mus
+00000c50: 7420 696d 706c 656d 656e 7420 7468 6973  t implement this
+00000c60: 206d 6574 686f 642e 2229 0a0a 2020 2020   method.")..    
+00000c70: 4061 6273 7472 6163 746d 6574 686f 640a  @abstractmethod.
+00000c80: 2020 2020 6465 6620 7265 6164 2873 656c      def read(sel
+00000c90: 662c 2064 6174 613a 2053 6571 7565 6e63  f, data: Sequenc
+00000ca0: 655b 5061 7468 4c69 6b65 5d20 7c20 5061  e[PathLike] | Pa
+00000cb0: 7468 4c69 6b65 2c20 2a2a 6b77 6172 6773  thLike, **kwargs
+00000cc0: 2920 2d3e 2053 6571 7565 6e63 655b 416e  ) -> Sequence[An
+00000cd0: 795d 207c 2041 6e79 3a0a 2020 2020 2020  y] | Any:.      
+00000ce0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
+00000cf0: 6164 2069 6d61 6765 2064 6174 6120 6672  ad image data fr
+00000d00: 6f6d 2073 7065 6369 6669 6564 2066 696c  om specified fil
+00000d10: 6520 6f72 2066 696c 6573 2e0a 2020 2020  e or files..    
+00000d20: 2020 2020 4e6f 7465 2074 6861 7420 6974      Note that it
+00000d30: 2072 6574 7572 6e73 2061 2064 6174 6120   returns a data 
+00000d40: 6f62 6a65 6374 206f 7220 6120 7365 7175  object or a sequ
+00000d50: 656e 6365 206f 6620 6461 7461 206f 626a  ence of data obj
+00000d60: 6563 7473 2e0a 0a20 2020 2020 2020 2041  ects...        A
+00000d70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00000d80: 2064 6174 613a 2066 696c 6520 6e61 6d65   data: file name
+00000d90: 206f 7220 6120 6c69 7374 206f 6620 6669   or a list of fi
+00000da0: 6c65 206e 616d 6573 2074 6f20 7265 6164  le names to read
+00000db0: 2e0a 2020 2020 2020 2020 2020 2020 6b77  ..            kw
+00000dc0: 6172 6773 3a20 6164 6469 7469 6f6e 616c  args: additional
+00000dd0: 2061 7267 7320 666f 7220 6163 7475 616c   args for actual
+00000de0: 2060 7265 6164 6020 4150 4920 6f66 2033   `read` API of 3
+00000df0: 7264 2070 6172 7479 206c 6962 732e 0a0a  rd party libs...
+00000e00: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00000e10: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+00000e20: 6c65 6d65 6e74 6564 4572 726f 7228 6622  lementedError(f"
+00000e30: 5375 6263 6c61 7373 207b 7365 6c66 2e5f  Subclass {self._
+00000e40: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
+00000e50: 5f7d 206d 7573 7420 696d 706c 656d 656e  _} must implemen
+00000e60: 7420 7468 6973 206d 6574 686f 642e 2229  t this method.")
+00000e70: 0a0a 2020 2020 4061 6273 7472 6163 746d  ..    @abstractm
+00000e80: 6574 686f 640a 2020 2020 6465 6620 6765  ethod.    def ge
+00000e90: 745f 6461 7461 2873 656c 662c 2069 6d67  t_data(self, img
+00000ea0: 2920 2d3e 2074 7570 6c65 5b6e 702e 6e64  ) -> tuple[np.nd
+00000eb0: 6172 7261 792c 2064 6963 745d 3a0a 2020  array, dict]:.  
+00000ec0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000ed0: 2020 4578 7472 6163 7420 6461 7461 2061    Extract data a
+00000ee0: 7272 6179 2061 6e64 206d 6574 6164 6174  rray and metadat
+00000ef0: 6120 6672 6f6d 206c 6f61 6465 6420 696d  a from loaded im
+00000f00: 6167 6520 616e 6420 7265 7475 726e 2074  age and return t
+00000f10: 6865 6d2e 0a20 2020 2020 2020 2054 6869  hem..        Thi
+00000f20: 7320 6675 6e63 7469 6f6e 206d 7573 7420  s function must 
+00000f30: 7265 7475 726e 2074 776f 206f 626a 6563  return two objec
+00000f40: 7473 2c20 7468 6520 6669 7273 7420 6973  ts, the first is
+00000f50: 2061 206e 756d 7079 2061 7272 6179 206f   a numpy array o
+00000f60: 6620 696d 6167 6520 6461 7461 2c0a 2020  f image data,.  
+00000f70: 2020 2020 2020 7468 6520 7365 636f 6e64        the second
+00000f80: 2069 7320 6120 6469 6374 696f 6e61 7279   is a dictionary
+00000f90: 206f 6620 6d65 7461 6461 7461 2e0a 0a20   of metadata... 
+00000fa0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00000fb0: 2020 2020 2020 2020 2069 6d67 3a20 616e           img: an
+00000fc0: 2069 6d61 6765 206f 626a 6563 7420 6c6f   image object lo
+00000fd0: 6164 6564 2066 726f 6d20 616e 2069 6d61  aded from an ima
+00000fe0: 6765 2066 696c 6520 6f72 2061 206c 6973  ge file or a lis
+00000ff0: 7420 6f66 2069 6d61 6765 206f 626a 6563  t of image objec
+00001000: 7473 2e0a 0a20 2020 2020 2020 2022 2222  ts...        """
+00001010: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
+00001020: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
+00001030: 6f72 2866 2253 7562 636c 6173 7320 7b73  or(f"Subclass {s
+00001040: 656c 662e 5f5f 636c 6173 735f 5f2e 5f5f  elf.__class__.__
+00001050: 6e61 6d65 5f5f 7d20 6d75 7374 2069 6d70  name__} must imp
+00001060: 6c65 6d65 6e74 2074 6869 7320 6d65 7468  lement this meth
+00001070: 6f64 2e22 290a 0a0a 6465 6620 5f63 6f70  od.")...def _cop
+00001080: 795f 636f 6d70 6174 6962 6c65 5f64 6963  y_compatible_dic
+00001090: 7428 6672 6f6d 5f64 6963 743a 2064 6963  t(from_dict: dic
+000010a0: 742c 2074 6f5f 6469 6374 3a20 6469 6374  t, to_dict: dict
+000010b0: 293a 0a20 2020 2069 6620 6e6f 7420 6973  ):.    if not is
+000010c0: 696e 7374 616e 6365 2874 6f5f 6469 6374  instance(to_dict
+000010d0: 2c20 6469 6374 293a 0a20 2020 2020 2020  , dict):.       
+000010e0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+000010f0: 7228 6622 746f 5f64 6963 7420 6d75 7374  r(f"to_dict must
+00001100: 2062 6520 6120 4469 6374 2c20 676f 7420   be a Dict, got 
+00001110: 7b74 7970 6528 746f 5f64 6963 7429 7d2e  {type(to_dict)}.
+00001120: 2229 0a20 2020 2069 6620 6e6f 7420 746f  ").    if not to
+00001130: 5f64 6963 743a 0a20 2020 2020 2020 2066  _dict:.        f
+00001140: 6f72 206b 6579 2069 6e20 6672 6f6d 5f64  or key in from_d
+00001150: 6963 743a 0a20 2020 2020 2020 2020 2020  ict:.           
+00001160: 2064 6174 756d 203d 2066 726f 6d5f 6469   datum = from_di
+00001170: 6374 5b6b 6579 5d0a 2020 2020 2020 2020  ct[key].        
+00001180: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00001190: 6528 6461 7475 6d2c 206e 702e 6e64 6172  e(datum, np.ndar
+000011a0: 7261 7929 2061 6e64 206e 705f 7374 725f  ray) and np_str_
+000011b0: 6f62 6a5f 6172 7261 795f 7061 7474 6572  obj_array_patter
+000011c0: 6e2e 7365 6172 6368 2864 6174 756d 2e64  n.search(datum.d
+000011d0: 7479 7065 2e73 7472 2920 6973 206e 6f74  type.str) is not
+000011e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000011f0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00001200: 2020 2020 2020 2020 2020 2020 746f 5f64              to_d
+00001210: 6963 745b 6b65 795d 203d 2073 7472 2854  ict[key] = str(T
+00001220: 7261 6365 4b65 7973 2e4e 4f4e 4529 2069  raceKeys.NONE) i
+00001230: 6620 6461 7475 6d20 6973 204e 6f6e 6520  f datum is None 
+00001240: 656c 7365 2064 6174 756d 2020 2320 4e6f  else datum  # No
+00001250: 6e65 5479 7065 2074 6f20 7374 7269 6e67  neType to string
+00001260: 2066 6f72 2064 6566 6175 6c74 5f63 6f6c   for default_col
+00001270: 6c61 7465 0a20 2020 2065 6c73 653a 0a20  late.    else:. 
+00001280: 2020 2020 2020 2061 6666 696e 655f 6b65         affine_ke
+00001290: 792c 2073 6861 7065 5f6b 6579 203d 204d  y, shape_key = M
+000012a0: 6574 614b 6579 732e 4146 4649 4e45 2c20  etaKeys.AFFINE, 
+000012b0: 4d65 7461 4b65 7973 2e53 5041 5449 414c  MetaKeys.SPATIAL
+000012c0: 5f53 4841 5045 0a20 2020 2020 2020 2069  _SHAPE.        i
+000012d0: 6620 6166 6669 6e65 5f6b 6579 2069 6e20  f affine_key in 
+000012e0: 6672 6f6d 5f64 6963 7420 616e 6420 6e6f  from_dict and no
+000012f0: 7420 6e70 2e61 6c6c 636c 6f73 6528 6672  t np.allclose(fr
+00001300: 6f6d 5f64 6963 745b 6166 6669 6e65 5f6b  om_dict[affine_k
+00001310: 6579 5d2c 2074 6f5f 6469 6374 5b61 6666  ey], to_dict[aff
+00001320: 696e 655f 6b65 795d 293a 0a20 2020 2020  ine_key]):.     
+00001330: 2020 2020 2020 2072 6169 7365 2052 756e         raise Run
+00001340: 7469 6d65 4572 726f 7228 0a20 2020 2020  timeError(.     
+00001350: 2020 2020 2020 2020 2020 2022 6166 6669             "affi
+00001360: 6e65 206d 6174 7269 7820 6f66 2061 6c6c  ne matrix of all
+00001370: 2069 6d61 6765 7320 7368 6f75 6c64 2062   images should b
+00001380: 6520 7468 6520 7361 6d65 2066 6f72 2063  e the same for c
+00001390: 6861 6e6e 656c 2d77 6973 6520 636f 6e63  hannel-wise conc
+000013a0: 6174 656e 6174 696f 6e2e 2022 0a20 2020  atenation. ".   
+000013b0: 2020 2020 2020 2020 2020 2020 2066 2247               f"G
+000013c0: 6f74 207b 6672 6f6d 5f64 6963 745b 6166  ot {from_dict[af
+000013d0: 6669 6e65 5f6b 6579 5d7d 2061 6e64 207b  fine_key]} and {
+000013e0: 746f 5f64 6963 745b 6166 6669 6e65 5f6b  to_dict[affine_k
+000013f0: 6579 5d7d 2e22 0a20 2020 2020 2020 2020  ey]}.".         
+00001400: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00001410: 7368 6170 655f 6b65 7920 696e 2066 726f  shape_key in fro
+00001420: 6d5f 6469 6374 2061 6e64 206e 6f74 206e  m_dict and not n
+00001430: 702e 616c 6c63 6c6f 7365 2866 726f 6d5f  p.allclose(from_
+00001440: 6469 6374 5b73 6861 7065 5f6b 6579 5d2c  dict[shape_key],
+00001450: 2074 6f5f 6469 6374 5b73 6861 7065 5f6b   to_dict[shape_k
+00001460: 6579 5d29 3a0a 2020 2020 2020 2020 2020  ey]):.          
+00001470: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
+00001480: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00001490: 2020 2020 2020 2273 7061 7469 616c 5f73        "spatial_s
+000014a0: 6861 7065 206f 6620 616c 6c20 696d 6167  hape of all imag
+000014b0: 6573 2073 686f 756c 6420 6265 2074 6865  es should be the
+000014c0: 2073 616d 6520 666f 7220 6368 616e 6e65   same for channe
+000014d0: 6c2d 7769 7365 2063 6f6e 6361 7465 6e61  l-wise concatena
+000014e0: 7469 6f6e 2e20 220a 2020 2020 2020 2020  tion. ".        
+000014f0: 2020 2020 2020 2020 6622 476f 7420 7b66          f"Got {f
+00001500: 726f 6d5f 6469 6374 5b73 6861 7065 5f6b  rom_dict[shape_k
+00001510: 6579 5d7d 2061 6e64 207b 746f 5f64 6963  ey]} and {to_dic
+00001520: 745b 7368 6170 655f 6b65 795d 7d2e 220a  t[shape_key]}.".
+00001530: 2020 2020 2020 2020 2020 2020 290a 0a0a              )...
+00001540: 6465 6620 5f73 7461 636b 5f69 6d61 6765  def _stack_image
+00001550: 7328 696d 6167 655f 6c69 7374 3a20 6c69  s(image_list: li
+00001560: 7374 2c20 6d65 7461 5f64 6963 743a 2064  st, meta_dict: d
+00001570: 6963 7429 3a0a 2020 2020 6966 206c 656e  ict):.    if len
+00001580: 2869 6d61 6765 5f6c 6973 7429 203c 3d20  (image_list) <= 
+00001590: 313a 0a20 2020 2020 2020 2072 6574 7572  1:.        retur
+000015a0: 6e20 696d 6167 655f 6c69 7374 5b30 5d0a  n image_list[0].
+000015b0: 2020 2020 6966 206e 6f74 2069 735f 6e6f      if not is_no
+000015c0: 5f63 6861 6e6e 656c 286d 6574 615f 6469  _channel(meta_di
+000015d0: 6374 2e67 6574 284d 6574 614b 6579 732e  ct.get(MetaKeys.
+000015e0: 4f52 4947 494e 414c 5f43 4841 4e4e 454c  ORIGINAL_CHANNEL
+000015f0: 5f44 494d 2c20 4e6f 6e65 2929 3a0a 2020  _DIM, None)):.  
+00001600: 2020 2020 2020 6368 616e 6e65 6c5f 6469        channel_di
+00001610: 6d20 3d20 696e 7428 6d65 7461 5f64 6963  m = int(meta_dic
+00001620: 745b 4d65 7461 4b65 7973 2e4f 5249 4749  t[MetaKeys.ORIGI
+00001630: 4e41 4c5f 4348 414e 4e45 4c5f 4449 4d5d  NAL_CHANNEL_DIM]
+00001640: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00001650: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
+00001660: 696d 6167 655f 6c69 7374 2c20 6178 6973  image_list, axis
+00001670: 3d63 6861 6e6e 656c 5f64 696d 290a 2020  =channel_dim).  
+00001680: 2020 2320 7374 6163 6b20 6174 2061 206e    # stack at a n
+00001690: 6577 2066 6972 7374 2064 696d 2061 7320  ew first dim as 
+000016a0: 7468 6520 6368 616e 6e65 6c20 6469 6d2c  the channel dim,
+000016b0: 2069 6620 6027 6f72 6967 696e 616c 5f63   if `'original_c
+000016c0: 6861 6e6e 656c 5f64 696d 2760 2069 7320  hannel_dim'` is 
+000016d0: 756e 7370 6563 6966 6965 640a 2020 2020  unspecified.    
+000016e0: 6d65 7461 5f64 6963 745b 4d65 7461 4b65  meta_dict[MetaKe
+000016f0: 7973 2e4f 5249 4749 4e41 4c5f 4348 414e  ys.ORIGINAL_CHAN
+00001700: 4e45 4c5f 4449 4d5d 203d 2030 0a20 2020  NEL_DIM] = 0.   
+00001710: 2072 6574 7572 6e20 6e70 2e73 7461 636b   return np.stack
+00001720: 2869 6d61 6765 5f6c 6973 742c 2061 7869  (image_list, axi
+00001730: 733d 3029 0a0a 0a40 7265 7175 6972 655f  s=0)...@require_
+00001740: 706b 6728 706b 675f 6e61 6d65 3d22 6974  pkg(pkg_name="it
+00001750: 6b22 290a 636c 6173 7320 4954 4b52 6561  k").class ITKRea
+00001760: 6465 7228 496d 6167 6552 6561 6465 7229  der(ImageReader)
+00001770: 3a0a 2020 2020 2222 220a 2020 2020 4c6f  :.    """.    Lo
+00001780: 6164 206d 6564 6963 616c 2069 6d61 6765  ad medical image
+00001790: 7320 6261 7365 6420 6f6e 2049 544b 206c  s based on ITK l
+000017a0: 6962 7261 7279 2e0a 2020 2020 416c 6c20  ibrary..    All 
+000017b0: 7468 6520 7375 7070 6f72 7465 6420 696d  the supported im
+000017c0: 6167 6520 666f 726d 6174 7320 6361 6e20  age formats can 
+000017d0: 6265 2066 6f75 6e64 2061 743a 0a20 2020  be found at:.   
+000017e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+000017f0: 636f 6d2f 496e 7369 6768 7453 6f66 7477  com/InsightSoftw
+00001800: 6172 6543 6f6e 736f 7274 6975 6d2f 4954  areConsortium/IT
+00001810: 4b2f 7472 6565 2f6d 6173 7465 722f 4d6f  K/tree/master/Mo
+00001820: 6475 6c65 732f 494f 0a20 2020 2054 6865  dules/IO.    The
+00001830: 206c 6f61 6465 6420 6461 7461 2061 7272   loaded data arr
+00001840: 6179 2077 696c 6c20 6265 2069 6e20 4320  ay will be in C 
+00001850: 6f72 6465 722c 2066 6f72 2065 7861 6d70  order, for examp
+00001860: 6c65 2c20 6120 3344 2069 6d61 6765 204e  le, a 3D image N
+00001870: 756d 5079 0a20 2020 2061 7272 6179 2069  umPy.    array i
+00001880: 6e64 6578 206f 7264 6572 2077 696c 6c20  ndex order will 
+00001890: 6265 2060 4344 5748 602e 0a0a 2020 2020  be `CDWH`...    
+000018a0: 4172 6773 3a0a 2020 2020 2020 2020 6368  Args:.        ch
+000018b0: 616e 6e65 6c5f 6469 6d3a 2074 6865 2063  annel_dim: the c
+000018c0: 6861 6e6e 656c 2064 696d 656e 7369 6f6e  hannel dimension
+000018d0: 206f 6620 7468 6520 696e 7075 7420 696d   of the input im
+000018e0: 6167 652c 2064 6566 6175 6c74 2069 7320  age, default is 
+000018f0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+00001900: 2020 5468 6973 2069 7320 7573 6564 2074    This is used t
+00001910: 6f20 7365 7420 6f72 6967 696e 616c 5f63  o set original_c
+00001920: 6861 6e6e 656c 5f64 696d 2069 6e20 7468  hannel_dim in th
+00001930: 6520 6d65 7461 6461 7461 2c20 456e 7375  e metadata, Ensu
+00001940: 7265 4368 616e 6e65 6c46 6972 7374 4420  reChannelFirstD 
+00001950: 7265 6164 7320 7468 6973 2066 6965 6c64  reads this field
+00001960: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00001970: 204e 6f6e 652c 2060 6f72 6967 696e 616c   None, `original
+00001980: 5f63 6861 6e6e 656c 5f64 696d 6020 7769  _channel_dim` wi
+00001990: 6c6c 2062 6520 6569 7468 6572 2060 6e6f  ll be either `no
+000019a0: 5f63 6861 6e6e 656c 6020 6f72 2060 2d31  _channel` or `-1
+000019b0: 602e 0a0a 2020 2020 2020 2020 2020 2020  `...            
+000019c0: 2020 2020 2d20 4e69 6674 6920 6669 6c65      - Nifti file
+000019d0: 2069 7320 7573 7561 6c6c 7920 2263 6861   is usually "cha
+000019e0: 6e6e 656c 206c 6173 7422 2c20 736f 2074  nnel last", so t
+000019f0: 6865 7265 2069 7320 6e6f 206e 6565 6420  here is no need 
+00001a00: 746f 2073 7065 6369 6679 2074 6869 7320  to specify this 
+00001a10: 6172 6775 6d65 6e74 2e0a 2020 2020 2020  argument..      
+00001a20: 2020 2020 2020 2020 2020 2d20 504e 4720            - PNG 
+00001a30: 6669 6c65 2075 7375 616c 6c79 2068 6173  file usually has
+00001a40: 2060 4765 744e 756d 6265 724f 6643 6f6d   `GetNumberOfCom
+00001a50: 706f 6e65 6e74 7350 6572 5069 7865 6c28  ponentsPerPixel(
+00001a60: 293d 3d33 602c 2073 6f20 7468 6572 6520  )==3`, so there 
+00001a70: 6973 206e 6f20 6e65 6564 2074 6f20 7370  is no need to sp
+00001a80: 6563 6966 7920 7468 6973 2061 7267 756d  ecify this argum
+00001a90: 656e 742e 0a0a 2020 2020 2020 2020 7365  ent...        se
+00001aa0: 7269 6573 5f6e 616d 653a 2074 6865 206e  ries_name: the n
+00001ab0: 616d 6520 6f66 2074 6865 2044 4943 4f4d  ame of the DICOM
+00001ac0: 2073 6572 6965 7320 6966 2074 6865 7265   series if there
+00001ad0: 2061 7265 206d 756c 7469 706c 6520 6f6e   are multiple on
+00001ae0: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+00001af0: 7573 6564 2077 6865 6e20 6c6f 6164 696e  used when loadin
+00001b00: 6720 4449 434f 4d20 7365 7269 6573 2e0a  g DICOM series..
+00001b10: 2020 2020 2020 2020 7265 7665 7273 655f          reverse_
+00001b20: 696e 6465 7869 6e67 3a20 7768 6574 6865  indexing: whethe
+00001b30: 7220 746f 2075 7365 2061 2072 6576 6572  r to use a rever
+00001b40: 7365 6420 7370 6174 6961 6c20 696e 6465  sed spatial inde
+00001b50: 7869 6e67 2063 6f6e 7665 6e74 696f 6e20  xing convention 
+00001b60: 666f 7220 7468 6520 7265 7475 726e 6564  for the returned
+00001b70: 2064 6174 6120 6172 7261 792e 0a20 2020   data array..   
+00001b80: 2020 2020 2020 2020 2049 6620 6060 4661           If ``Fa
+00001b90: 6c73 6560 602c 2074 6865 2073 7061 7469  lse``, the spati
+00001ba0: 616c 2069 6e64 6578 696e 6720 666f 6c6c  al indexing foll
+00001bb0: 6f77 7320 7468 6520 6e75 6d70 7920 636f  ows the numpy co
+00001bc0: 6e76 656e 7469 6f6e 3b0a 2020 2020 2020  nvention;.      
+00001bd0: 2020 2020 2020 6f74 6865 7277 6973 652c        otherwise,
+00001be0: 2074 6865 2073 7061 7469 616c 2069 6e64   the spatial ind
+00001bf0: 6578 696e 6720 636f 6e76 656e 7469 6f6e  exing convention
+00001c00: 2069 7320 7265 7665 7273 6564 2074 6f20   is reversed to 
+00001c10: 6265 2063 6f6d 7061 7469 626c 6520 7769  be compatible wi
+00001c20: 7468 2049 544b 2e20 4465 6661 756c 7420  th ITK. Default 
+00001c30: 6973 2060 6046 616c 7365 6060 2e0a 2020  is ``False``..  
+00001c40: 2020 2020 2020 2020 2020 5468 6973 206f            This o
+00001c50: 7074 696f 6e20 646f 6573 206e 6f74 2061  ption does not a
+00001c60: 6666 6563 7420 7468 6520 6d65 7461 6461  ffect the metada
+00001c70: 7461 2e0a 2020 2020 2020 2020 7365 7269  ta..        seri
+00001c80: 6573 5f6d 6574 613a 2077 6865 7468 6572  es_meta: whether
+00001c90: 2074 6f20 6c6f 6164 2074 6865 206d 6574   to load the met
+00001ca0: 6164 6174 6120 6f66 2074 6865 2044 4943  adata of the DIC
+00001cb0: 4f4d 2073 6572 6965 7320 2875 7369 6e67  OM series (using
+00001cc0: 2074 6865 206d 6574 6164 6174 6120 6672   the metadata fr
+00001cd0: 6f6d 2074 6865 2066 6972 7374 2073 6c69  om the first sli
+00001ce0: 6365 292e 0a20 2020 2020 2020 2020 2020  ce)..           
+00001cf0: 2054 6869 7320 666c 6167 2069 7320 6368   This flag is ch
+00001d00: 6563 6b65 6420 6f6e 6c79 2077 6865 6e20  ecked only when 
+00001d10: 6c6f 6164 696e 6720 4449 434f 4d20 7365  loading DICOM se
+00001d20: 7269 6573 2e20 4465 6661 756c 7420 6973  ries. Default is
+00001d30: 2060 6046 616c 7365 6060 2e0a 2020 2020   ``False``..    
+00001d40: 2020 2020 6166 6669 6e65 5f6c 7073 5f74      affine_lps_t
+00001d50: 6f5f 7261 733a 2077 6865 7468 6572 2074  o_ras: whether t
+00001d60: 6f20 636f 6e76 6572 7420 7468 6520 6166  o convert the af
+00001d70: 6669 6e65 206d 6174 7269 7820 6672 6f6d  fine matrix from
+00001d80: 2022 4c50 5322 2074 6f20 2252 4153 222e   "LPS" to "RAS".
+00001d90: 2044 6566 6175 6c74 7320 746f 2060 6054   Defaults to ``T
+00001da0: 7275 6560 602e 0a20 2020 2020 2020 2020  rue``..         
+00001db0: 2020 2053 6574 2074 6f20 6060 5472 7565     Set to ``True
+00001dc0: 6060 2074 6f20 6265 2063 6f6e 7369 7374  `` to be consist
+00001dd0: 656e 7420 7769 7468 2060 604e 6962 6162  ent with ``Nibab
+00001de0: 656c 5265 6164 6572 6060 2c20 6f74 6865  elReader``, othe
+00001df0: 7277 6973 6520 7468 6520 6166 6669 6e65  rwise the affine
+00001e00: 206d 6174 7269 7820 7265 6d61 696e 7320   matrix remains 
+00001e10: 696e 2074 6865 2049 544b 2063 6f6e 7665  in the ITK conve
+00001e20: 6e74 696f 6e2e 0a20 2020 2020 2020 206b  ntion..        k
+00001e30: 7761 7267 733a 2061 6464 6974 696f 6e61  wargs: additiona
+00001e40: 6c20 6172 6773 2066 6f72 2060 6974 6b2e  l args for `itk.
+00001e50: 696d 7265 6164 6020 4150 492e 206d 6f72  imread` API. mor
+00001e60: 6520 6465 7461 696c 7320 6162 6f75 7420  e details about 
+00001e70: 6176 6169 6c61 626c 6520 6172 6773 3a0a  available args:.
+00001e80: 2020 2020 2020 2020 2020 2020 6874 7470              http
+00001e90: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f49  s://github.com/I
+00001ea0: 6e73 6967 6874 536f 6674 7761 7265 436f  nsightSoftwareCo
+00001eb0: 6e73 6f72 7469 756d 2f49 544b 2f62 6c6f  nsortium/ITK/blo
+00001ec0: 622f 6d61 7374 6572 2f57 7261 7070 696e  b/master/Wrappin
+00001ed0: 672f 4765 6e65 7261 746f 7273 2f50 7974  g/Generators/Pyt
+00001ee0: 686f 6e2f 6974 6b2f 7375 7070 6f72 742f  hon/itk/support/
+00001ef0: 6578 7472 6173 2e70 790a 0a20 2020 2022  extras.py..    "
+00001f00: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+00001f10: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00001f20: 6c66 2c0a 2020 2020 2020 2020 6368 616e  lf,.        chan
+00001f30: 6e65 6c5f 6469 6d3a 2073 7472 207c 2069  nel_dim: str | i
+00001f40: 6e74 207c 204e 6f6e 6520 3d20 4e6f 6e65  nt | None = None
+00001f50: 2c0a 2020 2020 2020 2020 7365 7269 6573  ,.        series
+00001f60: 5f6e 616d 653a 2073 7472 203d 2022 222c  _name: str = "",
+00001f70: 0a20 2020 2020 2020 2072 6576 6572 7365  .        reverse
+00001f80: 5f69 6e64 6578 696e 673a 2062 6f6f 6c20  _indexing: bool 
+00001f90: 3d20 4661 6c73 652c 0a20 2020 2020 2020  = False,.       
+00001fa0: 2073 6572 6965 735f 6d65 7461 3a20 626f   series_meta: bo
+00001fb0: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+00001fc0: 2020 2020 6166 6669 6e65 5f6c 7073 5f74      affine_lps_t
+00001fd0: 6f5f 7261 733a 2062 6f6f 6c20 3d20 5472  o_ras: bool = Tr
+00001fe0: 7565 2c0a 2020 2020 2020 2020 2a2a 6b77  ue,.        **kw
+00001ff0: 6172 6773 2c0a 2020 2020 293a 0a20 2020  args,.    ):.   
+00002000: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
+00002010: 6e69 745f 5f28 290a 2020 2020 2020 2020  nit__().        
+00002020: 7365 6c66 2e6b 7761 7267 7320 3d20 6b77  self.kwargs = kw
+00002030: 6172 6773 0a20 2020 2020 2020 2073 656c  args.        sel
+00002040: 662e 6368 616e 6e65 6c5f 6469 6d20 3d20  f.channel_dim = 
+00002050: 666c 6f61 7428 226e 616e 2229 2069 6620  float("nan") if 
+00002060: 6368 616e 6e65 6c5f 6469 6d20 3d3d 2022  channel_dim == "
+00002070: 6e6f 5f63 6861 6e6e 656c 2220 656c 7365  no_channel" else
+00002080: 2063 6861 6e6e 656c 5f64 696d 0a20 2020   channel_dim.   
+00002090: 2020 2020 2073 656c 662e 7365 7269 6573       self.series
+000020a0: 5f6e 616d 6520 3d20 7365 7269 6573 5f6e  _name = series_n
+000020b0: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
+000020c0: 2e72 6576 6572 7365 5f69 6e64 6578 696e  .reverse_indexin
+000020d0: 6720 3d20 7265 7665 7273 655f 696e 6465  g = reverse_inde
+000020e0: 7869 6e67 0a20 2020 2020 2020 2073 656c  xing.        sel
+000020f0: 662e 7365 7269 6573 5f6d 6574 6120 3d20  f.series_meta = 
+00002100: 7365 7269 6573 5f6d 6574 610a 2020 2020  series_meta.    
+00002110: 2020 2020 7365 6c66 2e61 6666 696e 655f      self.affine_
+00002120: 6c70 735f 746f 5f72 6173 203d 2061 6666  lps_to_ras = aff
+00002130: 696e 655f 6c70 735f 746f 5f72 6173 0a0a  ine_lps_to_ras..
+00002140: 2020 2020 6465 6620 7665 7269 6679 5f73      def verify_s
+00002150: 7566 6669 7828 7365 6c66 2c20 6669 6c65  uffix(self, file
+00002160: 6e61 6d65 3a20 5365 7175 656e 6365 5b50  name: Sequence[P
+00002170: 6174 684c 696b 655d 207c 2050 6174 684c  athLike] | PathL
+00002180: 696b 6529 202d 3e20 626f 6f6c 3a0a 2020  ike) -> bool:.  
+00002190: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000021a0: 2020 5665 7269 6679 2077 6865 7468 6572    Verify whether
+000021b0: 2074 6865 2073 7065 6369 6669 6564 2066   the specified f
+000021c0: 696c 6520 6f72 2066 696c 6573 2066 6f72  ile or files for
+000021d0: 6d61 7420 6973 2073 7570 706f 7274 6564  mat is supported
+000021e0: 2062 7920 4954 4b20 7265 6164 6572 2e0a   by ITK reader..
+000021f0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00002200: 2020 2020 2020 2020 2020 2066 696c 656e             filen
+00002210: 616d 653a 2066 696c 6520 6e61 6d65 206f  ame: file name o
+00002220: 7220 6120 6c69 7374 206f 6620 6669 6c65  r a list of file
+00002230: 206e 616d 6573 2074 6f20 7265 6164 2e0a   names to read..
+00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002250: 6966 2061 206c 6973 7420 6f66 2066 696c  if a list of fil
+00002260: 6573 2c20 7665 7269 6679 2061 6c6c 2074  es, verify all t
+00002270: 6865 2073 7566 6669 7865 732e 0a0a 2020  he suffixes...  
+00002280: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00002290: 2020 7265 7475 726e 2068 6173 5f69 746b    return has_itk
+000022a0: 0a0a 2020 2020 6465 6620 7265 6164 2873  ..    def read(s
+000022b0: 656c 662c 2064 6174 613a 2053 6571 7565  elf, data: Seque
+000022c0: 6e63 655b 5061 7468 4c69 6b65 5d20 7c20  nce[PathLike] | 
+000022d0: 5061 7468 4c69 6b65 2c20 2a2a 6b77 6172  PathLike, **kwar
+000022e0: 6773 293a 0a20 2020 2020 2020 2022 2222  gs):.        """
+000022f0: 0a20 2020 2020 2020 2052 6561 6420 696d  .        Read im
+00002300: 6167 6520 6461 7461 2066 726f 6d20 7370  age data from sp
+00002310: 6563 6966 6965 6420 6669 6c65 206f 7220  ecified file or 
+00002320: 6669 6c65 732c 2069 7420 6361 6e20 7265  files, it can re
+00002330: 6164 2061 206c 6973 7420 6f66 2069 6d61  ad a list of ima
+00002340: 6765 730a 2020 2020 2020 2020 616e 6420  ges.        and 
+00002350: 7374 6163 6b20 7468 656d 2074 6f67 6574  stack them toget
+00002360: 6865 7220 6173 206d 756c 7469 2d63 6861  her as multi-cha
+00002370: 6e6e 656c 2064 6174 6120 696e 2060 6765  nnel data in `ge
+00002380: 745f 6461 7461 2829 602e 0a20 2020 2020  t_data()`..     
+00002390: 2020 2049 6620 7061 7373 696e 6720 6469     If passing di
+000023a0: 7265 6374 6f72 7920 7061 7468 2069 6e73  rectory path ins
+000023b0: 7465 6164 206f 6620 6669 6c65 2070 6174  tead of file pat
+000023c0: 682c 2077 696c 6c20 7472 6561 7420 6974  h, will treat it
+000023d0: 2061 7320 4449 434f 4d20 696d 6167 6573   as DICOM images
+000023e0: 2073 6572 6965 7320 616e 6420 7265 6164   series and read
+000023f0: 2e0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
+00002400: 6861 7420 7468 6520 7265 7475 726e 6564  hat the returned
+00002410: 206f 626a 6563 7420 6973 2049 544b 2069   object is ITK i
+00002420: 6d61 6765 206f 626a 6563 7420 6f72 206c  mage object or l
+00002430: 6973 7420 6f66 2049 544b 2069 6d61 6765  ist of ITK image
+00002440: 206f 626a 6563 7473 2e0a 0a20 2020 2020   objects...     
+00002450: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00002460: 2020 2020 2064 6174 613a 2066 696c 6520       data: file 
+00002470: 6e61 6d65 206f 7220 6120 6c69 7374 206f  name or a list o
+00002480: 6620 6669 6c65 206e 616d 6573 2074 6f20  f file names to 
+00002490: 7265 6164 2c0a 2020 2020 2020 2020 2020  read,.          
+000024a0: 2020 6b77 6172 6773 3a20 6164 6469 7469    kwargs: additi
+000024b0: 6f6e 616c 2061 7267 7320 666f 7220 6069  onal args for `i
+000024c0: 746b 2e69 6d72 6561 6460 2041 5049 2c20  tk.imread` API, 
+000024d0: 7769 6c6c 206f 7665 7272 6964 6520 6073  will override `s
+000024e0: 656c 662e 6b77 6172 6773 6020 666f 7220  elf.kwargs` for 
+000024f0: 6578 6973 7469 6e67 206b 6579 732e 0a20  existing keys.. 
+00002500: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+00002510: 6f72 6520 6465 7461 696c 7320 6162 6f75  ore details abou
+00002520: 7420 6176 6169 6c61 626c 6520 6172 6773  t available args
+00002530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002540: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
+00002550: 2e63 6f6d 2f49 6e73 6967 6874 536f 6674  .com/InsightSoft
+00002560: 7761 7265 436f 6e73 6f72 7469 756d 2f49  wareConsortium/I
+00002570: 544b 2f62 6c6f 622f 6d61 7374 6572 2f57  TK/blob/master/W
+00002580: 7261 7070 696e 672f 4765 6e65 7261 746f  rapping/Generato
+00002590: 7273 2f50 7974 686f 6e2f 6974 6b45 7874  rs/Python/itkExt
+000025a0: 7261 732e 7079 0a0a 2020 2020 2020 2020  ras.py..        
+000025b0: 2222 220a 2020 2020 2020 2020 696d 675f  """.        img_
+000025c0: 203d 205b 5d0a 0a20 2020 2020 2020 2066   = []..        f
+000025d0: 696c 656e 616d 6573 3a20 5365 7175 656e  ilenames: Sequen
+000025e0: 6365 5b50 6174 684c 696b 655d 203d 2065  ce[PathLike] = e
+000025f0: 6e73 7572 655f 7475 706c 6528 6461 7461  nsure_tuple(data
+00002600: 290a 2020 2020 2020 2020 6b77 6172 6773  ).        kwargs
+00002610: 5f20 3d20 7365 6c66 2e6b 7761 7267 732e  _ = self.kwargs.
+00002620: 636f 7079 2829 0a20 2020 2020 2020 206b  copy().        k
+00002630: 7761 7267 735f 2e75 7064 6174 6528 6b77  wargs_.update(kw
+00002640: 6172 6773 290a 2020 2020 2020 2020 666f  args).        fo
+00002650: 7220 6e61 6d65 2069 6e20 6669 6c65 6e61  r name in filena
+00002660: 6d65 733a 0a20 2020 2020 2020 2020 2020  mes:.           
+00002670: 206e 616d 6520 3d20 6622 7b6e 616d 657d   name = f"{name}
+00002680: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
+00002690: 2050 6174 6828 6e61 6d65 292e 6973 5f64   Path(name).is_d
+000026a0: 6972 2829 3a0a 2020 2020 2020 2020 2020  ir():.          
+000026b0: 2020 2020 2020 2320 7265 6164 2044 4943        # read DIC
+000026c0: 4f4d 2073 6572 6965 730a 2020 2020 2020  OM series.      
+000026d0: 2020 2020 2020 2020 2020 2320 6874 7470            # http
+000026e0: 733a 2f2f 6974 6b2e 6f72 672f 4954 4b45  s://itk.org/ITKE
+000026f0: 7861 6d70 6c65 732f 7372 632f 494f 2f47  xamples/src/IO/G
+00002700: 4443 4d2f 5265 6164 4449 434f 4d53 6572  DCM/ReadDICOMSer
+00002710: 6965 7341 6e64 5772 6974 6533 4449 6d61  iesAndWrite3DIma
+00002720: 6765 0a20 2020 2020 2020 2020 2020 2020  ge.             
+00002730: 2020 206e 616d 6573 5f67 656e 6572 6174     names_generat
+00002740: 6f72 203d 2069 746b 2e47 4443 4d53 6572  or = itk.GDCMSer
+00002750: 6965 7346 696c 654e 616d 6573 2e4e 6577  iesFileNames.New
+00002760: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00002770: 2020 206e 616d 6573 5f67 656e 6572 6174     names_generat
+00002780: 6f72 2e53 6574 5573 6553 6572 6965 7344  or.SetUseSeriesD
+00002790: 6574 6169 6c73 2854 7275 6529 0a20 2020  etails(True).   
+000027a0: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+000027b0: 6573 5f67 656e 6572 6174 6f72 2e41 6464  es_generator.Add
+000027c0: 5365 7269 6573 5265 7374 7269 6374 696f  SeriesRestrictio
+000027d0: 6e28 2230 3030 387c 3030 3231 2229 2020  n("0008|0021")  
+000027e0: 2320 5365 7269 6573 2044 6174 650a 2020  # Series Date.  
+000027f0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+00002800: 6d65 735f 6765 6e65 7261 746f 722e 5365  mes_generator.Se
+00002810: 7444 6972 6563 746f 7279 286e 616d 6529  tDirectory(name)
+00002820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002830: 2073 6572 6965 735f 7569 6420 3d20 6e61   series_uid = na
+00002840: 6d65 735f 6765 6e65 7261 746f 722e 4765  mes_generator.Ge
+00002850: 7453 6572 6965 7355 4944 7328 290a 0a20  tSeriesUIDs().. 
+00002860: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002870: 6620 6c65 6e28 7365 7269 6573 5f75 6964  f len(series_uid
+00002880: 2920 3c20 313a 0a20 2020 2020 2020 2020  ) < 1:.         
+00002890: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000028a0: 2046 696c 654e 6f74 466f 756e 6445 7272   FileNotFoundErr
+000028b0: 6f72 2866 226e 6f20 4449 434f 4d73 2069  or(f"no DICOMs i
+000028c0: 6e3a 207b 6e61 6d65 7d2e 2229 0a20 2020  n: {name}.").   
+000028d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000028e0: 6c65 6e28 7365 7269 6573 5f75 6964 2920  len(series_uid) 
+000028f0: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
+00002900: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+00002910: 732e 7761 726e 2866 2274 6865 2064 6972  s.warn(f"the dir
+00002920: 6563 746f 7279 3a20 7b6e 616d 657d 2063  ectory: {name} c
+00002930: 6f6e 7461 696e 7320 6d6f 7265 2074 6861  ontains more tha
+00002940: 6e20 6f6e 6520 4449 434f 4d20 7365 7269  n one DICOM seri
+00002950: 6573 2e22 290a 2020 2020 2020 2020 2020  es.").          
+00002960: 2020 2020 2020 7365 7269 6573 5f69 6465        series_ide
+00002970: 6e74 6966 6965 7220 3d20 7365 7269 6573  ntifier = series
+00002980: 5f75 6964 5b30 5d20 6966 206e 6f74 2073  _uid[0] if not s
+00002990: 656c 662e 7365 7269 6573 5f6e 616d 6520  elf.series_name 
+000029a0: 656c 7365 2073 656c 662e 7365 7269 6573  else self.series
+000029b0: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
+000029c0: 2020 2020 2020 6e61 6d65 203d 206e 616d        name = nam
+000029d0: 6573 5f67 656e 6572 6174 6f72 2e47 6574  es_generator.Get
+000029e0: 4669 6c65 4e61 6d65 7328 7365 7269 6573  FileNames(series
+000029f0: 5f69 6465 6e74 6966 6965 7229 0a0a 2020  _identifier)..  
+00002a00: 2020 2020 2020 2020 2020 2020 2020 5f6f                _o
+00002a10: 626a 203d 2069 746b 2e69 6d72 6561 6428  bj = itk.imread(
+00002a20: 6e61 6d65 2c20 2a2a 6b77 6172 6773 5f29  name, **kwargs_)
+00002a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a40: 2069 6620 7365 6c66 2e73 6572 6965 735f   if self.series_
+00002a50: 6d65 7461 3a0a 2020 2020 2020 2020 2020  meta:.          
+00002a60: 2020 2020 2020 2020 2020 5f72 6561 6465            _reade
+00002a70: 7220 3d20 6974 6b2e 496d 6167 6553 6572  r = itk.ImageSer
+00002a80: 6965 7352 6561 6465 722e 4e65 7728 4669  iesReader.New(Fi
+00002a90: 6c65 4e61 6d65 733d 6e61 6d65 290a 2020  leNames=name).  
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ab0: 2020 5f72 6561 6465 722e 5570 6461 7465    _reader.Update
+00002ac0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00002ad0: 2020 2020 2020 205f 6d65 7461 203d 205f         _meta = _
+00002ae0: 7265 6164 6572 2e47 6574 4d65 7461 4461  reader.GetMetaDa
+00002af0: 7461 4469 6374 696f 6e61 7279 4172 7261  taDictionaryArra
+00002b00: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+00002b10: 2020 2020 2020 2020 6966 206c 656e 285f          if len(_
+00002b20: 6d65 7461 2920 3e20 303a 0a20 2020 2020  meta) > 0:.     
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b40: 2020 2023 2054 4f44 4f3a 2075 7369 6e67     # TODO: using
+00002b50: 2074 6865 2066 6972 7374 2073 6c69 6365   the first slice
+00002b60: 2773 206d 6574 612e 2074 6869 7320 636f  's meta. this co
+00002b70: 756c 6420 6265 2069 6d70 726f 7665 6420  uld be improved 
+00002b80: 746f 2066 696c 7465 7220 756e 6e65 6365  to filter unnece
+00002b90: 7373 6172 7920 7461 6773 2e0a 2020 2020  ssary tags..    
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bb0: 2020 2020 5f6f 626a 2e53 6574 4d65 7461      _obj.SetMeta
+00002bc0: 4461 7461 4469 6374 696f 6e61 7279 285f  DataDictionary(_
+00002bd0: 6d65 7461 5b30 5d29 0a20 2020 2020 2020  meta[0]).       
+00002be0: 2020 2020 2020 2020 2069 6d67 5f2e 6170           img_.ap
+00002bf0: 7065 6e64 285f 6f62 6a29 0a20 2020 2020  pend(_obj).     
+00002c00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00002c10: 2020 2020 2020 2020 2020 2020 2069 6d67               img
+00002c20: 5f2e 6170 7065 6e64 2869 746b 2e69 6d72  _.append(itk.imr
+00002c30: 6561 6428 6e61 6d65 2c20 2a2a 6b77 6172  ead(name, **kwar
+00002c40: 6773 5f29 290a 2020 2020 2020 2020 7265  gs_)).        re
+00002c50: 7475 726e 2069 6d67 5f20 6966 206c 656e  turn img_ if len
+00002c60: 2866 696c 656e 616d 6573 2920 3e20 3120  (filenames) > 1 
+00002c70: 656c 7365 2069 6d67 5f5b 305d 0a0a 2020  else img_[0]..  
+00002c80: 2020 6465 6620 6765 745f 6461 7461 2873    def get_data(s
+00002c90: 656c 662c 2069 6d67 2920 2d3e 2074 7570  elf, img) -> tup
+00002ca0: 6c65 5b6e 702e 6e64 6172 7261 792c 2064  le[np.ndarray, d
+00002cb0: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
+00002cc0: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
+00002cd0: 7420 6461 7461 2061 7272 6179 2061 6e64  t data array and
+00002ce0: 206d 6574 6164 6174 6120 6672 6f6d 206c   metadata from l
+00002cf0: 6f61 6465 6420 696d 6167 6520 616e 6420  oaded image and 
+00002d00: 7265 7475 726e 2074 6865 6d2e 0a20 2020  return them..   
+00002d10: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+00002d20: 6f6e 2072 6574 7572 6e73 2074 776f 206f  on returns two o
+00002d30: 626a 6563 7473 2c20 6669 7273 7420 6973  bjects, first is
+00002d40: 206e 756d 7079 2061 7272 6179 206f 6620   numpy array of 
+00002d50: 696d 6167 6520 6461 7461 2c20 7365 636f  image data, seco
+00002d60: 6e64 2069 7320 6469 6374 206f 6620 6d65  nd is dict of me
+00002d70: 7461 6461 7461 2e0a 2020 2020 2020 2020  tadata..        
+00002d80: 4974 2063 6f6e 7374 7275 6374 7320 6061  It constructs `a
+00002d90: 6666 696e 6560 2c20 606f 7269 6769 6e61  ffine`, `origina
+00002da0: 6c5f 6166 6669 6e65 602c 2061 6e64 2060  l_affine`, and `
+00002db0: 7370 6174 6961 6c5f 7368 6170 6560 2061  spatial_shape` a
+00002dc0: 6e64 2073 746f 7265 7320 7468 656d 2069  nd stores them i
+00002dd0: 6e20 6d65 7461 2064 6963 742e 0a20 2020  n meta dict..   
+00002de0: 2020 2020 2057 6865 6e20 6c6f 6164 696e       When loadin
+00002df0: 6720 6120 6c69 7374 206f 6620 6669 6c65  g a list of file
+00002e00: 732c 2074 6865 7920 6172 6520 7374 6163  s, they are stac
+00002e10: 6b65 6420 746f 6765 7468 6572 2061 7420  ked together at 
+00002e20: 6120 6e65 7720 6469 6d65 6e73 696f 6e20  a new dimension 
+00002e30: 6173 2074 6865 2066 6972 7374 2064 696d  as the first dim
+00002e40: 656e 7369 6f6e 2c0a 2020 2020 2020 2020  ension,.        
+00002e50: 616e 6420 7468 6520 6d65 7461 6461 7461  and the metadata
+00002e60: 206f 6620 7468 6520 6669 7273 7420 696d   of the first im
+00002e70: 6167 6520 6973 2075 7365 6420 746f 2072  age is used to r
+00002e80: 6570 7265 7365 6e74 2074 6865 206f 7574  epresent the out
+00002e90: 7075 7420 6d65 7461 6461 7461 2e0a 0a20  put metadata... 
+00002ea0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00002eb0: 2020 2020 2020 2020 2069 6d67 3a20 616e           img: an
+00002ec0: 2049 544b 2069 6d61 6765 206f 626a 6563   ITK image objec
+00002ed0: 7420 6c6f 6164 6564 2066 726f 6d20 616e  t loaded from an
+00002ee0: 2069 6d61 6765 2066 696c 6520 6f72 2061   image file or a
+00002ef0: 206c 6973 7420 6f66 2049 544b 2069 6d61   list of ITK ima
+00002f00: 6765 206f 626a 6563 7473 2e0a 0a20 2020  ge objects...   
+00002f10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00002f20: 2069 6d67 5f61 7272 6179 3a20 6c69 7374   img_array: list
+00002f30: 5b6e 702e 6e64 6172 7261 795d 203d 205b  [np.ndarray] = [
+00002f40: 5d0a 2020 2020 2020 2020 636f 6d70 6174  ].        compat
+00002f50: 6962 6c65 5f6d 6574 613a 2064 6963 7420  ible_meta: dict 
+00002f60: 3d20 7b7d 0a0a 2020 2020 2020 2020 666f  = {}..        fo
+00002f70: 7220 6920 696e 2065 6e73 7572 655f 7475  r i in ensure_tu
+00002f80: 706c 6528 696d 6729 3a0a 2020 2020 2020  ple(img):.      
+00002f90: 2020 2020 2020 6461 7461 203d 2073 656c        data = sel
+00002fa0: 662e 5f67 6574 5f61 7272 6179 5f64 6174  f._get_array_dat
+00002fb0: 6128 6929 0a20 2020 2020 2020 2020 2020  a(i).           
+00002fc0: 2069 6d67 5f61 7272 6179 2e61 7070 656e   img_array.appen
+00002fd0: 6428 6461 7461 290a 2020 2020 2020 2020  d(data).        
+00002fe0: 2020 2020 6865 6164 6572 203d 2073 656c      header = sel
+00002ff0: 662e 5f67 6574 5f6d 6574 615f 6469 6374  f._get_meta_dict
+00003000: 2869 290a 2020 2020 2020 2020 2020 2020  (i).            
+00003010: 6865 6164 6572 5b4d 6574 614b 6579 732e  header[MetaKeys.
+00003020: 4f52 4947 494e 414c 5f41 4646 494e 455d  ORIGINAL_AFFINE]
+00003030: 203d 2073 656c 662e 5f67 6574 5f61 6666   = self._get_aff
+00003040: 696e 6528 692c 2073 656c 662e 6166 6669  ine(i, self.affi
+00003050: 6e65 5f6c 7073 5f74 6f5f 7261 7329 0a20  ne_lps_to_ras). 
+00003060: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+00003070: 725b 4d65 7461 4b65 7973 2e53 5041 4345  r[MetaKeys.SPACE
+00003080: 5d20 3d20 5370 6163 654b 6579 732e 5241  ] = SpaceKeys.RA
+00003090: 5320 6966 2073 656c 662e 6166 6669 6e65  S if self.affine
+000030a0: 5f6c 7073 5f74 6f5f 7261 7320 656c 7365  _lps_to_ras else
+000030b0: 2053 7061 6365 4b65 7973 2e4c 5053 0a20   SpaceKeys.LPS. 
+000030c0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+000030d0: 725b 4d65 7461 4b65 7973 2e41 4646 494e  r[MetaKeys.AFFIN
+000030e0: 455d 203d 2068 6561 6465 725b 4d65 7461  E] = header[Meta
+000030f0: 4b65 7973 2e4f 5249 4749 4e41 4c5f 4146  Keys.ORIGINAL_AF
+00003100: 4649 4e45 5d2e 636f 7079 2829 0a20 2020  FINE].copy().   
+00003110: 2020 2020 2020 2020 2068 6561 6465 725b           header[
+00003120: 4d65 7461 4b65 7973 2e53 5041 5449 414c  MetaKeys.SPATIAL
+00003130: 5f53 4841 5045 5d20 3d20 7365 6c66 2e5f  _SHAPE] = self._
+00003140: 6765 745f 7370 6174 6961 6c5f 7368 6170  get_spatial_shap
+00003150: 6528 6929 0a20 2020 2020 2020 2020 2020  e(i).           
+00003160: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+00003170: 5f64 696d 2069 7320 4e6f 6e65 3a20 2023  _dim is None:  #
+00003180: 2064 6566 6175 6c74 2074 6f20 226e 6f5f   default to "no_
+00003190: 6368 616e 6e65 6c22 206f 7220 2d31 0a20  channel" or -1. 
+000031a0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+000031b0: 6561 6465 725b 4d65 7461 4b65 7973 2e4f  eader[MetaKeys.O
+000031c0: 5249 4749 4e41 4c5f 4348 414e 4e45 4c5f  RIGINAL_CHANNEL_
+000031d0: 4449 4d5d 203d 2028 0a20 2020 2020 2020  DIM] = (.       
+000031e0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+000031f0: 6174 2822 6e61 6e22 2920 6966 206c 656e  at("nan") if len
+00003200: 2864 6174 612e 7368 6170 6529 203d 3d20  (data.shape) == 
+00003210: 6c65 6e28 6865 6164 6572 5b4d 6574 614b  len(header[MetaK
+00003220: 6579 732e 5350 4154 4941 4c5f 5348 4150  eys.SPATIAL_SHAP
+00003230: 455d 2920 656c 7365 202d 310a 2020 2020  E]) else -1.    
+00003240: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00003250: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003270: 6865 6164 6572 5b4d 6574 614b 6579 732e  header[MetaKeys.
+00003280: 4f52 4947 494e 414c 5f43 4841 4e4e 454c  ORIGINAL_CHANNEL
+00003290: 5f44 494d 5d20 3d20 7365 6c66 2e63 6861  _DIM] = self.cha
+000032a0: 6e6e 656c 5f64 696d 0a20 2020 2020 2020  nnel_dim.       
+000032b0: 2020 2020 205f 636f 7079 5f63 6f6d 7061       _copy_compa
+000032c0: 7469 626c 655f 6469 6374 2868 6561 6465  tible_dict(heade
+000032d0: 722c 2063 6f6d 7061 7469 626c 655f 6d65  r, compatible_me
+000032e0: 7461 290a 0a20 2020 2020 2020 2072 6574  ta)..        ret
+000032f0: 7572 6e20 5f73 7461 636b 5f69 6d61 6765  urn _stack_image
+00003300: 7328 696d 675f 6172 7261 792c 2063 6f6d  s(img_array, com
+00003310: 7061 7469 626c 655f 6d65 7461 292c 2063  patible_meta), c
+00003320: 6f6d 7061 7469 626c 655f 6d65 7461 0a0a  ompatible_meta..
+00003330: 2020 2020 6465 6620 5f67 6574 5f6d 6574      def _get_met
+00003340: 615f 6469 6374 2873 656c 662c 2069 6d67  a_dict(self, img
+00003350: 2920 2d3e 2064 6963 743a 0a20 2020 2020  ) -> dict:.     
+00003360: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00003370: 6574 2061 6c6c 2074 6865 206d 6574 6164  et all the metad
+00003380: 6174 6120 6f66 2074 6865 2069 6d61 6765  ata of the image
+00003390: 2061 6e64 2063 6f6e 7665 7274 2074 6f20   and convert to 
+000033a0: 6469 6374 2074 7970 652e 0a0a 2020 2020  dict type...    
+000033b0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000033c0: 2020 2020 2020 696d 673a 2061 6e20 4954        img: an IT
+000033d0: 4b20 696d 6167 6520 6f62 6a65 6374 206c  K image object l
+000033e0: 6f61 6465 6420 6672 6f6d 2061 6e20 696d  oaded from an im
+000033f0: 6167 6520 6669 6c65 2e0a 0a20 2020 2020  age file...     
+00003400: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00003410: 6d67 5f6d 6574 615f 6469 6374 203d 2069  mg_meta_dict = i
+00003420: 6d67 2e47 6574 4d65 7461 4461 7461 4469  mg.GetMetaDataDi
+00003430: 6374 696f 6e61 7279 2829 0a20 2020 2020  ctionary().     
+00003440: 2020 206d 6574 615f 6469 6374 203d 207b     meta_dict = {
+00003450: 7d0a 2020 2020 2020 2020 666f 7220 6b65  }.        for ke
+00003460: 7920 696e 2069 6d67 5f6d 6574 615f 6469  y in img_meta_di
+00003470: 6374 2e47 6574 4b65 7973 2829 3a0a 2020  ct.GetKeys():.  
+00003480: 2020 2020 2020 2020 2020 6966 206b 6579            if key
+00003490: 2e73 7461 7274 7377 6974 6828 2249 544b  .startswith("ITK
+000034a0: 5f22 293a 0a20 2020 2020 2020 2020 2020  _"):.           
+000034b0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+000034c0: 2020 2020 2020 2020 2020 7661 6c20 3d20            val = 
+000034d0: 696d 675f 6d65 7461 5f64 6963 745b 6b65  img_meta_dict[ke
+000034e0: 795d 0a20 2020 2020 2020 2020 2020 206d  y].            m
+000034f0: 6574 615f 6469 6374 5b6b 6579 5d20 3d20  eta_dict[key] = 
+00003500: 6e70 2e61 7361 7272 6179 2876 616c 2920  np.asarray(val) 
+00003510: 6966 2074 7970 6528 7661 6c29 2e5f 5f6e  if type(val).__n
+00003520: 616d 655f 5f2e 7374 6172 7473 7769 7468  ame__.startswith
+00003530: 2822 6974 6b22 2920 656c 7365 2076 616c  ("itk") else val
+00003540: 0a0a 2020 2020 2020 2020 6d65 7461 5f64  ..        meta_d
+00003550: 6963 745b 2273 7061 6369 6e67 225d 203d  ict["spacing"] =
+00003560: 206e 702e 6173 6172 7261 7928 696d 672e   np.asarray(img.
+00003570: 4765 7453 7061 6369 6e67 2829 290a 2020  GetSpacing()).  
+00003580: 2020 2020 2020 7265 7475 726e 206d 6574        return met
+00003590: 615f 6469 6374 0a0a 2020 2020 6465 6620  a_dict..    def 
+000035a0: 5f67 6574 5f61 6666 696e 6528 7365 6c66  _get_affine(self
+000035b0: 2c20 696d 672c 206c 7073 5f74 6f5f 7261  , img, lps_to_ra
+000035c0: 733a 2062 6f6f 6c20 3d20 5472 7565 293a  s: bool = True):
+000035d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000035e0: 2020 2020 2047 6574 206f 7220 636f 6e73       Get or cons
+000035f0: 7472 7563 7420 7468 6520 6166 6669 6e65  truct the affine
+00003600: 206d 6174 7269 7820 6f66 2074 6865 2069   matrix of the i
+00003610: 6d61 6765 2c20 6974 2063 616e 2062 6520  mage, it can be 
+00003620: 7573 6564 2074 6f20 636f 7272 6563 740a  used to correct.
+00003630: 2020 2020 2020 2020 7370 6163 696e 672c          spacing,
+00003640: 206f 7269 656e 7461 7469 6f6e 206f 7220   orientation or 
+00003650: 6578 6563 7574 6520 7370 6174 6961 6c20  execute spatial 
+00003660: 7472 616e 7366 6f72 6d73 2e0a 0a20 2020  transforms...   
+00003670: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00003680: 2020 2020 2020 2069 6d67 3a20 616e 2049         img: an I
+00003690: 544b 2069 6d61 6765 206f 626a 6563 7420  TK image object 
+000036a0: 6c6f 6164 6564 2066 726f 6d20 616e 2069  loaded from an i
+000036b0: 6d61 6765 2066 696c 652e 0a20 2020 2020  mage file..     
+000036c0: 2020 2020 2020 206c 7073 5f74 6f5f 7261         lps_to_ra
+000036d0: 733a 2077 6865 7468 6572 2074 6f20 636f  s: whether to co
+000036e0: 6e76 6572 7420 7468 6520 6166 6669 6e65  nvert the affine
+000036f0: 206d 6174 7269 7820 6672 6f6d 2022 4c50   matrix from "LP
+00003700: 5322 2074 6f20 2252 4153 222e 2044 6566  S" to "RAS". Def
+00003710: 6175 6c74 7320 746f 2054 7275 652e 0a0a  aults to True...
+00003720: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003730: 2020 2020 6469 7265 6374 696f 6e20 3d20      direction = 
+00003740: 6974 6b2e 6172 7261 795f 6672 6f6d 5f6d  itk.array_from_m
+00003750: 6174 7269 7828 696d 672e 4765 7444 6972  atrix(img.GetDir
+00003760: 6563 7469 6f6e 2829 290a 2020 2020 2020  ection()).      
+00003770: 2020 7370 6163 696e 6720 3d20 6e70 2e61    spacing = np.a
+00003780: 7361 7272 6179 2869 6d67 2e47 6574 5370  sarray(img.GetSp
+00003790: 6163 696e 6728 2929 0a20 2020 2020 2020  acing()).       
+000037a0: 206f 7269 6769 6e20 3d20 6e70 2e61 7361   origin = np.asa
+000037b0: 7272 6179 2869 6d67 2e47 6574 4f72 6967  rray(img.GetOrig
+000037c0: 696e 2829 290a 0a20 2020 2020 2020 2064  in())..        d
+000037d0: 6972 6563 7469 6f6e 203d 206e 702e 6173  irection = np.as
+000037e0: 6172 7261 7928 6469 7265 6374 696f 6e29  array(direction)
+000037f0: 0a20 2020 2020 2020 2073 7220 3d20 6d69  .        sr = mi
+00003800: 6e28 6d61 7828 6469 7265 6374 696f 6e2e  n(max(direction.
+00003810: 7368 6170 655b 305d 2c20 3129 2c20 3329  shape[0], 1), 3)
+00003820: 0a20 2020 2020 2020 2061 6666 696e 653a  .        affine:
+00003830: 206e 702e 6e64 6172 7261 7920 3d20 6e70   np.ndarray = np
+00003840: 2e65 7965 2873 7220 2b20 3129 0a20 2020  .eye(sr + 1).   
+00003850: 2020 2020 2061 6666 696e 655b 3a73 722c       affine[:sr,
+00003860: 203a 7372 5d20 3d20 6469 7265 6374 696f   :sr] = directio
+00003870: 6e5b 3a73 722c 203a 7372 5d20 4020 6e70  n[:sr, :sr] @ np
+00003880: 2e64 6961 6728 7370 6163 696e 675b 3a73  .diag(spacing[:s
+00003890: 725d 290a 2020 2020 2020 2020 6166 6669  r]).        affi
+000038a0: 6e65 5b3a 7372 2c20 2d31 5d20 3d20 6f72  ne[:sr, -1] = or
+000038b0: 6967 696e 5b3a 7372 5d0a 2020 2020 2020  igin[:sr].      
+000038c0: 2020 6966 206c 7073 5f74 6f5f 7261 733a    if lps_to_ras:
+000038d0: 0a20 2020 2020 2020 2020 2020 2061 6666  .            aff
+000038e0: 696e 6520 3d20 6f72 6965 6e74 6174 696f  ine = orientatio
+000038f0: 6e5f 7261 735f 6c70 7328 6166 6669 6e65  n_ras_lps(affine
+00003900: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00003910: 2061 6666 696e 650a 0a20 2020 2064 6566   affine..    def
+00003920: 205f 6765 745f 7370 6174 6961 6c5f 7368   _get_spatial_sh
+00003930: 6170 6528 7365 6c66 2c20 696d 6729 3a0a  ape(self, img):.
+00003940: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00003950: 2020 2020 4765 7420 7468 6520 7370 6174      Get the spat
+00003960: 6961 6c20 7368 6170 6520 6f66 2060 696d  ial shape of `im
+00003970: 6760 2e0a 0a20 2020 2020 2020 2041 7267  g`...        Arg
+00003980: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00003990: 6d67 3a20 616e 2049 544b 2069 6d61 6765  mg: an ITK image
+000039a0: 206f 626a 6563 7420 6c6f 6164 6564 2066   object loaded f
+000039b0: 726f 6d20 616e 2069 6d61 6765 2066 696c  rom an image fil
+000039c0: 652e 0a0a 2020 2020 2020 2020 2222 220a  e...        """.
+000039d0: 2020 2020 2020 2020 7372 203d 2069 746b          sr = itk
+000039e0: 2e61 7272 6179 5f66 726f 6d5f 6d61 7472  .array_from_matr
+000039f0: 6978 2869 6d67 2e47 6574 4469 7265 6374  ix(img.GetDirect
+00003a00: 696f 6e28 2929 2e73 6861 7065 5b30 5d0a  ion()).shape[0].
+00003a10: 2020 2020 2020 2020 7372 203d 206d 6178          sr = max
+00003a20: 286d 696e 2873 722c 2033 292c 2031 290a  (min(sr, 3), 1).
+00003a30: 2020 2020 2020 2020 5f73 697a 6520 3d20          _size = 
+00003a40: 6c69 7374 2869 746b 2e73 697a 6528 696d  list(itk.size(im
+00003a50: 6729 290a 2020 2020 2020 2020 6966 2069  g)).        if i
+00003a60: 7369 6e73 7461 6e63 6528 7365 6c66 2e63  sinstance(self.c
+00003a70: 6861 6e6e 656c 5f64 696d 2c20 696e 7429  hannel_dim, int)
+00003a80: 3a0a 2020 2020 2020 2020 2020 2020 5f73  :.            _s
+00003a90: 697a 652e 706f 7028 7365 6c66 2e63 6861  ize.pop(self.cha
+00003aa0: 6e6e 656c 5f64 696d 290a 2020 2020 2020  nnel_dim).      
+00003ab0: 2020 7265 7475 726e 206e 702e 6173 6172    return np.asar
+00003ac0: 7261 7928 5f73 697a 655b 3a73 725d 290a  ray(_size[:sr]).
+00003ad0: 0a20 2020 2064 6566 205f 6765 745f 6172  .    def _get_ar
+00003ae0: 7261 795f 6461 7461 2873 656c 662c 2069  ray_data(self, i
+00003af0: 6d67 293a 0a20 2020 2020 2020 2022 2222  mg):.        """
+00003b00: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
+00003b10: 2072 6177 2061 7272 6179 2064 6174 6120   raw array data 
+00003b20: 6f66 2074 6865 2069 6d61 6765 2c20 636f  of the image, co
+00003b30: 6e76 6572 7465 6420 746f 204e 756d 7079  nverted to Numpy
+00003b40: 2061 7272 6179 2e0a 0a20 2020 2020 2020   array...       
+00003b50: 2046 6f6c 6c6f 7769 6e67 2050 7954 6f72   Following PyTor
+00003b60: 6368 2063 6f6e 7665 6e74 696f 6e73 2c20  ch conventions, 
+00003b70: 7468 6520 7265 7475 726e 6564 2061 7272  the returned arr
+00003b80: 6179 2064 6174 6120 6861 7320 636f 6e74  ay data has cont
+00003b90: 6967 756f 7573 2063 6861 6e6e 656c 732c  iguous channels,
+00003ba0: 0a20 2020 2020 2020 2065 2e67 2e20 666f  .        e.g. fo
+00003bb0: 7220 616e 2052 4742 2069 6d61 6765 2c20  r an RGB image, 
+00003bc0: 616c 6c20 7265 6420 6368 616e 6e65 6c20  all red channel 
+00003bd0: 696d 6167 6520 7069 7865 6c73 2061 7265  image pixels are
+00003be0: 2063 6f6e 7469 6775 6f75 7320 696e 206d   contiguous in m
+00003bf0: 656d 6f72 792e 0a20 2020 2020 2020 2054  emory..        T
+00003c00: 6865 206c 6173 7420 6178 6973 206f 6620  he last axis of 
+00003c10: 7468 6520 7265 7475 726e 6564 2061 7272  the returned arr
+00003c20: 6179 2069 7320 7468 6520 6368 616e 6e65  ay is the channe
+00003c30: 6c20 6178 6973 2e0a 0a20 2020 2020 2020  l axis...       
+00003c40: 2053 6565 2061 6c73 6f3a 0a0a 2020 2020   See also:..    
+00003c50: 2020 2020 2020 2020 2d20 6874 7470 733a          - https:
+00003c60: 2f2f 6769 7468 7562 2e63 6f6d 2f49 6e73  //github.com/Ins
+00003c70: 6967 6874 536f 6674 7761 7265 436f 6e73  ightSoftwareCons
+00003c80: 6f72 7469 756d 2f49 544b 2f62 6c6f 622f  ortium/ITK/blob/
+00003c90: 7635 2e32 2e31 2f4d 6f64 756c 6573 2f42  v5.2.1/Modules/B
+00003ca0: 7269 6467 652f 4e75 6d50 792f 7772 6170  ridge/NumPy/wrap
+00003cb0: 7069 6e67 2f50 7942 7566 6665 722e 692e  ping/PyBuffer.i.
+00003cc0: 696e 0a0a 2020 2020 2020 2020 4172 6773  in..        Args
+00003cd0: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
+00003ce0: 673a 2061 6e20 4954 4b20 696d 6167 6520  g: an ITK image 
+00003cf0: 6f62 6a65 6374 206c 6f61 6465 6420 6672  object loaded fr
+00003d00: 6f6d 2061 6e20 696d 6167 6520 6669 6c65  om an image file
+00003d10: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
+00003d20: 2020 2020 2020 206e 705f 696d 6720 3d20         np_img = 
+00003d30: 6974 6b2e 6172 7261 795f 7669 6577 5f66  itk.array_view_f
+00003d40: 726f 6d5f 696d 6167 6528 696d 672c 206b  rom_image(img, k
+00003d50: 6565 705f 6178 6573 3d46 616c 7365 290a  eep_axes=False).
+00003d60: 2020 2020 2020 2020 6966 2069 6d67 2e47          if img.G
+00003d70: 6574 4e75 6d62 6572 4f66 436f 6d70 6f6e  etNumberOfCompon
+00003d80: 656e 7473 5065 7250 6978 656c 2829 203d  entsPerPixel() =
+00003d90: 3d20 313a 2020 2320 6861 6e64 6c69 6e67  = 1:  # handling
+00003da0: 2073 7061 7469 616c 2069 6d61 6765 730a   spatial images.
+00003db0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003dc0: 726e 206e 705f 696d 6720 6966 2073 656c  rn np_img if sel
+00003dd0: 662e 7265 7665 7273 655f 696e 6465 7869  f.reverse_indexi
+00003de0: 6e67 2065 6c73 6520 6e70 5f69 6d67 2e54  ng else np_img.T
+00003df0: 0a20 2020 2020 2020 2023 2068 616e 646c  .        # handl
+00003e00: 696e 6720 6d75 6c74 692d 6368 616e 6e65  ing multi-channe
+00003e10: 6c20 696d 6167 6573 0a20 2020 2020 2020  l images.       
+00003e20: 2072 6574 7572 6e20 6e70 5f69 6d67 2069   return np_img i
+00003e30: 6620 7365 6c66 2e72 6576 6572 7365 5f69  f self.reverse_i
+00003e40: 6e64 6578 696e 6720 656c 7365 206e 702e  ndexing else np.
+00003e50: 6d6f 7665 6178 6973 286e 705f 696d 672e  moveaxis(np_img.
+00003e60: 542c 2030 2c20 2d31 290a 0a0a 4072 6571  T, 0, -1)...@req
+00003e70: 7569 7265 5f70 6b67 2870 6b67 5f6e 616d  uire_pkg(pkg_nam
+00003e80: 653d 2270 7964 6963 6f6d 2229 0a63 6c61  e="pydicom").cla
+00003e90: 7373 2050 7964 6963 6f6d 5265 6164 6572  ss PydicomReader
+00003ea0: 2849 6d61 6765 5265 6164 6572 293a 0a20  (ImageReader):. 
+00003eb0: 2020 2022 2222 0a20 2020 204c 6f61 6420     """.    Load 
+00003ec0: 6d65 6469 6361 6c20 696d 6167 6573 2062  medical images b
+00003ed0: 6173 6564 206f 6e20 5079 6469 636f 6d20  ased on Pydicom 
+00003ee0: 6c69 6272 6172 792e 0a20 2020 2041 6c6c  library..    All
+00003ef0: 2074 6865 2073 7570 706f 7274 6564 2069   the supported i
+00003f00: 6d61 6765 2066 6f72 6d61 7473 2063 616e  mage formats can
+00003f10: 2062 6520 666f 756e 6420 6174 3a0a 2020   be found at:.  
+00003f20: 2020 6874 7470 733a 2f2f 6469 636f 6d2e    https://dicom.
+00003f30: 6e65 6d61 2e6f 7267 2f6d 6564 6963 616c  nema.org/medical
+00003f40: 2f64 6963 6f6d 2f63 7572 7265 6e74 2f6f  /dicom/current/o
+00003f50: 7574 7075 742f 6368 746d 6c2f 7061 7274  utput/chtml/part
+00003f60: 3130 2f63 6861 7074 6572 5f37 2e68 746d  10/chapter_7.htm
+00003f70: 6c0a 0a20 2020 2050 7964 6963 6f6d 5265  l..    PydicomRe
+00003f80: 6164 6572 2069 7320 616c 736f 2061 626c  ader is also abl
+00003f90: 6520 746f 206c 6f61 6420 7365 676d 656e  e to load segmen
+00003fa0: 7461 7469 6f6e 732c 2069 6620 6120 6469  tations, if a di
+00003fb0: 636f 6d20 6669 6c65 2063 6f6e 7461 696e  com file contain
+00003fc0: 7320 7461 673a 2060 5365 676d 656e 7453  s tag: `SegmentS
+00003fd0: 6571 7565 6e63 6560 2c20 7468 6520 7265  equence`, the re
+00003fe0: 6164 6572 0a20 2020 2077 696c 6c20 636f  ader.    will co
+00003ff0: 6e73 6964 6572 2069 7420 6173 2073 6567  nsider it as seg
+00004000: 6d65 6e74 6174 696f 6e20 6461 7461 2c20  mentation data, 
+00004010: 616e 6420 746f 206c 6f61 6420 6974 2073  and to load it s
+00004020: 7563 6365 7373 6675 6c6c 792c 2060 5065  uccessfully, `Pe
+00004030: 7246 7261 6d65 4675 6e63 7469 6f6e 616c  rFrameFunctional
+00004040: 4772 6f75 7073 5365 7175 656e 6365 6020  GroupsSequence` 
+00004050: 6973 2072 6571 7569 7265 640a 2020 2020  is required.    
+00004060: 666f 7220 6469 636f 6d20 6669 6c65 2c20  for dicom file, 
+00004070: 616e 6420 666f 7220 6561 6368 2066 7261  and for each fra
+00004080: 6d65 206f 6620 6469 636f 6d20 6669 6c65  me of dicom file
+00004090: 2c20 6053 6567 6d65 6e74 4964 656e 7469  , `SegmentIdenti
+000040a0: 6669 6361 7469 6f6e 5365 7175 656e 6365  ficationSequence
+000040b0: 6020 6973 2072 6571 7569 7265 642e 0a20  ` is required.. 
+000040c0: 2020 2054 6869 7320 6d65 7468 6f64 2072     This method r
+000040d0: 6566 6572 7320 746f 2074 6865 2048 6967  efers to the Hig
+000040e0: 6864 6963 6f6d 206c 6962 7261 7279 2e0a  hdicom library..
+000040f0: 0a20 2020 2054 6869 7320 636c 6173 7320  .    This class 
+00004100: 7265 6665 7273 2074 6f3a 0a20 2020 2068  refers to:.    h
+00004110: 7474 7073 3a2f 2f6e 6970 792e 6f72 672f  ttps://nipy.org/
+00004120: 6e69 6261 6265 6c2f 6469 636f 6d2f 6469  nibabel/dicom/di
+00004130: 636f 6d5f 6f72 6965 6e74 6174 696f 6e2e  com_orientation.
+00004140: 6874 6d6c 2364 6963 6f6d 2d61 6666 696e  html#dicom-affin
+00004150: 652d 666f 726d 756c 610a 2020 2020 6874  e-formula.    ht
+00004160: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00004170: 2f70 7964 6963 6f6d 2f63 6f6e 7472 6962  /pydicom/contrib
+00004180: 2d70 7964 6963 6f6d 2f62 6c6f 622f 6d61  -pydicom/blob/ma
+00004190: 7374 6572 2f69 6e70 7574 2d6f 7574 7075  ster/input-outpu
+000041a0: 742f 7079 6469 636f 6d5f 7365 7269 6573  t/pydicom_series
+000041b0: 2e70 790a 2020 2020 6874 7470 733a 2f2f  .py.    https://
+000041c0: 6869 6768 6469 636f 6d2e 7265 6164 7468  highdicom.readth
+000041d0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000041e0: 7374 2f75 7361 6765 2e68 746d 6c23 7061  st/usage.html#pa
+000041f0: 7273 696e 672d 7365 676d 656e 7461 7469  rsing-segmentati
+00004200: 6f6e 2d73 6567 2d69 6d61 6765 730a 0a20  on-seg-images.. 
+00004210: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00004220: 2063 6861 6e6e 656c 5f64 696d 3a20 7468   channel_dim: th
+00004230: 6520 6368 616e 6e65 6c20 6469 6d65 6e73  e channel dimens
+00004240: 696f 6e20 6f66 2074 6865 2069 6e70 7574  ion of the input
+00004250: 2069 6d61 6765 2c20 6465 6661 756c 7420   image, default 
+00004260: 6973 204e 6f6e 652e 0a20 2020 2020 2020  is None..       
+00004270: 2020 2020 2054 6869 7320 6973 2075 7365       This is use
+00004280: 6420 746f 2073 6574 206f 7269 6769 6e61  d to set origina
+00004290: 6c5f 6368 616e 6e65 6c5f 6469 6d20 696e  l_channel_dim in
+000042a0: 2074 6865 206d 6574 6164 6174 612c 2045   the metadata, E
+000042b0: 6e73 7572 6543 6861 6e6e 656c 4669 7273  nsureChannelFirs
+000042c0: 7444 2072 6561 6473 2074 6869 7320 6669  tD reads this fi
+000042d0: 656c 642e 0a20 2020 2020 2020 2020 2020  eld..           
+000042e0: 2049 6620 4e6f 6e65 2c20 606f 7269 6769   If None, `origi
+000042f0: 6e61 6c5f 6368 616e 6e65 6c5f 6469 6d60  nal_channel_dim`
+00004300: 2077 696c 6c20 6265 2065 6974 6865 7220   will be either 
+00004310: 606e 6f5f 6368 616e 6e65 6c60 206f 7220  `no_channel` or 
+00004320: 602d 3160 2e0a 2020 2020 2020 2020 6166  `-1`..        af
+00004330: 6669 6e65 5f6c 7073 5f74 6f5f 7261 733a  fine_lps_to_ras:
+00004340: 2077 6865 7468 6572 2074 6f20 636f 6e76   whether to conv
+00004350: 6572 7420 7468 6520 6166 6669 6e65 206d  ert the affine m
+00004360: 6174 7269 7820 6672 6f6d 2022 4c50 5322  atrix from "LPS"
+00004370: 2074 6f20 2252 4153 222e 2044 6566 6175   to "RAS". Defau
+00004380: 6c74 7320 746f 2060 6054 7275 6560 602e  lts to ``True``.
+00004390: 0a20 2020 2020 2020 2020 2020 2053 6574  .            Set
+000043a0: 2074 6f20 6060 5472 7565 6060 2074 6f20   to ``True`` to 
+000043b0: 6265 2063 6f6e 7369 7374 656e 7420 7769  be consistent wi
+000043c0: 7468 2060 604e 6962 6162 656c 5265 6164  th ``NibabelRead
+000043d0: 6572 6060 2c0a 2020 2020 2020 2020 2020  er``,.          
+000043e0: 2020 6f74 6865 7277 6973 6520 7468 6520    otherwise the 
+000043f0: 6166 6669 6e65 206d 6174 7269 7820 7265  affine matrix re
+00004400: 6d61 696e 7320 696e 2074 6865 2044 6963  mains in the Dic
+00004410: 6f6d 2063 6f6e 7665 6e74 696f 6e2e 0a20  om convention.. 
+00004420: 2020 2020 2020 2073 7761 705f 696a 3a20         swap_ij: 
+00004430: 7768 6574 6865 7220 746f 2073 7761 7020  whether to swap 
+00004440: 7468 6520 6669 7273 7420 7477 6f20 7370  the first two sp
+00004450: 6174 6961 6c20 6178 6573 2e20 4465 6661  atial axes. Defa
+00004460: 756c 7420 746f 2060 6054 7275 6560 602c  ult to ``True``,
+00004470: 2073 6f20 7468 6174 2074 6865 206f 7574   so that the out
+00004480: 7075 7473 0a20 2020 2020 2020 2020 2020  puts.           
+00004490: 2061 7265 2063 6f6e 7369 7374 656e 7420   are consistent 
+000044a0: 7769 7468 2074 6865 206f 7468 6572 2072  with the other r
+000044b0: 6561 6465 7273 2e0a 2020 2020 2020 2020  eaders..        
+000044c0: 7072 756e 655f 6d65 7461 6461 7461 3a20  prune_metadata: 
+000044d0: 7768 6574 6865 7220 746f 2070 7275 6e65  whether to prune
+000044e0: 2074 6865 2073 6176 6564 2069 6e66 6f72   the saved infor
+000044f0: 6d61 7469 6f6e 2069 6e20 6d65 7461 6461  mation in metada
+00004500: 7461 2e20 5468 6973 2061 7267 756d 656e  ta. This argumen
+00004510: 7420 6973 2075 7365 6420 666f 720a 2020  t is used for.  
+00004520: 2020 2020 2020 2020 2020 6067 6574 5f64            `get_d
+00004530: 6174 6160 2066 756e 6374 696f 6e2e 2049  ata` function. I
+00004540: 6620 5472 7565 2c20 6f6e 6c79 2069 7465  f True, only ite
+00004550: 6d73 2074 6861 7420 6172 6520 7265 6c61  ms that are rela
+00004560: 7465 6420 746f 2074 6865 2061 6666 696e  ted to the affin
+00004570: 6520 6d61 7472 6978 2077 696c 6c20 6265  e matrix will be
+00004580: 2073 6176 6564 2e0a 2020 2020 2020 2020   saved..        
+00004590: 2020 2020 4465 6661 756c 7420 746f 2060      Default to `
+000045a0: 6054 7275 6560 602e 0a20 2020 2020 2020  `True``..       
+000045b0: 206c 6162 656c 5f64 6963 743a 206c 6162   label_dict: lab
+000045c0: 656c 206f 6620 7468 6520 6469 636f 6d20  el of the dicom 
+000045d0: 6461 7461 2e20 4966 2070 726f 7669 6465  data. If provide
+000045e0: 642c 2069 7420 7769 6c6c 2062 6520 7573  d, it will be us
+000045f0: 6564 2077 6865 6e20 6c6f 6164 696e 6720  ed when loading 
+00004600: 7365 676d 656e 7461 7469 6f6e 2064 6174  segmentation dat
+00004610: 612e 0a20 2020 2020 2020 2020 2020 204b  a..            K
+00004620: 6579 7320 6f66 2074 6865 2064 6963 7420  eys of the dict 
+00004630: 6172 6520 7468 6520 636c 6173 7365 732c  are the classes,
+00004640: 2061 6e64 2076 616c 7565 7320 6172 6520   and values are 
+00004650: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+00004660: 6720 636c 6173 7320 6e75 6d62 6572 2e20  g class number. 
+00004670: 466f 7220 6578 616d 706c 653a 0a20 2020  For example:.   
+00004680: 2020 2020 2020 2020 2066 6f72 2054 4349           for TCI
+00004690: 4120 636f 6c6c 6563 7469 6f6e 2022 4334  A collection "C4
+000046a0: 4b43 2d4b 6954 5322 2c20 6974 2063 616e  KC-KiTS", it can
+000046b0: 2062 653a 207b 224b 6964 6e65 7922 3a20   be: {"Kidney": 
+000046c0: 302c 2022 5265 6e61 6c20 5475 6d6f 7222  0, "Renal Tumor"
+000046d0: 3a20 317d 2e0a 2020 2020 2020 2020 6b77  : 1}..        kw
+000046e0: 6172 6773 3a20 6164 6469 7469 6f6e 616c  args: additional
+000046f0: 2061 7267 7320 666f 7220 6070 7964 6963   args for `pydic
+00004700: 6f6d 2e64 636d 7265 6164 6020 4150 492e  om.dcmread` API.
+00004710: 206d 6f72 6520 6465 7461 696c 7320 6162   more details ab
+00004720: 6f75 7420 6176 6169 6c61 626c 6520 6172  out available ar
+00004730: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00004740: 6874 7470 733a 2f2f 7079 6469 636f 6d2e  https://pydicom.
+00004750: 6769 7468 7562 2e69 6f2f 7079 6469 636f  github.io/pydico
+00004760: 6d2f 7374 6162 6c65 2f72 6566 6572 656e  m/stable/referen
+00004770: 6365 2f67 656e 6572 6174 6564 2f70 7964  ce/generated/pyd
+00004780: 6963 6f6d 2e66 696c 6572 6561 6465 722e  icom.filereader.
+00004790: 6463 6d72 6561 642e 6874 6d6c 2370 7964  dcmread.html#pyd
+000047a0: 6963 6f6d 2e66 696c 6572 6561 6465 722e  icom.filereader.
+000047b0: 6463 6d72 6561 640a 2020 2020 2020 2020  dcmread.        
+000047c0: 2020 2020 4966 2074 6865 2060 6765 745f      If the `get_
+000047d0: 6461 7461 6020 6675 6e63 7469 6f6e 2077  data` function w
+000047e0: 696c 6c20 6265 2063 616c 6c65 640a 2020  ill be called.  
+000047f0: 2020 2020 2020 2020 2020 2866 6f72 2065            (for e
+00004800: 7861 6d70 6c65 2c20 7768 656e 2075 7369  xample, when usi
+00004810: 6e67 2074 6869 7320 7265 6164 6572 2077  ng this reader w
+00004820: 6974 6820 606d 6f6e 6169 2e74 7261 6e73  ith `monai.trans
+00004830: 666f 726d 732e 4c6f 6164 496d 6167 6560  forms.LoadImage`
+00004840: 292c 2070 6c65 6173 6520 656e 7375 7265  ), please ensure
+00004850: 2074 6861 7420 7468 6520 6172 6775 6d65   that the argume
+00004860: 6e74 0a20 2020 2020 2020 2020 2020 2060  nt.            `
+00004870: 7374 6f70 5f62 6566 6f72 655f 7069 7865  stop_before_pixe
+00004880: 6c73 6020 6973 2060 5472 7565 602c 2061  ls` is `True`, a
+00004890: 6e64 2060 7370 6563 6966 6963 5f74 6167  nd `specific_tag
+000048a0: 7360 2063 6f76 6572 7320 616c 6c20 6e65  s` covers all ne
+000048b0: 6365 7373 6172 7920 7461 6773 2c20 7375  cessary tags, su
+000048c0: 6368 2061 7320 6050 6978 656c 5370 6163  ch as `PixelSpac
+000048d0: 696e 6760 2c0a 2020 2020 2020 2020 2020  ing`,.          
+000048e0: 2020 6049 6d61 6765 506f 7369 7469 6f6e    `ImagePosition
+000048f0: 5061 7469 656e 7460 2c20 6049 6d61 6765  Patient`, `Image
+00004900: 4f72 6965 6e74 6174 696f 6e50 6174 6965  OrientationPatie
+00004910: 6e74 6020 616e 6420 616c 6c20 6070 6978  nt` and all `pix
+00004920: 656c 5f61 7272 6179 6020 7265 6c61 7465  el_array` relate
+00004930: 6420 7461 6773 2e0a 2020 2020 2222 220a  d tags..    """.
+00004940: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00004950: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
+00004960: 0a20 2020 2020 2020 2063 6861 6e6e 656c  .        channel
+00004970: 5f64 696d 3a20 7374 7220 7c20 696e 7420  _dim: str | int 
+00004980: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
+00004990: 2020 2020 2020 2061 6666 696e 655f 6c70         affine_lp
+000049a0: 735f 746f 5f72 6173 3a20 626f 6f6c 203d  s_to_ras: bool =
+000049b0: 2054 7275 652c 0a20 2020 2020 2020 2073   True,.        s
+000049c0: 7761 705f 696a 3a20 626f 6f6c 203d 2054  wap_ij: bool = T
+000049d0: 7275 652c 0a20 2020 2020 2020 2070 7275  rue,.        pru
+000049e0: 6e65 5f6d 6574 6164 6174 613a 2062 6f6f  ne_metadata: boo
+000049f0: 6c20 3d20 5472 7565 2c0a 2020 2020 2020  l = True,.      
+00004a00: 2020 6c61 6265 6c5f 6469 6374 3a20 6469    label_dict: di
+00004a10: 6374 207c 204e 6f6e 6520 3d20 4e6f 6e65  ct | None = None
+00004a20: 2c0a 2020 2020 2020 2020 2a2a 6b77 6172  ,.        **kwar
+00004a30: 6773 2c0a 2020 2020 293a 0a20 2020 2020  gs,.    ):.     
+00004a40: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00004a50: 745f 5f28 290a 2020 2020 2020 2020 7365  t__().        se
+00004a60: 6c66 2e6b 7761 7267 7320 3d20 6b77 6172  lf.kwargs = kwar
+00004a70: 6773 0a20 2020 2020 2020 2073 656c 662e  gs.        self.
+00004a80: 6368 616e 6e65 6c5f 6469 6d20 3d20 666c  channel_dim = fl
+00004a90: 6f61 7428 226e 616e 2229 2069 6620 6368  oat("nan") if ch
+00004aa0: 616e 6e65 6c5f 6469 6d20 3d3d 2022 6e6f  annel_dim == "no
+00004ab0: 5f63 6861 6e6e 656c 2220 656c 7365 2063  _channel" else c
+00004ac0: 6861 6e6e 656c 5f64 696d 0a20 2020 2020  hannel_dim.     
+00004ad0: 2020 2073 656c 662e 6166 6669 6e65 5f6c     self.affine_l
+00004ae0: 7073 5f74 6f5f 7261 7320 3d20 6166 6669  ps_to_ras = affi
+00004af0: 6e65 5f6c 7073 5f74 6f5f 7261 730a 2020  ne_lps_to_ras.  
+00004b00: 2020 2020 2020 7365 6c66 2e73 7761 705f        self.swap_
+00004b10: 696a 203d 2073 7761 705f 696a 0a20 2020  ij = swap_ij.   
+00004b20: 2020 2020 2073 656c 662e 7072 756e 655f       self.prune_
+00004b30: 6d65 7461 6461 7461 203d 2070 7275 6e65  metadata = prune
+00004b40: 5f6d 6574 6164 6174 610a 2020 2020 2020  _metadata.      
+00004b50: 2020 7365 6c66 2e6c 6162 656c 5f64 6963    self.label_dic
+00004b60: 7420 3d20 6c61 6265 6c5f 6469 6374 0a0a  t = label_dict..
+00004b70: 2020 2020 6465 6620 7665 7269 6679 5f73      def verify_s
+00004b80: 7566 6669 7828 7365 6c66 2c20 6669 6c65  uffix(self, file
+00004b90: 6e61 6d65 3a20 5365 7175 656e 6365 5b50  name: Sequence[P
+00004ba0: 6174 684c 696b 655d 207c 2050 6174 684c  athLike] | PathL
+00004bb0: 696b 6529 202d 3e20 626f 6f6c 3a0a 2020  ike) -> bool:.  
+00004bc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004bd0: 2020 5665 7269 6679 2077 6865 7468 6572    Verify whether
+00004be0: 2074 6865 2073 7065 6369 6669 6564 2066   the specified f
+00004bf0: 696c 6520 6f72 2066 696c 6573 2066 6f72  ile or files for
+00004c00: 6d61 7420 6973 2073 7570 706f 7274 6564  mat is supported
+00004c10: 2062 7920 5079 6469 636f 6d20 7265 6164   by Pydicom read
+00004c20: 6572 2e0a 0a20 2020 2020 2020 2041 7267  er...        Arg
+00004c30: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
+00004c40: 696c 656e 616d 653a 2066 696c 6520 6e61  ilename: file na
+00004c50: 6d65 206f 7220 6120 6c69 7374 206f 6620  me or a list of 
+00004c60: 6669 6c65 206e 616d 6573 2074 6f20 7265  file names to re
+00004c70: 6164 2e0a 2020 2020 2020 2020 2020 2020  ad..            
+00004c80: 2020 2020 6966 2061 206c 6973 7420 6f66      if a list of
+00004c90: 2066 696c 6573 2c20 7665 7269 6679 2061   files, verify a
+00004ca0: 6c6c 2074 6865 2073 7566 6669 7865 732e  ll the suffixes.
+00004cb0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00004cc0: 2020 2020 2020 7265 7475 726e 2068 6173        return has
+00004cd0: 5f70 7964 6963 6f6d 0a0a 2020 2020 6465  _pydicom..    de
+00004ce0: 6620 7265 6164 2873 656c 662c 2064 6174  f read(self, dat
+00004cf0: 613a 2053 6571 7565 6e63 655b 5061 7468  a: Sequence[Path
+00004d00: 4c69 6b65 5d20 7c20 5061 7468 4c69 6b65  Like] | PathLike
+00004d10: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00004d20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00004d30: 2052 6561 6420 696d 6167 6520 6461 7461   Read image data
+00004d40: 2066 726f 6d20 7370 6563 6966 6965 6420   from specified 
+00004d50: 6669 6c65 206f 7220 6669 6c65 732c 2069  file or files, i
+00004d60: 7420 6361 6e20 7265 6164 2061 206c 6973  t can read a lis
+00004d70: 7420 6f66 2069 6d61 6765 730a 2020 2020  t of images.    
+00004d80: 2020 2020 616e 6420 7374 6163 6b20 7468      and stack th
+00004d90: 656d 2074 6f67 6574 6865 7220 6173 206d  em together as m
+00004da0: 756c 7469 2d63 6861 6e6e 656c 2064 6174  ulti-channel dat
+00004db0: 6120 696e 2060 6765 745f 6461 7461 2829  a in `get_data()
+00004dc0: 602e 0a20 2020 2020 2020 2049 6620 7061  `..        If pa
+00004dd0: 7373 696e 6720 6469 7265 6374 6f72 7920  ssing directory 
+00004de0: 7061 7468 2069 6e73 7465 6164 206f 6620  path instead of 
+00004df0: 6669 6c65 2070 6174 682c 2077 696c 6c20  file path, will 
+00004e00: 7472 6561 7420 6974 2061 7320 4449 434f  treat it as DICO
+00004e10: 4d20 696d 6167 6573 2073 6572 6965 7320  M images series 
+00004e20: 616e 6420 7265 6164 2e0a 0a20 2020 2020  and read...     
+00004e30: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00004e40: 2020 2020 2064 6174 613a 2066 696c 6520       data: file 
+00004e50: 6e61 6d65 206f 7220 6120 6c69 7374 206f  name or a list o
+00004e60: 6620 6669 6c65 206e 616d 6573 2074 6f20  f file names to 
+00004e70: 7265 6164 2c0a 2020 2020 2020 2020 2020  read,.          
+00004e80: 2020 6b77 6172 6773 3a20 6164 6469 7469    kwargs: additi
+00004e90: 6f6e 616c 2061 7267 7320 666f 7220 6070  onal args for `p
+00004ea0: 7964 6963 6f6d 2e64 636d 7265 6164 6020  ydicom.dcmread` 
+00004eb0: 4150 492c 2077 696c 6c20 6f76 6572 7269  API, will overri
+00004ec0: 6465 2060 7365 6c66 2e6b 7761 7267 7360  de `self.kwargs`
+00004ed0: 2066 6f72 2065 7869 7374 696e 6720 6b65   for existing ke
+00004ee0: 7973 2e0a 0a20 2020 2020 2020 2052 6574  ys...        Ret
+00004ef0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00004f00: 2020 4966 2060 6461 7461 6020 7265 7072    If `data` repr
+00004f10: 6573 656e 7473 2061 2066 696c 656e 616d  esents a filenam
+00004f20: 653a 2072 6574 7572 6e20 6120 7079 6469  e: return a pydi
+00004f30: 636f 6d20 6461 7461 7365 7420 6f62 6a65  com dataset obje
+00004f40: 6374 2e0a 2020 2020 2020 2020 2020 2020  ct..            
+00004f50: 4966 2060 6461 7461 6020 7265 7072 6573  If `data` repres
+00004f60: 656e 7473 2061 206c 6973 7420 6f66 2066  ents a list of f
+00004f70: 696c 656e 616d 6573 206f 7220 6120 6469  ilenames or a di
+00004f80: 7265 6374 6f72 793a 2072 6574 7572 6e20  rectory: return 
+00004f90: 6120 6c69 7374 206f 6620 7079 6469 636f  a list of pydico
+00004fa0: 6d20 6461 7461 7365 7420 6f62 6a65 6374  m dataset object
+00004fb0: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00004fc0: 2060 6461 7461 6020 7265 7072 6573 656e   `data` represen
+00004fd0: 7473 2061 206c 6973 7420 6f66 2064 6972  ts a list of dir
+00004fe0: 6563 746f 7269 6573 3a20 7265 7475 726e  ectories: return
+00004ff0: 2061 206c 6973 7420 6f66 206c 6973 7420   a list of list 
+00005000: 6f66 2070 7964 6963 6f6d 2064 6174 6173  of pydicom datas
+00005010: 6574 206f 626a 6563 742e 0a0a 2020 2020  et object...    
+00005020: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00005030: 696d 675f 203d 205b 5d0a 0a20 2020 2020  img_ = []..     
+00005040: 2020 2066 696c 656e 616d 6573 3a20 5365     filenames: Se
+00005050: 7175 656e 6365 5b50 6174 684c 696b 655d  quence[PathLike]
+00005060: 203d 2065 6e73 7572 655f 7475 706c 6528   = ensure_tuple(
+00005070: 6461 7461 290a 2020 2020 2020 2020 6b77  data).        kw
+00005080: 6172 6773 5f20 3d20 7365 6c66 2e6b 7761  args_ = self.kwa
+00005090: 7267 732e 636f 7079 2829 0a20 2020 2020  rgs.copy().     
+000050a0: 2020 206b 7761 7267 735f 2e75 7064 6174     kwargs_.updat
+000050b0: 6528 6b77 6172 6773 290a 0a20 2020 2020  e(kwargs)..     
+000050c0: 2020 2073 656c 662e 6861 735f 7365 7269     self.has_seri
+000050d0: 6573 203d 2046 616c 7365 0a0a 2020 2020  es = False..    
+000050e0: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
+000050f0: 6669 6c65 6e61 6d65 733a 0a20 2020 2020  filenames:.     
+00005100: 2020 2020 2020 206e 616d 6520 3d20 6622         name = f"
+00005110: 7b6e 616d 657d 220a 2020 2020 2020 2020  {name}".        
+00005120: 2020 2020 6966 2050 6174 6828 6e61 6d65      if Path(name
+00005130: 292e 6973 5f64 6972 2829 3a0a 2020 2020  ).is_dir():.    
+00005140: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+00005150: 6164 2044 4943 4f4d 2073 6572 6965 730a  ad DICOM series.
+00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005170: 7365 7269 6573 5f73 6c63 7320 3d20 676c  series_slcs = gl
+00005180: 6f62 2e67 6c6f 6228 6f73 2e70 6174 682e  ob.glob(os.path.
+00005190: 6a6f 696e 286e 616d 652c 2022 2a22 2929  join(name, "*"))
+000051a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000051b0: 2073 6572 6965 735f 736c 6373 203d 205b   series_slcs = [
+000051c0: 736c 6320 666f 7220 736c 6320 696e 2073  slc for slc in s
+000051d0: 6572 6965 735f 736c 6373 2069 6620 224c  eries_slcs if "L
+000051e0: 4943 454e 5345 2220 6e6f 7420 696e 2073  ICENSE" not in s
+000051f0: 6c63 5d0a 2020 2020 2020 2020 2020 2020  lc].            
+00005200: 2020 2020 736c 6963 6573 203d 205b 7079      slices = [py
+00005210: 6469 636f 6d2e 6463 6d72 6561 6428 6670  dicom.dcmread(fp
+00005220: 3d73 6c63 2c20 2a2a 6b77 6172 6773 5f29  =slc, **kwargs_)
+00005230: 2066 6f72 2073 6c63 2069 6e20 7365 7269   for slc in seri
+00005240: 6573 5f73 6c63 735d 0a20 2020 2020 2020  es_slcs].       
+00005250: 2020 2020 2020 2020 2069 6d67 5f2e 6170           img_.ap
+00005260: 7065 6e64 2873 6c69 6365 7320 6966 206c  pend(slices if l
+00005270: 656e 2873 6c69 6365 7329 203e 2031 2065  en(slices) > 1 e
+00005280: 6c73 6520 736c 6963 6573 5b30 5d29 0a20  lse slices[0]). 
+00005290: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000052a0: 6620 6c65 6e28 736c 6963 6573 2920 3e20  f len(slices) > 
+000052b0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+000052c0: 2020 2020 2020 2073 656c 662e 6861 735f         self.has_
+000052d0: 7365 7269 6573 203d 2054 7275 650a 2020  series = True.  
+000052e0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005300: 6473 203d 2070 7964 6963 6f6d 2e64 636d  ds = pydicom.dcm
+00005310: 7265 6164 2866 703d 6e61 6d65 2c20 2a2a  read(fp=name, **
+00005320: 6b77 6172 6773 5f29 0a20 2020 2020 2020  kwargs_).       
+00005330: 2020 2020 2020 2020 2069 6d67 5f2e 6170           img_.ap
+00005340: 7065 6e64 2864 7329 0a20 2020 2020 2020  pend(ds).       
+00005350: 2072 6574 7572 6e20 696d 675f 2069 6620   return img_ if 
+00005360: 6c65 6e28 6669 6c65 6e61 6d65 7329 203e  len(filenames) >
+00005370: 2031 2065 6c73 6520 696d 675f 5b30 5d0a   1 else img_[0].
+00005380: 0a20 2020 2064 6566 205f 636f 6d62 696e  .    def _combin
+00005390: 655f 6469 636f 6d5f 7365 7269 6573 2873  e_dicom_series(s
+000053a0: 656c 662c 2064 6174 613a 2049 7465 7261  elf, data: Itera
+000053b0: 626c 6529 3a0a 2020 2020 2020 2020 2222  ble):.        ""
+000053c0: 220a 2020 2020 2020 2020 436f 6d62 696e  ".        Combin
+000053d0: 6520 6469 636f 6d20 7365 7269 6573 2028  e dicom series (
+000053e0: 6120 6c69 7374 206f 6620 7079 6469 636f  a list of pydico
+000053f0: 6d20 6461 7461 7365 7420 6f62 6a65 6374  m dataset object
+00005400: 7329 2e20 5468 6569 7220 6461 7461 2061  s). Their data a
+00005410: 7272 6179 7320 7769 6c6c 2062 6520 7374  rrays will be st
+00005420: 6163 6b65 6420 746f 6765 7468 6572 2061  acked together a
+00005430: 7420 6120 6e65 770a 2020 2020 2020 2020  t a new.        
+00005440: 6469 6d65 6e73 696f 6e20 6173 2074 6865  dimension as the
+00005450: 206c 6173 7420 6469 6d65 6e73 696f 6e2e   last dimension.
+00005460: 0a0a 2020 2020 2020 2020 5468 6520 7374  ..        The st
+00005470: 6163 6b20 6f72 6465 7220 6465 7065 6e64  ack order depend
+00005480: 7320 6f6e 2049 6e73 7461 6e63 6520 4e75  s on Instance Nu
+00005490: 6d62 6572 2e20 5468 6520 6d65 7461 6461  mber. The metada
+000054a0: 7461 2077 696c 6c20 6265 2062 6173 6564  ta will be based
+000054b0: 206f 6e20 7468 650a 2020 2020 2020 2020   on the.        
+000054c0: 6669 7273 7420 736c 6963 6527 7320 6d65  first slice's me
+000054d0: 7461 6461 7461 2c20 616e 6420 736f 6d65  tadata, and some
+000054e0: 206e 6577 2069 7465 6d73 2077 696c 6c20   new items will 
+000054f0: 6265 2061 6464 6564 3a0a 0a20 2020 2020  be added:..     
+00005500: 2020 2022 7370 6163 696e 6722 3a20 7468     "spacing": th
+00005510: 6520 6e65 7720 7370 6163 696e 6720 6f66  e new spacing of
+00005520: 2074 6865 2073 7461 636b 6564 2073 6c69   the stacked sli
+00005530: 6365 732e 0a20 2020 2020 2020 2022 6c61  ces..        "la
+00005540: 7374 496d 6167 6550 6f73 6974 696f 6e50  stImagePositionP
+00005550: 6174 6965 6e74 223a 2060 496d 6167 6550  atient": `ImageP
+00005560: 6f73 6974 696f 6e50 6174 6965 6e74 6020  ositionPatient` 
+00005570: 666f 7220 7468 6520 6c61 7374 2073 6c69  for the last sli
+00005580: 6365 2c20 6974 2077 696c 6c20 6265 2075  ce, it will be u
+00005590: 7365 6420 746f 2061 6368 6965 7665 2074  sed to achieve t
+000055a0: 6865 2061 6666 696e 650a 2020 2020 2020  he affine.      
+000055b0: 2020 2020 2020 6d61 7472 6978 2e0a 2020        matrix..  
+000055c0: 2020 2020 2020 2273 7061 7469 616c 5f73        "spatial_s
+000055d0: 6861 7065 223a 2074 6865 2073 7061 7469  hape": the spati
+000055e0: 616c 2073 6861 7065 206f 6620 7468 6520  al shape of the 
+000055f0: 7374 6163 6b65 6420 736c 6963 6573 2e0a  stacked slices..
+00005600: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00005610: 2020 2020 2020 2020 2020 2064 6174 613a             data:
+00005620: 2061 206c 6973 7420 6f66 2070 7964 6963   a list of pydic
+00005630: 6f6d 2064 6174 6173 6574 206f 626a 6563  om dataset objec
+00005640: 7473 2e0a 2020 2020 2020 2020 5265 7475  ts..        Retu
+00005650: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00005660: 2061 2074 7570 6c65 2074 6861 7420 636f   a tuple that co
+00005670: 6e73 6973 7465 6420 7769 7468 2064 6174  nsisted with dat
+00005680: 6120 6172 7261 7920 616e 6420 6d65 7461  a array and meta
+00005690: 6461 7461 2e0a 2020 2020 2020 2020 2222  data..        ""
+000056a0: 220a 2020 2020 2020 2020 736c 6963 6573  ".        slices
+000056b0: 3a20 6c69 7374 203d 205b 5d0a 2020 2020  : list = [].    
+000056c0: 2020 2020 2320 666f 7220 6120 6469 636f      # for a dico
+000056d0: 6d20 7365 7269 6573 0a20 2020 2020 2020  m series.       
+000056e0: 2066 6f72 2073 6c63 5f64 7320 696e 2064   for slc_ds in d
+000056f0: 6174 613a 0a20 2020 2020 2020 2020 2020  ata:.           
+00005700: 2069 6620 6861 7361 7474 7228 736c 635f   if hasattr(slc_
+00005710: 6473 2c20 2249 6e73 7461 6e63 654e 756d  ds, "InstanceNum
+00005720: 6265 7222 293a 0a20 2020 2020 2020 2020  ber"):.         
+00005730: 2020 2020 2020 2073 6c69 6365 732e 6170         slices.ap
+00005740: 7065 6e64 2873 6c63 5f64 7329 0a20 2020  pend(slc_ds).   
+00005750: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00005760: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00005770: 6172 6e69 6e67 732e 7761 726e 2866 2273  arnings.warn(f"s
+00005780: 6c69 6365 3a20 7b73 6c63 5f64 732e 6669  lice: {slc_ds.fi
+00005790: 6c65 6e61 6d65 7d20 646f 6573 206e 6f74  lename} does not
+000057a0: 2068 6176 6520 496e 7374 616e 6365 4e75   have InstanceNu
+000057b0: 6d62 6572 2074 6167 2c20 736b 6970 2069  mber tag, skip i
+000057c0: 742e 2229 0a20 2020 2020 2020 2073 6c69  t.").        sli
+000057d0: 6365 7320 3d20 736f 7274 6564 2873 6c69  ces = sorted(sli
+000057e0: 6365 732c 206b 6579 3d6c 616d 6264 6120  ces, key=lambda 
+000057f0: 733a 2073 2e49 6e73 7461 6e63 654e 756d  s: s.InstanceNum
+00005800: 6265 7229 2020 2320 7479 7065 3a20 6967  ber)  # type: ig
+00005810: 6e6f 7265 0a0a 2020 2020 2020 2020 6966  nore..        if
+00005820: 206c 656e 2873 6c69 6365 7329 203d 3d20   len(slices) == 
+00005830: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+00005840: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00005850: 2274 6865 2069 6e70 7574 2064 6f65 7320  "the input does 
+00005860: 6e6f 7420 6861 7665 2076 616c 6964 2073  not have valid s
+00005870: 6c69 6365 732e 2229 0a0a 2020 2020 2020  lices.")..      
+00005880: 2020 6669 7273 745f 736c 6963 6520 3d20    first_slice = 
+00005890: 736c 6963 6573 5b30 5d0a 2020 2020 2020  slices[0].      
+000058a0: 2020 6176 6572 6167 655f 6469 7374 616e    average_distan
+000058b0: 6365 203d 2030 2e30 0a20 2020 2020 2020  ce = 0.0.       
+000058c0: 2066 6972 7374 5f61 7272 6179 203d 2073   first_array = s
+000058d0: 656c 662e 5f67 6574 5f61 7272 6179 5f64  elf._get_array_d
+000058e0: 6174 6128 6669 7273 745f 736c 6963 6529  ata(first_slice)
+000058f0: 0a20 2020 2020 2020 2073 6861 7065 203d  .        shape =
+00005900: 2066 6972 7374 5f61 7272 6179 2e73 6861   first_array.sha
+00005910: 7065 0a20 2020 2020 2020 2073 7061 6369  pe.        spaci
+00005920: 6e67 203d 2067 6574 6174 7472 2866 6972  ng = getattr(fir
+00005930: 7374 5f73 6c69 6365 2c20 2250 6978 656c  st_slice, "Pixel
+00005940: 5370 6163 696e 6722 2c20 5b31 2e30 2c20  Spacing", [1.0, 
+00005950: 312e 302c 2031 2e30 5d29 0a20 2020 2020  1.0, 1.0]).     
+00005960: 2020 2070 6f73 203d 2067 6574 6174 7472     pos = getattr
+00005970: 2866 6972 7374 5f73 6c69 6365 2c20 2249  (first_slice, "I
+00005980: 6d61 6765 506f 7369 7469 6f6e 5061 7469  magePositionPati
+00005990: 656e 7422 2c20 2830 2e30 2c20 302e 302c  ent", (0.0, 0.0,
+000059a0: 2030 2e30 2929 5b32 5d0a 2020 2020 2020   0.0))[2].      
+000059b0: 2020 7374 6163 6b5f 6172 7261 7920 3d20    stack_array = 
+000059c0: 5b66 6972 7374 5f61 7272 6179 5d0a 2020  [first_array].  
+000059d0: 2020 2020 2020 666f 7220 6964 7820 696e        for idx in
+000059e0: 2072 616e 6765 2831 2c20 6c65 6e28 736c   range(1, len(sl
+000059f0: 6963 6573 2929 3a0a 2020 2020 2020 2020  ices)):.        
+00005a00: 2020 2020 736c 635f 6172 7261 7920 3d20      slc_array = 
+00005a10: 7365 6c66 2e5f 6765 745f 6172 7261 795f  self._get_array_
+00005a20: 6461 7461 2873 6c69 6365 735b 6964 785d  data(slices[idx]
+00005a30: 290a 2020 2020 2020 2020 2020 2020 736c  ).            sl
+00005a40: 635f 7368 6170 6520 3d20 736c 635f 6172  c_shape = slc_ar
+00005a50: 7261 792e 7368 6170 650a 2020 2020 2020  ray.shape.      
+00005a60: 2020 2020 2020 736c 635f 7370 6163 696e        slc_spacin
+00005a70: 6720 3d20 6765 7461 7474 7228 6669 7273  g = getattr(firs
+00005a80: 745f 736c 6963 652c 2022 5069 7865 6c53  t_slice, "PixelS
+00005a90: 7061 6369 6e67 222c 2028 312e 302c 2031  pacing", (1.0, 1
+00005aa0: 2e30 2c20 312e 3029 290a 2020 2020 2020  .0, 1.0)).      
+00005ab0: 2020 2020 2020 736c 635f 706f 7320 3d20        slc_pos = 
+00005ac0: 6765 7461 7474 7228 6669 7273 745f 736c  getattr(first_sl
+00005ad0: 6963 652c 2022 496d 6167 6550 6f73 6974  ice, "ImagePosit
+00005ae0: 696f 6e50 6174 6965 6e74 222c 2028 302e  ionPatient", (0.
+00005af0: 302c 2030 2e30 2c20 666c 6f61 7428 6964  0, 0.0, float(id
+00005b00: 7829 2929 5b32 5d0a 2020 2020 2020 2020  x)))[2].        
+00005b10: 2020 2020 6966 2073 7061 6369 6e67 2021      if spacing !
+00005b20: 3d20 736c 635f 7370 6163 696e 673a 0a20  = slc_spacing:. 
+00005b30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00005b40: 6172 6e69 6e67 732e 7761 726e 2866 2274  arnings.warn(f"t
+00005b50: 6865 206c 6973 7420 636f 6e74 6169 6e73  he list contains
+00005b60: 2073 6c69 6365 7320 7468 6174 2068 6176   slices that hav
+00005b70: 6520 6469 6666 6572 656e 7420 7370 6163  e different spac
+00005b80: 696e 6773 207b 7370 6163 696e 677d 2061  ings {spacing} a
+00005b90: 6e64 207b 736c 635f 7370 6163 696e 677d  nd {slc_spacing}
+00005ba0: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
+00005bb0: 6966 2073 6861 7065 2021 3d20 736c 635f  if shape != slc_
+00005bc0: 7368 6170 653a 0a20 2020 2020 2020 2020  shape:.         
+00005bd0: 2020 2020 2020 2077 6172 6e69 6e67 732e         warnings.
+00005be0: 7761 726e 2866 2274 6865 206c 6973 7420  warn(f"the list 
+00005bf0: 636f 6e74 6169 6e73 2073 6c69 6365 7320  contains slices 
+00005c00: 7468 6174 2068 6176 6520 6469 6666 6572  that have differ
+00005c10: 656e 7420 7368 6170 6573 207b 7368 6170  ent shapes {shap
+00005c20: 657d 2061 6e64 207b 736c 635f 7368 6170  e} and {slc_shap
+00005c30: 657d 2e22 290a 2020 2020 2020 2020 2020  e}.").          
+00005c40: 2020 6176 6572 6167 655f 6469 7374 616e    average_distan
+00005c50: 6365 202b 3d20 6162 7328 706f 7320 2d20  ce += abs(pos - 
+00005c60: 736c 635f 706f 7329 0a20 2020 2020 2020  slc_pos).       
+00005c70: 2020 2020 2070 6f73 203d 2073 6c63 5f70       pos = slc_p
+00005c80: 6f73 0a20 2020 2020 2020 2020 2020 2073  os.            s
+00005c90: 7461 636b 5f61 7272 6179 2e61 7070 656e  tack_array.appen
+00005ca0: 6428 736c 635f 6172 7261 7929 0a0a 2020  d(slc_array)..  
+00005cb0: 2020 2020 2020 6966 206c 656e 2873 6c69        if len(sli
+00005cc0: 6365 7329 203e 2031 3a0a 2020 2020 2020  ces) > 1:.      
+00005cd0: 2020 2020 2020 6176 6572 6167 655f 6469        average_di
+00005ce0: 7374 616e 6365 202f 3d20 6c65 6e28 736c  stance /= len(sl
+00005cf0: 6963 6573 2920 2d20 310a 2020 2020 2020  ices) - 1.      
+00005d00: 2020 2020 2020 7370 6163 696e 672e 6170        spacing.ap
+00005d10: 7065 6e64 2861 7665 7261 6765 5f64 6973  pend(average_dis
+00005d20: 7461 6e63 6529 0a20 2020 2020 2020 2020  tance).         
+00005d30: 2020 2073 7461 636b 5f61 7272 6179 203d     stack_array =
+00005d40: 206e 702e 7374 6163 6b28 7374 6163 6b5f   np.stack(stack_
+00005d50: 6172 7261 792c 2061 7869 733d 2d31 290a  array, axis=-1).
+00005d60: 2020 2020 2020 2020 2020 2020 7374 6163              stac
+00005d70: 6b5f 6d65 7461 6461 7461 203d 2073 656c  k_metadata = sel
+00005d80: 662e 5f67 6574 5f6d 6574 615f 6469 6374  f._get_meta_dict
+00005d90: 2866 6972 7374 5f73 6c69 6365 290a 2020  (first_slice).  
+00005da0: 2020 2020 2020 2020 2020 7374 6163 6b5f            stack_
+00005db0: 6d65 7461 6461 7461 5b22 7370 6163 696e  metadata["spacin
+00005dc0: 6722 5d20 3d20 6e70 2e61 7361 7272 6179  g"] = np.asarray
+00005dd0: 2873 7061 6369 6e67 290a 2020 2020 2020  (spacing).      
+00005de0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+00005df0: 2873 6c69 6365 735b 2d31 5d2c 2022 496d  (slices[-1], "Im
+00005e00: 6167 6550 6f73 6974 696f 6e50 6174 6965  agePositionPatie
+00005e10: 6e74 2229 3a0a 2020 2020 2020 2020 2020  nt"):.          
+00005e20: 2020 2020 2020 7374 6163 6b5f 6d65 7461        stack_meta
+00005e30: 6461 7461 5b22 6c61 7374 496d 6167 6550  data["lastImageP
+00005e40: 6f73 6974 696f 6e50 6174 6965 6e74 225d  ositionPatient"]
+00005e50: 203d 206e 702e 6173 6172 7261 7928 736c   = np.asarray(sl
+00005e60: 6963 6573 5b2d 315d 2e49 6d61 6765 506f  ices[-1].ImagePo
+00005e70: 7369 7469 6f6e 5061 7469 656e 7429 0a20  sitionPatient). 
+00005e80: 2020 2020 2020 2020 2020 2073 7461 636b             stack
+00005e90: 5f6d 6574 6164 6174 615b 4d65 7461 4b65  _metadata[MetaKe
+00005ea0: 7973 2e53 5041 5449 414c 5f53 4841 5045  ys.SPATIAL_SHAPE
+00005eb0: 5d20 3d20 7368 6170 6520 2b20 286c 656e  ] = shape + (len
+00005ec0: 2873 6c69 6365 7329 2c29 0a20 2020 2020  (slices),).     
+00005ed0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00005ee0: 2020 2020 2073 7461 636b 5f61 7272 6179       stack_array
+00005ef0: 203d 2073 7461 636b 5f61 7272 6179 5b30   = stack_array[0
+00005f00: 5d0a 2020 2020 2020 2020 2020 2020 7374  ].            st
+00005f10: 6163 6b5f 6d65 7461 6461 7461 203d 2073  ack_metadata = s
+00005f20: 656c 662e 5f67 6574 5f6d 6574 615f 6469  elf._get_meta_di
+00005f30: 6374 2866 6972 7374 5f73 6c69 6365 290a  ct(first_slice).
+00005f40: 2020 2020 2020 2020 2020 2020 7374 6163              stac
+00005f50: 6b5f 6d65 7461 6461 7461 5b22 7370 6163  k_metadata["spac
+00005f60: 696e 6722 5d20 3d20 6e70 2e61 7361 7272  ing"] = np.asarr
+00005f70: 6179 2873 7061 6369 6e67 290a 2020 2020  ay(spacing).    
+00005f80: 2020 2020 2020 2020 7374 6163 6b5f 6d65          stack_me
+00005f90: 7461 6461 7461 5b4d 6574 614b 6579 732e  tadata[MetaKeys.
+00005fa0: 5350 4154 4941 4c5f 5348 4150 455d 203d  SPATIAL_SHAPE] =
+00005fb0: 2073 6861 7065 0a0a 2020 2020 2020 2020   shape..        
+00005fc0: 7265 7475 726e 2073 7461 636b 5f61 7272  return stack_arr
+00005fd0: 6179 2c20 7374 6163 6b5f 6d65 7461 6461  ay, stack_metada
+00005fe0: 7461 0a0a 2020 2020 6465 6620 6765 745f  ta..    def get_
+00005ff0: 6461 7461 2873 656c 662c 2064 6174 6129  data(self, data)
+00006000: 202d 3e20 7475 706c 655b 6e70 2e6e 6461   -> tuple[np.nda
+00006010: 7272 6179 2c20 6469 6374 5d3a 0a20 2020  rray, dict]:.   
+00006020: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00006030: 2045 7874 7261 6374 2064 6174 6120 6172   Extract data ar
+00006040: 7261 7920 616e 6420 6d65 7461 6461 7461  ray and metadata
+00006050: 2066 726f 6d20 6c6f 6164 6564 2069 6d61   from loaded ima
+00006060: 6765 2061 6e64 2072 6574 7572 6e20 7468  ge and return th
+00006070: 656d 2e0a 2020 2020 2020 2020 5468 6973  em..        This
+00006080: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
+00006090: 7320 7477 6f20 6f62 6a65 6374 732c 2066  s two objects, f
+000060a0: 6972 7374 2069 7320 6e75 6d70 7920 6172  irst is numpy ar
+000060b0: 7261 7920 6f66 2069 6d61 6765 2064 6174  ray of image dat
+000060c0: 612c 2073 6563 6f6e 6420 6973 2064 6963  a, second is dic
+000060d0: 7420 6f66 206d 6574 6164 6174 612e 0a20  t of metadata.. 
+000060e0: 2020 2020 2020 2049 7420 636f 6e73 7472         It constr
+000060f0: 7563 7473 2060 6166 6669 6e65 602c 2060  ucts `affine`, `
+00006100: 6f72 6967 696e 616c 5f61 6666 696e 6560  original_affine`
+00006110: 2c20 616e 6420 6073 7061 7469 616c 5f73  , and `spatial_s
+00006120: 6861 7065 6020 616e 6420 7374 6f72 6573  hape` and stores
+00006130: 2074 6865 6d20 696e 206d 6574 6120 6469   them in meta di
+00006140: 6374 2e0a 2020 2020 2020 2020 466f 7220  ct..        For 
+00006150: 6469 636f 6d20 7365 7269 6573 2077 6974  dicom series wit
+00006160: 6869 6e20 7468 6520 696e 7075 742c 2061  hin the input, a
+00006170: 6c6c 2073 6c69 6365 7320 7769 6c6c 2062  ll slices will b
+00006180: 6520 7374 6163 6b65 6420 6669 7273 742c  e stacked first,
+00006190: 0a20 2020 2020 2020 2057 6865 6e20 6c6f  .        When lo
+000061a0: 6164 696e 6720 6120 6c69 7374 206f 6620  ading a list of 
+000061b0: 6669 6c65 7320 2864 6963 6f6d 2066 696c  files (dicom fil
+000061c0: 652c 206f 7220 7374 6163 6b65 6420 6469  e, or stacked di
+000061d0: 636f 6d20 7365 7269 6573 292c 2074 6865  com series), the
+000061e0: 7920 6172 6520 7374 6163 6b65 6420 746f  y are stacked to
+000061f0: 6765 7468 6572 2061 7420 6120 6e65 770a  gether at a new.
+00006200: 2020 2020 2020 2020 6469 6d65 6e73 696f          dimensio
+00006210: 6e20 6173 2074 6865 2066 6972 7374 2064  n as the first d
+00006220: 696d 656e 7369 6f6e 2c20 616e 6420 7468  imension, and th
+00006230: 6520 6d65 7461 6461 7461 206f 6620 7468  e metadata of th
+00006240: 6520 6669 7273 7420 696d 6167 6520 6973  e first image is
+00006250: 2075 7365 6420 746f 2072 6570 7265 7365   used to represe
+00006260: 6e74 2074 6865 206f 7574 7075 7420 6d65  nt the output me
+00006270: 7461 6461 7461 2e0a 0a20 2020 2020 2020  tadata...       
+00006280: 2054 6f20 7573 6520 7468 6973 2066 756e   To use this fun
+00006290: 6374 696f 6e2c 2061 6c6c 2070 7964 6963  ction, all pydic
+000062a0: 6f6d 2064 6174 6173 6574 206f 626a 6563  om dataset objec
+000062b0: 7473 2028 6966 206e 6f74 2073 6567 6d65  ts (if not segme
+000062c0: 6e74 6174 696f 6e20 6461 7461 2920 7368  ntation data) sh
+000062d0: 6f75 6c64 2063 6f6e 7461 696e 3a0a 2020  ould contain:.  
+000062e0: 2020 2020 2020 6070 6978 656c 5f61 7272        `pixel_arr
+000062f0: 6179 602c 2060 5069 7865 6c53 7061 6369  ay`, `PixelSpaci
+00006300: 6e67 602c 2060 496d 6167 6550 6f73 6974  ng`, `ImagePosit
+00006310: 696f 6e50 6174 6965 6e74 6020 616e 6420  ionPatient` and 
+00006320: 6049 6d61 6765 4f72 6965 6e74 6174 696f  `ImageOrientatio
+00006330: 6e50 6174 6965 6e74 602e 0a0a 2020 2020  nPatient`...    
+00006340: 2020 2020 466f 7220 7365 676d 656e 7461      For segmenta
+00006350: 7469 6f6e 2064 6174 612c 2077 6520 6173  tion data, we as
+00006360: 7375 6d65 2074 6861 7420 7468 6520 696e  sume that the in
+00006370: 7075 7420 6973 206e 6f74 2061 2064 6963  put is not a dic
+00006380: 6f6d 2073 6572 6965 732c 2061 6e64 2074  om series, and t
+00006390: 6865 206f 626a 6563 7420 7368 6f75 6c64  he object should
+000063a0: 2063 6f6e 7461 696e 0a20 2020 2020 2020   contain.       
+000063b0: 2060 5365 676d 656e 7453 6571 7565 6e63   `SegmentSequenc
+000063c0: 6560 2069 6e20 6f72 6465 7220 746f 2069  e` in order to i
+000063d0: 6465 6e74 6966 7920 6974 2e0a 2020 2020  dentify it..    
+000063e0: 2020 2020 496e 2061 6464 6974 696f 6e2c      In addition,
+000063f0: 2074 6167 7320 2835 3230 302c 2039 3232   tags (5200, 922
+00006400: 3929 2061 6e64 2028 3532 3030 2c20 3932  9) and (5200, 92
+00006410: 3330 2920 6172 6520 7265 7175 6972 6564  30) are required
+00006420: 2074 6f20 6163 6869 6576 650a 2020 2020   to achieve.    
+00006430: 2020 2020 6050 6978 656c 5370 6163 696e      `PixelSpacin
+00006440: 6760 2c20 6049 6d61 6765 4f72 6965 6e74  g`, `ImageOrient
+00006450: 6174 696f 6e50 6174 6965 6e74 6020 616e  ationPatient` an
+00006460: 6420 6049 6d61 6765 506f 7369 7469 6f6e  d `ImagePosition
+00006470: 5061 7469 656e 7460 2e0a 0a20 2020 2020  Patient`...     
+00006480: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00006490: 2020 2020 2064 6174 613a 2061 2070 7964       data: a pyd
+000064a0: 6963 6f6d 2064 6174 6173 6574 206f 626a  icom dataset obj
+000064b0: 6563 742c 206f 7220 6120 6c69 7374 206f  ect, or a list o
+000064c0: 6620 7079 6469 636f 6d20 6461 7461 7365  f pydicom datase
+000064d0: 7420 6f62 6a65 6374 732c 206f 7220 6120  t objects, or a 
+000064e0: 6c69 7374 206f 6620 6c69 7374 206f 660a  list of list of.
+000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006500: 7079 6469 636f 6d20 6461 7461 7365 7420  pydicom dataset 
+00006510: 6f62 6a65 6374 732e 0a0a 2020 2020 2020  objects...      
+00006520: 2020 2222 220a 0a20 2020 2020 2020 2064    """..        d
+00006530: 6963 6f6d 5f64 6174 6120 3d20 5b5d 0a20  icom_data = []. 
+00006540: 2020 2020 2020 2023 2063 6f6d 6269 6e65         # combine
+00006550: 2064 6963 6f6d 2073 6572 6965 7320 6966   dicom series if
+00006560: 2065 7869 7374 730a 2020 2020 2020 2020   exists.        
+00006570: 6966 2073 656c 662e 6861 735f 7365 7269  if self.has_seri
+00006580: 6573 2069 7320 5472 7565 3a0a 2020 2020  es is True:.    
+00006590: 2020 2020 2020 2020 2320 6120 6c69 7374          # a list
+000065a0: 2c20 616c 6c20 6f62 6a65 6374 7320 7769  , all objects wi
+000065b0: 7468 696e 2061 206c 6973 7420 6265 6c6f  thin a list belo
+000065c0: 6e67 2074 6f20 6f6e 6520 6469 636f 6d20  ng to one dicom 
+000065d0: 7365 7269 6573 0a20 2020 2020 2020 2020  series.         
+000065e0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+000065f0: 616e 6365 2864 6174 615b 305d 2c20 6c69  ance(data[0], li
+00006600: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00006610: 2020 2020 2064 6963 6f6d 5f64 6174 612e       dicom_data.
+00006620: 6170 7065 6e64 2873 656c 662e 5f63 6f6d  append(self._com
+00006630: 6269 6e65 5f64 6963 6f6d 5f73 6572 6965  bine_dicom_serie
+00006640: 7328 6461 7461 2929 0a20 2020 2020 2020  s(data)).       
+00006650: 2020 2020 2023 2061 206c 6973 7420 6f66       # a list of
+00006660: 206c 6973 742c 2065 6163 6820 696e 6e65   list, each inne
+00006670: 7220 6c69 7374 2072 6570 7265 7365 6e74  r list represent
+00006680: 7320 6120 6469 636f 6d20 7365 7269 6573  s a dicom series
+00006690: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+000066a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000066b0: 2020 2066 6f72 2073 6572 6965 7320 696e     for series in
+000066c0: 2064 6174 613a 0a20 2020 2020 2020 2020   data:.         
+000066d0: 2020 2020 2020 2020 2020 2064 6963 6f6d             dicom
+000066e0: 5f64 6174 612e 6170 7065 6e64 2873 656c  _data.append(sel
+000066f0: 662e 5f63 6f6d 6269 6e65 5f64 6963 6f6d  f._combine_dicom
+00006700: 5f73 6572 6965 7328 7365 7269 6573 2929  _series(series))
+00006710: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00006720: 2020 2020 2020 2020 2020 2023 2061 2073             # a s
+00006730: 696e 676c 6520 7079 6469 636f 6d20 6461  ingle pydicom da
+00006740: 7461 7365 7420 6f62 6a65 6374 0a20 2020  taset object.   
+00006750: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00006760: 6973 696e 7374 616e 6365 2864 6174 612c  isinstance(data,
+00006770: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
+00006780: 2020 2020 2020 2020 6461 7461 203d 205b          data = [
+00006790: 6461 7461 5d0a 2020 2020 2020 2020 2020  data].          
+000067a0: 2020 666f 7220 6420 696e 2064 6174 613a    for d in data:
+000067b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000067c0: 2069 6620 6861 7361 7474 7228 642c 2022   if hasattr(d, "
+000067d0: 5365 676d 656e 7453 6571 7565 6e63 6522  SegmentSequence"
+000067e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000067f0: 2020 2020 2020 2064 6174 615f 6172 7261         data_arra
+00006800: 792c 206d 6574 6164 6174 6120 3d20 7365  y, metadata = se
+00006810: 6c66 2e5f 6765 745f 7365 675f 6461 7461  lf._get_seg_data
+00006820: 2864 290a 2020 2020 2020 2020 2020 2020  (d).            
+00006830: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00006840: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00006850: 7461 5f61 7272 6179 203d 2073 656c 662e  ta_array = self.
+00006860: 5f67 6574 5f61 7272 6179 5f64 6174 6128  _get_array_data(
+00006870: 6429 0a20 2020 2020 2020 2020 2020 2020  d).             
+00006880: 2020 2020 2020 206d 6574 6164 6174 6120         metadata 
+00006890: 3d20 7365 6c66 2e5f 6765 745f 6d65 7461  = self._get_meta
+000068a0: 5f64 6963 7428 6429 0a20 2020 2020 2020  _dict(d).       
+000068b0: 2020 2020 2020 2020 2020 2020 206d 6574               met
+000068c0: 6164 6174 615b 4d65 7461 4b65 7973 2e53  adata[MetaKeys.S
+000068d0: 5041 5449 414c 5f53 4841 5045 5d20 3d20  PATIAL_SHAPE] = 
+000068e0: 6461 7461 5f61 7272 6179 2e73 6861 7065  data_array.shape
+000068f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006900: 2064 6963 6f6d 5f64 6174 612e 6170 7065   dicom_data.appe
+00006910: 6e64 2828 6461 7461 5f61 7272 6179 2c20  nd((data_array, 
+00006920: 6d65 7461 6461 7461 2929 0a0a 2020 2020  metadata))..    
+00006930: 2020 2020 696d 675f 6172 7261 793a 206c      img_array: l
+00006940: 6973 745b 6e70 2e6e 6461 7272 6179 5d20  ist[np.ndarray] 
+00006950: 3d20 5b5d 0a20 2020 2020 2020 2063 6f6d  = [].        com
+00006960: 7061 7469 626c 655f 6d65 7461 3a20 6469  patible_meta: di
+00006970: 6374 203d 207b 7d0a 0a20 2020 2020 2020  ct = {}..       
+00006980: 2066 6f72 2064 6174 615f 6172 7261 792c   for data_array,
+00006990: 206d 6574 6164 6174 6120 696e 2065 6e73   metadata in ens
+000069a0: 7572 655f 7475 706c 6528 6469 636f 6d5f  ure_tuple(dicom_
+000069b0: 6461 7461 293a 0a20 2020 2020 2020 2020  data):.         
+000069c0: 2020 2069 6d67 5f61 7272 6179 2e61 7070     img_array.app
+000069d0: 656e 6428 6e70 2e61 7363 6f6e 7469 6775  end(np.ascontigu
+000069e0: 6f75 7361 7272 6179 286e 702e 7377 6170  ousarray(np.swap
+000069f0: 6178 6573 2864 6174 615f 6172 7261 792c  axes(data_array,
+00006a00: 2030 2c20 3129 2069 6620 7365 6c66 2e73   0, 1) if self.s
+00006a10: 7761 705f 696a 2065 6c73 6520 6461 7461  wap_ij else data
+00006a20: 5f61 7272 6179 2929 0a20 2020 2020 2020  _array)).       
+00006a30: 2020 2020 2061 6666 696e 6520 3d20 7365       affine = se
+00006a40: 6c66 2e5f 6765 745f 6166 6669 6e65 286d  lf._get_affine(m
+00006a50: 6574 6164 6174 612c 2073 656c 662e 6166  etadata, self.af
+00006a60: 6669 6e65 5f6c 7073 5f74 6f5f 7261 7329  fine_lps_to_ras)
+00006a70: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+00006a80: 6164 6174 615b 4d65 7461 4b65 7973 2e53  adata[MetaKeys.S
+00006a90: 5041 4345 5d20 3d20 5370 6163 654b 6579  PACE] = SpaceKey
+00006aa0: 732e 5241 5320 6966 2073 656c 662e 6166  s.RAS if self.af
+00006ab0: 6669 6e65 5f6c 7073 5f74 6f5f 7261 7320  fine_lps_to_ras 
+00006ac0: 656c 7365 2053 7061 6365 4b65 7973 2e4c  else SpaceKeys.L
+00006ad0: 5053 0a20 2020 2020 2020 2020 2020 2069  PS.            i
+00006ae0: 6620 7365 6c66 2e73 7761 705f 696a 3a0a  f self.swap_ij:.
+00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b00: 6166 6669 6e65 203d 2061 6666 696e 6520  affine = affine 
+00006b10: 4020 6e70 2e61 7272 6179 285b 5b30 2c20  @ np.array([[0, 
+00006b20: 312c 2030 2c20 305d 2c20 5b31 2c20 302c  1, 0, 0], [1, 0,
+00006b30: 2030 2c20 305d 2c20 5b30 2c20 302c 2031   0, 0], [0, 0, 1
+00006b40: 2c20 305d 2c20 5b30 2c20 302c 2030 2c20  , 0], [0, 0, 0, 
+00006b50: 315d 5d29 0a20 2020 2020 2020 2020 2020  1]]).           
+00006b60: 2020 2020 2073 705f 7369 7a65 203d 206c       sp_size = l
+00006b70: 6973 7428 6d65 7461 6461 7461 5b4d 6574  ist(metadata[Met
+00006b80: 614b 6579 732e 5350 4154 4941 4c5f 5348  aKeys.SPATIAL_SH
+00006b90: 4150 455d 290a 2020 2020 2020 2020 2020  APE]).          
+00006ba0: 2020 2020 2020 7370 5f73 697a 655b 305d        sp_size[0]
+00006bb0: 2c20 7370 5f73 697a 655b 315d 203d 2073  , sp_size[1] = s
+00006bc0: 705f 7369 7a65 5b31 5d2c 2073 705f 7369  p_size[1], sp_si
+00006bd0: 7a65 5b30 5d0a 2020 2020 2020 2020 2020  ze[0].          
+00006be0: 2020 2020 2020 6d65 7461 6461 7461 5b4d        metadata[M
+00006bf0: 6574 614b 6579 732e 5350 4154 4941 4c5f  etaKeys.SPATIAL_
+00006c00: 5348 4150 455d 203d 2065 6e73 7572 655f  SHAPE] = ensure_
+00006c10: 7475 706c 6528 7370 5f73 697a 6529 0a20  tuple(sp_size). 
+00006c20: 2020 2020 2020 2020 2020 206d 6574 6164             metad
+00006c30: 6174 615b 4d65 7461 4b65 7973 2e4f 5249  ata[MetaKeys.ORI
+00006c40: 4749 4e41 4c5f 4146 4649 4e45 5d20 3d20  GINAL_AFFINE] = 
+00006c50: 6166 6669 6e65 0a20 2020 2020 2020 2020  affine.         
+00006c60: 2020 206d 6574 6164 6174 615b 4d65 7461     metadata[Meta
+00006c70: 4b65 7973 2e41 4646 494e 455d 203d 2061  Keys.AFFINE] = a
+00006c80: 6666 696e 652e 636f 7079 2829 0a20 2020  ffine.copy().   
+00006c90: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00006ca0: 2e63 6861 6e6e 656c 5f64 696d 2069 7320  .channel_dim is 
+00006cb0: 4e6f 6e65 3a20 2023 2064 6566 6175 6c74  None:  # default
+00006cc0: 2074 6f20 226e 6f5f 6368 616e 6e65 6c22   to "no_channel"
+00006cd0: 206f 7220 2d31 0a20 2020 2020 2020 2020   or -1.         
+00006ce0: 2020 2020 2020 206d 6574 6164 6174 615b         metadata[
+00006cf0: 4d65 7461 4b65 7973 2e4f 5249 4749 4e41  MetaKeys.ORIGINA
+00006d00: 4c5f 4348 414e 4e45 4c5f 4449 4d5d 203d  L_CHANNEL_DIM] =
+00006d10: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00006d20: 2020 2020 2020 2066 6c6f 6174 2822 6e61         float("na
+00006d30: 6e22 2920 6966 206c 656e 2864 6174 615f  n") if len(data_
+00006d40: 6172 7261 792e 7368 6170 6529 203d 3d20  array.shape) == 
+00006d50: 6c65 6e28 6d65 7461 6461 7461 5b4d 6574  len(metadata[Met
+00006d60: 614b 6579 732e 5350 4154 4941 4c5f 5348  aKeys.SPATIAL_SH
+00006d70: 4150 455d 2920 656c 7365 202d 310a 2020  APE]) else -1.  
+00006d80: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00006d90: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00006da0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00006db0: 2020 6d65 7461 6461 7461 5b4d 6574 614b    metadata[MetaK
+00006dc0: 6579 732e 4f52 4947 494e 414c 5f43 4841  eys.ORIGINAL_CHA
+00006dd0: 4e4e 454c 5f44 494d 5d20 3d20 7365 6c66  NNEL_DIM] = self
+00006de0: 2e63 6861 6e6e 656c 5f64 696d 0a20 2020  .channel_dim.   
+00006df0: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
+00006e00: 615b 2273 7061 6369 6e67 225d 203d 2061  a["spacing"] = a
+00006e10: 6666 696e 655f 746f 5f73 7061 6369 6e67  ffine_to_spacing
+00006e20: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00006e30: 2020 6d65 7461 6461 7461 5b4d 6574 614b    metadata[MetaK
+00006e40: 6579 732e 4f52 4947 494e 414c 5f41 4646  eys.ORIGINAL_AFF
+00006e50: 494e 455d 2c20 723d 6c65 6e28 6d65 7461  INE], r=len(meta
+00006e60: 6461 7461 5b4d 6574 614b 6579 732e 5350  data[MetaKeys.SP
+00006e70: 4154 4941 4c5f 5348 4150 455d 290a 2020  ATIAL_SHAPE]).  
+00006e80: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00006e90: 2020 2020 2020 2020 205f 636f 7079 5f63           _copy_c
+00006ea0: 6f6d 7061 7469 626c 655f 6469 6374 286d  ompatible_dict(m
+00006eb0: 6574 6164 6174 612c 2063 6f6d 7061 7469  etadata, compati
+00006ec0: 626c 655f 6d65 7461 290a 0a20 2020 2020  ble_meta)..     
+00006ed0: 2020 2072 6574 7572 6e20 5f73 7461 636b     return _stack
+00006ee0: 5f69 6d61 6765 7328 696d 675f 6172 7261  _images(img_arra
+00006ef0: 792c 2063 6f6d 7061 7469 626c 655f 6d65  y, compatible_me
+00006f00: 7461 292c 2063 6f6d 7061 7469 626c 655f  ta), compatible_
+00006f10: 6d65 7461 0a0a 2020 2020 6465 6620 5f67  meta..    def _g
+00006f20: 6574 5f6d 6574 615f 6469 6374 2873 656c  et_meta_dict(sel
+00006f30: 662c 2069 6d67 2920 2d3e 2064 6963 743a  f, img) -> dict:
+00006f40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00006f50: 2020 2020 2047 6574 2061 6c6c 2074 6865       Get all the
+00006f60: 206d 6574 6164 6174 6120 6f66 2074 6865   metadata of the
+00006f70: 2069 6d61 6765 2061 6e64 2063 6f6e 7665   image and conve
+00006f80: 7274 2074 6f20 6469 6374 2074 7970 652e  rt to dict type.
+00006f90: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00006fa0: 2020 2020 2020 2020 2020 2020 696d 673a              img:
+00006fb0: 2061 2050 7964 6963 6f6d 2064 6174 6173   a Pydicom datas
+00006fc0: 6574 206f 626a 6563 742e 0a0a 2020 2020  et object...    
+00006fd0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+00006fe0: 206d 6574 6164 6174 6120 3d20 696d 672e   metadata = img.
+00006ff0: 746f 5f6a 736f 6e5f 6469 6374 2873 7570  to_json_dict(sup
+00007000: 7072 6573 735f 696e 7661 6c69 645f 7461  press_invalid_ta
+00007010: 6773 3d54 7275 6529 0a0a 2020 2020 2020  gs=True)..      
+00007020: 2020 6966 2073 656c 662e 7072 756e 655f    if self.prune_
+00007030: 6d65 7461 6461 7461 3a0a 2020 2020 2020  metadata:.      
+00007040: 2020 2020 2020 7072 756e 655f 6d65 7461        prune_meta
+00007050: 6461 7461 203d 207b 7d0a 2020 2020 2020  data = {}.      
+00007060: 2020 2020 2020 666f 7220 6b65 7920 696e        for key in
+00007070: 205b 2230 3032 3030 3033 3722 2c20 2230   ["00200037", "0
+00007080: 3032 3030 3033 3222 2c20 2235 3230 3039  0200032", "52009
+00007090: 3232 3922 2c20 2235 3230 3039 3233 3022  229", "52009230"
+000070a0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+000070b0: 2020 2069 6620 6b65 7920 696e 206d 6574     if key in met
+000070c0: 6164 6174 612e 6b65 7973 2829 3a0a 2020  adata.keys():.  
+000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070e0: 2020 7072 756e 655f 6d65 7461 6461 7461    prune_metadata
+000070f0: 5b6b 6579 5d20 3d20 6d65 7461 6461 7461  [key] = metadata
+00007100: 5b6b 6579 5d0a 2020 2020 2020 2020 2020  [key].          
+00007110: 2020 7265 7475 726e 2070 7275 6e65 5f6d    return prune_m
+00007120: 6574 6164 6174 610a 0a20 2020 2020 2020  etadata..       
+00007130: 2023 2061 6c77 6179 7320 7265 6d6f 7665   # always remove
+00007140: 2050 6978 656c 2044 6174 6120 2237 4645   Pixel Data "7FE
+00007150: 3030 3030 3822 206f 7220 2237 4645 3030  00008" or "7FE00
+00007160: 3030 3922 206f 7220 2237 4645 3030 3031  009" or "7FE0001
+00007170: 3022 0a20 2020 2020 2020 2023 2061 6c77  0".        # alw
+00007180: 6179 7320 7265 6d6f 7665 2044 6174 6120  ays remove Data 
+00007190: 5365 7420 5472 6169 6c69 6e67 2050 6164  Set Trailing Pad
+000071a0: 6469 6e67 2022 4646 4643 4646 4643 220a  ding "FFFCFFFC".
+000071b0: 2020 2020 2020 2020 666f 7220 6b65 7920          for key 
+000071c0: 696e 205b 2237 4645 3030 3030 3822 2c20  in ["7FE00008", 
+000071d0: 2237 4645 3030 3030 3922 2c20 2237 4645  "7FE00009", "7FE
+000071e0: 3030 3031 3022 2c20 2246 4646 4346 4646  00010", "FFFCFFF
+000071f0: 4322 5d3a 0a20 2020 2020 2020 2020 2020  C"]:.           
+00007200: 2069 6620 6b65 7920 696e 206d 6574 6164   if key in metad
+00007210: 6174 612e 6b65 7973 2829 3a0a 2020 2020  ata.keys():.    
+00007220: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00007230: 6461 7461 2e70 6f70 286b 6579 290a 0a20  data.pop(key).. 
+00007240: 2020 2020 2020 2072 6574 7572 6e20 6d65         return me
+00007250: 7461 6461 7461 2020 2320 7479 7065 3a20  tadata  # type: 
+00007260: 6967 6e6f 7265 0a0a 2020 2020 6465 6620  ignore..    def 
+00007270: 5f67 6574 5f61 6666 696e 6528 7365 6c66  _get_affine(self
+00007280: 2c20 6d65 7461 6461 7461 3a20 6469 6374  , metadata: dict
+00007290: 2c20 6c70 735f 746f 5f72 6173 3a20 626f  , lps_to_ras: bo
+000072a0: 6f6c 203d 2054 7275 6529 3a0a 2020 2020  ol = True):.    
+000072b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000072c0: 4765 7420 6f72 2063 6f6e 7374 7275 6374  Get or construct
+000072d0: 2074 6865 2061 6666 696e 6520 6d61 7472   the affine matr
+000072e0: 6978 206f 6620 7468 6520 696d 6167 652c  ix of the image,
+000072f0: 2069 7420 6361 6e20 6265 2075 7365 6420   it can be used 
+00007300: 746f 2063 6f72 7265 6374 0a20 2020 2020  to correct.     
+00007310: 2020 2073 7061 6369 6e67 2c20 6f72 6965     spacing, orie
+00007320: 6e74 6174 696f 6e20 6f72 2065 7865 6375  ntation or execu
+00007330: 7465 2073 7061 7469 616c 2074 7261 6e73  te spatial trans
+00007340: 666f 726d 732e 0a0a 2020 2020 2020 2020  forms...        
+00007350: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00007360: 2020 6d65 7461 6461 7461 3a20 6d65 7461    metadata: meta
+00007370: 6461 7461 2077 6974 6820 6469 6374 2074  data with dict t
+00007380: 7970 652e 0a20 2020 2020 2020 2020 2020  ype..           
+00007390: 206c 7073 5f74 6f5f 7261 733a 2077 6865   lps_to_ras: whe
+000073a0: 7468 6572 2074 6f20 636f 6e76 6572 7420  ther to convert 
+000073b0: 7468 6520 6166 6669 6e65 206d 6174 7269  the affine matri
+000073c0: 7820 6672 6f6d 2022 4c50 5322 2074 6f20  x from "LPS" to 
+000073d0: 2252 4153 222e 2044 6566 6175 6c74 7320  "RAS". Defaults 
+000073e0: 746f 2054 7275 652e 0a0a 2020 2020 2020  to True...      
+000073f0: 2020 2222 220a 2020 2020 2020 2020 6166    """.        af
+00007400: 6669 6e65 3a20 6e70 2e6e 6461 7272 6179  fine: np.ndarray
+00007410: 203d 206e 702e 6579 6528 3429 0a20 2020   = np.eye(4).   
+00007420: 2020 2020 2069 6620 6e6f 7420 2822 3030       if not ("00
+00007430: 3230 3030 3337 2220 696e 206d 6574 6164  200037" in metad
+00007440: 6174 6120 616e 6420 2230 3032 3030 3033  ata and "0020003
+00007450: 3222 2069 6e20 6d65 7461 6461 7461 293a  2" in metadata):
+00007460: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007470: 7572 6e20 6166 6669 6e65 0a20 2020 2020  urn affine.     
+00007480: 2020 2023 2022 3030 3230 3030 3337 2220     # "00200037" 
+00007490: 6973 2074 6865 2074 6167 206f 6620 6049  is the tag of `I
+000074a0: 6d61 6765 4f72 6965 6e74 6174 696f 6e50  mageOrientationP
+000074b0: 6174 6965 6e74 600a 2020 2020 2020 2020  atient`.        
+000074c0: 7278 2c20 7279 2c20 727a 2c20 6378 2c20  rx, ry, rz, cx, 
+000074d0: 6379 2c20 637a 203d 206d 6574 6164 6174  cy, cz = metadat
+000074e0: 615b 2230 3032 3030 3033 3722 5d5b 2256  a["00200037"]["V
+000074f0: 616c 7565 225d 0a20 2020 2020 2020 2023  alue"].        #
+00007500: 2022 3030 3230 3030 3332 2220 6973 2074   "00200032" is t
+00007510: 6865 2074 6167 206f 6620 6049 6d61 6765  he tag of `Image
+00007520: 506f 7369 7469 6f6e 5061 7469 656e 7460  PositionPatient`
+00007530: 0a20 2020 2020 2020 2073 782c 2073 792c  .        sx, sy,
+00007540: 2073 7a20 3d20 6d65 7461 6461 7461 5b22   sz = metadata["
+00007550: 3030 3230 3030 3332 225d 5b22 5661 6c75  00200032"]["Valu
+00007560: 6522 5d0a 2020 2020 2020 2020 6472 2c20  e"].        dr, 
+00007570: 6463 203d 206d 6574 6164 6174 612e 6765  dc = metadata.ge
+00007580: 7428 2273 7061 6369 6e67 222c 2028 312e  t("spacing", (1.
+00007590: 302c 2031 2e30 2929 5b3a 325d 0a20 2020  0, 1.0))[:2].   
+000075a0: 2020 2020 2061 6666 696e 655b 302c 2030       affine[0, 0
+000075b0: 5d20 3d20 6378 202a 2064 720a 2020 2020  ] = cx * dr.    
+000075c0: 2020 2020 6166 6669 6e65 5b30 2c20 315d      affine[0, 1]
+000075d0: 203d 2072 7820 2a20 6463 0a20 2020 2020   = rx * dc.     
+000075e0: 2020 2061 6666 696e 655b 302c 2033 5d20     affine[0, 3] 
+000075f0: 3d20 7378 0a20 2020 2020 2020 2061 6666  = sx.        aff
+00007600: 696e 655b 312c 2030 5d20 3d20 6379 202a  ine[1, 0] = cy *
+00007610: 2064 720a 2020 2020 2020 2020 6166 6669   dr.        affi
+00007620: 6e65 5b31 2c20 315d 203d 2072 7920 2a20  ne[1, 1] = ry * 
+00007630: 6463 0a20 2020 2020 2020 2061 6666 696e  dc.        affin
+00007640: 655b 312c 2033 5d20 3d20 7379 0a20 2020  e[1, 3] = sy.   
+00007650: 2020 2020 2061 6666 696e 655b 322c 2030       affine[2, 0
+00007660: 5d20 3d20 637a 202a 2064 720a 2020 2020  ] = cz * dr.    
+00007670: 2020 2020 6166 6669 6e65 5b32 2c20 315d      affine[2, 1]
+00007680: 203d 2072 7a20 2a20 6463 0a20 2020 2020   = rz * dc.     
+00007690: 2020 2061 6666 696e 655b 322c 2032 5d20     affine[2, 2] 
+000076a0: 3d20 300a 2020 2020 2020 2020 6166 6669  = 0.        affi
+000076b0: 6e65 5b32 2c20 335d 203d 2073 7a0a 0a20  ne[2, 3] = sz.. 
+000076c0: 2020 2020 2020 2023 2033 640a 2020 2020         # 3d.    
+000076d0: 2020 2020 6966 2022 6c61 7374 496d 6167      if "lastImag
+000076e0: 6550 6f73 6974 696f 6e50 6174 6965 6e74  ePositionPatient
+000076f0: 2220 696e 206d 6574 6164 6174 613a 0a20  " in metadata:. 
+00007700: 2020 2020 2020 2020 2020 2074 316e 2c20             t1n, 
+00007710: 7432 6e2c 2074 336e 203d 206d 6574 6164  t2n, t3n = metad
+00007720: 6174 615b 226c 6173 7449 6d61 6765 506f  ata["lastImagePo
+00007730: 7369 7469 6f6e 5061 7469 656e 7422 5d0a  sitionPatient"].
+00007740: 2020 2020 2020 2020 2020 2020 6e20 3d20              n = 
+00007750: 6d65 7461 6461 7461 5b4d 6574 614b 6579  metadata[MetaKey
+00007760: 732e 5350 4154 4941 4c5f 5348 4150 455d  s.SPATIAL_SHAPE]
+00007770: 5b2d 315d 0a20 2020 2020 2020 2020 2020  [-1].           
+00007780: 206b 312c 206b 322c 206b 3320 3d20 2874   k1, k2, k3 = (t
+00007790: 316e 202d 2073 7829 202f 2028 6e20 2d20  1n - sx) / (n - 
+000077a0: 3129 2c20 2874 326e 202d 2073 7929 202f  1), (t2n - sy) /
+000077b0: 2028 6e20 2d20 3129 2c20 2874 336e 202d   (n - 1), (t3n -
+000077c0: 2073 7a29 202f 2028 6e20 2d20 3129 0a20   sz) / (n - 1). 
+000077d0: 2020 2020 2020 2020 2020 2061 6666 696e             affin
+000077e0: 655b 302c 2032 5d20 3d20 6b31 0a20 2020  e[0, 2] = k1.   
+000077f0: 2020 2020 2020 2020 2061 6666 696e 655b           affine[
+00007800: 312c 2032 5d20 3d20 6b32 0a20 2020 2020  1, 2] = k2.     
+00007810: 2020 2020 2020 2061 6666 696e 655b 322c         affine[2,
+00007820: 2032 5d20 3d20 6b33 0a0a 2020 2020 2020   2] = k3..      
+00007830: 2020 6966 206c 7073 5f74 6f5f 7261 733a    if lps_to_ras:
+00007840: 0a20 2020 2020 2020 2020 2020 2061 6666  .            aff
+00007850: 696e 6520 3d20 6f72 6965 6e74 6174 696f  ine = orientatio
+00007860: 6e5f 7261 735f 6c70 7328 6166 6669 6e65  n_ras_lps(affine
+00007870: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00007880: 2061 6666 696e 650a 0a20 2020 2064 6566   affine..    def
+00007890: 205f 6765 745f 6672 616d 655f 6461 7461   _get_frame_data
+000078a0: 2873 656c 662c 2069 6d67 2920 2d3e 2049  (self, img) -> I
+000078b0: 7465 7261 746f 723a 0a20 2020 2020 2020  terator:.       
+000078c0: 2022 2222 0a20 2020 2020 2020 2079 6965   """.        yie
+000078d0: 6c64 2066 7261 6d65 7320 616e 6420 6465  ld frames and de
+000078e0: 7363 7269 7074 696f 6e20 6672 6f6d 2074  scription from t
+000078f0: 6865 2073 6567 6d65 6e74 6174 696f 6e20  he segmentation 
+00007900: 696d 6167 652e 0a20 2020 2020 2020 2054  image..        T
+00007910: 6869 7320 6675 6e63 7469 6f6e 2069 7320  his function is 
+00007920: 6164 6170 7465 6420 6672 6f6d 2048 6967  adapted from Hig
+00007930: 6864 6963 6f6d 3a0a 2020 2020 2020 2020  hdicom:.        
+00007940: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00007950: 6f6d 2f68 6572 726d 616e 6e6c 6162 2f68  om/herrmannlab/h
+00007960: 6967 6864 6963 6f6d 2f62 6c6f 622f 7630  ighdicom/blob/v0
+00007970: 2e31 382e 322f 7372 632f 6869 6768 6469  .18.2/src/highdi
+00007980: 636f 6d2f 7365 672f 7574 696c 732e 7079  com/seg/utils.py
+00007990: 0a0a 2020 2020 2020 2020 7768 6963 6820  ..        which 
+000079a0: 6861 7320 7468 6520 666f 6c6c 6f77 696e  has the followin
+000079b0: 6720 6c69 6365 6e73 652e 2e2e 0a0a 2020  g license.....  
+000079c0: 2020 2020 2020 2320 3d3d 3d3d 3d3d 3d3d        # ========
+000079d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000079e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000079f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007a00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007a10: 3d0a 2020 2020 2020 2020 2320 6874 7470  =.        # http
+00007a20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+00007a30: 6572 726d 616e 6e6c 6162 2f68 6967 6864  errmannlab/highd
+00007a40: 6963 6f6d 2f62 6c6f 622f 7630 2e31 382e  icom/blob/v0.18.
+00007a50: 322f 4c49 4345 4e53 450a 2020 2020 2020  2/LICENSE.      
+00007a60: 2020 230a 2020 2020 2020 2020 2320 436f    #.        # Co
+00007a70: 7079 7269 6768 7420 3230 3230 204d 4748  pyright 2020 MGH
+00007a80: 2043 6f6d 7075 7461 7469 6f6e 616c 2050   Computational P
+00007a90: 6174 686f 6c6f 6779 0a20 2020 2020 2020  athology.       
+00007aa0: 2023 2050 6572 6d69 7373 696f 6e20 6973   # Permission is
+00007ab0: 2068 6572 6562 7920 6772 616e 7465 642c   hereby granted,
+00007ac0: 2066 7265 6520 6f66 2063 6861 7267 652c   free of charge,
+00007ad0: 2074 6f20 616e 7920 7065 7273 6f6e 206f   to any person o
+00007ae0: 6274 6169 6e69 6e67 2061 0a20 2020 2020  btaining a.     
+00007af0: 2020 2023 2063 6f70 7920 6f66 2074 6869     # copy of thi
+00007b00: 7320 736f 6674 7761 7265 2061 6e64 2061  s software and a
+00007b10: 7373 6f63 6961 7465 6420 646f 6375 6d65  ssociated docume
+00007b20: 6e74 6174 696f 6e20 6669 6c65 7320 2874  ntation files (t
+00007b30: 6865 0a20 2020 2020 2020 2023 2022 536f  he.        # "So
+00007b40: 6674 7761 7265 2229 2c20 746f 2064 6561  ftware"), to dea
+00007b50: 6c20 696e 2074 6865 2053 6f66 7477 6172  l in the Softwar
+00007b60: 6520 7769 7468 6f75 7420 7265 7374 7269  e without restri
+00007b70: 6374 696f 6e2c 2069 6e63 6c75 6469 6e67  ction, including
+00007b80: 0a20 2020 2020 2020 2023 2077 6974 686f  .        # witho
+00007b90: 7574 206c 696d 6974 6174 696f 6e20 7468  ut limitation th
+00007ba0: 6520 7269 6768 7473 2074 6f20 7573 652c  e rights to use,
+00007bb0: 2063 6f70 792c 206d 6f64 6966 792c 206d   copy, modify, m
+00007bc0: 6572 6765 2c20 7075 626c 6973 682c 0a20  erge, publish,. 
+00007bd0: 2020 2020 2020 2023 2064 6973 7472 6962         # distrib
+00007be0: 7574 652c 2073 7562 6c69 6365 6e73 652c  ute, sublicense,
+00007bf0: 2061 6e64 2f6f 7220 7365 6c6c 2063 6f70   and/or sell cop
+00007c00: 6965 7320 6f66 2074 6865 2053 6f66 7477  ies of the Softw
+00007c10: 6172 652c 2061 6e64 2074 6f0a 2020 2020  are, and to.    
+00007c20: 2020 2020 2320 7065 726d 6974 2070 6572      # permit per
+00007c30: 736f 6e73 2074 6f20 7768 6f6d 2074 6865  sons to whom the
+00007c40: 2053 6f66 7477 6172 6520 6973 2066 7572   Software is fur
+00007c50: 6e69 7368 6564 2074 6f20 646f 2073 6f2c  nished to do so,
+00007c60: 2073 7562 6a65 6374 2074 6f0a 2020 2020   subject to.    
+00007c70: 2020 2020 2320 7468 6520 666f 6c6c 6f77      # the follow
+00007c80: 696e 6720 636f 6e64 6974 696f 6e73 3a0a  ing conditions:.
+00007c90: 2020 2020 2020 2020 2320 5468 6520 6162          # The ab
+00007ca0: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
+00007cb0: 7469 6365 2061 6e64 2074 6869 7320 7065  tice and this pe
+00007cc0: 726d 6973 7369 6f6e 206e 6f74 6963 6520  rmission notice 
+00007cd0: 7368 616c 6c20 6265 2069 6e63 6c75 6465  shall be include
+00007ce0: 640a 2020 2020 2020 2020 2320 696e 2061  d.        # in a
+00007cf0: 6c6c 2063 6f70 6965 7320 6f72 2073 7562  ll copies or sub
+00007d00: 7374 616e 7469 616c 2070 6f72 7469 6f6e  stantial portion
+00007d10: 7320 6f66 2074 6865 2053 6f66 7477 6172  s of the Softwar
+00007d20: 652e 0a20 2020 2020 2020 2023 2054 4845  e..        # THE
+00007d30: 2053 4f46 5457 4152 4520 4953 2050 524f   SOFTWARE IS PRO
+00007d40: 5649 4445 4420 2241 5320 4953 222c 2057  VIDED "AS IS", W
+00007d50: 4954 484f 5554 2057 4152 5241 4e54 5920  ITHOUT WARRANTY 
+00007d60: 4f46 2041 4e59 204b 494e 442c 2045 5850  OF ANY KIND, EXP
+00007d70: 5245 5353 0a20 2020 2020 2020 2023 204f  RESS.        # O
+00007d80: 5220 494d 504c 4945 442c 2049 4e43 4c55  R IMPLIED, INCLU
+00007d90: 4449 4e47 2042 5554 204e 4f54 204c 494d  DING BUT NOT LIM
+00007da0: 4954 4544 2054 4f20 5448 4520 5741 5252  ITED TO THE WARR
+00007db0: 414e 5449 4553 204f 460a 2020 2020 2020  ANTIES OF.      
+00007dc0: 2020 2320 4d45 5243 4841 4e54 4142 494c    # MERCHANTABIL
+00007dd0: 4954 592c 2046 4954 4e45 5353 2046 4f52  ITY, FITNESS FOR
+00007de0: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
+00007df0: 5250 4f53 4520 414e 4420 4e4f 4e49 4e46  RPOSE AND NONINF
+00007e00: 5249 4e47 454d 454e 542e 0a20 2020 2020  RINGEMENT..     
+00007e10: 2020 2023 2049 4e20 4e4f 2045 5645 4e54     # IN NO EVENT
+00007e20: 2053 4841 4c4c 2054 4845 2041 5554 484f   SHALL THE AUTHO
+00007e30: 5253 204f 5220 434f 5059 5249 4748 5420  RS OR COPYRIGHT 
+00007e40: 484f 4c44 4552 5320 4245 204c 4941 424c  HOLDERS BE LIABL
+00007e50: 4520 464f 5220 414e 590a 2020 2020 2020  E FOR ANY.      
+00007e60: 2020 2320 434c 4149 4d2c 2044 414d 4147    # CLAIM, DAMAG
+00007e70: 4553 204f 5220 4f54 4845 5220 4c49 4142  ES OR OTHER LIAB
+00007e80: 494c 4954 592c 2057 4845 5448 4552 2049  ILITY, WHETHER I
+00007e90: 4e20 414e 2041 4354 494f 4e20 4f46 2043  N AN ACTION OF C
+00007ea0: 4f4e 5452 4143 542c 0a20 2020 2020 2020  ONTRACT,.       
+00007eb0: 2023 2054 4f52 5420 4f52 204f 5448 4552   # TORT OR OTHER
+00007ec0: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
+00007ed0: 4f4d 2c20 4f55 5420 4f46 204f 5220 494e  OM, OUT OF OR IN
+00007ee0: 2043 4f4e 4e45 4354 494f 4e20 5749 5448   CONNECTION WITH
+00007ef0: 2054 4845 0a20 2020 2020 2020 2023 2053   THE.        # S
+00007f00: 4f46 5457 4152 4520 4f52 2054 4845 2055  OFTWARE OR THE U
+00007f10: 5345 204f 5220 4f54 4845 5220 4445 414c  SE OR OTHER DEAL
+00007f20: 494e 4753 2049 4e20 5448 4520 534f 4654  INGS IN THE SOFT
+00007f30: 5741 5245 2e0a 2020 2020 2020 2020 2320  WARE..        # 
+00007f40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007f50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007f60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007f70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007f80: 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020 2020  =========..     
+00007f90: 2020 2028 6874 7470 733a 2f2f 6769 7468     (https://gith
+00007fa0: 7562 2e63 6f6d 2f68 6572 726d 616e 6e6c  ub.com/herrmannl
+00007fb0: 6162 2f68 6967 6864 6963 6f6d 2f69 7373  ab/highdicom/iss
+00007fc0: 7565 732f 3138 3829 0a0a 2020 2020 2020  ues/188)..      
+00007fd0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00007fe0: 2020 2020 696d 673a 2061 2050 7964 6963      img: a Pydic
+00007ff0: 6f6d 2064 6174 6173 6574 206f 626a 6563  om dataset objec
+00008000: 7420 7468 6174 2068 6173 2061 7474 7269  t that has attri
+00008010: 6275 7465 2022 5365 676d 656e 7453 6571  bute "SegmentSeq
+00008020: 7565 6e63 6522 2e0a 0a20 2020 2020 2020  uence"...       
+00008030: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+00008040: 206e 6f74 2068 6173 6174 7472 2869 6d67   not hasattr(img
+00008050: 2c20 2250 6572 4672 616d 6546 756e 6374  , "PerFrameFunct
+00008060: 696f 6e61 6c47 726f 7570 7353 6571 7565  ionalGroupsSeque
+00008070: 6e63 6522 293a 0a20 2020 2020 2020 2020  nce"):.         
+00008080: 2020 2072 6169 7365 204e 6f74 496d 706c     raise NotImpl
+00008090: 656d 656e 7465 6445 7272 6f72 280a 2020  ementedError(.  
+000080a0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000080b0: 546f 2072 6561 6420 6469 636f 6d20 7365  To read dicom se
+000080c0: 673a 207b 696d 672e 6669 6c65 6e61 6d65  g: {img.filename
+000080d0: 7d2c 2027 5065 7246 7261 6d65 4675 6e63  }, 'PerFrameFunc
+000080e0: 7469 6f6e 616c 4772 6f75 7073 5365 7175  tionalGroupsSequ
+000080f0: 656e 6365 2720 6973 2072 6571 7569 7265  ence' is require
+00008100: 642e 220a 2020 2020 2020 2020 2020 2020  d.".            
+00008110: 290a 0a20 2020 2020 2020 2066 7261 6d65  )..        frame
+00008120: 5f73 6567 5f6e 756d 7320 3d20 5b5d 0a20  _seg_nums = []. 
+00008130: 2020 2020 2020 2066 6f72 2066 2069 6e20         for f in 
+00008140: 696d 672e 5065 7246 7261 6d65 4675 6e63  img.PerFrameFunc
+00008150: 7469 6f6e 616c 4772 6f75 7073 5365 7175  tionalGroupsSequ
+00008160: 656e 6365 3a0a 2020 2020 2020 2020 2020  ence:.          
+00008170: 2020 6966 206e 6f74 2068 6173 6174 7472    if not hasattr
+00008180: 2866 2c20 2253 6567 6d65 6e74 4964 656e  (f, "SegmentIden
+00008190: 7469 6669 6361 7469 6f6e 5365 7175 656e  tificationSequen
 000081a0: 6365 2229 3a0a 2020 2020 2020 2020 2020  ce"):.          
-000081b0: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
-000081c0: 6d65 6e74 6564 4572 726f 7228 0a20 2020  mentedError(.   
-000081d0: 2020 2020 2020 2020 2020 2020 2066 2254               f"T
-000081e0: 6f20 7265 6164 2064 6963 6f6d 2073 6567  o read dicom seg
-000081f0: 3a20 7b69 6d67 2e66 696c 656e 616d 657d  : {img.filename}
-00008200: 2c20 2750 6572 4672 616d 6546 756e 6374  , 'PerFrameFunct
-00008210: 696f 6e61 6c47 726f 7570 7353 6571 7565  ionalGroupsSeque
-00008220: 6e63 6527 2069 7320 7265 7175 6972 6564  nce' is required
-00008230: 2e22 0a20 2020 2020 2020 2020 2020 2029  .".            )
-00008240: 0a0a 2020 2020 2020 2020 6672 616d 655f  ..        frame_
-00008250: 7365 675f 6e75 6d73 203d 205b 5d0a 2020  seg_nums = [].  
-00008260: 2020 2020 2020 666f 7220 6620 696e 2069        for f in i
-00008270: 6d67 2e50 6572 4672 616d 6546 756e 6374  mg.PerFrameFunct
-00008280: 696f 6e61 6c47 726f 7570 7353 6571 7565  ionalGroupsSeque
-00008290: 6e63 653a 0a20 2020 2020 2020 2020 2020  nce:.           
-000082a0: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
-000082b0: 662c 2022 5365 676d 656e 7449 6465 6e74  f, "SegmentIdent
-000082c0: 6966 6963 6174 696f 6e53 6571 7565 6e63  ificationSequenc
-000082d0: 6522 293a 0a20 2020 2020 2020 2020 2020  e"):.           
-000082e0: 2020 2020 2072 6169 7365 204e 6f74 496d       raise NotIm
-000082f0: 706c 656d 656e 7465 6445 7272 6f72 280a  plementedError(.
-00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008310: 2020 2020 6622 546f 2072 6561 6420 6469      f"To read di
-00008320: 636f 6d20 7365 673a 207b 696d 672e 6669  com seg: {img.fi
-00008330: 6c65 6e61 6d65 7d2c 2027 5365 676d 656e  lename}, 'Segmen
-00008340: 7449 6465 6e74 6966 6963 6174 696f 6e53  tIdentificationS
-00008350: 6571 7565 6e63 6527 2069 7320 7265 7175  equence' is requ
-00008360: 6972 6564 2066 6f72 2065 6163 6820 6672  ired for each fr
-00008370: 616d 652e 220a 2020 2020 2020 2020 2020  ame.".          
-00008380: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00008390: 2020 2020 6672 616d 655f 7365 675f 6e75      frame_seg_nu
-000083a0: 6d73 2e61 7070 656e 6428 696e 7428 662e  ms.append(int(f.
-000083b0: 5365 676d 656e 7449 6465 6e74 6966 6963  SegmentIdentific
-000083c0: 6174 696f 6e53 6571 7565 6e63 655b 305d  ationSequence[0]
-000083d0: 2e52 6566 6572 656e 6365 6453 6567 6d65  .ReferencedSegme
-000083e0: 6e74 4e75 6d62 6572 2929 0a0a 2020 2020  ntNumber))..    
-000083f0: 2020 2020 6672 616d 655f 7365 675f 6e75      frame_seg_nu
-00008400: 6d73 5f61 7272 203d 206e 702e 6172 7261  ms_arr = np.arra
-00008410: 7928 6672 616d 655f 7365 675f 6e75 6d73  y(frame_seg_nums
-00008420: 290a 0a20 2020 2020 2020 2073 6567 5f64  )..        seg_d
-00008430: 6573 6372 6970 7469 6f6e 7320 3d20 7b69  escriptions = {i
-00008440: 6e74 2866 2e53 6567 6d65 6e74 4e75 6d62  nt(f.SegmentNumb
-00008450: 6572 293a 2066 2066 6f72 2066 2069 6e20  er): f for f in 
-00008460: 696d 672e 5365 676d 656e 7453 6571 7565  img.SegmentSeque
-00008470: 6e63 657d 0a0a 2020 2020 2020 2020 666f  nce}..        fo
-00008480: 7220 6920 696e 206e 702e 756e 6971 7565  r i in np.unique
-00008490: 2866 7261 6d65 5f73 6567 5f6e 756d 735f  (frame_seg_nums_
-000084a0: 6172 7229 3a0a 2020 2020 2020 2020 2020  arr):.          
-000084b0: 2020 696e 6469 6365 7320 3d20 6e70 2e77    indices = np.w
-000084c0: 6865 7265 2866 7261 6d65 5f73 6567 5f6e  here(frame_seg_n
-000084d0: 756d 735f 6172 7220 3d3d 2069 295b 305d  ums_arr == i)[0]
-000084e0: 0a20 2020 2020 2020 2020 2020 2079 6965  .            yie
-000084f0: 6c64 2028 696d 672e 7069 7865 6c5f 6172  ld (img.pixel_ar
-00008500: 7261 795b 696e 6469 6365 732c 202e 2e2e  ray[indices, ...
-00008510: 5d2c 2073 6567 5f64 6573 6372 6970 7469  ], seg_descripti
-00008520: 6f6e 735b 695d 290a 0a20 2020 2064 6566  ons[i])..    def
-00008530: 205f 6765 745f 7365 675f 6461 7461 2873   _get_seg_data(s
-00008540: 656c 662c 2069 6d67 293a 0a20 2020 2020  elf, img):.     
-00008550: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00008560: 6574 2074 6865 2061 7272 6179 2064 6174  et the array dat
-00008570: 6120 616e 6420 6d65 7461 6461 7461 206f  a and metadata o
-00008580: 6620 7468 6520 7365 676d 656e 7461 7469  f the segmentati
-00008590: 6f6e 2069 6d61 6765 2e0a 0a20 2020 2020  on image...     
-000085a0: 2020 2041 6567 733a 0a20 2020 2020 2020     Aegs:.       
-000085b0: 2020 2020 2069 6d67 3a20 6120 5079 6469       img: a Pydi
-000085c0: 636f 6d20 6461 7461 7365 7420 6f62 6a65  com dataset obje
-000085d0: 6374 2074 6861 7420 6861 7320 6174 7472  ct that has attr
-000085e0: 6962 7574 6520 2253 6567 6d65 6e74 5365  ibute "SegmentSe
-000085f0: 7175 656e 6365 222e 0a0a 2020 2020 2020  quence"...      
-00008600: 2020 2222 220a 0a20 2020 2020 2020 206d    """..        m
-00008610: 6574 6164 6174 6120 3d20 7365 6c66 2e5f  etadata = self._
-00008620: 6765 745f 6d65 7461 5f64 6963 7428 696d  get_meta_dict(im
-00008630: 6729 0a20 2020 2020 2020 206e 5f63 6c61  g).        n_cla
-00008640: 7373 6573 203d 206c 656e 2869 6d67 2e53  sses = len(img.S
-00008650: 6567 6d65 6e74 5365 7175 656e 6365 290a  egmentSequence).
-00008660: 2020 2020 2020 2020 7370 6174 6961 6c5f          spatial_
-00008670: 7368 6170 6520 3d20 6c69 7374 2869 6d67  shape = list(img
-00008680: 2e70 6978 656c 5f61 7272 6179 2e73 6861  .pixel_array.sha
-00008690: 7065 290a 2020 2020 2020 2020 7370 6174  pe).        spat
-000086a0: 6961 6c5f 7368 6170 655b 305d 203d 2073  ial_shape[0] = s
-000086b0: 7061 7469 616c 5f73 6861 7065 5b30 5d20  patial_shape[0] 
-000086c0: 2f2f 206e 5f63 6c61 7373 6573 0a0a 2020  // n_classes..  
-000086d0: 2020 2020 2020 6966 2073 656c 662e 6c61        if self.la
-000086e0: 6265 6c5f 6469 6374 2069 7320 6e6f 7420  bel_dict is not 
-000086f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00008700: 2020 6d65 7461 6461 7461 5b22 6c61 6265    metadata["labe
-00008710: 6c73 225d 203d 2073 656c 662e 6c61 6265  ls"] = self.labe
-00008720: 6c5f 6469 6374 0a20 2020 2020 2020 2020  l_dict.         
-00008730: 2020 2061 6c6c 5f73 6567 7320 3d20 6e70     all_segs = np
-00008740: 2e7a 6572 6f73 285b 2a73 7061 7469 616c  .zeros([*spatial
-00008750: 5f73 6861 7065 2c20 6c65 6e28 7365 6c66  _shape, len(self
-00008760: 2e6c 6162 656c 5f64 6963 7429 5d29 0a20  .label_dict)]). 
-00008770: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00008780: 2020 2020 2020 2020 206d 6574 6164 6174           metadat
-00008790: 615b 226c 6162 656c 7322 5d20 3d20 7b7d  a["labels"] = {}
-000087a0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-000087b0: 5f73 6567 7320 3d20 6e70 2e7a 6572 6f73  _segs = np.zeros
-000087c0: 285b 2a73 7061 7469 616c 5f73 6861 7065  ([*spatial_shape
-000087d0: 2c20 6e5f 636c 6173 7365 735d 290a 0a20  , n_classes]).. 
-000087e0: 2020 2020 2020 2066 6f72 2069 2c20 2866         for i, (f
-000087f0: 7261 6d65 732c 2064 6573 6372 6970 7469  rames, descripti
-00008800: 6f6e 2920 696e 2065 6e75 6d65 7261 7465  on) in enumerate
-00008810: 2873 656c 662e 5f67 6574 5f66 7261 6d65  (self._get_frame
-00008820: 5f64 6174 6128 696d 6729 293a 0a20 2020  _data(img)):.   
-00008830: 2020 2020 2020 2020 2063 6c61 7373 5f6e           class_n
-00008840: 616d 6520 3d20 6465 7363 7269 7074 696f  ame = descriptio
-00008850: 6e2e 5365 676d 656e 7444 6573 6372 6970  n.SegmentDescrip
-00008860: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00008870: 2069 6620 636c 6173 735f 6e61 6d65 206e   if class_name n
-00008880: 6f74 2069 6e20 6d65 7461 6461 7461 5b22  ot in metadata["
-00008890: 6c61 6265 6c73 225d 2e6b 6579 7328 293a  labels"].keys():
-000088a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088b0: 206d 6574 6164 6174 615b 226c 6162 656c   metadata["label
-000088c0: 7322 5d5b 636c 6173 735f 6e61 6d65 5d20  s"][class_name] 
-000088d0: 3d20 690a 2020 2020 2020 2020 2020 2020  = i.            
-000088e0: 636c 6173 735f 6e75 6d20 3d20 6d65 7461  class_num = meta
-000088f0: 6461 7461 5b22 6c61 6265 6c73 225d 5b63  data["labels"][c
-00008900: 6c61 7373 5f6e 616d 655d 0a20 2020 2020  lass_name].     
-00008910: 2020 2020 2020 2061 6c6c 5f73 6567 735b         all_segs[
-00008920: 2e2e 2e2c 2063 6c61 7373 5f6e 756d 5d20  ..., class_num] 
-00008930: 3d20 6672 616d 6573 0a0a 2020 2020 2020  = frames..      
-00008940: 2020 616c 6c5f 7365 6773 203d 2061 6c6c    all_segs = all
-00008950: 5f73 6567 732e 7472 616e 7370 6f73 6528  _segs.transpose(
-00008960: 5b31 2c20 322c 2030 2c20 335d 290a 2020  [1, 2, 0, 3]).  
-00008970: 2020 2020 2020 6d65 7461 6461 7461 5b4d        metadata[M
-00008980: 6574 614b 6579 732e 5350 4154 4941 4c5f  etaKeys.SPATIAL_
-00008990: 5348 4150 455d 203d 2061 6c6c 5f73 6567  SHAPE] = all_seg
-000089a0: 732e 7368 6170 655b 3a2d 315d 0a0a 2020  s.shape[:-1]..  
-000089b0: 2020 2020 2020 6966 2022 3532 3030 3932        if "520092
-000089c0: 3239 2220 696e 206d 6574 6164 6174 612e  29" in metadata.
-000089d0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
-000089e0: 2020 2020 7368 6172 6564 5f66 756e 635f      shared_func_
-000089f0: 6772 6f75 705f 7365 7120 3d20 6d65 7461  group_seq = meta
-00008a00: 6461 7461 5b22 3532 3030 3932 3239 225d  data["52009229"]
-00008a10: 5b22 5661 6c75 6522 5d5b 305d 0a0a 2020  ["Value"][0]..  
-00008a20: 2020 2020 2020 2020 2020 2320 6765 7420            # get 
-00008a30: 6049 6d61 6765 4f72 6965 6e74 6174 696f  `ImageOrientatio
-00008a40: 6e50 6174 6965 6e74 600a 2020 2020 2020  nPatient`.      
-00008a50: 2020 2020 2020 6966 2022 3030 3230 3931        if "002091
-00008a60: 3136 2220 696e 2073 6861 7265 645f 6675  16" in shared_fu
-00008a70: 6e63 5f67 726f 7570 5f73 6571 2e6b 6579  nc_group_seq.key
-00008a80: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00008a90: 2020 2020 2070 6c61 6e65 5f6f 7269 656e       plane_orien
-00008aa0: 745f 7365 7120 3d20 7368 6172 6564 5f66  t_seq = shared_f
-00008ab0: 756e 635f 6772 6f75 705f 7365 715b 2230  unc_group_seq["0
-00008ac0: 3032 3039 3131 3622 5d5b 2256 616c 7565  0209116"]["Value
-00008ad0: 225d 5b30 5d0a 2020 2020 2020 2020 2020  "][0].          
-00008ae0: 2020 2020 2020 6966 2022 3030 3230 3030        if "002000
-00008af0: 3337 2220 696e 2070 6c61 6e65 5f6f 7269  37" in plane_ori
-00008b00: 656e 745f 7365 712e 6b65 7973 2829 3a0a  ent_seq.keys():.
-00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b20: 2020 2020 6d65 7461 6461 7461 5b22 3030      metadata["00
-00008b30: 3230 3030 3337 225d 203d 2070 6c61 6e65  200037"] = plane
-00008b40: 5f6f 7269 656e 745f 7365 715b 2230 3032  _orient_seq["002
-00008b50: 3030 3033 3722 5d0a 0a20 2020 2020 2020  00037"]..       
-00008b60: 2020 2020 2023 2067 6574 2060 5069 7865       # get `Pixe
-00008b70: 6c53 7061 6369 6e67 600a 2020 2020 2020  lSpacing`.      
-00008b80: 2020 2020 2020 6966 2022 3030 3238 3931        if "002891
-00008b90: 3130 2220 696e 2073 6861 7265 645f 6675  10" in shared_fu
-00008ba0: 6e63 5f67 726f 7570 5f73 6571 2e6b 6579  nc_group_seq.key
-00008bb0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00008bc0: 2020 2020 2070 6978 656c 5f6d 6561 7375       pixel_measu
-00008bd0: 7265 5f73 6571 203d 2073 6861 7265 645f  re_seq = shared_
-00008be0: 6675 6e63 5f67 726f 7570 5f73 6571 5b22  func_group_seq["
-00008bf0: 3030 3238 3931 3130 225d 5b22 5661 6c75  00289110"]["Valu
-00008c00: 6522 5d5b 305d 0a0a 2020 2020 2020 2020  e"][0]..        
-00008c10: 2020 2020 2020 2020 6966 2022 3030 3238          if "0028
-00008c20: 3030 3330 2220 696e 2070 6978 656c 5f6d  0030" in pixel_m
-00008c30: 6561 7375 7265 5f73 6571 2e6b 6579 7328  easure_seq.keys(
-00008c40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008c50: 2020 2020 2020 2070 6978 656c 5f73 7061         pixel_spa
-00008c60: 6369 6e67 203d 2070 6978 656c 5f6d 6561  cing = pixel_mea
-00008c70: 7375 7265 5f73 6571 5b22 3030 3238 3030  sure_seq["002800
-00008c80: 3330 225d 5b22 5661 6c75 6522 5d0a 2020  30"]["Value"].  
-00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ca0: 2020 6d65 7461 6461 7461 5b22 7370 6163    metadata["spac
-00008cb0: 696e 6722 5d20 3d20 7069 7865 6c5f 7370  ing"] = pixel_sp
-00008cc0: 6163 696e 670a 2020 2020 2020 2020 2020  acing.          
-00008cd0: 2020 2020 2020 2020 2020 6966 2022 3030            if "00
-00008ce0: 3138 3030 3530 2220 696e 2070 6978 656c  180050" in pixel
-00008cf0: 5f6d 6561 7375 7265 5f73 6571 2e6b 6579  _measure_seq.key
-00008d00: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00008d10: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00008d20: 6164 6174 615b 2273 7061 6369 6e67 225d  adata["spacing"]
-00008d30: 202b 3d20 7069 7865 6c5f 6d65 6173 7572   += pixel_measur
-00008d40: 655f 7365 715b 2230 3031 3830 3035 3022  e_seq["00180050"
-00008d50: 5d5b 2256 616c 7565 225d 0a0a 2020 2020  ]["Value"]..    
-00008d60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00008d70: 7072 756e 655f 6d65 7461 6461 7461 3a0a  prune_metadata:.
-00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 6d65 7461 6461 7461 2e70 6f70 2822 3532  metadata.pop("52
-00008da0: 3030 3932 3239 2229 0a0a 2020 2020 2020  009229")..      
-00008db0: 2020 2320 6765 7420 6049 6d61 6765 506f    # get `ImagePo
-00008dc0: 7369 7469 6f6e 5061 7469 656e 7460 0a20  sitionPatient`. 
-00008dd0: 2020 2020 2020 2069 6620 2235 3230 3039         if "52009
-00008de0: 3233 3022 2069 6e20 6d65 7461 6461 7461  230" in metadata
-00008df0: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
-00008e00: 2020 2020 2066 6972 7374 5f66 7261 6d65       first_frame
-00008e10: 5f66 756e 635f 6772 6f75 705f 7365 7120  _func_group_seq 
-00008e20: 3d20 6d65 7461 6461 7461 5b22 3532 3030  = metadata["5200
-00008e30: 3932 3330 225d 5b22 5661 6c75 6522 5d5b  9230"]["Value"][
-00008e40: 305d 0a20 2020 2020 2020 2020 2020 2069  0].            i
-00008e50: 6620 2230 3032 3039 3131 3322 2069 6e20  f "00209113" in 
-00008e60: 6669 7273 745f 6672 616d 655f 6675 6e63  first_frame_func
-00008e70: 5f67 726f 7570 5f73 6571 2e6b 6579 7328  _group_seq.keys(
-00008e80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008e90: 2020 2070 6c61 6e65 5f70 6f73 6974 696f     plane_positio
-00008ea0: 6e5f 7365 7120 3d20 6669 7273 745f 6672  n_seq = first_fr
-00008eb0: 616d 655f 6675 6e63 5f67 726f 7570 5f73  ame_func_group_s
-00008ec0: 6571 5b22 3030 3230 3931 3133 225d 5b22  eq["00209113"]["
-00008ed0: 5661 6c75 6522 5d5b 305d 0a20 2020 2020  Value"][0].     
-00008ee0: 2020 2020 2020 2020 2020 2069 6620 2230             if "0
-00008ef0: 3032 3030 3033 3222 2069 6e20 706c 616e  0200032" in plan
-00008f00: 655f 706f 7369 7469 6f6e 5f73 6571 2e6b  e_position_seq.k
-00008f10: 6579 7328 293a 0a20 2020 2020 2020 2020  eys():.         
-00008f20: 2020 2020 2020 2020 2020 206d 6574 6164             metad
-00008f30: 6174 615b 2230 3032 3030 3033 3222 5d20  ata["00200032"] 
-00008f40: 3d20 706c 616e 655f 706f 7369 7469 6f6e  = plane_position
-00008f50: 5f73 6571 5b22 3030 3230 3030 3332 225d  _seq["00200032"]
-00008f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008f70: 2020 2020 206d 6574 6164 6174 615b 226c       metadata["l
-00008f80: 6173 7449 6d61 6765 506f 7369 7469 6f6e  astImagePosition
-00008f90: 5061 7469 656e 7422 5d20 3d20 6d65 7461  Patient"] = meta
-00008fa0: 6461 7461 5b22 3532 3030 3932 3330 225d  data["52009230"]
-00008fb0: 5b22 5661 6c75 6522 5d5b 2d31 5d5b 2230  ["Value"][-1]["0
-00008fc0: 3032 3039 3131 3322 5d5b 2256 616c 7565  0209113"]["Value
-00008fd0: 225d 5b30 5d5b 0a20 2020 2020 2020 2020  "][0][.         
-00008fe0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00008ff0: 3030 3230 3030 3332 220a 2020 2020 2020  00200032".      
-00009000: 2020 2020 2020 2020 2020 2020 2020 5d5b                ][
-00009010: 2256 616c 7565 225d 0a20 2020 2020 2020  "Value"].       
-00009020: 2020 2020 2069 6620 7365 6c66 2e70 7275       if self.pru
-00009030: 6e65 5f6d 6574 6164 6174 613a 0a20 2020  ne_metadata:.   
-00009040: 2020 2020 2020 2020 2020 2020 206d 6574               met
-00009050: 6164 6174 612e 706f 7028 2235 3230 3039  adata.pop("52009
-00009060: 3233 3022 290a 0a20 2020 2020 2020 2072  230")..        r
-00009070: 6574 7572 6e20 616c 6c5f 7365 6773 2c20  eturn all_segs, 
-00009080: 6d65 7461 6461 7461 0a0a 2020 2020 6465  metadata..    de
-00009090: 6620 5f67 6574 5f61 7272 6179 5f64 6174  f _get_array_dat
-000090a0: 6128 7365 6c66 2c20 696d 6729 3a0a 2020  a(self, img):.  
-000090b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000090c0: 2020 4765 7420 7468 6520 6172 7261 7920    Get the array 
-000090d0: 6461 7461 206f 6620 7468 6520 696d 6167  data of the imag
-000090e0: 652e 2049 6620 6052 6573 6361 6c65 536c  e. If `RescaleSl
-000090f0: 6f70 6560 2061 6e64 2060 5265 7363 616c  ope` and `Rescal
-00009100: 6549 6e74 6572 6365 7074 6020 6172 6520  eIntercept` are 
-00009110: 6176 6169 6c61 626c 652c 2074 6865 2072  available, the r
-00009120: 6177 2061 7272 6179 2064 6174 610a 2020  aw array data.  
-00009130: 2020 2020 2020 7769 6c6c 2062 6520 7265        will be re
-00009140: 7363 616c 6564 2e20 5468 6520 6f75 7470  scaled. The outp
-00009150: 7574 2064 6174 6120 6861 7320 7468 6520  ut data has the 
-00009160: 6474 7970 6520 6e70 2e66 6c6f 6174 3332  dtype np.float32
-00009170: 2069 6620 7468 6520 7265 7363 616c 696e   if the rescalin
-00009180: 6720 6973 2061 7070 6c69 6564 2e0a 0a20  g is applied... 
-00009190: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000091a0: 2020 2020 2020 2020 2069 6d67 3a20 6120           img: a 
-000091b0: 5079 6469 636f 6d20 6461 7461 7365 7420  Pydicom dataset 
-000091c0: 6f62 6a65 6374 2e0a 0a20 2020 2020 2020  object...       
-000091d0: 2022 2222 0a20 2020 2020 2020 2023 2070   """.        # p
-000091e0: 726f 6365 7373 2044 6963 6f6d 2073 6572  rocess Dicom ser
-000091f0: 6965 730a 2020 2020 2020 2020 6966 206e  ies.        if n
-00009200: 6f74 2068 6173 6174 7472 2869 6d67 2c20  ot hasattr(img, 
-00009210: 2270 6978 656c 5f61 7272 6179 2229 3a0a  "pixel_array"):.
-00009220: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00009230: 6520 5661 6c75 6545 7272 6f72 2866 2264  e ValueError(f"d
-00009240: 6963 6f6d 2064 6174 613a 207b 696d 672e  icom data: {img.
-00009250: 6669 6c65 6e61 6d65 7d20 646f 6573 206e  filename} does n
-00009260: 6f74 2068 6176 6520 7069 7865 6c5f 6172  ot have pixel_ar
-00009270: 7261 792e 2229 0a20 2020 2020 2020 2064  ray.").        d
-00009280: 6174 6120 3d20 696d 672e 7069 7865 6c5f  ata = img.pixel_
-00009290: 6172 7261 790a 0a20 2020 2020 2020 2073  array..        s
-000092a0: 6c6f 7065 2c20 6f66 6673 6574 203d 2031  lope, offset = 1
-000092b0: 2e30 2c20 302e 300a 2020 2020 2020 2020  .0, 0.0.        
-000092c0: 7265 7363 616c 655f 666c 6167 203d 2046  rescale_flag = F
-000092d0: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
-000092e0: 6861 7361 7474 7228 696d 672c 2022 5265  hasattr(img, "Re
-000092f0: 7363 616c 6553 6c6f 7065 2229 3a0a 2020  scaleSlope"):.  
-00009300: 2020 2020 2020 2020 2020 736c 6f70 6520            slope 
-00009310: 3d20 696d 672e 5265 7363 616c 6553 6c6f  = img.RescaleSlo
-00009320: 7065 0a20 2020 2020 2020 2020 2020 2072  pe.            r
-00009330: 6573 6361 6c65 5f66 6c61 6720 3d20 5472  escale_flag = Tr
-00009340: 7565 0a20 2020 2020 2020 2069 6620 6861  ue.        if ha
-00009350: 7361 7474 7228 696d 672c 2022 5265 7363  sattr(img, "Resc
-00009360: 616c 6549 6e74 6572 6365 7074 2229 3a0a  aleIntercept"):.
-00009370: 2020 2020 2020 2020 2020 2020 6f66 6673              offs
-00009380: 6574 203d 2069 6d67 2e52 6573 6361 6c65  et = img.Rescale
-00009390: 496e 7465 7263 6570 740a 2020 2020 2020  Intercept.      
-000093a0: 2020 2020 2020 7265 7363 616c 655f 666c        rescale_fl
-000093b0: 6167 203d 2054 7275 650a 2020 2020 2020  ag = True.      
-000093c0: 2020 6966 2072 6573 6361 6c65 5f66 6c61    if rescale_fla
-000093d0: 673a 0a20 2020 2020 2020 2020 2020 2064  g:.            d
-000093e0: 6174 6120 3d20 6461 7461 2e61 7374 7970  ata = data.astyp
-000093f0: 6528 6e70 2e66 6c6f 6174 3332 2920 2a20  e(np.float32) * 
-00009400: 736c 6f70 6520 2b20 6f66 6673 6574 0a0a  slope + offset..
-00009410: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00009420: 6174 610a 0a0a 4072 6571 7569 7265 5f70  ata...@require_p
-00009430: 6b67 2870 6b67 5f6e 616d 653d 226e 6962  kg(pkg_name="nib
-00009440: 6162 656c 2229 0a63 6c61 7373 204e 6962  abel").class Nib
-00009450: 6162 656c 5265 6164 6572 2849 6d61 6765  abelReader(Image
-00009460: 5265 6164 6572 293a 0a20 2020 2022 2222  Reader):.    """
-00009470: 0a20 2020 204c 6f61 6420 4e49 6654 4920  .    Load NIfTI 
-00009480: 666f 726d 6174 2069 6d61 6765 7320 6261  format images ba
-00009490: 7365 6420 6f6e 204e 6962 6162 656c 206c  sed on Nibabel l
-000094a0: 6962 7261 7279 2e0a 0a20 2020 2041 7267  ibrary...    Arg
-000094b0: 733a 0a20 2020 2020 2020 2061 735f 636c  s:.        as_cl
-000094c0: 6f73 6573 745f 6361 6e6f 6e69 6361 6c3a  osest_canonical:
-000094d0: 2069 6620 5472 7565 2c20 6c6f 6164 2074   if True, load t
-000094e0: 6865 2069 6d61 6765 2061 7320 636c 6f73  he image as clos
-000094f0: 6573 7420 746f 2063 616e 6f6e 6963 616c  est to canonical
-00009500: 2061 7869 7320 666f 726d 6174 2e0a 2020   axis format..  
-00009510: 2020 2020 2020 7371 7565 657a 655f 6e6f        squeeze_no
-00009520: 6e5f 7370 6174 6961 6c5f 6469 6d73 3a20  n_spatial_dims: 
-00009530: 6966 2054 7275 652c 206e 6f6e 2d73 7061  if True, non-spa
-00009540: 7469 616c 2073 696e 676c 6574 6f6e 7320  tial singletons 
-00009550: 7769 6c6c 2062 6520 7371 7565 657a 6564  will be squeezed
-00009560: 2c20 652e 672e 2028 3235 362c 3235 362c  , e.g. (256,256,
-00009570: 312c 3329 202d 3e20 2832 3536 2c32 3536  1,3) -> (256,256
-00009580: 2c33 290a 2020 2020 2020 2020 6368 616e  ,3).        chan
-00009590: 6e65 6c5f 6469 6d3a 2074 6865 2063 6861  nel_dim: the cha
-000095a0: 6e6e 656c 2064 696d 656e 7369 6f6e 206f  nnel dimension o
-000095b0: 6620 7468 6520 696e 7075 7420 696d 6167  f the input imag
-000095c0: 652c 2064 6566 6175 6c74 2069 7320 4e6f  e, default is No
-000095d0: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
-000095e0: 7468 6973 2069 7320 7573 6564 2074 6f20  this is used to 
-000095f0: 7365 7420 6f72 6967 696e 616c 5f63 6861  set original_cha
-00009600: 6e6e 656c 5f64 696d 2069 6e20 7468 6520  nnel_dim in the 
-00009610: 6d65 7461 6461 7461 2c20 456e 7375 7265  metadata, Ensure
-00009620: 4368 616e 6e65 6c46 6972 7374 4420 7265  ChannelFirstD re
-00009630: 6164 7320 7468 6973 2066 6965 6c64 2e0a  ads this field..
-00009640: 2020 2020 2020 2020 2020 2020 6966 204e              if N
-00009650: 6f6e 652c 2060 6f72 6967 696e 616c 5f63  one, `original_c
-00009660: 6861 6e6e 656c 5f64 696d 6020 7769 6c6c  hannel_dim` will
-00009670: 2062 6520 6569 7468 6572 2060 6e6f 5f63   be either `no_c
-00009680: 6861 6e6e 656c 6020 6f72 2060 2d31 602e  hannel` or `-1`.
-00009690: 0a20 2020 2020 2020 2020 2020 206d 6f73  .            mos
-000096a0: 7420 4e69 6674 6920 6669 6c65 7320 6172  t Nifti files ar
-000096b0: 6520 7573 7561 6c6c 7920 2263 6861 6e6e  e usually "chann
-000096c0: 656c 206c 6173 7422 2c20 6e6f 206e 6565  el last", no nee
-000096d0: 6420 746f 2073 7065 6369 6679 2074 6869  d to specify thi
-000096e0: 7320 6172 6775 6d65 6e74 2066 6f72 2074  s argument for t
-000096f0: 6865 6d2e 0a20 2020 2020 2020 206b 7761  hem..        kwa
-00009700: 7267 733a 2061 6464 6974 696f 6e61 6c20  rgs: additional 
-00009710: 6172 6773 2066 6f72 2060 6e69 6261 6265  args for `nibabe
-00009720: 6c2e 6c6f 6164 6020 4150 492e 206d 6f72  l.load` API. mor
-00009730: 6520 6465 7461 696c 7320 6162 6f75 7420  e details about 
-00009740: 6176 6169 6c61 626c 6520 6172 6773 3a0a  available args:.
-00009750: 2020 2020 2020 2020 2020 2020 6874 7470              http
-00009760: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6e  s://github.com/n
-00009770: 6970 792f 6e69 6261 6265 6c2f 626c 6f62  ipy/nibabel/blob
-00009780: 2f6d 6173 7465 722f 6e69 6261 6265 6c2f  /master/nibabel/
-00009790: 6c6f 6164 7361 7665 2e70 790a 0a20 2020  loadsave.py..   
-000097a0: 2022 2222 0a0a 2020 2020 4064 6570 7265   """..    @depre
-000097b0: 6361 7465 645f 6172 6728 2264 7479 7065  cated_arg("dtype
-000097c0: 222c 2073 696e 6365 3d22 312e 3022 2c20  ", since="1.0", 
-000097d0: 6d73 675f 7375 6666 6978 3d22 706c 6561  msg_suffix="plea
-000097e0: 7365 206d 6f64 6966 7920 6474 7970 6520  se modify dtype 
-000097f0: 6f66 2074 6865 2072 6574 7572 6e65 6420  of the returned 
-00009800: 6279 2060 6067 6574 5f64 6174 6160 6020  by ``get_data`` 
-00009810: 696e 7374 6561 642e 2229 0a20 2020 2064  instead.").    d
-00009820: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-00009830: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00009840: 2020 2063 6861 6e6e 656c 5f64 696d 3a20     channel_dim: 
-00009850: 7374 7220 7c20 696e 7420 7c20 4e6f 6e65  str | int | None
-00009860: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00009870: 2061 735f 636c 6f73 6573 745f 6361 6e6f   as_closest_cano
-00009880: 6e69 6361 6c3a 2062 6f6f 6c20 3d20 4661  nical: bool = Fa
-00009890: 6c73 652c 0a20 2020 2020 2020 2073 7175  lse,.        squ
-000098a0: 6565 7a65 5f6e 6f6e 5f73 7061 7469 616c  eeze_non_spatial
-000098b0: 5f64 696d 733a 2062 6f6f 6c20 3d20 4661  _dims: bool = Fa
-000098c0: 6c73 652c 0a20 2020 2020 2020 2064 7479  lse,.        dty
-000098d0: 7065 3a20 4474 7970 654c 696b 6520 3d20  pe: DtypeLike = 
-000098e0: 6e70 2e66 6c6f 6174 3332 2c0a 2020 2020  np.float32,.    
-000098f0: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
-00009900: 2020 293a 0a20 2020 2020 2020 2073 7570    ):.        sup
-00009910: 6572 2829 2e5f 5f69 6e69 745f 5f28 290a  er().__init__().
-00009920: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00009930: 6e6e 656c 5f64 696d 203d 2066 6c6f 6174  nnel_dim = float
-00009940: 2822 6e61 6e22 2920 6966 2063 6861 6e6e  ("nan") if chann
-00009950: 656c 5f64 696d 203d 3d20 226e 6f5f 6368  el_dim == "no_ch
-00009960: 616e 6e65 6c22 2065 6c73 6520 6368 616e  annel" else chan
-00009970: 6e65 6c5f 6469 6d0a 2020 2020 2020 2020  nel_dim.        
-00009980: 7365 6c66 2e61 735f 636c 6f73 6573 745f  self.as_closest_
-00009990: 6361 6e6f 6e69 6361 6c20 3d20 6173 5f63  canonical = as_c
-000099a0: 6c6f 7365 7374 5f63 616e 6f6e 6963 616c  losest_canonical
-000099b0: 0a20 2020 2020 2020 2073 656c 662e 7371  .        self.sq
-000099c0: 7565 657a 655f 6e6f 6e5f 7370 6174 6961  ueeze_non_spatia
-000099d0: 6c5f 6469 6d73 203d 2073 7175 6565 7a65  l_dims = squeeze
-000099e0: 5f6e 6f6e 5f73 7061 7469 616c 5f64 696d  _non_spatial_dim
-000099f0: 730a 2020 2020 2020 2020 7365 6c66 2e64  s.        self.d
-00009a00: 7479 7065 203d 2064 7479 7065 2020 2320  type = dtype  # 
-00009a10: 6465 7072 6563 6174 6564 0a20 2020 2020  deprecated.     
-00009a20: 2020 2073 656c 662e 6b77 6172 6773 203d     self.kwargs =
-00009a30: 206b 7761 7267 730a 0a20 2020 2064 6566   kwargs..    def
-00009a40: 2076 6572 6966 795f 7375 6666 6978 2873   verify_suffix(s
-00009a50: 656c 662c 2066 696c 656e 616d 653a 2053  elf, filename: S
-00009a60: 6571 7565 6e63 655b 5061 7468 4c69 6b65  equence[PathLike
-00009a70: 5d20 7c20 5061 7468 4c69 6b65 2920 2d3e  ] | PathLike) ->
-00009a80: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00009a90: 2222 0a20 2020 2020 2020 2056 6572 6966  "".        Verif
-00009aa0: 7920 7768 6574 6865 7220 7468 6520 7370  y whether the sp
-00009ab0: 6563 6966 6965 6420 6669 6c65 206f 7220  ecified file or 
-00009ac0: 6669 6c65 7320 666f 726d 6174 2069 7320  files format is 
-00009ad0: 7375 7070 6f72 7465 6420 6279 204e 6962  supported by Nib
-00009ae0: 6162 656c 2072 6561 6465 722e 0a0a 2020  abel reader...  
-00009af0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00009b00: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-00009b10: 3a20 6669 6c65 206e 616d 6520 6f72 2061  : file name or a
-00009b20: 206c 6973 7420 6f66 2066 696c 6520 6e61   list of file na
-00009b30: 6d65 7320 746f 2072 6561 642e 0a20 2020  mes to read..   
-00009b40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009b50: 6120 6c69 7374 206f 6620 6669 6c65 732c  a list of files,
-00009b60: 2076 6572 6966 7920 616c 6c20 7468 6520   verify all the 
-00009b70: 7375 6666 6978 6573 2e0a 0a20 2020 2020  suffixes...     
-00009b80: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00009b90: 7566 6669 7865 733a 2053 6571 7565 6e63  uffixes: Sequenc
-00009ba0: 655b 7374 725d 203d 205b 226e 6969 222c  e[str] = ["nii",
-00009bb0: 2022 6e69 692e 677a 225d 0a20 2020 2020   "nii.gz"].     
-00009bc0: 2020 2072 6574 7572 6e20 6861 735f 6e69     return has_ni
-00009bd0: 6220 616e 6420 6973 5f73 7570 706f 7274  b and is_support
-00009be0: 6564 5f66 6f72 6d61 7428 6669 6c65 6e61  ed_format(filena
-00009bf0: 6d65 2c20 7375 6666 6978 6573 290a 0a20  me, suffixes).. 
-00009c00: 2020 2064 6566 2072 6561 6428 7365 6c66     def read(self
-00009c10: 2c20 6461 7461 3a20 5365 7175 656e 6365  , data: Sequence
-00009c20: 5b50 6174 684c 696b 655d 207c 2050 6174  [PathLike] | Pat
-00009c30: 684c 696b 652c 202a 2a6b 7761 7267 7329  hLike, **kwargs)
-00009c40: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00009c50: 2020 2020 2020 5265 6164 2069 6d61 6765        Read image
-00009c60: 2064 6174 6120 6672 6f6d 2073 7065 6369   data from speci
-00009c70: 6669 6564 2066 696c 6520 6f72 2066 696c  fied file or fil
-00009c80: 6573 2c20 6974 2063 616e 2072 6561 6420  es, it can read 
-00009c90: 6120 6c69 7374 206f 6620 696d 6167 6573  a list of images
-00009ca0: 0a20 2020 2020 2020 2061 6e64 2073 7461  .        and sta
-00009cb0: 636b 2074 6865 6d20 746f 6765 7468 6572  ck them together
-00009cc0: 2061 7320 6d75 6c74 692d 6368 616e 6e65   as multi-channe
-00009cd0: 6c20 6461 7461 2069 6e20 6067 6574 5f64  l data in `get_d
-00009ce0: 6174 6128 2960 2e0a 2020 2020 2020 2020  ata()`..        
-00009cf0: 4e6f 7465 2074 6861 7420 7468 6520 7265  Note that the re
-00009d00: 7475 726e 6564 206f 626a 6563 7420 6973  turned object is
-00009d10: 204e 6962 6162 656c 2069 6d61 6765 206f   Nibabel image o
-00009d20: 626a 6563 7420 6f72 206c 6973 7420 6f66  bject or list of
-00009d30: 204e 6962 6162 656c 2069 6d61 6765 206f   Nibabel image o
-00009d40: 626a 6563 7473 2e0a 0a20 2020 2020 2020  bjects...       
-00009d50: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00009d60: 2020 2064 6174 613a 2066 696c 6520 6e61     data: file na
-00009d70: 6d65 206f 7220 6120 6c69 7374 206f 6620  me or a list of 
-00009d80: 6669 6c65 206e 616d 6573 2074 6f20 7265  file names to re
-00009d90: 6164 2e0a 2020 2020 2020 2020 2020 2020  ad..            
-00009da0: 6b77 6172 6773 3a20 6164 6469 7469 6f6e  kwargs: addition
-00009db0: 616c 2061 7267 7320 666f 7220 606e 6962  al args for `nib
-00009dc0: 6162 656c 2e6c 6f61 6460 2041 5049 2c20  abel.load` API, 
-00009dd0: 7769 6c6c 206f 7665 7272 6964 6520 6073  will override `s
-00009de0: 656c 662e 6b77 6172 6773 6020 666f 7220  elf.kwargs` for 
-00009df0: 6578 6973 7469 6e67 206b 6579 732e 0a20  existing keys.. 
-00009e00: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-00009e10: 6f72 6520 6465 7461 696c 7320 6162 6f75  ore details abou
-00009e20: 7420 6176 6169 6c61 626c 6520 6172 6773  t available args
-00009e30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009e40: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
-00009e50: 2e63 6f6d 2f6e 6970 792f 6e69 6261 6265  .com/nipy/nibabe
-00009e60: 6c2f 626c 6f62 2f6d 6173 7465 722f 6e69  l/blob/master/ni
-00009e70: 6261 6265 6c2f 6c6f 6164 7361 7665 2e70  babel/loadsave.p
-00009e80: 790a 0a20 2020 2020 2020 2022 2222 0a20  y..        """. 
-00009e90: 2020 2020 2020 2069 6d67 5f3a 206c 6973         img_: lis
-00009ea0: 745b 4e69 6674 6931 496d 6167 655d 203d  t[Nifti1Image] =
-00009eb0: 205b 5d0a 0a20 2020 2020 2020 2066 696c   []..        fil
-00009ec0: 656e 616d 6573 3a20 5365 7175 656e 6365  enames: Sequence
-00009ed0: 5b50 6174 684c 696b 655d 203d 2065 6e73  [PathLike] = ens
-00009ee0: 7572 655f 7475 706c 6528 6461 7461 290a  ure_tuple(data).
-00009ef0: 2020 2020 2020 2020 6b77 6172 6773 5f20          kwargs_ 
-00009f00: 3d20 7365 6c66 2e6b 7761 7267 732e 636f  = self.kwargs.co
-00009f10: 7079 2829 0a20 2020 2020 2020 206b 7761  py().        kwa
-00009f20: 7267 735f 2e75 7064 6174 6528 6b77 6172  rgs_.update(kwar
-00009f30: 6773 290a 2020 2020 2020 2020 666f 7220  gs).        for 
-00009f40: 6e61 6d65 2069 6e20 6669 6c65 6e61 6d65  name in filename
-00009f50: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00009f60: 6d67 203d 206e 6962 2e6c 6f61 6428 6e61  mg = nib.load(na
-00009f70: 6d65 2c20 2a2a 6b77 6172 6773 5f29 0a20  me, **kwargs_). 
-00009f80: 2020 2020 2020 2020 2020 2069 6d67 203d             img =
-00009f90: 2063 6f72 7265 6374 5f6e 6966 7469 5f68   correct_nifti_h
-00009fa0: 6561 6465 725f 6966 5f6e 6563 6573 7361  eader_if_necessa
-00009fb0: 7279 2869 6d67 290a 2020 2020 2020 2020  ry(img).        
-00009fc0: 2020 2020 696d 675f 2e61 7070 656e 6428      img_.append(
-00009fd0: 696d 6729 0a20 2020 2020 2020 2072 6574  img).        ret
-00009fe0: 7572 6e20 696d 675f 2069 6620 6c65 6e28  urn img_ if len(
-00009ff0: 6669 6c65 6e61 6d65 7329 203e 2031 2065  filenames) > 1 e
-0000a000: 6c73 6520 696d 675f 5b30 5d0a 0a20 2020  lse img_[0]..   
-0000a010: 2064 6566 2067 6574 5f64 6174 6128 7365   def get_data(se
-0000a020: 6c66 2c20 696d 6729 202d 3e20 7475 706c  lf, img) -> tupl
-0000a030: 655b 6e70 2e6e 6461 7272 6179 2c20 6469  e[np.ndarray, di
-0000a040: 6374 5d3a 0a20 2020 2020 2020 2022 2222  ct]:.        """
-0000a050: 0a20 2020 2020 2020 2045 7874 7261 6374  .        Extract
-0000a060: 2064 6174 6120 6172 7261 7920 616e 6420   data array and 
-0000a070: 6d65 7461 6461 7461 2066 726f 6d20 6c6f  metadata from lo
-0000a080: 6164 6564 2069 6d61 6765 2061 6e64 2072  aded image and r
-0000a090: 6574 7572 6e20 7468 656d 2e0a 2020 2020  eturn them..    
-0000a0a0: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-0000a0b0: 6e20 7265 7475 726e 7320 7477 6f20 6f62  n returns two ob
-0000a0c0: 6a65 6374 732c 2066 6972 7374 2069 7320  jects, first is 
-0000a0d0: 6e75 6d70 7920 6172 7261 7920 6f66 2069  numpy array of i
-0000a0e0: 6d61 6765 2064 6174 612c 2073 6563 6f6e  mage data, secon
-0000a0f0: 6420 6973 2064 6963 7420 6f66 206d 6574  d is dict of met
-0000a100: 6164 6174 612e 0a20 2020 2020 2020 2049  adata..        I
-0000a110: 7420 636f 6e73 7472 7563 7473 2060 6166  t constructs `af
-0000a120: 6669 6e65 602c 2060 6f72 6967 696e 616c  fine`, `original
-0000a130: 5f61 6666 696e 6560 2c20 616e 6420 6073  _affine`, and `s
-0000a140: 7061 7469 616c 5f73 6861 7065 6020 616e  patial_shape` an
-0000a150: 6420 7374 6f72 6573 2074 6865 6d20 696e  d stores them in
-0000a160: 206d 6574 6120 6469 6374 2e0a 2020 2020   meta dict..    
-0000a170: 2020 2020 5768 656e 206c 6f61 6469 6e67      When loading
-0000a180: 2061 206c 6973 7420 6f66 2066 696c 6573   a list of files
-0000a190: 2c20 7468 6579 2061 7265 2073 7461 636b  , they are stack
-0000a1a0: 6564 2074 6f67 6574 6865 7220 6174 2061  ed together at a
-0000a1b0: 206e 6577 2064 696d 656e 7369 6f6e 2061   new dimension a
-0000a1c0: 7320 7468 6520 6669 7273 7420 6469 6d65  s the first dime
-0000a1d0: 6e73 696f 6e2c 0a20 2020 2020 2020 2061  nsion,.        a
-0000a1e0: 6e64 2074 6865 206d 6574 6164 6174 6120  nd the metadata 
-0000a1f0: 6f66 2074 6865 2066 6972 7374 2069 6d61  of the first ima
-0000a200: 6765 2069 7320 7573 6564 2074 6f20 7072  ge is used to pr
-0000a210: 6573 656e 7420 7468 6520 6f75 7470 7574  esent the output
-0000a220: 206d 6574 6164 6174 612e 0a0a 2020 2020   metadata...    
-0000a230: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000a240: 2020 2020 2020 696d 673a 2061 204e 6962        img: a Nib
-0000a250: 6162 656c 2069 6d61 6765 206f 626a 6563  abel image objec
-0000a260: 7420 6c6f 6164 6564 2066 726f 6d20 616e  t loaded from an
-0000a270: 2069 6d61 6765 2066 696c 6520 6f72 2061   image file or a
-0000a280: 206c 6973 7420 6f66 204e 6962 6162 656c   list of Nibabel
-0000a290: 2069 6d61 6765 206f 626a 6563 7473 2e0a   image objects..
-0000a2a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a2b0: 2020 2020 2069 6d67 5f61 7272 6179 3a20       img_array: 
-0000a2c0: 6c69 7374 5b6e 702e 6e64 6172 7261 795d  list[np.ndarray]
-0000a2d0: 203d 205b 5d0a 2020 2020 2020 2020 636f   = [].        co
-0000a2e0: 6d70 6174 6962 6c65 5f6d 6574 613a 2064  mpatible_meta: d
-0000a2f0: 6963 7420 3d20 7b7d 0a0a 2020 2020 2020  ict = {}..      
-0000a300: 2020 666f 7220 6920 696e 2065 6e73 7572    for i in ensur
-0000a310: 655f 7475 706c 6528 696d 6729 3a0a 2020  e_tuple(img):.  
-0000a320: 2020 2020 2020 2020 2020 6865 6164 6572            header
-0000a330: 203d 2073 656c 662e 5f67 6574 5f6d 6574   = self._get_met
-0000a340: 615f 6469 6374 2869 290a 2020 2020 2020  a_dict(i).      
-0000a350: 2020 2020 2020 6865 6164 6572 5b4d 6574        header[Met
-0000a360: 614b 6579 732e 4146 4649 4e45 5d20 3d20  aKeys.AFFINE] = 
-0000a370: 7365 6c66 2e5f 6765 745f 6166 6669 6e65  self._get_affine
-0000a380: 2869 290a 2020 2020 2020 2020 2020 2020  (i).            
-0000a390: 6865 6164 6572 5b4d 6574 614b 6579 732e  header[MetaKeys.
-0000a3a0: 4f52 4947 494e 414c 5f41 4646 494e 455d  ORIGINAL_AFFINE]
-0000a3b0: 203d 2073 656c 662e 5f67 6574 5f61 6666   = self._get_aff
-0000a3c0: 696e 6528 6929 0a20 2020 2020 2020 2020  ine(i).         
-0000a3d0: 2020 2068 6561 6465 725b 2261 735f 636c     header["as_cl
-0000a3e0: 6f73 6573 745f 6361 6e6f 6e69 6361 6c22  osest_canonical"
-0000a3f0: 5d20 3d20 7365 6c66 2e61 735f 636c 6f73  ] = self.as_clos
-0000a400: 6573 745f 6361 6e6f 6e69 6361 6c0a 2020  est_canonical.  
-0000a410: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000a420: 662e 6173 5f63 6c6f 7365 7374 5f63 616e  f.as_closest_can
-0000a430: 6f6e 6963 616c 3a0a 2020 2020 2020 2020  onical:.        
-0000a440: 2020 2020 2020 2020 6920 3d20 6e69 622e          i = nib.
-0000a450: 6173 5f63 6c6f 7365 7374 5f63 616e 6f6e  as_closest_canon
-0000a460: 6963 616c 2869 290a 2020 2020 2020 2020  ical(i).        
-0000a470: 2020 2020 2020 2020 6865 6164 6572 5b4d          header[M
-0000a480: 6574 614b 6579 732e 4146 4649 4e45 5d20  etaKeys.AFFINE] 
-0000a490: 3d20 7365 6c66 2e5f 6765 745f 6166 6669  = self._get_affi
-0000a4a0: 6e65 2869 290a 2020 2020 2020 2020 2020  ne(i).          
-0000a4b0: 2020 6865 6164 6572 5b4d 6574 614b 6579    header[MetaKey
-0000a4c0: 732e 5350 4154 4941 4c5f 5348 4150 455d  s.SPATIAL_SHAPE]
-0000a4d0: 203d 2073 656c 662e 5f67 6574 5f73 7061   = self._get_spa
-0000a4e0: 7469 616c 5f73 6861 7065 2869 290a 2020  tial_shape(i).  
-0000a4f0: 2020 2020 2020 2020 2020 6865 6164 6572            header
-0000a500: 5b4d 6574 614b 6579 732e 5350 4143 455d  [MetaKeys.SPACE]
-0000a510: 203d 2053 7061 6365 4b65 7973 2e52 4153   = SpaceKeys.RAS
-0000a520: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-0000a530: 6120 3d20 7365 6c66 2e5f 6765 745f 6172  a = self._get_ar
-0000a540: 7261 795f 6461 7461 2869 290a 2020 2020  ray_data(i).    
-0000a550: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000a560: 7371 7565 657a 655f 6e6f 6e5f 7370 6174  squeeze_non_spat
-0000a570: 6961 6c5f 6469 6d73 3a0a 2020 2020 2020  ial_dims:.      
-0000a580: 2020 2020 2020 2020 2020 666f 7220 6420            for d 
-0000a590: 696e 2072 616e 6765 286c 656e 2864 6174  in range(len(dat
-0000a5a0: 612e 7368 6170 6529 2c20 6c65 6e28 6865  a.shape), len(he
-0000a5b0: 6164 6572 5b4d 6574 614b 6579 732e 5350  ader[MetaKeys.SP
-0000a5c0: 4154 4941 4c5f 5348 4150 455d 292c 202d  ATIAL_SHAPE]), -
-0000a5d0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-0000a5e0: 2020 2020 2020 2020 6966 2064 6174 612e          if data.
-0000a5f0: 7368 6170 655b 6420 2d20 315d 203d 3d20  shape[d - 1] == 
-0000a600: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-0000a610: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-0000a620: 3d20 6461 7461 2e73 7175 6565 7a65 2861  = data.squeeze(a
-0000a630: 7869 733d 6420 2d20 3129 0a20 2020 2020  xis=d - 1).     
-0000a640: 2020 2020 2020 2069 6d67 5f61 7272 6179         img_array
-0000a650: 2e61 7070 656e 6428 6461 7461 290a 2020  .append(data).  
-0000a660: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0000a670: 662e 6368 616e 6e65 6c5f 6469 6d20 6973  f.channel_dim is
-0000a680: 204e 6f6e 653a 2020 2320 6465 6661 756c   None:  # defaul
-0000a690: 7420 746f 2022 6e6f 5f63 6861 6e6e 656c  t to "no_channel
-0000a6a0: 2220 6f72 202d 310a 2020 2020 2020 2020  " or -1.        
-0000a6b0: 2020 2020 2020 2020 6865 6164 6572 5b4d          header[M
-0000a6c0: 6574 614b 6579 732e 4f52 4947 494e 414c  etaKeys.ORIGINAL
-0000a6d0: 5f43 4841 4e4e 454c 5f44 494d 5d20 3d20  _CHANNEL_DIM] = 
-0000a6e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000a6f0: 2020 2020 2020 666c 6f61 7428 226e 616e        float("nan
-0000a700: 2229 2069 6620 6c65 6e28 6461 7461 2e73  ") if len(data.s
-0000a710: 6861 7065 2920 3d3d 206c 656e 2868 6561  hape) == len(hea
-0000a720: 6465 725b 4d65 7461 4b65 7973 2e53 5041  der[MetaKeys.SPA
-0000a730: 5449 414c 5f53 4841 5045 5d29 2065 6c73  TIAL_SHAPE]) els
-0000a740: 6520 2d31 0a20 2020 2020 2020 2020 2020  e -1.           
-0000a750: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000a760: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000a770: 2020 2020 2020 2020 2068 6561 6465 725b           header[
-0000a780: 4d65 7461 4b65 7973 2e4f 5249 4749 4e41  MetaKeys.ORIGINA
-0000a790: 4c5f 4348 414e 4e45 4c5f 4449 4d5d 203d  L_CHANNEL_DIM] =
-0000a7a0: 2073 656c 662e 6368 616e 6e65 6c5f 6469   self.channel_di
-0000a7b0: 6d0a 2020 2020 2020 2020 2020 2020 5f63  m.            _c
-0000a7c0: 6f70 795f 636f 6d70 6174 6962 6c65 5f64  opy_compatible_d
-0000a7d0: 6963 7428 6865 6164 6572 2c20 636f 6d70  ict(header, comp
-0000a7e0: 6174 6962 6c65 5f6d 6574 6129 0a0a 2020  atible_meta)..  
-0000a7f0: 2020 2020 2020 7265 7475 726e 205f 7374        return _st
-0000a800: 6163 6b5f 696d 6167 6573 2869 6d67 5f61  ack_images(img_a
-0000a810: 7272 6179 2c20 636f 6d70 6174 6962 6c65  rray, compatible
-0000a820: 5f6d 6574 6129 2c20 636f 6d70 6174 6962  _meta), compatib
-0000a830: 6c65 5f6d 6574 610a 0a20 2020 2064 6566  le_meta..    def
-0000a840: 205f 6765 745f 6d65 7461 5f64 6963 7428   _get_meta_dict(
-0000a850: 7365 6c66 2c20 696d 6729 202d 3e20 6469  self, img) -> di
-0000a860: 6374 3a0a 2020 2020 2020 2020 2222 220a  ct:.        """.
-0000a870: 2020 2020 2020 2020 4765 7420 7468 6520          Get the 
-0000a880: 616c 6c20 7468 6520 6d65 7461 6461 7461  all the metadata
-0000a890: 206f 6620 7468 6520 696d 6167 6520 616e   of the image an
-0000a8a0: 6420 636f 6e76 6572 7420 746f 2064 6963  d convert to dic
-0000a8b0: 7420 7479 7065 2e0a 0a20 2020 2020 2020  t type...       
-0000a8c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000a8d0: 2020 2069 6d67 3a20 6120 4e69 6261 6265     img: a Nibabe
-0000a8e0: 6c20 696d 6167 6520 6f62 6a65 6374 206c  l image object l
-0000a8f0: 6f61 6465 6420 6672 6f6d 2061 6e20 696d  oaded from an im
-0000a900: 6167 6520 6669 6c65 2e0a 0a20 2020 2020  age file...     
-0000a910: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
-0000a920: 2073 7761 7020 746f 206c 6974 746c 6520   swap to little 
-0000a930: 656e 6469 616e 2061 7320 5079 546f 7263  endian as PyTorc
-0000a940: 6820 646f 6573 6e27 7420 7375 7070 6f72  h doesn't suppor
-0000a950: 7420 6269 6720 656e 6469 616e 0a20 2020  t big endian.   
-0000a960: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0000a970: 2020 2020 2020 6865 6164 6572 203d 2069        header = i
-0000a980: 6d67 2e68 6561 6465 722e 6173 5f62 7974  mg.header.as_byt
-0000a990: 6573 7761 7070 6564 2822 3c22 290a 2020  eswapped("<").  
-0000a9a0: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
-0000a9b0: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
-0000a9c0: 2020 2020 2068 6561 6465 7220 3d20 696d       header = im
-0000a9d0: 672e 6865 6164 6572 0a20 2020 2020 2020  g.header.       
-0000a9e0: 2072 6574 7572 6e20 6469 6374 2868 6561   return dict(hea
-0000a9f0: 6465 7229 0a0a 2020 2020 6465 6620 5f67  der)..    def _g
-0000aa00: 6574 5f61 6666 696e 6528 7365 6c66 2c20  et_affine(self, 
-0000aa10: 696d 6729 3a0a 2020 2020 2020 2020 2222  img):.        ""
-0000aa20: 220a 2020 2020 2020 2020 4765 7420 7468  ".        Get th
-0000aa30: 6520 6166 6669 6e65 206d 6174 7269 7820  e affine matrix 
-0000aa40: 6f66 2074 6865 2069 6d61 6765 2c20 6974  of the image, it
-0000aa50: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-0000aa60: 636f 7272 6563 740a 2020 2020 2020 2020  correct.        
-0000aa70: 7370 6163 696e 672c 206f 7269 656e 7461  spacing, orienta
-0000aa80: 7469 6f6e 206f 7220 6578 6563 7574 6520  tion or execute 
-0000aa90: 7370 6174 6961 6c20 7472 616e 7366 6f72  spatial transfor
-0000aaa0: 6d73 2e0a 0a20 2020 2020 2020 2041 7267  ms...        Arg
-0000aab0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-0000aac0: 6d67 3a20 6120 4e69 6261 6265 6c20 696d  mg: a Nibabel im
-0000aad0: 6167 6520 6f62 6a65 6374 206c 6f61 6465  age object loade
-0000aae0: 6420 6672 6f6d 2061 6e20 696d 6167 6520  d from an image 
-0000aaf0: 6669 6c65 2e0a 0a20 2020 2020 2020 2022  file...        "
-0000ab00: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0000ab10: 6e20 6e70 2e61 7272 6179 2869 6d67 2e61  n np.array(img.a
-0000ab20: 6666 696e 652c 2063 6f70 793d 5472 7565  ffine, copy=True
-0000ab30: 290a 0a20 2020 2064 6566 205f 6765 745f  )..    def _get_
-0000ab40: 7370 6174 6961 6c5f 7368 6170 6528 7365  spatial_shape(se
-0000ab50: 6c66 2c20 696d 6729 3a0a 2020 2020 2020  lf, img):.      
-0000ab60: 2020 2222 220a 2020 2020 2020 2020 4765    """.        Ge
-0000ab70: 7420 7468 6520 7370 6174 6961 6c20 7368  t the spatial sh
-0000ab80: 6170 6520 6f66 2069 6d61 6765 2064 6174  ape of image dat
-0000ab90: 612c 2069 7420 646f 6573 6e27 7420 636f  a, it doesn't co
-0000aba0: 6e74 6169 6e20 7468 6520 6368 616e 6e65  ntain the channe
-0000abb0: 6c20 6469 6d2e 0a0a 2020 2020 2020 2020  l dim...        
-0000abc0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000abd0: 2020 696d 673a 2061 204e 6962 6162 656c    img: a Nibabel
-0000abe0: 2069 6d61 6765 206f 626a 6563 7420 6c6f   image object lo
-0000abf0: 6164 6564 2066 726f 6d20 616e 2069 6d61  aded from an ima
-0000ac00: 6765 2066 696c 652e 0a0a 2020 2020 2020  ge file...      
-0000ac10: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
-0000ac20: 7377 6170 2074 6f20 6c69 7474 6c65 2065  swap to little e
-0000ac30: 6e64 6961 6e20 6173 2050 7954 6f72 6368  ndian as PyTorch
-0000ac40: 2064 6f65 736e 2774 2073 7570 706f 7274   doesn't support
-0000ac50: 2062 6967 2065 6e64 6961 6e0a 2020 2020   big endian.    
-0000ac60: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000ac70: 2020 2020 2068 6561 6465 7220 3d20 696d       header = im
-0000ac80: 672e 6865 6164 6572 2e61 735f 6279 7465  g.header.as_byte
-0000ac90: 7377 6170 7065 6428 223c 2229 0a20 2020  swapped("<").   
-0000aca0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
-0000acb0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
-0000acc0: 2020 2020 6865 6164 6572 203d 2069 6d67      header = img
-0000acd0: 2e68 6561 6465 720a 2020 2020 2020 2020  .header.        
-0000ace0: 6469 6d20 3d20 6865 6164 6572 2e67 6574  dim = header.get
-0000acf0: 2822 6469 6d22 2c20 4e6f 6e65 290a 2020  ("dim", None).  
-0000ad00: 2020 2020 2020 6966 2064 696d 2069 7320        if dim is 
-0000ad10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000ad20: 2020 6469 6d20 3d20 6865 6164 6572 2e67    dim = header.g
-0000ad30: 6574 2822 6469 6d73 2229 2020 2320 6d67  et("dims")  # mg
-0000ad40: 6820 666f 726d 6174 3f0a 2020 2020 2020  h format?.      
-0000ad50: 2020 2020 2020 6469 6d20 3d20 6e70 2e69        dim = np.i
-0000ad60: 6e73 6572 7428 6469 6d2c 2030 2c20 3329  nsert(dim, 0, 3)
-0000ad70: 0a20 2020 2020 2020 206e 6469 6d20 3d20  .        ndim = 
-0000ad80: 6469 6d5b 305d 0a20 2020 2020 2020 2073  dim[0].        s
-0000ad90: 697a 6520 3d20 6c69 7374 2864 696d 5b31  ize = list(dim[1
-0000ada0: 3a5d 290a 2020 2020 2020 2020 6966 206e  :]).        if n
-0000adb0: 6f74 2069 735f 6e6f 5f63 6861 6e6e 656c  ot is_no_channel
-0000adc0: 2873 656c 662e 6368 616e 6e65 6c5f 6469  (self.channel_di
-0000add0: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
-0000ade0: 7369 7a65 2e70 6f70 2869 6e74 2873 656c  size.pop(int(sel
-0000adf0: 662e 6368 616e 6e65 6c5f 6469 6d29 2920  f.channel_dim)) 
-0000ae00: 2023 2074 7970 653a 2069 676e 6f72 650a   # type: ignore.
-0000ae10: 2020 2020 2020 2020 7370 6174 6961 6c5f          spatial_
-0000ae20: 7261 6e6b 203d 206d 6178 286d 696e 286e  rank = max(min(n
-0000ae30: 6469 6d2c 2033 292c 2031 290a 2020 2020  dim, 3), 1).    
-0000ae40: 2020 2020 7265 7475 726e 206e 702e 6173      return np.as
-0000ae50: 6172 7261 7928 7369 7a65 5b3a 7370 6174  array(size[:spat
-0000ae60: 6961 6c5f 7261 6e6b 5d29 0a0a 2020 2020  ial_rank])..    
-0000ae70: 6465 6620 5f67 6574 5f61 7272 6179 5f64  def _get_array_d
-0000ae80: 6174 6128 7365 6c66 2c20 696d 6729 3a0a  ata(self, img):.
-0000ae90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000aea0: 2020 2020 4765 7420 7468 6520 7261 7720      Get the raw 
-0000aeb0: 6172 7261 7920 6461 7461 206f 6620 7468  array data of th
-0000aec0: 6520 696d 6167 652c 2063 6f6e 7665 7274  e image, convert
-0000aed0: 6564 2074 6f20 4e75 6d70 7920 6172 7261  ed to Numpy arra
-0000aee0: 792e 0a0a 2020 2020 2020 2020 4172 6773  y...        Args
-0000aef0: 3a0a 2020 2020 2020 2020 2020 2020 696d  :.            im
-0000af00: 673a 2061 204e 6962 6162 656c 2069 6d61  g: a Nibabel ima
-0000af10: 6765 206f 626a 6563 7420 6c6f 6164 6564  ge object loaded
-0000af20: 2066 726f 6d20 616e 2069 6d61 6765 2066   from an image f
-0000af30: 696c 652e 0a0a 2020 2020 2020 2020 2222  ile...        ""
-0000af40: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0000af50: 206e 702e 6173 616e 7961 7272 6179 2869   np.asanyarray(i
-0000af60: 6d67 2e64 6174 616f 626a 2c20 6f72 6465  mg.dataobj, orde
-0000af70: 723d 2243 2229 0a0a 0a63 6c61 7373 204e  r="C")...class N
-0000af80: 756d 7079 5265 6164 6572 2849 6d61 6765  umpyReader(Image
-0000af90: 5265 6164 6572 293a 0a20 2020 2022 2222  Reader):.    """
-0000afa0: 0a20 2020 204c 6f61 6420 4e50 5920 6f72  .    Load NPY or
-0000afb0: 204e 505a 2066 6f72 6d61 7420 6461 7461   NPZ format data
-0000afc0: 2062 6173 6564 206f 6e20 4e75 6d70 7920   based on Numpy 
-0000afd0: 6c69 6272 6172 792c 2074 6865 7920 6361  library, they ca
-0000afe0: 6e20 6265 2061 7272 6179 7320 6f72 2070  n be arrays or p
-0000aff0: 6963 6b6c 6564 206f 626a 6563 7473 2e0a  ickled objects..
-0000b000: 2020 2020 4120 7479 7069 6361 6c20 7573      A typical us
-0000b010: 6167 6520 6973 2074 6f20 6c6f 6164 2074  age is to load t
-0000b020: 6865 2060 6d61 736b 6020 6461 7461 2066  he `mask` data f
-0000b030: 6f72 2063 6c61 7373 6966 6963 6174 696f  or classificatio
-0000b040: 6e20 7461 736b 2e0a 2020 2020 4974 2063  n task..    It c
-0000b050: 616e 206c 6f61 6420 7061 7274 206f 6620  an load part of 
-0000b060: 7468 6520 6e70 7a20 6669 6c65 2077 6974  the npz file wit
-0000b070: 6820 7370 6563 6966 6965 6420 606e 707a  h specified `npz
-0000b080: 5f6b 6579 7360 2e0a 0a20 2020 2041 7267  _keys`...    Arg
-0000b090: 733a 0a20 2020 2020 2020 206e 707a 5f6b  s:.        npz_k
-0000b0a0: 6579 733a 2069 6620 6c6f 6164 696e 6720  eys: if loading 
-0000b0b0: 6e70 7a20 6669 6c65 2c20 6f6e 6c79 206c  npz file, only l
-0000b0c0: 6f61 6420 7468 6520 7370 6563 6966 6965  oad the specifie
-0000b0d0: 6420 6b65 7973 2c20 6966 204e 6f6e 652c  d keys, if None,
-0000b0e0: 206c 6f61 6420 616c 6c20 7468 6520 6974   load all the it
-0000b0f0: 656d 732e 0a20 2020 2020 2020 2020 2020  ems..           
-0000b100: 2073 7461 636b 2074 6865 206c 6f61 6465   stack the loade
-0000b110: 6420 6974 656d 7320 746f 6765 7468 6572  d items together
-0000b120: 2074 6f20 636f 6e73 7472 7563 7420 6120   to construct a 
-0000b130: 6e65 7720 6669 7273 7420 6469 6d65 6e73  new first dimens
-0000b140: 696f 6e2e 0a20 2020 2020 2020 2063 6861  ion..        cha
-0000b150: 6e6e 656c 5f64 696d 3a20 6966 206e 6f74  nnel_dim: if not
-0000b160: 204e 6f6e 652c 2065 7870 6c69 6369 746c   None, explicitl
-0000b170: 7920 7370 6563 6966 7920 7468 6520 6368  y specify the ch
-0000b180: 616e 6e65 6c20 6469 6d2c 206f 7468 6572  annel dim, other
-0000b190: 7769 7365 2c20 7472 6561 7420 7468 6520  wise, treat the 
-0000b1a0: 6172 7261 7920 6173 206e 6f20 6368 616e  array as no chan
-0000b1b0: 6e65 6c2e 0a20 2020 2020 2020 206b 7761  nel..        kwa
-0000b1c0: 7267 733a 2061 6464 6974 696f 6e61 6c20  rgs: additional 
-0000b1d0: 6172 6773 2066 6f72 2060 6e75 6d70 792e  args for `numpy.
-0000b1e0: 6c6f 6164 6020 4150 4920 6578 6365 7074  load` API except
-0000b1f0: 2060 616c 6c6f 775f 7069 636b 6c65 602e   `allow_pickle`.
-0000b200: 206d 6f72 6520 6465 7461 696c 7320 6162   more details ab
-0000b210: 6f75 7420 6176 6169 6c61 626c 6520 6172  out available ar
-0000b220: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000b230: 6874 7470 733a 2f2f 6e75 6d70 792e 6f72  https://numpy.or
-0000b240: 672f 646f 632f 7374 6162 6c65 2f72 6566  g/doc/stable/ref
-0000b250: 6572 656e 6365 2f67 656e 6572 6174 6564  erence/generated
-0000b260: 2f6e 756d 7079 2e6c 6f61 642e 6874 6d6c  /numpy.load.html
-0000b270: 0a0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-0000b280: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0000b290: 2c20 6e70 7a5f 6b65 7973 3a20 4b65 7973  , npz_keys: Keys
-0000b2a0: 436f 6c6c 6563 7469 6f6e 207c 204e 6f6e  Collection | Non
-0000b2b0: 6520 3d20 4e6f 6e65 2c20 6368 616e 6e65  e = None, channe
-0000b2c0: 6c5f 6469 6d3a 2073 7472 207c 2069 6e74  l_dim: str | int
-0000b2d0: 207c 204e 6f6e 6520 3d20 4e6f 6e65 2c20   | None = None, 
-0000b2e0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-0000b2f0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0000b300: 745f 5f28 290a 2020 2020 2020 2020 6966  t__().        if
-0000b310: 206e 707a 5f6b 6579 7320 6973 206e 6f74   npz_keys is not
-0000b320: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000b330: 2020 206e 707a 5f6b 6579 7320 3d20 656e     npz_keys = en
-0000b340: 7375 7265 5f74 7570 6c65 286e 707a 5f6b  sure_tuple(npz_k
-0000b350: 6579 7329 0a20 2020 2020 2020 2073 656c  eys).        sel
-0000b360: 662e 6e70 7a5f 6b65 7973 203d 206e 707a  f.npz_keys = npz
-0000b370: 5f6b 6579 730a 2020 2020 2020 2020 7365  _keys.        se
-0000b380: 6c66 2e63 6861 6e6e 656c 5f64 696d 203d  lf.channel_dim =
-0000b390: 2066 6c6f 6174 2822 6e61 6e22 2920 6966   float("nan") if
-0000b3a0: 2063 6861 6e6e 656c 5f64 696d 203d 3d20   channel_dim == 
-0000b3b0: 226e 6f5f 6368 616e 6e65 6c22 2065 6c73  "no_channel" els
-0000b3c0: 6520 6368 616e 6e65 6c5f 6469 6d0a 2020  e channel_dim.  
-0000b3d0: 2020 2020 2020 7365 6c66 2e6b 7761 7267        self.kwarg
-0000b3e0: 7320 3d20 6b77 6172 6773 0a0a 2020 2020  s = kwargs..    
-0000b3f0: 6465 6620 7665 7269 6679 5f73 7566 6669  def verify_suffi
-0000b400: 7828 7365 6c66 2c20 6669 6c65 6e61 6d65  x(self, filename
-0000b410: 3a20 5365 7175 656e 6365 5b50 6174 684c  : Sequence[PathL
-0000b420: 696b 655d 207c 2050 6174 684c 696b 6529  ike] | PathLike)
-0000b430: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
-0000b440: 2020 2222 220a 2020 2020 2020 2020 5665    """.        Ve
-0000b450: 7269 6679 2077 6865 7468 6572 2074 6865  rify whether the
-0000b460: 2073 7065 6369 6669 6564 2066 696c 6520   specified file 
-0000b470: 6f72 2066 696c 6573 2066 6f72 6d61 7420  or files format 
-0000b480: 6973 2073 7570 706f 7274 6564 2062 7920  is supported by 
-0000b490: 4e75 6d70 7920 7265 6164 6572 2e0a 0a20  Numpy reader... 
-0000b4a0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000b4b0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
-0000b4c0: 653a 2066 696c 6520 6e61 6d65 206f 7220  e: file name or 
-0000b4d0: 6120 6c69 7374 206f 6620 6669 6c65 206e  a list of file n
-0000b4e0: 616d 6573 2074 6f20 7265 6164 2e0a 2020  ames to read..  
-0000b4f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000b500: 2061 206c 6973 7420 6f66 2066 696c 6573   a list of files
-0000b510: 2c20 7665 7269 6679 2061 6c6c 2074 6865  , verify all the
-0000b520: 2073 7566 6669 7865 732e 0a20 2020 2020   suffixes..     
-0000b530: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-0000b540: 7566 6669 7865 733a 2053 6571 7565 6e63  uffixes: Sequenc
-0000b550: 655b 7374 725d 203d 205b 226e 707a 222c  e[str] = ["npz",
-0000b560: 2022 6e70 7922 5d0a 2020 2020 2020 2020   "npy"].        
-0000b570: 7265 7475 726e 2069 735f 7375 7070 6f72  return is_suppor
-0000b580: 7465 645f 666f 726d 6174 2866 696c 656e  ted_format(filen
-0000b590: 616d 652c 2073 7566 6669 7865 7329 0a0a  ame, suffixes)..
-0000b5a0: 2020 2020 6465 6620 7265 6164 2873 656c      def read(sel
-0000b5b0: 662c 2064 6174 613a 2053 6571 7565 6e63  f, data: Sequenc
-0000b5c0: 655b 5061 7468 4c69 6b65 5d20 7c20 5061  e[PathLike] | Pa
-0000b5d0: 7468 4c69 6b65 2c20 2a2a 6b77 6172 6773  thLike, **kwargs
-0000b5e0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000b5f0: 2020 2020 2020 2052 6561 6420 696d 6167         Read imag
-0000b600: 6520 6461 7461 2066 726f 6d20 7370 6563  e data from spec
-0000b610: 6966 6965 6420 6669 6c65 206f 7220 6669  ified file or fi
-0000b620: 6c65 732c 2069 7420 6361 6e20 7265 6164  les, it can read
-0000b630: 2061 206c 6973 7420 6f66 2064 6174 6120   a list of data 
-0000b640: 6669 6c65 730a 2020 2020 2020 2020 616e  files.        an
-0000b650: 6420 7374 6163 6b20 7468 656d 2074 6f67  d stack them tog
-0000b660: 6574 6865 7220 6173 206d 756c 7469 2d63  ether as multi-c
-0000b670: 6861 6e6e 656c 2064 6174 6120 696e 2060  hannel data in `
-0000b680: 6765 745f 6461 7461 2829 602e 0a20 2020  get_data()`..   
-0000b690: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
-0000b6a0: 6865 2072 6574 7572 6e65 6420 6f62 6a65  he returned obje
-0000b6b0: 6374 2069 7320 4e75 6d70 7920 6172 7261  ct is Numpy arra
-0000b6c0: 7920 6f72 206c 6973 7420 6f66 204e 756d  y or list of Num
-0000b6d0: 7079 2061 7272 6179 732e 0a0a 2020 2020  py arrays...    
-0000b6e0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000b6f0: 2020 2020 2020 6461 7461 3a20 6669 6c65        data: file
-0000b700: 206e 616d 6520 6f72 2061 206c 6973 7420   name or a list 
-0000b710: 6f66 2066 696c 6520 6e61 6d65 7320 746f  of file names to
-0000b720: 2072 6561 642e 0a20 2020 2020 2020 2020   read..         
-0000b730: 2020 206b 7761 7267 733a 2061 6464 6974     kwargs: addit
-0000b740: 696f 6e61 6c20 6172 6773 2066 6f72 2060  ional args for `
-0000b750: 6e75 6d70 792e 6c6f 6164 6020 4150 4920  numpy.load` API 
-0000b760: 6578 6365 7074 2060 616c 6c6f 775f 7069  except `allow_pi
-0000b770: 636b 6c65 602c 2077 696c 6c20 6f76 6572  ckle`, will over
-0000b780: 7269 6465 2060 7365 6c66 2e6b 7761 7267  ride `self.kwarg
-0000b790: 7360 2066 6f72 2065 7869 7374 696e 6720  s` for existing 
-0000b7a0: 6b65 7973 2e0a 2020 2020 2020 2020 2020  keys..          
-0000b7b0: 2020 2020 2020 4d6f 7265 2064 6574 6169        More detai
-0000b7c0: 6c73 2061 626f 7574 2061 7661 696c 6162  ls about availab
-0000b7d0: 6c65 2061 7267 733a 0a20 2020 2020 2020  le args:.       
-0000b7e0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-0000b7f0: 2f6e 756d 7079 2e6f 7267 2f64 6f63 2f73  /numpy.org/doc/s
-0000b800: 7461 626c 652f 7265 6665 7265 6e63 652f  table/reference/
-0000b810: 6765 6e65 7261 7465 642f 6e75 6d70 792e  generated/numpy.
-0000b820: 6c6f 6164 2e68 746d 6c0a 0a20 2020 2020  load.html..     
-0000b830: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0000b840: 6d67 5f3a 206c 6973 745b 4e69 6674 6931  mg_: list[Nifti1
-0000b850: 496d 6167 655d 203d 205b 5d0a 0a20 2020  Image] = []..   
-0000b860: 2020 2020 2066 696c 656e 616d 6573 3a20       filenames: 
-0000b870: 5365 7175 656e 6365 5b50 6174 684c 696b  Sequence[PathLik
-0000b880: 655d 203d 2065 6e73 7572 655f 7475 706c  e] = ensure_tupl
-0000b890: 6528 6461 7461 290a 2020 2020 2020 2020  e(data).        
-0000b8a0: 6b77 6172 6773 5f20 3d20 7365 6c66 2e6b  kwargs_ = self.k
-0000b8b0: 7761 7267 732e 636f 7079 2829 0a20 2020  wargs.copy().   
-0000b8c0: 2020 2020 206b 7761 7267 735f 2e75 7064       kwargs_.upd
-0000b8d0: 6174 6528 6b77 6172 6773 290a 2020 2020  ate(kwargs).    
-0000b8e0: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
-0000b8f0: 6669 6c65 6e61 6d65 733a 0a20 2020 2020  filenames:.     
-0000b900: 2020 2020 2020 2069 6d67 203d 206e 702e         img = np.
-0000b910: 6c6f 6164 286e 616d 652c 2061 6c6c 6f77  load(name, allow
-0000b920: 5f70 6963 6b6c 653d 5472 7565 2c20 2a2a  _pickle=True, **
-0000b930: 6b77 6172 6773 5f29 0a20 2020 2020 2020  kwargs_).       
-0000b940: 2020 2020 2069 6620 5061 7468 286e 616d       if Path(nam
-0000b950: 6529 2e6e 616d 652e 656e 6473 7769 7468  e).name.endswith
-0000b960: 2822 2e6e 707a 2229 3a0a 2020 2020 2020  (".npz"):.      
-0000b970: 2020 2020 2020 2020 2020 2320 6c6f 6164            # load
-0000b980: 2065 7870 6563 7465 6420 6974 656d 7320   expected items 
-0000b990: 6672 6f6d 204e 505a 2066 696c 650a 2020  from NPZ file.  
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-0000b9b0: 7a5f 6b65 7973 203d 205b 6622 6172 725f  z_keys = [f"arr_
-0000b9c0: 7b69 7d22 2066 6f72 2069 2069 6e20 7261  {i}" for i in ra
-0000b9d0: 6e67 6528 6c65 6e28 696d 6729 295d 2069  nge(len(img))] i
-0000b9e0: 6620 7365 6c66 2e6e 707a 5f6b 6579 7320  f self.npz_keys 
-0000b9f0: 6973 204e 6f6e 6520 656c 7365 2073 656c  is None else sel
-0000ba00: 662e 6e70 7a5f 6b65 7973 0a20 2020 2020  f.npz_keys.     
-0000ba10: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0000ba20: 2069 6e20 6e70 7a5f 6b65 7973 3a0a 2020   in npz_keys:.  
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba40: 2020 696d 675f 2e61 7070 656e 6428 696d    img_.append(im
-0000ba50: 675b 6b5d 290a 2020 2020 2020 2020 2020  g[k]).          
-0000ba60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000ba70: 2020 2020 2020 2020 696d 675f 2e61 7070          img_.app
-0000ba80: 656e 6428 696d 6729 0a0a 2020 2020 2020  end(img)..      
-0000ba90: 2020 7265 7475 726e 2069 6d67 5f20 6966    return img_ if
-0000baa0: 206c 656e 2869 6d67 5f29 203e 2031 2065   len(img_) > 1 e
-0000bab0: 6c73 6520 696d 675f 5b30 5d0a 0a20 2020  lse img_[0]..   
-0000bac0: 2064 6566 2067 6574 5f64 6174 6128 7365   def get_data(se
-0000bad0: 6c66 2c20 696d 6729 202d 3e20 7475 706c  lf, img) -> tupl
-0000bae0: 655b 6e70 2e6e 6461 7272 6179 2c20 6469  e[np.ndarray, di
-0000baf0: 6374 5d3a 0a20 2020 2020 2020 2022 2222  ct]:.        """
-0000bb00: 0a20 2020 2020 2020 2045 7874 7261 6374  .        Extract
-0000bb10: 2064 6174 6120 6172 7261 7920 616e 6420   data array and 
-0000bb20: 6d65 7461 6461 7461 2066 726f 6d20 6c6f  metadata from lo
-0000bb30: 6164 6564 2069 6d61 6765 2061 6e64 2072  aded image and r
-0000bb40: 6574 7572 6e20 7468 656d 2e0a 2020 2020  eturn them..    
-0000bb50: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-0000bb60: 6e20 7265 7475 726e 7320 7477 6f20 6f62  n returns two ob
-0000bb70: 6a65 6374 732c 2066 6972 7374 2069 7320  jects, first is 
-0000bb80: 6e75 6d70 7920 6172 7261 7920 6f66 2069  numpy array of i
-0000bb90: 6d61 6765 2064 6174 612c 2073 6563 6f6e  mage data, secon
-0000bba0: 6420 6973 2064 6963 7420 6f66 206d 6574  d is dict of met
-0000bbb0: 6164 6174 612e 0a20 2020 2020 2020 2049  adata..        I
-0000bbc0: 7420 636f 6e73 7472 7563 7473 2060 6166  t constructs `af
-0000bbd0: 6669 6e65 602c 2060 6f72 6967 696e 616c  fine`, `original
-0000bbe0: 5f61 6666 696e 6560 2c20 616e 6420 6073  _affine`, and `s
-0000bbf0: 7061 7469 616c 5f73 6861 7065 6020 616e  patial_shape` an
-0000bc00: 6420 7374 6f72 6573 2074 6865 6d20 696e  d stores them in
-0000bc10: 206d 6574 6120 6469 6374 2e0a 2020 2020   meta dict..    
-0000bc20: 2020 2020 5768 656e 206c 6f61 6469 6e67      When loading
-0000bc30: 2061 206c 6973 7420 6f66 2066 696c 6573   a list of files
-0000bc40: 2c20 7468 6579 2061 7265 2073 7461 636b  , they are stack
-0000bc50: 6564 2074 6f67 6574 6865 7220 6174 2061  ed together at a
-0000bc60: 206e 6577 2064 696d 656e 7369 6f6e 2061   new dimension a
-0000bc70: 7320 7468 6520 6669 7273 7420 6469 6d65  s the first dime
-0000bc80: 6e73 696f 6e2c 0a20 2020 2020 2020 2061  nsion,.        a
-0000bc90: 6e64 2074 6865 206d 6574 6164 6174 6120  nd the metadata 
-0000bca0: 6f66 2074 6865 2066 6972 7374 2069 6d61  of the first ima
-0000bcb0: 6765 2069 7320 7573 6564 2074 6f20 7265  ge is used to re
-0000bcc0: 7072 6573 656e 7420 7468 6520 6f75 7470  present the outp
-0000bcd0: 7574 206d 6574 6164 6174 612e 0a0a 2020  ut metadata...  
-0000bce0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000bcf0: 2020 2020 2020 2020 696d 673a 2061 204e          img: a N
-0000bd00: 756d 7079 2061 7272 6179 206c 6f61 6465  umpy array loade
-0000bd10: 6420 6672 6f6d 2061 2066 696c 6520 6f72  d from a file or
-0000bd20: 2061 206c 6973 7420 6f66 204e 756d 7079   a list of Numpy
-0000bd30: 2061 7272 6179 732e 0a0a 2020 2020 2020   arrays...      
-0000bd40: 2020 2222 220a 2020 2020 2020 2020 696d    """.        im
-0000bd50: 675f 6172 7261 793a 206c 6973 745b 6e70  g_array: list[np
-0000bd60: 2e6e 6461 7272 6179 5d20 3d20 5b5d 0a20  .ndarray] = []. 
-0000bd70: 2020 2020 2020 2063 6f6d 7061 7469 626c         compatibl
-0000bd80: 655f 6d65 7461 3a20 6469 6374 203d 207b  e_meta: dict = {
-0000bd90: 7d0a 2020 2020 2020 2020 6966 2069 7369  }.        if isi
-0000bda0: 6e73 7461 6e63 6528 696d 672c 206e 702e  nstance(img, np.
-0000bdb0: 6e64 6172 7261 7929 3a0a 2020 2020 2020  ndarray):.      
-0000bdc0: 2020 2020 2020 696d 6720 3d20 2869 6d67        img = (img
-0000bdd0: 2c29 0a0a 2020 2020 2020 2020 666f 7220  ,)..        for 
-0000bde0: 6920 696e 2065 6e73 7572 655f 7475 706c  i in ensure_tupl
-0000bdf0: 6528 696d 6729 3a0a 2020 2020 2020 2020  e(img):.        
-0000be00: 2020 2020 6865 6164 6572 3a20 6469 6374      header: dict
-0000be10: 5b4d 6574 614b 6579 732c 2041 6e79 5d20  [MetaKeys, Any] 
-0000be20: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
-0000be30: 2069 6620 6973 696e 7374 616e 6365 2869   if isinstance(i
-0000be40: 2c20 6e70 2e6e 6461 7272 6179 293a 0a20  , np.ndarray):. 
-0000be50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000be60: 2069 6620 6063 6861 6e6e 656c 5f64 696d   if `channel_dim
-0000be70: 6020 6973 204e 6f6e 652c 2063 616e 206e  ` is None, can n
-0000be80: 6f74 2064 6574 6563 7420 7468 6520 6368  ot detect the ch
-0000be90: 616e 6e65 6c20 6469 6d2c 2075 7365 2061  annel dim, use a
-0000bea0: 6c6c 2074 6865 2064 696d 7320 6173 2073  ll the dims as s
-0000beb0: 7061 7469 616c 5f73 6861 7065 0a20 2020  patial_shape.   
-0000bec0: 2020 2020 2020 2020 2020 2020 2073 7061               spa
-0000bed0: 7469 616c 5f73 6861 7065 203d 206e 702e  tial_shape = np.
-0000bee0: 6173 6172 7261 7928 692e 7368 6170 6529  asarray(i.shape)
-0000bef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bf00: 2069 6620 6973 696e 7374 616e 6365 2873   if isinstance(s
-0000bf10: 656c 662e 6368 616e 6e65 6c5f 6469 6d2c  elf.channel_dim,
-0000bf20: 2069 6e74 293a 0a20 2020 2020 2020 2020   int):.         
-0000bf30: 2020 2020 2020 2020 2020 2073 7061 7469             spati
-0000bf40: 616c 5f73 6861 7065 203d 206e 702e 6465  al_shape = np.de
-0000bf50: 6c65 7465 2873 7061 7469 616c 5f73 6861  lete(spatial_sha
-0000bf60: 7065 2c20 7365 6c66 2e63 6861 6e6e 656c  pe, self.channel
-0000bf70: 5f64 696d 290a 2020 2020 2020 2020 2020  _dim).          
-0000bf80: 2020 2020 2020 6865 6164 6572 5b4d 6574        header[Met
-0000bf90: 614b 6579 732e 5350 4154 4941 4c5f 5348  aKeys.SPATIAL_SH
-0000bfa0: 4150 455d 203d 2073 7061 7469 616c 5f73  APE] = spatial_s
-0000bfb0: 6861 7065 0a20 2020 2020 2020 2020 2020  hape.           
-0000bfc0: 2020 2020 2068 6561 6465 725b 4d65 7461       header[Meta
-0000bfd0: 4b65 7973 2e53 5041 4345 5d20 3d20 5370  Keys.SPACE] = Sp
-0000bfe0: 6163 654b 6579 732e 5241 530a 2020 2020  aceKeys.RAS.    
-0000bff0: 2020 2020 2020 2020 696d 675f 6172 7261          img_arra
-0000c000: 792e 6170 7065 6e64 2869 290a 2020 2020  y.append(i).    
-0000c010: 2020 2020 2020 2020 6865 6164 6572 5b4d          header[M
-0000c020: 6574 614b 6579 732e 4f52 4947 494e 414c  etaKeys.ORIGINAL
-0000c030: 5f43 4841 4e4e 454c 5f44 494d 5d20 3d20  _CHANNEL_DIM] = 
-0000c040: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000c050: 2020 7365 6c66 2e63 6861 6e6e 656c 5f64    self.channel_d
-0000c060: 696d 2069 6620 6973 696e 7374 616e 6365  im if isinstance
-0000c070: 2873 656c 662e 6368 616e 6e65 6c5f 6469  (self.channel_di
-0000c080: 6d2c 2069 6e74 2920 656c 7365 2066 6c6f  m, int) else flo
-0000c090: 6174 2822 6e61 6e22 290a 2020 2020 2020  at("nan").      
-0000c0a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000c0b0: 2020 2020 5f63 6f70 795f 636f 6d70 6174      _copy_compat
-0000c0c0: 6962 6c65 5f64 6963 7428 6865 6164 6572  ible_dict(header
-0000c0d0: 2c20 636f 6d70 6174 6962 6c65 5f6d 6574  , compatible_met
-0000c0e0: 6129 0a0a 2020 2020 2020 2020 7265 7475  a)..        retu
-0000c0f0: 726e 205f 7374 6163 6b5f 696d 6167 6573  rn _stack_images
-0000c100: 2869 6d67 5f61 7272 6179 2c20 636f 6d70  (img_array, comp
-0000c110: 6174 6962 6c65 5f6d 6574 6129 2c20 636f  atible_meta), co
-0000c120: 6d70 6174 6962 6c65 5f6d 6574 610a 0a0a  mpatible_meta...
-0000c130: 4072 6571 7569 7265 5f70 6b67 2870 6b67  @require_pkg(pkg
-0000c140: 5f6e 616d 653d 2250 494c 2229 0a63 6c61  _name="PIL").cla
-0000c150: 7373 2050 494c 5265 6164 6572 2849 6d61  ss PILReader(Ima
-0000c160: 6765 5265 6164 6572 293a 0a20 2020 2022  geReader):.    "
-0000c170: 2222 0a20 2020 204c 6f61 6420 636f 6d6d  "".    Load comm
-0000c180: 6f6e 2032 4420 696d 6167 6520 666f 726d  on 2D image form
-0000c190: 6174 2028 7375 7070 6f72 7473 2050 4e47  at (supports PNG
-0000c1a0: 2c20 4a50 472c 2042 4d50 2920 6669 6c65  , JPG, BMP) file
-0000c1b0: 206f 7220 6669 6c65 7320 6672 6f6d 2070   or files from p
-0000c1c0: 726f 7669 6465 6420 7061 7468 2e0a 0a20  rovided path... 
-0000c1d0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000c1e0: 2063 6f6e 7665 7274 6572 3a20 6164 6469   converter: addi
-0000c1f0: 7469 6f6e 616c 2066 756e 6374 696f 6e20  tional function 
-0000c200: 746f 2063 6f6e 7665 7274 2074 6865 2069  to convert the i
-0000c210: 6d61 6765 2064 6174 6120 6166 7465 7220  mage data after 
-0000c220: 6072 6561 6428 2960 2e0a 2020 2020 2020  `read()`..      
-0000c230: 2020 2020 2020 666f 7220 6578 616d 706c        for exampl
-0000c240: 652c 2075 7365 2060 636f 6e76 6572 7465  e, use `converte
-0000c250: 723d 6c61 6d62 6461 2069 6d61 6765 3a20  r=lambda image: 
-0000c260: 696d 6167 652e 636f 6e76 6572 7428 224c  image.convert("L
-0000c270: 4122 2960 2074 6f20 636f 6e76 6572 7420  A")` to convert 
-0000c280: 696d 6167 6520 666f 726d 6174 2e0a 2020  image format..  
-0000c290: 2020 2020 2020 7265 7665 7273 655f 696e        reverse_in
-0000c2a0: 6465 7869 6e67 3a20 7768 6574 6865 7220  dexing: whether 
-0000c2b0: 746f 2073 7761 7020 6178 6973 2030 2061  to swap axis 0 a
-0000c2c0: 6e64 2031 2061 6674 6572 206c 6f61 6469  nd 1 after loadi
-0000c2d0: 6e67 2074 6865 2061 7272 6179 2c20 7468  ng the array, th
-0000c2e0: 6973 2069 7320 656e 6162 6c65 6420 6279  is is enabled by
-0000c2f0: 2064 6566 6175 6c74 2c0a 2020 2020 2020   default,.      
-0000c300: 2020 2020 2020 736f 2074 6861 7420 6f75        so that ou
-0000c310: 7470 7574 206f 6620 7468 6520 7265 6164  tput of the read
-0000c320: 6572 2069 7320 636f 6e73 6973 7465 6e74  er is consistent
-0000c330: 2077 6974 6820 7468 6520 6f74 6865 7220   with the other 
-0000c340: 7265 6164 6572 732e 2053 6574 2074 6869  readers. Set thi
-0000c350: 7320 6f70 7469 6f6e 2074 6f20 6060 4661  s option to ``Fa
-0000c360: 6c73 6560 6020 746f 2075 7365 0a20 2020  lse`` to use.   
-0000c370: 2020 2020 2020 2020 2074 6865 2050 494c           the PIL
-0000c380: 2062 6163 6b65 6e64 2773 206f 7269 6769   backend's origi
-0000c390: 6e61 6c20 7370 6174 6961 6c20 6178 6573  nal spatial axes
-0000c3a0: 2063 6f6e 7665 6e74 696f 6e2e 0a20 2020   convention..   
-0000c3b0: 2020 2020 206b 7761 7267 733a 2061 6464       kwargs: add
-0000c3c0: 6974 696f 6e61 6c20 6172 6773 2066 6f72  itional args for
-0000c3d0: 2060 496d 6167 652e 6f70 656e 6020 4150   `Image.open` AP
-0000c3e0: 4920 696e 2060 7265 6164 2829 602c 206d  I in `read()`, m
-0000c3f0: 6f64 6520 6465 7461 696c 7320 6162 6f75  ode details abou
-0000c400: 7420 6176 6169 6c61 626c 6520 6172 6773  t available args
-0000c410: 3a0a 2020 2020 2020 2020 2020 2020 6874  :.            ht
-0000c420: 7470 733a 2f2f 7069 6c6c 6f77 2e72 6561  tps://pillow.rea
-0000c430: 6474 6865 646f 6373 2e69 6f2f 656e 2f73  dthedocs.io/en/s
-0000c440: 7461 626c 652f 7265 6665 7265 6e63 652f  table/reference/
-0000c450: 496d 6167 652e 6874 6d6c 2350 494c 2e49  Image.html#PIL.I
-0000c460: 6d61 6765 2e6f 7065 6e0a 2020 2020 2222  mage.open.    ""
-0000c470: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-0000c480: 745f 5f28 7365 6c66 2c20 636f 6e76 6572  t__(self, conver
-0000c490: 7465 723a 2043 616c 6c61 626c 6520 7c20  ter: Callable | 
-0000c4a0: 4e6f 6e65 203d 204e 6f6e 652c 2072 6576  None = None, rev
-0000c4b0: 6572 7365 5f69 6e64 6578 696e 673a 2062  erse_indexing: b
-0000c4c0: 6f6f 6c20 3d20 5472 7565 2c20 2a2a 6b77  ool = True, **kw
-0000c4d0: 6172 6773 293a 0a20 2020 2020 2020 2073  args):.        s
-0000c4e0: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-0000c4f0: 290a 2020 2020 2020 2020 7365 6c66 2e63  ).        self.c
-0000c500: 6f6e 7665 7274 6572 203d 2063 6f6e 7665  onverter = conve
-0000c510: 7274 6572 0a20 2020 2020 2020 2073 656c  rter.        sel
-0000c520: 662e 7265 7665 7273 655f 696e 6465 7869  f.reverse_indexi
-0000c530: 6e67 203d 2072 6576 6572 7365 5f69 6e64  ng = reverse_ind
-0000c540: 6578 696e 670a 2020 2020 2020 2020 7365  exing.        se
-0000c550: 6c66 2e6b 7761 7267 7320 3d20 6b77 6172  lf.kwargs = kwar
-0000c560: 6773 0a0a 2020 2020 6465 6620 7665 7269  gs..    def veri
-0000c570: 6679 5f73 7566 6669 7828 7365 6c66 2c20  fy_suffix(self, 
-0000c580: 6669 6c65 6e61 6d65 3a20 5365 7175 656e  filename: Sequen
-0000c590: 6365 5b50 6174 684c 696b 655d 207c 2050  ce[PathLike] | P
-0000c5a0: 6174 684c 696b 6529 202d 3e20 626f 6f6c  athLike) -> bool
-0000c5b0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000c5c0: 2020 2020 2020 5665 7269 6679 2077 6865        Verify whe
-0000c5d0: 7468 6572 2074 6865 2073 7065 6369 6669  ther the specifi
-0000c5e0: 6564 2066 696c 6520 6f72 2066 696c 6573  ed file or files
-0000c5f0: 2066 6f72 6d61 7420 6973 2073 7570 706f   format is suppo
-0000c600: 7274 6564 2062 7920 5049 4c20 7265 6164  rted by PIL read
-0000c610: 6572 2e0a 0a20 2020 2020 2020 2041 7267  er...        Arg
-0000c620: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-0000c630: 696c 656e 616d 653a 2066 696c 6520 6e61  ilename: file na
-0000c640: 6d65 206f 7220 6120 6c69 7374 206f 6620  me or a list of 
-0000c650: 6669 6c65 206e 616d 6573 2074 6f20 7265  file names to re
-0000c660: 6164 2e0a 2020 2020 2020 2020 2020 2020  ad..            
-0000c670: 2020 2020 6966 2061 206c 6973 7420 6f66      if a list of
-0000c680: 2066 696c 6573 2c20 7665 7269 6679 2061   files, verify a
-0000c690: 6c6c 2074 6865 2073 7566 6669 7865 732e  ll the suffixes.
-0000c6a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c6b0: 2020 2020 2073 7566 6669 7865 733a 2053       suffixes: S
-0000c6c0: 6571 7565 6e63 655b 7374 725d 203d 205b  equence[str] = [
-0000c6d0: 2270 6e67 222c 2022 6a70 6722 2c20 226a  "png", "jpg", "j
-0000c6e0: 7065 6722 2c20 2262 6d70 225d 0a20 2020  peg", "bmp"].   
-0000c6f0: 2020 2020 2072 6574 7572 6e20 6861 735f       return has_
-0000c700: 7069 6c20 616e 6420 6973 5f73 7570 706f  pil and is_suppo
-0000c710: 7274 6564 5f66 6f72 6d61 7428 6669 6c65  rted_format(file
-0000c720: 6e61 6d65 2c20 7375 6666 6978 6573 290a  name, suffixes).
-0000c730: 0a20 2020 2064 6566 2072 6561 6428 7365  .    def read(se
-0000c740: 6c66 2c20 6461 7461 3a20 5365 7175 656e  lf, data: Sequen
-0000c750: 6365 5b50 6174 684c 696b 655d 207c 2050  ce[PathLike] | P
-0000c760: 6174 684c 696b 6520 7c20 6e70 2e6e 6461  athLike | np.nda
-0000c770: 7272 6179 2c20 2a2a 6b77 6172 6773 293a  rray, **kwargs):
-0000c780: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c790: 2020 2020 2052 6561 6420 696d 6167 6520       Read image 
-0000c7a0: 6461 7461 2066 726f 6d20 7370 6563 6966  data from specif
-0000c7b0: 6965 6420 6669 6c65 206f 7220 6669 6c65  ied file or file
-0000c7c0: 732c 2069 7420 6361 6e20 7265 6164 2061  s, it can read a
-0000c7d0: 206c 6973 7420 6f66 2069 6d61 6765 730a   list of images.
-0000c7e0: 2020 2020 2020 2020 616e 6420 7374 6163          and stac
-0000c7f0: 6b20 7468 656d 2074 6f67 6574 6865 7220  k them together 
-0000c800: 6173 206d 756c 7469 2d63 6861 6e6e 656c  as multi-channel
-0000c810: 2064 6174 6120 696e 2060 6765 745f 6461   data in `get_da
-0000c820: 7461 2829 602e 0a20 2020 2020 2020 204e  ta()`..        N
-0000c830: 6f74 6520 7468 6174 2074 6865 2072 6574  ote that the ret
-0000c840: 7572 6e65 6420 6f62 6a65 6374 2069 7320  urned object is 
-0000c850: 5049 4c20 696d 6167 6520 6f72 206c 6973  PIL image or lis
-0000c860: 7420 6f66 2050 494c 2069 6d61 6765 2e0a  t of PIL image..
-0000c870: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000c880: 2020 2020 2020 2020 2020 2064 6174 613a             data:
-0000c890: 2066 696c 6520 6e61 6d65 206f 7220 6120   file name or a 
-0000c8a0: 6c69 7374 206f 6620 6669 6c65 206e 616d  list of file nam
-0000c8b0: 6573 2074 6f20 7265 6164 2e0a 2020 2020  es to read..    
-0000c8c0: 2020 2020 2020 2020 6b77 6172 6773 3a20          kwargs: 
-0000c8d0: 6164 6469 7469 6f6e 616c 2061 7267 7320  additional args 
-0000c8e0: 666f 7220 6049 6d61 6765 2e6f 7065 6e60  for `Image.open`
-0000c8f0: 2041 5049 2069 6e20 6072 6561 6428 2960   API in `read()`
-0000c900: 2c20 7769 6c6c 206f 7665 7272 6964 6520  , will override 
-0000c910: 6073 656c 662e 6b77 6172 6773 6020 666f  `self.kwargs` fo
-0000c920: 7220 6578 6973 7469 6e67 206b 6579 732e  r existing keys.
-0000c930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c940: 204d 6f64 6520 6465 7461 696c 7320 6162   Mode details ab
-0000c950: 6f75 7420 6176 6169 6c61 626c 6520 6172  out available ar
-0000c960: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000c970: 2020 2020 6874 7470 733a 2f2f 7069 6c6c      https://pill
-0000c980: 6f77 2e72 6561 6474 6865 646f 6373 2e69  ow.readthedocs.i
-0000c990: 6f2f 656e 2f73 7461 626c 652f 7265 6665  o/en/stable/refe
-0000c9a0: 7265 6e63 652f 496d 6167 652e 6874 6d6c  rence/Image.html
-0000c9b0: 2350 494c 2e49 6d61 6765 2e6f 7065 6e0a  #PIL.Image.open.
-0000c9c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c9d0: 2020 2020 2069 6d67 5f3a 206c 6973 745b       img_: list[
-0000c9e0: 5049 4c49 6d61 6765 2e49 6d61 6765 5d20  PILImage.Image] 
-0000c9f0: 3d20 5b5d 0a0a 2020 2020 2020 2020 6669  = []..        fi
-0000ca00: 6c65 6e61 6d65 733a 2053 6571 7565 6e63  lenames: Sequenc
-0000ca10: 655b 5061 7468 4c69 6b65 5d20 3d20 656e  e[PathLike] = en
-0000ca20: 7375 7265 5f74 7570 6c65 2864 6174 6129  sure_tuple(data)
-0000ca30: 0a20 2020 2020 2020 206b 7761 7267 735f  .        kwargs_
-0000ca40: 203d 2073 656c 662e 6b77 6172 6773 2e63   = self.kwargs.c
-0000ca50: 6f70 7928 290a 2020 2020 2020 2020 6b77  opy().        kw
-0000ca60: 6172 6773 5f2e 7570 6461 7465 286b 7761  args_.update(kwa
-0000ca70: 7267 7329 0a20 2020 2020 2020 2066 6f72  rgs).        for
-0000ca80: 206e 616d 6520 696e 2066 696c 656e 616d   name in filenam
-0000ca90: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-0000caa0: 696d 6720 3d20 5049 4c49 6d61 6765 2e6f  img = PILImage.o
-0000cab0: 7065 6e28 6e61 6d65 2c20 2a2a 6b77 6172  pen(name, **kwar
-0000cac0: 6773 5f29 0a20 2020 2020 2020 2020 2020  gs_).           
-0000cad0: 2069 6620 6361 6c6c 6162 6c65 2873 656c   if callable(sel
-0000cae0: 662e 636f 6e76 6572 7465 7229 3a0a 2020  f.converter):.  
-0000caf0: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0000cb00: 6720 3d20 7365 6c66 2e63 6f6e 7665 7274  g = self.convert
-0000cb10: 6572 2869 6d67 290a 2020 2020 2020 2020  er(img).        
-0000cb20: 2020 2020 696d 675f 2e61 7070 656e 6428      img_.append(
-0000cb30: 696d 6729 0a0a 2020 2020 2020 2020 7265  img)..        re
-0000cb40: 7475 726e 2069 6d67 5f20 6966 206c 656e  turn img_ if len
-0000cb50: 2866 696c 656e 616d 6573 2920 3e20 3120  (filenames) > 1 
-0000cb60: 656c 7365 2069 6d67 5f5b 305d 0a0a 2020  else img_[0]..  
-0000cb70: 2020 6465 6620 6765 745f 6461 7461 2873    def get_data(s
-0000cb80: 656c 662c 2069 6d67 2920 2d3e 2074 7570  elf, img) -> tup
-0000cb90: 6c65 5b6e 702e 6e64 6172 7261 792c 2064  le[np.ndarray, d
-0000cba0: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
-0000cbb0: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
-0000cbc0: 7420 6461 7461 2061 7272 6179 2061 6e64  t data array and
-0000cbd0: 206d 6574 6164 6174 6120 6672 6f6d 206c   metadata from l
-0000cbe0: 6f61 6465 6420 696d 6167 6520 616e 6420  oaded image and 
-0000cbf0: 7265 7475 726e 2074 6865 6d2e 0a20 2020  return them..   
-0000cc00: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
-0000cc10: 6f6e 2072 6574 7572 6e73 2074 776f 206f  on returns two o
-0000cc20: 626a 6563 7473 2c20 6669 7273 7420 6973  bjects, first is
-0000cc30: 206e 756d 7079 2061 7272 6179 206f 6620   numpy array of 
-0000cc40: 696d 6167 6520 6461 7461 2c20 7365 636f  image data, seco
-0000cc50: 6e64 2069 7320 6469 6374 206f 6620 6d65  nd is dict of me
-0000cc60: 7461 6461 7461 2e0a 2020 2020 2020 2020  tadata..        
-0000cc70: 4974 2063 6f6d 7075 7465 7320 6073 7061  It computes `spa
-0000cc80: 7469 616c 5f73 6861 7065 6020 616e 6420  tial_shape` and 
-0000cc90: 7374 6f72 6573 2069 7420 696e 206d 6574  stores it in met
-0000cca0: 6120 6469 6374 2e0a 2020 2020 2020 2020  a dict..        
-0000ccb0: 5768 656e 206c 6f61 6469 6e67 2061 206c  When loading a l
-0000ccc0: 6973 7420 6f66 2066 696c 6573 2c20 7468  ist of files, th
-0000ccd0: 6579 2061 7265 2073 7461 636b 6564 2074  ey are stacked t
-0000cce0: 6f67 6574 6865 7220 6174 2061 206e 6577  ogether at a new
-0000ccf0: 2064 696d 656e 7369 6f6e 2061 7320 7468   dimension as th
-0000cd00: 6520 6669 7273 7420 6469 6d65 6e73 696f  e first dimensio
-0000cd10: 6e2c 0a20 2020 2020 2020 2061 6e64 2074  n,.        and t
-0000cd20: 6865 206d 6574 6164 6174 6120 6f66 2074  he metadata of t
-0000cd30: 6865 2066 6972 7374 2069 6d61 6765 2069  he first image i
-0000cd40: 7320 7573 6564 2074 6f20 7265 7072 6573  s used to repres
-0000cd50: 656e 7420 7468 6520 6f75 7470 7574 206d  ent the output m
-0000cd60: 6574 6164 6174 612e 0a20 2020 2020 2020  etadata..       
-0000cd70: 204e 6f74 6520 7468 6174 2062 7920 6465   Note that by de
-0000cd80: 6661 756c 7420 6073 656c 662e 7265 7665  fault `self.reve
-0000cd90: 7273 655f 696e 6465 7869 6e67 6020 6973  rse_indexing` is
-0000cda0: 2073 6574 2074 6f20 6060 5472 7565 6060   set to ``True``
-0000cdb0: 2c20 7768 6963 6820 7377 6170 7320 6178  , which swaps ax
-0000cdc0: 6973 2030 2061 6e64 2031 2061 6674 6572  is 0 and 1 after
-0000cdd0: 206c 6f61 6469 6e67 0a20 2020 2020 2020   loading.       
-0000cde0: 2074 6865 2061 7272 6179 2062 6563 6175   the array becau
-0000cdf0: 7365 2074 6865 2073 7061 7469 616c 2061  se the spatial a
-0000ce00: 7865 7320 6465 6669 6e69 7469 6f6e 2069  xes definition i
-0000ce10: 6e20 5049 4c20 6973 2064 6966 6665 7265  n PIL is differe
-0000ce20: 6e74 2066 726f 6d20 6f74 6865 7220 636f  nt from other co
-0000ce30: 6d6d 6f6e 206d 6564 6963 616c 2070 6163  mmon medical pac
-0000ce40: 6b61 6765 732e 0a0a 2020 2020 2020 2020  kages...        
-0000ce50: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000ce60: 2020 696d 673a 2061 2050 494c 2049 6d61    img: a PIL Ima
-0000ce70: 6765 206f 626a 6563 7420 6c6f 6164 6564  ge object loaded
-0000ce80: 2066 726f 6d20 6120 6669 6c65 206f 7220   from a file or 
-0000ce90: 6120 6c69 7374 206f 6620 5049 4c20 496d  a list of PIL Im
-0000cea0: 6167 6520 6f62 6a65 6374 732e 0a0a 2020  age objects...  
-0000ceb0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000cec0: 2020 696d 675f 6172 7261 793a 206c 6973    img_array: lis
-0000ced0: 745b 6e70 2e6e 6461 7272 6179 5d20 3d20  t[np.ndarray] = 
-0000cee0: 5b5d 0a20 2020 2020 2020 2063 6f6d 7061  [].        compa
-0000cef0: 7469 626c 655f 6d65 7461 3a20 6469 6374  tible_meta: dict
-0000cf00: 203d 207b 7d0a 0a20 2020 2020 2020 2066   = {}..        f
-0000cf10: 6f72 2069 2069 6e20 656e 7375 7265 5f74  or i in ensure_t
-0000cf20: 7570 6c65 2869 6d67 293a 0a20 2020 2020  uple(img):.     
-0000cf30: 2020 2020 2020 2068 6561 6465 7220 3d20         header = 
-0000cf40: 7365 6c66 2e5f 6765 745f 6d65 7461 5f64  self._get_meta_d
-0000cf50: 6963 7428 6929 0a20 2020 2020 2020 2020  ict(i).         
-0000cf60: 2020 2068 6561 6465 725b 4d65 7461 4b65     header[MetaKe
-0000cf70: 7973 2e53 5041 5449 414c 5f53 4841 5045  ys.SPATIAL_SHAPE
-0000cf80: 5d20 3d20 7365 6c66 2e5f 6765 745f 7370  ] = self._get_sp
-0000cf90: 6174 6961 6c5f 7368 6170 6528 6929 0a20  atial_shape(i). 
-0000cfa0: 2020 2020 2020 2020 2020 2064 6174 6120             data 
-0000cfb0: 3d20 6e70 2e6d 6f76 6561 7869 7328 6e70  = np.moveaxis(np
-0000cfc0: 2e61 7361 7272 6179 2869 292c 2030 2c20  .asarray(i), 0, 
-0000cfd0: 3129 2069 6620 7365 6c66 2e72 6576 6572  1) if self.rever
-0000cfe0: 7365 5f69 6e64 6578 696e 6720 656c 7365  se_indexing else
-0000cff0: 206e 702e 6173 6172 7261 7928 6929 0a20   np.asarray(i). 
-0000d000: 2020 2020 2020 2020 2020 2069 6d67 5f61             img_a
-0000d010: 7272 6179 2e61 7070 656e 6428 6461 7461  rray.append(data
-0000d020: 290a 2020 2020 2020 2020 2020 2020 6865  ).            he
-0000d030: 6164 6572 5b4d 6574 614b 6579 732e 4f52  ader[MetaKeys.OR
-0000d040: 4947 494e 414c 5f43 4841 4e4e 454c 5f44  IGINAL_CHANNEL_D
-0000d050: 494d 5d20 3d20 280a 2020 2020 2020 2020  IM] = (.        
-0000d060: 2020 2020 2020 2020 666c 6f61 7428 226e          float("n
-0000d070: 616e 2229 2069 6620 6c65 6e28 6461 7461  an") if len(data
-0000d080: 2e73 6861 7065 2920 3d3d 206c 656e 2868  .shape) == len(h
-0000d090: 6561 6465 725b 4d65 7461 4b65 7973 2e53  eader[MetaKeys.S
-0000d0a0: 5041 5449 414c 5f53 4841 5045 5d29 2065  PATIAL_SHAPE]) e
-0000d0b0: 6c73 6520 2d31 0a20 2020 2020 2020 2020  lse -1.         
-0000d0c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000d0d0: 205f 636f 7079 5f63 6f6d 7061 7469 626c   _copy_compatibl
-0000d0e0: 655f 6469 6374 2868 6561 6465 722c 2063  e_dict(header, c
-0000d0f0: 6f6d 7061 7469 626c 655f 6d65 7461 290a  ompatible_meta).
-0000d100: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000d110: 5f73 7461 636b 5f69 6d61 6765 7328 696d  _stack_images(im
-0000d120: 675f 6172 7261 792c 2063 6f6d 7061 7469  g_array, compati
-0000d130: 626c 655f 6d65 7461 292c 2063 6f6d 7061  ble_meta), compa
-0000d140: 7469 626c 655f 6d65 7461 0a0a 2020 2020  tible_meta..    
-0000d150: 6465 6620 5f67 6574 5f6d 6574 615f 6469  def _get_meta_di
-0000d160: 6374 2873 656c 662c 2069 6d67 2920 2d3e  ct(self, img) ->
-0000d170: 2064 6963 743a 0a20 2020 2020 2020 2022   dict:.        "
-0000d180: 2222 0a20 2020 2020 2020 2047 6574 2074  "".        Get t
-0000d190: 6865 2061 6c6c 2074 6865 206d 6574 6164  he all the metad
-0000d1a0: 6174 6120 6f66 2074 6865 2069 6d61 6765  ata of the image
-0000d1b0: 2061 6e64 2063 6f6e 7665 7274 2074 6f20   and convert to 
-0000d1c0: 6469 6374 2074 7970 652e 0a20 2020 2020  dict type..     
-0000d1d0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000d1e0: 2020 2020 2069 6d67 3a20 6120 5049 4c20       img: a PIL 
-0000d1f0: 496d 6167 6520 6f62 6a65 6374 206c 6f61  Image object loa
-0000d200: 6465 6420 6672 6f6d 2061 6e20 696d 6167  ded from an imag
-0000d210: 6520 6669 6c65 2e0a 0a20 2020 2020 2020  e file...       
-0000d220: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000d230: 7572 6e20 7b22 666f 726d 6174 223a 2069  urn {"format": i
-0000d240: 6d67 2e66 6f72 6d61 742c 2022 6d6f 6465  mg.format, "mode
-0000d250: 223a 2069 6d67 2e6d 6f64 652c 2022 7769  ": img.mode, "wi
-0000d260: 6474 6822 3a20 696d 672e 7769 6474 682c  dth": img.width,
-0000d270: 2022 6865 6967 6874 223a 2069 6d67 2e68   "height": img.h
-0000d280: 6569 6768 747d 0a0a 2020 2020 6465 6620  eight}..    def 
-0000d290: 5f67 6574 5f73 7061 7469 616c 5f73 6861  _get_spatial_sha
-0000d2a0: 7065 2873 656c 662c 2069 6d67 293a 0a20  pe(self, img):. 
-0000d2b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d2c0: 2020 2047 6574 2074 6865 2073 7061 7469     Get the spati
-0000d2d0: 616c 2073 6861 7065 206f 6620 696d 6167  al shape of imag
-0000d2e0: 6520 6461 7461 2c20 6974 2064 6f65 736e  e data, it doesn
-0000d2f0: 2774 2063 6f6e 7461 696e 2074 6865 2063  't contain the c
-0000d300: 6861 6e6e 656c 2064 696d 2e0a 2020 2020  hannel dim..    
-0000d310: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000d320: 2020 2020 2020 696d 673a 2061 2050 494c        img: a PIL
-0000d330: 2049 6d61 6765 206f 626a 6563 7420 6c6f   Image object lo
-0000d340: 6164 6564 2066 726f 6d20 616e 2069 6d61  aded from an ima
-0000d350: 6765 2066 696c 652e 0a20 2020 2020 2020  ge file..       
-0000d360: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
-0000d370: 7572 6e20 6e70 2e61 7361 7272 6179 2828  urn np.asarray((
-0000d380: 696d 672e 7769 6474 682c 2069 6d67 2e68  img.width, img.h
-0000d390: 6569 6768 7429 290a 0a0a 4064 6570 7265  eight))...@depre
-0000d3a0: 6361 7465 6428 7369 6e63 653d 2230 2e38  cated(since="0.8
-0000d3b0: 222c 206d 7367 5f73 7566 6669 783d 2275  ", msg_suffix="u
-0000d3c0: 7365 2060 6d6f 6e61 692e 7773 695f 7265  se `monai.wsi_re
-0000d3d0: 6164 6572 2e57 5349 5265 6164 6572 6020  ader.WSIReader` 
-0000d3e0: 696e 7374 6561 642e 2229 0a63 6c61 7373  instead.").class
-0000d3f0: 2057 5349 5265 6164 6572 2849 6d61 6765   WSIReader(Image
-0000d400: 5265 6164 6572 293a 0a20 2020 2022 2222  Reader):.    """
-0000d410: 0a20 2020 2052 6561 6420 7768 6f6c 6520  .    Read whole 
-0000d420: 736c 6964 6520 696d 6167 6573 2061 6e64  slide images and
-0000d430: 2065 7874 7261 6374 2070 6174 6368 6573   extract patches
-0000d440: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-0000d450: 2020 2020 2062 6163 6b65 6e64 3a20 6261       backend: ba
-0000d460: 636b 656e 6420 6c69 6272 6172 7920 746f  ckend library to
-0000d470: 206c 6f61 6420 7468 6520 696d 6167 6573   load the images
-0000d480: 2c20 6176 6169 6c61 626c 6520 6f70 7469  , available opti
-0000d490: 6f6e 733a 2022 6375 4349 4d22 2c20 224f  ons: "cuCIM", "O
-0000d4a0: 7065 6e53 6c69 6465 2220 616e 6420 2254  penSlide" and "T
-0000d4b0: 6966 6646 696c 6522 2e0a 2020 2020 2020  iffFile"..      
-0000d4c0: 2020 6c65 7665 6c3a 2074 6865 2077 686f    level: the who
-0000d4d0: 6c65 2073 6c69 6465 2069 6d61 6765 206c  le slide image l
-0000d4e0: 6576 656c 2061 7420 7768 6963 6820 7468  evel at which th
-0000d4f0: 6520 696d 6167 6520 6973 2065 7874 7261  e image is extra
-0000d500: 6374 6564 2e20 2864 6566 6175 6c74 3d30  cted. (default=0
-0000d510: 290a 2020 2020 2020 2020 2020 2020 5468  ).            Th
-0000d520: 6973 2069 7320 6f76 6572 7269 6464 656e  is is overridden
-0000d530: 2069 6620 7468 6520 6c65 7665 6c20 6172   if the level ar
-0000d540: 6775 6d65 6e74 2069 7320 7072 6f76 6964  gument is provid
-0000d550: 6564 2069 6e20 6067 6574 5f64 6174 6160  ed in `get_data`
-0000d560: 2e0a 2020 2020 2020 2020 6b77 6172 6773  ..        kwargs
-0000d570: 3a20 6164 6469 7469 6f6e 616c 2061 7267  : additional arg
-0000d580: 7320 666f 7220 6261 636b 656e 6420 7265  s for backend re
-0000d590: 6164 696e 6720 4150 4920 696e 2060 7265  ading API in `re
-0000d5a0: 6164 2829 602c 206d 6f72 6520 6465 7461  ad()`, more deta
-0000d5b0: 696c 7320 696e 2060 6375 4349 4d60 2c20  ils in `cuCIM`, 
-0000d5c0: 6054 6966 6646 696c 6560 2c20 604f 7065  `TiffFile`, `Ope
-0000d5d0: 6e53 6c69 6465 603a 0a20 2020 2020 2020  nSlide`:.       
-0000d5e0: 2020 2020 2068 7474 7073 3a2f 2f67 6974       https://git
-0000d5f0: 6875 622e 636f 6d2f 7261 7069 6473 6169  hub.com/rapidsai
-0000d600: 2f63 7563 696d 2f62 6c6f 622f 7632 312e  /cucim/blob/v21.
-0000d610: 3132 2e30 302f 6370 702f 696e 636c 7564  12.00/cpp/includ
-0000d620: 652f 6375 6369 6d2f 6375 696d 6167 652e  e/cucim/cuimage.
-0000d630: 6823 4c31 3030 2e0a 2020 2020 2020 2020  h#L100..        
-0000d640: 2020 2020 6874 7470 733a 2f2f 6769 7468      https://gith
-0000d650: 7562 2e63 6f6d 2f63 676f 686c 6b65 2f74  ub.com/cgohlke/t
-0000d660: 6966 6666 696c 652e 0a20 2020 2020 2020  ifffile..       
-0000d670: 2020 2020 2068 7474 7073 3a2f 2f6f 7065       https://ope
-0000d680: 6e73 6c69 6465 2e6f 7267 2f61 7069 2f70  nslide.org/api/p
-0000d690: 7974 686f 6e2f 236f 7065 6e73 6c69 6465  ython/#openslide
-0000d6a0: 2e4f 7065 6e53 6c69 6465 2e0a 0a20 2020  .OpenSlide...   
-0000d6b0: 204e 6f74 653a 0a20 2020 2020 2020 2057   Note:.        W
-0000d6c0: 6869 6c65 2022 6375 4349 4d22 2061 6e64  hile "cuCIM" and
-0000d6d0: 2022 4f70 656e 536c 6964 6522 2062 6163   "OpenSlide" bac
-0000d6e0: 6b65 6e64 7320 626f 7468 2063 616e 206c  kends both can l
-0000d6f0: 6f61 6420 7061 7463 6865 7320 6672 6f6d  oad patches from
-0000d700: 206c 6172 6765 2077 686f 6c65 2073 6c69   large whole sli
-0000d710: 6465 2069 6d61 6765 730a 2020 2020 2020  de images.      
-0000d720: 2020 7769 7468 6f75 7420 6c6f 6164 696e    without loadin
-0000d730: 6720 7468 6520 656e 7469 7265 2069 6d61  g the entire ima
-0000d740: 6765 2069 6e74 6f20 6d65 6d6f 7279 2c20  ge into memory, 
-0000d750: 2254 6966 6646 696c 6522 2062 6163 6b65  "TiffFile" backe
-0000d760: 6e64 206e 6565 6473 2074 6f20 6c6f 6164  nd needs to load
-0000d770: 2074 6865 2065 6e74 6972 6520 696d 6167   the entire imag
-0000d780: 6520 696e 746f 206d 656d 6f72 790a 2020  e into memory.  
-0000d790: 2020 2020 2020 6265 666f 7265 2065 7874        before ext
-0000d7a0: 7261 6374 696e 6720 616e 7920 7061 7463  racting any patc
-0000d7b0: 683b 2074 6875 732c 206d 656d 6f72 7920  h; thus, memory 
-0000d7c0: 636f 6e73 6964 6572 6174 696f 6e20 6973  consideration is
-0000d7d0: 206e 6565 6465 6420 7768 656e 2075 7369   needed when usi
-0000d7e0: 6e67 2022 5469 6666 4669 6c65 2220 6261  ng "TiffFile" ba
-0000d7f0: 636b 656e 6420 666f 720a 2020 2020 2020  ckend for.      
-0000d800: 2020 7061 7463 6820 6578 7472 6163 7469    patch extracti
-0000d810: 6f6e 2e0a 0a20 2020 2022 2222 0a0a 2020  on...    """..  
-0000d820: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000d830: 656c 662c 2062 6163 6b65 6e64 3a20 7374  elf, backend: st
-0000d840: 7220 3d20 224f 7065 6e53 6c69 6465 222c  r = "OpenSlide",
-0000d850: 206c 6576 656c 3a20 696e 7420 3d20 302c   level: int = 0,
-0000d860: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-0000d870: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-0000d880: 6974 5f5f 2829 0a20 2020 2020 2020 2073  it__().        s
-0000d890: 656c 662e 6261 636b 656e 6420 3d20 6261  elf.backend = ba
-0000d8a0: 636b 656e 642e 6c6f 7765 7228 290a 2020  ckend.lower().  
-0000d8b0: 2020 2020 2020 6675 6e63 203d 2072 6571        func = req
-0000d8c0: 7569 7265 5f70 6b67 2873 656c 662e 6261  uire_pkg(self.ba
-0000d8d0: 636b 656e 6429 2873 656c 662e 5f73 6574  ckend)(self._set
-0000d8e0: 5f72 6561 6465 7229 0a20 2020 2020 2020  _reader).       
-0000d8f0: 2073 656c 662e 7773 695f 7265 6164 6572   self.wsi_reader
-0000d900: 203d 2066 756e 6328 7365 6c66 2e62 6163   = func(self.bac
-0000d910: 6b65 6e64 290a 2020 2020 2020 2020 7365  kend).        se
-0000d920: 6c66 2e6c 6576 656c 203d 206c 6576 656c  lf.level = level
-0000d930: 0a20 2020 2020 2020 2073 656c 662e 6b77  .        self.kw
-0000d940: 6172 6773 203d 206b 7761 7267 730a 0a20  args = kwargs.. 
-0000d950: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-0000d960: 0a20 2020 2064 6566 205f 7365 745f 7265  .    def _set_re
-0000d970: 6164 6572 2862 6163 6b65 6e64 3a20 7374  ader(backend: st
-0000d980: 7229 3a0a 2020 2020 2020 2020 6966 2062  r):.        if b
-0000d990: 6163 6b65 6e64 203d 3d20 226f 7065 6e73  ackend == "opens
-0000d9a0: 6c69 6465 223a 0a20 2020 2020 2020 2020  lide":.         
-0000d9b0: 2020 2072 6574 7572 6e20 4f70 656e 536c     return OpenSl
-0000d9c0: 6964 650a 2020 2020 2020 2020 6966 2062  ide.        if b
-0000d9d0: 6163 6b65 6e64 203d 3d20 2263 7563 696d  ackend == "cucim
-0000d9e0: 223a 0a20 2020 2020 2020 2020 2020 2072  ":.            r
-0000d9f0: 6574 7572 6e20 6f70 7469 6f6e 616c 5f69  eturn optional_i
-0000da00: 6d70 6f72 7428 2263 7563 696d 222c 206e  mport("cucim", n
-0000da10: 616d 653d 2243 7549 6d61 6765 2229 5b30  ame="CuImage")[0
-0000da20: 5d0a 2020 2020 2020 2020 6966 2062 6163  ].        if bac
-0000da30: 6b65 6e64 203d 3d20 2274 6966 6666 696c  kend == "tifffil
-0000da40: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
-0000da50: 7265 7475 726e 2054 6966 6646 696c 650a  return TiffFile.
-0000da60: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0000da70: 6c75 6545 7272 6f72 2822 6062 6163 6b65  lueError("`backe
-0000da80: 6e64 6020 7368 6f75 6c64 2062 6520 2763  nd` should be 'c
-0000da90: 7543 494d 272c 2027 4f70 656e 536c 6964  uCIM', 'OpenSlid
-0000daa0: 6527 206f 7220 2754 6966 6646 696c 6527  e' or 'TiffFile'
-0000dab0: 2e22 290a 0a20 2020 2064 6566 2076 6572  .")..    def ver
-0000dac0: 6966 795f 7375 6666 6978 2873 656c 662c  ify_suffix(self,
-0000dad0: 2066 696c 656e 616d 653a 2053 6571 7565   filename: Seque
-0000dae0: 6e63 655b 5061 7468 4c69 6b65 5d20 7c20  nce[PathLike] | 
-0000daf0: 5061 7468 4c69 6b65 2920 2d3e 2062 6f6f  PathLike) -> boo
-0000db00: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
-0000db10: 2020 2020 2020 2056 6572 6966 7920 7768         Verify wh
-0000db20: 6574 6865 7220 7468 6520 7370 6563 6966  ether the specif
-0000db30: 6965 6420 6669 6c65 206f 7220 6669 6c65  ied file or file
-0000db40: 7320 666f 726d 6174 2069 7320 7375 7070  s format is supp
-0000db50: 6f72 7465 6420 6279 2057 5349 2072 6561  orted by WSI rea
-0000db60: 6465 722e 0a0a 2020 2020 2020 2020 4172  der...        Ar
-0000db70: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000db80: 6669 6c65 6e61 6d65 3a20 6669 6c65 206e  filename: file n
-0000db90: 616d 6520 6f72 2061 206c 6973 7420 6f66  ame or a list of
-0000dba0: 2066 696c 6520 6e61 6d65 7320 746f 2072   file names to r
-0000dbb0: 6561 642e 0a20 2020 2020 2020 2020 2020  ead..           
-0000dbc0: 2020 2020 2069 6620 6120 6c69 7374 206f       if a list o
-0000dbd0: 6620 6669 6c65 732c 2076 6572 6966 7920  f files, verify 
-0000dbe0: 616c 6c20 7468 6520 7375 6666 6978 6573  all the suffixes
-0000dbf0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000dc00: 2020 2020 2020 7265 7475 726e 2069 735f        return is_
-0000dc10: 7375 7070 6f72 7465 645f 666f 726d 6174  supported_format
-0000dc20: 2866 696c 656e 616d 652c 205b 2274 6966  (filename, ["tif
-0000dc30: 222c 2022 7469 6666 225d 290a 0a20 2020  ", "tiff"])..   
-0000dc40: 2064 6566 2072 6561 6428 7365 6c66 2c20   def read(self, 
-0000dc50: 6461 7461 3a20 5365 7175 656e 6365 5b50  data: Sequence[P
-0000dc60: 6174 684c 696b 655d 207c 2050 6174 684c  athLike] | PathL
-0000dc70: 696b 6520 7c20 6e70 2e6e 6461 7272 6179  ike | np.ndarray
-0000dc80: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-0000dc90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000dca0: 2052 6561 6420 696d 6167 6520 6461 7461   Read image data
-0000dcb0: 2066 726f 6d20 6769 7665 6e20 6669 6c65   from given file
-0000dcc0: 206f 7220 6c69 7374 206f 6620 6669 6c65   or list of file
-0000dcd0: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
-0000dce0: 3a0a 2020 2020 2020 2020 2020 2020 6461  :.            da
-0000dcf0: 7461 3a20 6669 6c65 206e 616d 6520 6f72  ta: file name or
-0000dd00: 2061 206c 6973 7420 6f66 2066 696c 6520   a list of file 
-0000dd10: 6e61 6d65 7320 746f 2072 6561 642e 0a20  names to read.. 
-0000dd20: 2020 2020 2020 2020 2020 206b 7761 7267             kwarg
-0000dd30: 733a 2061 6464 6974 696f 6e61 6c20 6172  s: additional ar
-0000dd40: 6773 2066 6f72 2062 6163 6b65 6e64 2072  gs for backend r
-0000dd50: 6561 6469 6e67 2041 5049 2069 6e20 6072  eading API in `r
-0000dd60: 6561 6428 2960 2c20 7769 6c6c 206f 7665  ead()`, will ove
-0000dd70: 7272 6964 6520 6073 656c 662e 6b77 6172  rride `self.kwar
-0000dd80: 6773 6020 666f 7220 6578 6973 7469 6e67  gs` for existing
-0000dd90: 206b 6579 732e 0a20 2020 2020 2020 2020   keys..         
-0000dda0: 2020 2020 2020 206d 6f72 6520 6465 7461         more deta
-0000ddb0: 696c 7320 696e 2060 6375 4349 4d60 2c20  ils in `cuCIM`, 
-0000ddc0: 6054 6966 6646 696c 6560 2c20 604f 7065  `TiffFile`, `Ope
-0000ddd0: 6e53 6c69 6465 603a 0a20 2020 2020 2020  nSlide`:.       
-0000dde0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-0000ddf0: 2f67 6974 6875 622e 636f 6d2f 7261 7069  /github.com/rapi
-0000de00: 6473 6169 2f63 7563 696d 2f62 6c6f 622f  dsai/cucim/blob/
-0000de10: 7632 312e 3132 2e30 302f 6370 702f 696e  v21.12.00/cpp/in
-0000de20: 636c 7564 652f 6375 6369 6d2f 6375 696d  clude/cucim/cuim
-0000de30: 6167 652e 6823 4c31 3030 2e0a 2020 2020  age.h#L100..    
-0000de40: 2020 2020 2020 2020 2020 2020 6874 7470              http
-0000de50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-0000de60: 676f 686c 6b65 2f74 6966 6666 696c 652e  gohlke/tifffile.
-0000de70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000de80: 2068 7474 7073 3a2f 2f6f 7065 6e73 6c69   https://opensli
-0000de90: 6465 2e6f 7267 2f61 7069 2f70 7974 686f  de.org/api/pytho
-0000dea0: 6e2f 236f 7065 6e73 6c69 6465 2e4f 7065  n/#openslide.Ope
-0000deb0: 6e53 6c69 6465 2e0a 0a20 2020 2020 2020  nSlide...       
-0000dec0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000ded0: 2020 2020 2020 696d 6167 6520 6f62 6a65        image obje
-0000dee0: 6374 206f 7220 6c69 7374 206f 6620 696d  ct or list of im
-0000def0: 6167 6520 6f62 6a65 6374 730a 0a20 2020  age objects..   
-0000df00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000df10: 2069 6d67 5f3a 206c 6973 7420 3d20 5b5d   img_: list = []
-0000df20: 0a0a 2020 2020 2020 2020 6669 6c65 6e61  ..        filena
-0000df30: 6d65 733a 2053 6571 7565 6e63 655b 5061  mes: Sequence[Pa
-0000df40: 7468 4c69 6b65 5d20 3d20 656e 7375 7265  thLike] = ensure
-0000df50: 5f74 7570 6c65 2864 6174 6129 0a20 2020  _tuple(data).   
-0000df60: 2020 2020 206b 7761 7267 735f 203d 2073       kwargs_ = s
-0000df70: 656c 662e 6b77 6172 6773 2e63 6f70 7928  elf.kwargs.copy(
-0000df80: 290a 2020 2020 2020 2020 6b77 6172 6773  ).        kwargs
-0000df90: 5f2e 7570 6461 7465 286b 7761 7267 7329  _.update(kwargs)
-0000dfa0: 0a20 2020 2020 2020 2066 6f72 206e 616d  .        for nam
-0000dfb0: 6520 696e 2066 696c 656e 616d 6573 3a0a  e in filenames:.
-0000dfc0: 2020 2020 2020 2020 2020 2020 696d 6720              img 
-0000dfd0: 3d20 7365 6c66 2e77 7369 5f72 6561 6465  = self.wsi_reade
-0000dfe0: 7228 6e61 6d65 2c20 2a2a 6b77 6172 6773  r(name, **kwargs
-0000dff0: 5f29 0a20 2020 2020 2020 2020 2020 2069  _).            i
-0000e000: 6620 7365 6c66 2e62 6163 6b65 6e64 203d  f self.backend =
-0000e010: 3d20 226f 7065 6e73 6c69 6465 223a 0a20  = "openslide":. 
-0000e020: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e030: 6d67 2e73 6861 7065 203d 2028 696d 672e  mg.shape = (img.
-0000e040: 6469 6d65 6e73 696f 6e73 5b31 5d2c 2069  dimensions[1], i
-0000e050: 6d67 2e64 696d 656e 7369 6f6e 735b 305d  mg.dimensions[0]
-0000e060: 2c20 3329 0a20 2020 2020 2020 2020 2020  , 3).           
-0000e070: 2069 6d67 5f2e 6170 7065 6e64 2869 6d67   img_.append(img
-0000e080: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-0000e090: 6e20 696d 675f 2069 6620 6c65 6e28 6669  n img_ if len(fi
-0000e0a0: 6c65 6e61 6d65 7329 203e 2031 2065 6c73  lenames) > 1 els
-0000e0b0: 6520 696d 675f 5b30 5d0a 0a20 2020 2064  e img_[0]..    d
-0000e0c0: 6566 2067 6574 5f64 6174 6128 0a20 2020  ef get_data(.   
-0000e0d0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000e0e0: 2020 2069 6d67 2c0a 2020 2020 2020 2020     img,.        
-0000e0f0: 6c6f 6361 7469 6f6e 3a20 7475 706c 655b  location: tuple[
-0000e100: 696e 742c 2069 6e74 5d20 3d20 2830 2c20  int, int] = (0, 
-0000e110: 3029 2c0a 2020 2020 2020 2020 7369 7a65  0),.        size
-0000e120: 3a20 7475 706c 655b 696e 742c 2069 6e74  : tuple[int, int
-0000e130: 5d20 7c20 4e6f 6e65 203d 204e 6f6e 652c  ] | None = None,
-0000e140: 0a20 2020 2020 2020 206c 6576 656c 3a20  .        level: 
-0000e150: 696e 7420 7c20 4e6f 6e65 203d 204e 6f6e  int | None = Non
-0000e160: 652c 0a20 2020 2020 2020 2064 7479 7065  e,.        dtype
-0000e170: 3a20 4474 7970 654c 696b 6520 3d20 6e70  : DtypeLike = np
-0000e180: 2e75 696e 7438 2c0a 2020 2020 2020 2020  .uint8,.        
-0000e190: 6772 6964 5f73 6861 7065 3a20 7475 706c  grid_shape: tupl
-0000e1a0: 655b 696e 742c 2069 6e74 5d20 3d20 2831  e[int, int] = (1
-0000e1b0: 2c20 3129 2c0a 2020 2020 2020 2020 7061  , 1),.        pa
-0000e1c0: 7463 685f 7369 7a65 3a20 696e 7420 7c20  tch_size: int | 
-0000e1d0: 7475 706c 655b 696e 742c 2069 6e74 5d20  tuple[int, int] 
-0000e1e0: 7c20 4e6f 6e65 203d 204e 6f6e 652c 0a20  | None = None,. 
-0000e1f0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-0000e200: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
-0000e210: 7420 7265 6769 6f6e 7320 6173 206e 756d  t regions as num
-0000e220: 7079 2061 7272 6179 2066 726f 6d20 5753  py array from WS
-0000e230: 4920 696d 6167 6520 616e 6420 7265 7475  I image and retu
-0000e240: 726e 2074 6865 6d2e 0a0a 2020 2020 2020  rn them...      
-0000e250: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-0000e260: 2020 2020 696d 673a 2061 2057 5349 5265      img: a WSIRe
-0000e270: 6164 6572 2069 6d61 6765 206f 626a 6563  ader image objec
-0000e280: 7420 6c6f 6164 6564 2066 726f 6d20 6120  t loaded from a 
-0000e290: 6669 6c65 2c20 6f72 206c 6973 7420 6f66  file, or list of
-0000e2a0: 2043 7549 6d61 6765 206f 626a 6563 7473   CuImage objects
-0000e2b0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-0000e2c0: 6174 696f 6e3a 2028 746f 702c 206c 6566  ation: (top, lef
-0000e2d0: 7429 2074 7570 6c65 2067 6976 696e 6720  t) tuple giving 
-0000e2e0: 7468 6520 746f 7020 6c65 6674 2070 6978  the top left pix
-0000e2f0: 656c 2069 6e20 7468 6520 6c65 7665 6c20  el in the level 
-0000e300: 3020 7265 6665 7265 6e63 6520 6672 616d  0 reference fram
-0000e310: 652c 0a20 2020 2020 2020 2020 2020 206f  e,.            o
-0000e320: 7220 6c69 7374 206f 6620 7475 706c 6573  r list of tuples
-0000e330: 2028 6465 6661 756c 743d 2830 2c20 3029   (default=(0, 0)
-0000e340: 290a 2020 2020 2020 2020 2020 2020 7369  ).            si
-0000e350: 7a65 3a20 2868 6569 6768 742c 2077 6964  ze: (height, wid
-0000e360: 7468 2920 7475 706c 6520 6769 7669 6e67  th) tuple giving
-0000e370: 2074 6865 2072 6567 696f 6e20 7369 7a65   the region size
-0000e380: 2c20 6f72 206c 6973 7420 6f66 2074 7570  , or list of tup
-0000e390: 6c65 7320 2864 6566 6175 6c74 2074 6f20  les (default to 
-0000e3a0: 6675 6c6c 2069 6d61 6765 2073 697a 6529  full image size)
-0000e3b0: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000e3c0: 7320 6973 2074 6865 2073 697a 6520 6f66  s is the size of
-0000e3d0: 2069 6d61 6765 2061 7420 7468 6520 6769   image at the gi
-0000e3e0: 7665 6e20 6c65 7665 6c20 2860 6c65 7665  ven level (`leve
-0000e3f0: 6c60 290a 2020 2020 2020 2020 2020 2020  l`).            
-0000e400: 6c65 7665 6c3a 2074 6865 206c 6576 656c  level: the level
-0000e410: 206e 756d 6265 722c 206f 7220 6c69 7374   number, or list
-0000e420: 206f 6620 6c65 7665 6c20 6e75 6d62 6572   of level number
-0000e430: 7320 2864 6566 6175 6c74 3d30 290a 2020  s (default=0).  
-0000e440: 2020 2020 2020 2020 2020 6474 7970 653a            dtype:
-0000e450: 2074 6865 2064 6174 6120 7479 7065 206f   the data type o
-0000e460: 6620 6f75 7470 7574 2069 6d61 6765 0a20  f output image. 
-0000e470: 2020 2020 2020 2020 2020 2067 7269 645f             grid_
-0000e480: 7368 6170 653a 2028 726f 772c 2063 6f6c  shape: (row, col
-0000e490: 756d 6e73 2920 7475 706c 6520 6465 6669  umns) tuple defi
-0000e4a0: 6e65 2061 2067 7269 6420 746f 2065 7874  ne a grid to ext
-0000e4b0: 7261 6374 2070 6174 6368 6573 206f 6e20  ract patches on 
-0000e4c0: 7468 6174 0a20 2020 2020 2020 2020 2020  that.           
-0000e4d0: 2070 6174 6368 5f73 697a 653a 2028 6865   patch_size: (he
-0000e4e0: 6967 6874 2c20 7769 6474 6829 2074 6865  ight, width) the
-0000e4f0: 2073 697a 6520 6f66 2065 7874 7261 6374   size of extract
-0000e500: 6564 2070 6174 6368 6573 2061 7420 7468  ed patches at th
-0000e510: 6520 6769 7665 6e20 6c65 7665 6c0a 2020  e given level.  
-0000e520: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000e530: 2020 2320 5665 7269 6679 2069 6e70 7574    # Verify input
-0000e540: 730a 2020 2020 2020 2020 6966 206c 6576  s.        if lev
-0000e550: 656c 2069 7320 4e6f 6e65 3a0a 2020 2020  el is None:.    
-0000e560: 2020 2020 2020 2020 6c65 7665 6c20 3d20          level = 
-0000e570: 7365 6c66 2e6c 6576 656c 0a20 2020 2020  self.level.     
-0000e580: 2020 206d 6178 5f6c 6576 656c 203d 2073     max_level = s
-0000e590: 656c 662e 5f67 6574 5f6d 6178 5f6c 6576  elf._get_max_lev
-0000e5a0: 656c 2869 6d67 290a 2020 2020 2020 2020  el(img).        
-0000e5b0: 6966 206c 6576 656c 203e 206d 6178 5f6c  if level > max_l
-0000e5c0: 6576 656c 3a0a 2020 2020 2020 2020 2020  evel:.          
-0000e5d0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000e5e0: 6f72 2866 2254 6865 206d 6178 696d 756d  or(f"The maximum
-0000e5f0: 206c 6576 656c 206f 6620 7468 6973 2069   level of this i
-0000e600: 6d61 6765 2069 7320 7b6d 6178 5f6c 6576  mage is {max_lev
-0000e610: 656c 7d20 7768 696c 6520 6c65 7665 6c3d  el} while level=
-0000e620: 7b6c 6576 656c 7d20 6973 2072 6571 7565  {level} is reque
-0000e630: 7374 6564 2921 2229 0a0a 2020 2020 2020  sted)!")..      
-0000e640: 2020 2320 4578 7472 6163 7420 6120 7265    # Extract a re
-0000e650: 6769 6f6e 206f 7220 7468 6520 656e 7469  gion or the enti
-0000e660: 7265 2069 6d61 6765 0a20 2020 2020 2020  re image.       
-0000e670: 2072 6567 696f 6e20 3d20 7365 6c66 2e5f   region = self._
-0000e680: 6578 7472 6163 745f 7265 6769 6f6e 2869  extract_region(i
-0000e690: 6d67 2c20 6c6f 6361 7469 6f6e 3d6c 6f63  mg, location=loc
-0000e6a0: 6174 696f 6e2c 2073 697a 653d 7369 7a65  ation, size=size
-0000e6b0: 2c20 6c65 7665 6c3d 6c65 7665 6c2c 2064  , level=level, d
-0000e6c0: 7479 7065 3d64 7479 7065 290a 0a20 2020  type=dtype)..   
-0000e6d0: 2020 2020 2023 2041 6464 206e 6563 6573       # Add neces
-0000e6e0: 7361 7279 206d 6574 6164 6174 610a 2020  sary metadata.  
-0000e6f0: 2020 2020 2020 6d65 7461 6461 7461 3a20        metadata: 
-0000e700: 6469 6374 203d 207b 7d0a 2020 2020 2020  dict = {}.      
-0000e710: 2020 6d65 7461 6461 7461 5b4d 6574 614b    metadata[MetaK
-0000e720: 6579 732e 5350 4154 4941 4c5f 5348 4150  eys.SPATIAL_SHAP
-0000e730: 455d 203d 206e 702e 6173 6172 7261 7928  E] = np.asarray(
-0000e740: 7265 6769 6f6e 2e73 6861 7065 5b3a 2d31  region.shape[:-1
-0000e750: 5d29 0a20 2020 2020 2020 206d 6574 6164  ]).        metad
-0000e760: 6174 615b 4d65 7461 4b65 7973 2e4f 5249  ata[MetaKeys.ORI
-0000e770: 4749 4e41 4c5f 4348 414e 4e45 4c5f 4449  GINAL_CHANNEL_DI
-0000e780: 4d5d 203d 202d 310a 0a20 2020 2020 2020  M] = -1..       
-0000e790: 2023 204d 616b 6520 6974 2063 6861 6e6e   # Make it chann
-0000e7a0: 656c 2066 6972 7374 0a20 2020 2020 2020  el first.       
-0000e7b0: 2072 6567 696f 6e20 3d20 456e 7375 7265   region = Ensure
-0000e7c0: 4368 616e 6e65 6c46 6972 7374 2829 2872  ChannelFirst()(r
-0000e7d0: 6567 696f 6e2c 206d 6574 6164 6174 6129  egion, metadata)
-0000e7e0: 0a0a 2020 2020 2020 2020 2320 5370 6c69  ..        # Spli
-0000e7f0: 7420 696e 746f 2070 6174 6368 6573 0a20  t into patches. 
-0000e800: 2020 2020 2020 2069 6620 7061 7463 685f         if patch_
-0000e810: 7369 7a65 2069 7320 4e6f 6e65 3a0a 2020  size is None:.  
-0000e820: 2020 2020 2020 2020 2020 7061 7463 6865            patche
-0000e830: 7320 3d20 7265 6769 6f6e 0a20 2020 2020  s = region.     
-0000e840: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e850: 2020 2020 2074 7570 6c65 5f70 6174 6368       tuple_patch
-0000e860: 5f73 697a 6520 3d20 656e 7375 7265 5f74  _size = ensure_t
-0000e870: 7570 6c65 5f72 6570 2870 6174 6368 5f73  uple_rep(patch_s
-0000e880: 697a 652c 2032 290a 2020 2020 2020 2020  ize, 2).        
-0000e890: 2020 2020 7061 7463 6865 7320 3d20 7365      patches = se
-0000e8a0: 6c66 2e5f 6578 7472 6163 745f 7061 7463  lf._extract_patc
-0000e8b0: 6865 7328 0a20 2020 2020 2020 2020 2020  hes(.           
-0000e8c0: 2020 2020 2072 6567 696f 6e2c 2070 6174       region, pat
-0000e8d0: 6368 5f73 697a 653d 7475 706c 655f 7061  ch_size=tuple_pa
-0000e8e0: 7463 685f 7369 7a65 2c20 6772 6964 5f73  tch_size, grid_s
-0000e8f0: 6861 7065 3d67 7269 645f 7368 6170 652c  hape=grid_shape,
-0000e900: 2064 7479 7065 3d64 7479 7065 2020 2320   dtype=dtype  # 
-0000e910: 7479 7065 3a20 6967 6e6f 7265 0a20 2020  type: ignore.   
-0000e920: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000e930: 2020 2020 7265 7475 726e 2070 6174 6368      return patch
-0000e940: 6573 2c20 6d65 7461 6461 7461 0a0a 2020  es, metadata..  
-0000e950: 2020 6465 6620 5f67 6574 5f6d 6178 5f6c    def _get_max_l
-0000e960: 6576 656c 2873 656c 662c 2069 6d67 5f6f  evel(self, img_o
-0000e970: 626a 293a 0a20 2020 2020 2020 2022 2222  bj):.        """
-0000e980: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-0000e990: 7468 6520 6d61 7869 6d75 6d20 6e75 6d62  the maximum numb
-0000e9a0: 6572 206f 6620 6c65 7665 6c73 2069 6e20  er of levels in 
-0000e9b0: 7468 6520 7768 6f6c 6520 736c 6964 6520  the whole slide 
-0000e9c0: 696d 6167 650a 2020 2020 2020 2020 4172  image.        Ar
-0000e9d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0000e9e0: 696d 673a 2074 6865 2077 686f 6c65 2073  img: the whole s
-0000e9f0: 6c69 6465 2069 6d61 6765 206f 626a 6563  lide image objec
-0000ea00: 740a 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
-0000ea10: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0000ea20: 6163 6b65 6e64 203d 3d20 226f 7065 6e73  ackend == "opens
-0000ea30: 6c69 6465 223a 0a20 2020 2020 2020 2020  lide":.         
-0000ea40: 2020 2072 6574 7572 6e20 696d 675f 6f62     return img_ob
-0000ea50: 6a2e 6c65 7665 6c5f 636f 756e 7420 2d20  j.level_count - 
-0000ea60: 310a 2020 2020 2020 2020 6966 2073 656c  1.        if sel
-0000ea70: 662e 6261 636b 656e 6420 3d3d 2022 6375  f.backend == "cu
-0000ea80: 6369 6d22 3a0a 2020 2020 2020 2020 2020  cim":.          
-0000ea90: 2020 7265 7475 726e 2069 6d67 5f6f 626a    return img_obj
-0000eaa0: 2e72 6573 6f6c 7574 696f 6e73 5b22 6c65  .resolutions["le
-0000eab0: 7665 6c5f 636f 756e 7422 5d20 2d20 310a  vel_count"] - 1.
-0000eac0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000ead0: 6261 636b 656e 6420 3d3d 2022 7469 6666  backend == "tiff
-0000eae0: 6669 6c65 223a 0a20 2020 2020 2020 2020  file":.         
-0000eaf0: 2020 2072 6574 7572 6e20 6c65 6e28 696d     return len(im
-0000eb00: 675f 6f62 6a2e 7061 6765 7329 202d 2031  g_obj.pages) - 1
-0000eb10: 0a0a 2020 2020 6465 6620 5f67 6574 5f69  ..    def _get_i
-0000eb20: 6d61 6765 5f73 697a 6528 7365 6c66 2c20  mage_size(self, 
-0000eb30: 696d 672c 2073 697a 652c 206c 6576 656c  img, size, level
-0000eb40: 2c20 6c6f 6361 7469 6f6e 293a 0a20 2020  , location):.   
-0000eb50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000eb60: 2043 616c 6375 6c61 7465 2074 6865 206d   Calculate the m
-0000eb70: 6178 696d 756d 2072 6567 696f 6e20 7369  aximum region si
-0000eb80: 7a65 2066 6f72 2074 6865 2067 6976 656e  ze for the given
-0000eb90: 206c 6576 656c 2061 6e64 2073 7461 7274   level and start
-0000eba0: 696e 6720 6c6f 6361 7469 6f6e 2028 6966  ing location (if
-0000ebb0: 2073 697a 6520 6973 204e 6f6e 6529 2e0a   size is None)..
-0000ebc0: 2020 2020 2020 2020 4e6f 7465 2074 6861          Note tha
-0000ebd0: 7420 7265 6769 6f6e 2073 697a 6520 696e  t region size in
-0000ebe0: 204f 7065 6e53 6c69 6465 2061 6e64 2063   OpenSlide and c
-0000ebf0: 7543 494d 2061 7265 2057 7848 2028 6275  uCIM are WxH (bu
-0000ec00: 7420 7468 6520 6669 6e61 6c20 696d 6167  t the final imag
-0000ec10: 6520 6f75 7470 7574 2077 6f75 6c64 2062  e output would b
-0000ec20: 6520 4878 5729 0a20 2020 2020 2020 2022  e HxW).        "
-0000ec30: 2222 0a20 2020 2020 2020 2069 6620 7369  "".        if si
-0000ec40: 7a65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ze is not None:.
-0000ec50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000ec60: 726e 2073 697a 655b 3a3a 2d31 5d0a 0a20  rn size[::-1].. 
-0000ec70: 2020 2020 2020 206d 6178 5f73 697a 6520         max_size 
-0000ec80: 3d20 5b5d 0a20 2020 2020 2020 2064 6f77  = [].        dow
-0000ec90: 6e73 616d 706c 696e 675f 6661 6374 6f72  nsampling_factor
-0000eca0: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-0000ecb0: 2073 656c 662e 6261 636b 656e 6420 3d3d   self.backend ==
-0000ecc0: 2022 6f70 656e 736c 6964 6522 3a0a 2020   "openslide":.  
-0000ecd0: 2020 2020 2020 2020 2020 646f 776e 7361            downsa
-0000ece0: 6d70 6c69 6e67 5f66 6163 746f 7220 3d20  mpling_factor = 
-0000ecf0: 696d 672e 6c65 7665 6c5f 646f 776e 7361  img.level_downsa
-0000ed00: 6d70 6c65 735b 6c65 7665 6c5d 0a20 2020  mples[level].   
-0000ed10: 2020 2020 2020 2020 206d 6178 5f73 697a           max_siz
-0000ed20: 6520 3d20 696d 672e 6c65 7665 6c5f 6469  e = img.level_di
-0000ed30: 6d65 6e73 696f 6e73 5b6c 6576 656c 5d0a  mensions[level].
-0000ed40: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
-0000ed50: 662e 6261 636b 656e 6420 3d3d 2022 6375  f.backend == "cu
-0000ed60: 6369 6d22 3a0a 2020 2020 2020 2020 2020  cim":.          
-0000ed70: 2020 646f 776e 7361 6d70 6c69 6e67 5f66    downsampling_f
-0000ed80: 6163 746f 7220 3d20 696d 672e 7265 736f  actor = img.reso
-0000ed90: 6c75 7469 6f6e 735b 226c 6576 656c 5f64  lutions["level_d
-0000eda0: 6f77 6e73 616d 706c 6573 225d 5b6c 6576  ownsamples"][lev
-0000edb0: 656c 5d0a 2020 2020 2020 2020 2020 2020  el].            
-0000edc0: 6d61 785f 7369 7a65 203d 2069 6d67 2e72  max_size = img.r
-0000edd0: 6573 6f6c 7574 696f 6e73 5b22 6c65 7665  esolutions["leve
-0000ede0: 6c5f 6469 6d65 6e73 696f 6e73 225d 5b6c  l_dimensions"][l
-0000edf0: 6576 656c 5d0a 0a20 2020 2020 2020 2023  evel]..        #
-0000ee00: 2073 7562 7472 6163 7420 7468 6520 746f   subtract the to
-0000ee10: 7020 6c65 6674 2063 6f72 6e65 7220 6f66  p left corner of
-0000ee20: 2074 6865 2070 6174 6368 2028 6174 2067   the patch (at g
-0000ee30: 6976 656e 206c 6576 656c 2920 6672 6f6d  iven level) from
-0000ee40: 206d 6178 696d 756d 2073 697a 650a 2020   maximum size.  
-0000ee50: 2020 2020 2020 6c6f 6361 7469 6f6e 5f61        location_a
-0000ee60: 745f 6c65 7665 6c20 3d20 2872 6f75 6e64  t_level = (round
-0000ee70: 286c 6f63 6174 696f 6e5b 315d 202f 2064  (location[1] / d
-0000ee80: 6f77 6e73 616d 706c 696e 675f 6661 6374  ownsampling_fact
-0000ee90: 6f72 292c 2072 6f75 6e64 286c 6f63 6174  or), round(locat
-0000eea0: 696f 6e5b 305d 202f 2064 6f77 6e73 616d  ion[0] / downsam
-0000eeb0: 706c 696e 675f 6661 6374 6f72 2929 0a20  pling_factor)). 
-0000eec0: 2020 2020 2020 2073 697a 6520 3d20 5b6d         size = [m
-0000eed0: 6178 5f73 697a 655b 695d 202d 206c 6f63  ax_size[i] - loc
-0000eee0: 6174 696f 6e5f 6174 5f6c 6576 656c 5b69  ation_at_level[i
-0000eef0: 5d20 666f 7220 6920 696e 2072 616e 6765  ] for i in range
-0000ef00: 286c 656e 286d 6178 5f73 697a 6529 295d  (len(max_size))]
-0000ef10: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000ef20: 2073 697a 650a 0a20 2020 2064 6566 205f   size..    def _
-0000ef30: 6578 7472 6163 745f 7265 6769 6f6e 280a  extract_region(.
-0000ef40: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-0000ef50: 2020 2020 2020 696d 675f 6f62 6a2c 0a20        img_obj,. 
-0000ef60: 2020 2020 2020 2073 697a 653a 2074 7570         size: tup
-0000ef70: 6c65 5b69 6e74 2c20 696e 745d 207c 204e  le[int, int] | N
-0000ef80: 6f6e 652c 0a20 2020 2020 2020 206c 6f63  one,.        loc
-0000ef90: 6174 696f 6e3a 2074 7570 6c65 5b69 6e74  ation: tuple[int
-0000efa0: 2c20 696e 745d 203d 2028 302c 2030 292c  , int] = (0, 0),
-0000efb0: 0a20 2020 2020 2020 206c 6576 656c 3a20  .        level: 
-0000efc0: 696e 7420 3d20 302c 0a20 2020 2020 2020  int = 0,.       
-0000efd0: 2064 7479 7065 3a20 4474 7970 654c 696b   dtype: DtypeLik
-0000efe0: 6520 3d20 6e70 2e75 696e 7438 2c0a 2020  e = np.uint8,.  
-0000eff0: 2020 293a 0a20 2020 2020 2020 2069 6620    ):.        if 
-0000f000: 7365 6c66 2e62 6163 6b65 6e64 203d 3d20  self.backend == 
-0000f010: 2274 6966 6666 696c 6522 3a0a 2020 2020  "tifffile":.    
-0000f020: 2020 2020 2020 2020 2320 5265 6164 2074          # Read t
-0000f030: 6865 2065 6e74 6972 6520 696d 6167 650a  he entire image.
-0000f040: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000f050: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
-0000f060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f070: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000f080: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000f090: 2020 2020 2020 2066 2254 6966 6646 696c         f"TiffFil
-0000f0a0: 6520 6261 636b 656e 6420 7265 6164 7320  e backend reads 
-0000f0b0: 7468 6520 656e 7469 7265 2069 6d61 6765  the entire image
-0000f0c0: 206f 6e6c 792c 2073 6f20 7369 7a65 2027   only, so size '
-0000f0d0: 7b73 697a 657d 2727 2073 686f 756c 6420  {size}'' should 
-0000f0e0: 6e6f 7420 6265 2070 726f 7669 6465 6421  not be provided!
-0000f0f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000f100: 2020 2020 2020 2022 466f 7220 6d6f 7265         "For more
-0000f110: 2066 6c65 7869 6269 6c69 7479 206f 7220   flexibility or 
-0000f120: 6578 7472 6163 7469 6e67 2072 6567 696f  extracting regio
-0000f130: 6e73 2c20 706c 6561 7365 2075 7365 2063  ns, please use c
-0000f140: 7543 494d 206f 7220 4f70 656e 536c 6964  uCIM or OpenSlid
-0000f150: 6520 6261 636b 656e 642e 222c 0a20 2020  e backend.",.   
-0000f160: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000f170: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
-0000f180: 6361 7469 6f6e 2021 3d20 2830 2c20 3029  cation != (0, 0)
-0000f190: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f1a0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000f1b0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000f1c0: 2020 2020 2020 2020 6622 5469 6666 4669          f"TiffFi
-0000f1d0: 6c65 2062 6163 6b65 6e64 2072 6561 6473  le backend reads
-0000f1e0: 2074 6865 2065 6e74 6972 6520 696d 6167   the entire imag
-0000f1f0: 6520 6f6e 6c79 2c20 736f 206c 6f63 6174  e only, so locat
-0000f200: 696f 6e20 277b 6c6f 6361 7469 6f6e 7d27  ion '{location}'
-0000f210: 2073 686f 756c 6420 6e6f 7420 6265 2070   should not be p
-0000f220: 726f 7669 6465 6421 222c 0a20 2020 2020  rovided!",.     
-0000f230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000f240: 466f 7220 6d6f 7265 2066 6c65 7869 6269  For more flexibi
-0000f250: 6c69 7479 2061 6e64 2065 7874 7261 6374  lity and extract
-0000f260: 696e 6720 7265 6769 6f6e 732c 2070 6c65  ing regions, ple
-0000f270: 6173 6520 7573 6520 6375 4349 4d20 6f72  ase use cuCIM or
-0000f280: 204f 7065 6e53 6c69 6465 2062 6163 6b65   OpenSlide backe
-0000f290: 6e64 2e22 2c0a 2020 2020 2020 2020 2020  nd.",.          
-0000f2a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000f2b0: 2020 2020 7265 6769 6f6e 203d 2069 6d67      region = img
-0000f2c0: 5f6f 626a 2e61 7361 7272 6179 286c 6576  _obj.asarray(lev
-0000f2d0: 656c 3d6c 6576 656c 290a 2020 2020 2020  el=level).      
-0000f2e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f2f0: 2020 2020 2320 4765 7420 7265 6769 6f6e      # Get region
-0000f300: 2073 697a 6520 746f 2062 6520 6578 7472   size to be extr
-0000f310: 6163 7465 640a 2020 2020 2020 2020 2020  acted.          
-0000f320: 2020 7265 6769 6f6e 5f73 697a 6520 3d20    region_size = 
-0000f330: 7365 6c66 2e5f 6765 745f 696d 6167 655f  self._get_image_
-0000f340: 7369 7a65 2869 6d67 5f6f 626a 2c20 7369  size(img_obj, si
-0000f350: 7a65 2c20 6c65 7665 6c2c 206c 6f63 6174  ze, level, locat
-0000f360: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
-0000f370: 2023 2072 6576 6572 7365 2074 6865 206f   # reverse the o
-0000f380: 7264 6572 206f 6620 6c6f 6361 7469 6f6e  rder of location
-0000f390: 2773 2064 696d 656e 7369 6f6e 7320 746f  's dimensions to
-0000f3a0: 2062 6563 6f6d 6520 5778 4820 2866 6f72   become WxH (for
-0000f3b0: 2063 7543 494d 2061 6e64 204f 7065 6e53   cuCIM and OpenS
-0000f3c0: 6c69 6465 290a 2020 2020 2020 2020 2020  lide).          
-0000f3d0: 2020 7265 6769 6f6e 5f6c 6f63 6174 696f    region_locatio
-0000f3e0: 6e20 3d20 6c6f 6361 7469 6f6e 5b3a 3a2d  n = location[::-
-0000f3f0: 315d 0a20 2020 2020 2020 2020 2020 2023  1].            #
-0000f400: 2045 7874 7261 6374 2061 2072 6567 696f   Extract a regio
-0000f410: 6e20 286f 7220 7468 6520 656e 7469 7265  n (or the entire
-0000f420: 2069 6d61 6765 290a 2020 2020 2020 2020   image).        
-0000f430: 2020 2020 7265 6769 6f6e 203d 2069 6d67      region = img
-0000f440: 5f6f 626a 2e72 6561 645f 7265 6769 6f6e  _obj.read_region
-0000f450: 286c 6f63 6174 696f 6e3d 7265 6769 6f6e  (location=region
-0000f460: 5f6c 6f63 6174 696f 6e2c 2073 697a 653d  _location, size=
-0000f470: 7265 6769 6f6e 5f73 697a 652c 206c 6576  region_size, lev
-0000f480: 656c 3d6c 6576 656c 290a 0a20 2020 2020  el=level)..     
-0000f490: 2020 2072 6567 696f 6e20 3d20 7365 6c66     region = self
-0000f4a0: 2e63 6f6e 7665 7274 5f74 6f5f 7267 625f  .convert_to_rgb_
-0000f4b0: 6172 7261 7928 7265 6769 6f6e 2c20 6474  array(region, dt
-0000f4c0: 7970 6529 0a20 2020 2020 2020 2072 6574  ype).        ret
-0000f4d0: 7572 6e20 7265 6769 6f6e 0a0a 2020 2020  urn region..    
-0000f4e0: 6465 6620 636f 6e76 6572 745f 746f 5f72  def convert_to_r
-0000f4f0: 6762 5f61 7272 6179 2873 656c 662c 2072  gb_array(self, r
-0000f500: 6177 5f72 6567 696f 6e2c 2064 7479 7065  aw_region, dtype
-0000f510: 3a20 4474 7970 654c 696b 6520 3d20 6e70  : DtypeLike = np
-0000f520: 2e75 696e 7438 293a 0a20 2020 2020 2020  .uint8):.       
-0000f530: 2022 2222 436f 6e76 6572 7420 746f 2052   """Convert to R
-0000f540: 4742 206d 6f64 6520 616e 6420 6e75 6d70  GB mode and nump
-0000f550: 7920 6172 7261 7922 2222 0a20 2020 2020  y array""".     
-0000f560: 2020 2069 6620 7365 6c66 2e62 6163 6b65     if self.backe
-0000f570: 6e64 203d 3d20 226f 7065 6e73 6c69 6465  nd == "openslide
-0000f580: 223a 0a20 2020 2020 2020 2020 2020 2023  ":.            #
-0000f590: 2063 6f6e 7665 7274 2074 6f20 5247 420a   convert to RGB.
-0000f5a0: 2020 2020 2020 2020 2020 2020 7261 775f              raw_
-0000f5b0: 7265 6769 6f6e 203d 2072 6177 5f72 6567  region = raw_reg
-0000f5c0: 696f 6e2e 636f 6e76 6572 7428 2252 4742  ion.convert("RGB
-0000f5d0: 2229 0a0a 2020 2020 2020 2020 2320 636f  ")..        # co
-0000f5e0: 6e76 6572 7420 746f 206e 756d 7079 2028  nvert to numpy (
-0000f5f0: 6966 206e 6f74 2061 6c72 6561 6479 2069  if not already i
-0000f600: 6e20 6e75 6d70 7929 0a20 2020 2020 2020  n numpy).       
-0000f610: 2072 6177 5f72 6567 696f 6e20 3d20 6e70   raw_region = np
-0000f620: 2e61 7361 7272 6179 2872 6177 5f72 6567  .asarray(raw_reg
-0000f630: 696f 6e2c 2064 7479 7065 3d64 7479 7065  ion, dtype=dtype
-0000f640: 290a 0a20 2020 2020 2020 2023 2063 6865  )..        # che
-0000f650: 636b 2069 6620 7468 6520 696d 6167 6520  ck if the image 
-0000f660: 6861 7320 7468 7265 6520 6469 6d65 6e73  has three dimens
-0000f670: 696f 6e73 2028 3244 202b 2063 6f6c 6f72  ions (2D + color
-0000f680: 290a 2020 2020 2020 2020 6966 2072 6177  ).        if raw
-0000f690: 5f72 6567 696f 6e2e 6e64 696d 2021 3d20  _region.ndim != 
-0000f6a0: 333a 0a20 2020 2020 2020 2020 2020 2072  3:.            r
-0000f6b0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000f6c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f6d0: 2066 2254 6865 2069 6e70 7574 2069 6d61   f"The input ima
-0000f6e0: 6765 2064 696d 656e 7369 6f6e 2073 686f  ge dimension sho
-0000f6f0: 756c 6420 6265 2033 2062 7574 207b 7261  uld be 3 but {ra
-0000f700: 775f 7265 6769 6f6e 2e6e 6469 6d7d 2069  w_region.ndim} i
-0000f710: 7320 6769 7665 6e2e 2022 0a20 2020 2020  s given. ".     
-0000f720: 2020 2020 2020 2020 2020 2022 6057 5349             "`WSI
-0000f730: 5265 6164 6572 6020 6973 2064 6573 6967  Reader` is desig
-0000f740: 6e65 6420 746f 2077 6f72 6b20 6f6e 6c79  ned to work only
-0000f750: 2077 6974 6820 3244 2063 6f6c 6f72 6564   with 2D colored
-0000f760: 2069 6d61 6765 732e 220a 2020 2020 2020   images.".      
-0000f770: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000f780: 2023 2063 6865 636b 2069 6620 7468 6520   # check if the 
-0000f790: 636f 6c6f 7220 6368 616e 6e65 6c20 6973  color channel is
-0000f7a0: 2033 2028 5247 4229 206f 7220 3420 2852   3 (RGB) or 4 (R
-0000f7b0: 4742 4129 0a20 2020 2020 2020 2069 6620  GBA).        if 
-0000f7c0: 7261 775f 7265 6769 6f6e 2e73 6861 7065  raw_region.shape
-0000f7d0: 5b2d 315d 206e 6f74 2069 6e20 5b33 2c20  [-1] not in [3, 
-0000f7e0: 345d 3a0a 2020 2020 2020 2020 2020 2020  4]:.            
-0000f7f0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000f800: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f810: 2020 6622 5468 6572 6520 7368 6f75 6c64    f"There should
-0000f820: 2062 6520 7468 7265 6520 6f72 2066 6f75   be three or fou
-0000f830: 7220 636f 6c6f 7220 6368 616e 6e65 6c73  r color channels
-0000f840: 2062 7574 207b 7261 775f 7265 6769 6f6e   but {raw_region
-0000f850: 2e73 6861 7065 5b2d 315d 7d20 6973 2067  .shape[-1]} is g
-0000f860: 6976 656e 2e20 220a 2020 2020 2020 2020  iven. ".        
-0000f870: 2020 2020 2020 2020 2260 5753 4952 6561          "`WSIRea
-0000f880: 6465 7260 2069 7320 6465 7369 676e 6564  der` is designed
-0000f890: 2074 6f20 776f 726b 206f 6e6c 7920 7769   to work only wi
-0000f8a0: 7468 2032 4420 636f 6c6f 7265 6420 696d  th 2D colored im
-0000f8b0: 6167 6573 2e22 0a20 2020 2020 2020 2020  ages.".         
-0000f8c0: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0000f8d0: 7265 6d6f 7665 2061 6c70 6861 2063 6861  remove alpha cha
-0000f8e0: 6e6e 656c 2069 6620 6578 6973 7420 2852  nnel if exist (R
-0000f8f0: 4742 4129 0a20 2020 2020 2020 2069 6620  GBA).        if 
-0000f900: 7261 775f 7265 6769 6f6e 2e73 6861 7065  raw_region.shape
-0000f910: 5b2d 315d 203e 2033 3a0a 2020 2020 2020  [-1] > 3:.      
-0000f920: 2020 2020 2020 7261 775f 7265 6769 6f6e        raw_region
-0000f930: 203d 2072 6177 5f72 6567 696f 6e5b 2e2e   = raw_region[..
-0000f940: 2e2c 203a 335d 0a0a 2020 2020 2020 2020  ., :3]..        
-0000f950: 7265 7475 726e 2072 6177 5f72 6567 696f  return raw_regio
-0000f960: 6e0a 0a20 2020 2064 6566 205f 6578 7472  n..    def _extr
-0000f970: 6163 745f 7061 7463 6865 7328 0a20 2020  act_patches(.   
-0000f980: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0000f990: 2020 2072 6567 696f 6e3a 206e 702e 6e64     region: np.nd
-0000f9a0: 6172 7261 792c 0a20 2020 2020 2020 2067  array,.        g
-0000f9b0: 7269 645f 7368 6170 653a 2074 7570 6c65  rid_shape: tuple
-0000f9c0: 5b69 6e74 2c20 696e 745d 203d 2028 312c  [int, int] = (1,
-0000f9d0: 2031 292c 0a20 2020 2020 2020 2070 6174   1),.        pat
-0000f9e0: 6368 5f73 697a 653a 2074 7570 6c65 5b69  ch_size: tuple[i
-0000f9f0: 6e74 2c20 696e 745d 207c 204e 6f6e 6520  nt, int] | None 
-0000fa00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000fa10: 6474 7970 653a 2044 7479 7065 4c69 6b65  dtype: DtypeLike
-0000fa20: 203d 206e 702e 7569 6e74 382c 0a20 2020   = np.uint8,.   
-0000fa30: 2029 3a0a 2020 2020 2020 2020 6966 2070   ):.        if p
-0000fa40: 6174 6368 5f73 697a 6520 6973 204e 6f6e  atch_size is Non
-0000fa50: 6520 616e 6420 6772 6964 5f73 6861 7065  e and grid_shape
-0000fa60: 203d 3d20 2831 2c20 3129 3a0a 2020 2020   == (1, 1):.    
-0000fa70: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000fa80: 6567 696f 6e0a 0a20 2020 2020 2020 206e  egion..        n
-0000fa90: 5f70 6174 6368 6573 203d 2067 7269 645f  _patches = grid_
-0000faa0: 7368 6170 655b 305d 202a 2067 7269 645f  shape[0] * grid_
-0000fab0: 7368 6170 655b 315d 0a20 2020 2020 2020  shape[1].       
-0000fac0: 2072 6567 696f 6e5f 7369 7a65 203d 2072   region_size = r
-0000fad0: 6567 696f 6e2e 7368 6170 655b 313a 5d0a  egion.shape[1:].
-0000fae0: 0a20 2020 2020 2020 2069 6620 7061 7463  .        if patc
-0000faf0: 685f 7369 7a65 2069 7320 4e6f 6e65 3a0a  h_size is None:.
-0000fb00: 2020 2020 2020 2020 2020 2020 7061 7463              patc
-0000fb10: 685f 7369 7a65 203d 2028 7265 6769 6f6e  h_size = (region
-0000fb20: 5f73 697a 655b 305d 202f 2f20 6772 6964  _size[0] // grid
-0000fb30: 5f73 6861 7065 5b30 5d2c 2072 6567 696f  _shape[0], regio
-0000fb40: 6e5f 7369 7a65 5b31 5d20 2f2f 2067 7269  n_size[1] // gri
-0000fb50: 645f 7368 6170 655b 315d 290a 0a20 2020  d_shape[1])..   
-0000fb60: 2020 2020 2023 2073 706c 6974 2074 6865       # split the
-0000fb70: 2072 6567 696f 6e20 696e 746f 2070 6174   region into pat
-0000fb80: 6368 6573 206f 6e20 7468 6520 6772 6964  ches on the grid
-0000fb90: 2061 6e64 2063 656e 7465 7220 6372 6f70   and center crop
-0000fba0: 2074 6865 6d20 746f 2070 6174 6368 2073   them to patch s
-0000fbb0: 697a 650a 2020 2020 2020 2020 666c 6174  ize.        flat
-0000fbc0: 5f70 6174 6368 5f67 7269 6420 3d20 6e70  _patch_grid = np
-0000fbd0: 2e7a 6572 6f73 2828 6e5f 7061 7463 6865  .zeros((n_patche
-0000fbe0: 732c 2033 2c20 7061 7463 685f 7369 7a65  s, 3, patch_size
-0000fbf0: 5b30 5d2c 2070 6174 6368 5f73 697a 655b  [0], patch_size[
-0000fc00: 315d 292c 2064 7479 7065 3d64 7479 7065  1]), dtype=dtype
-0000fc10: 290a 2020 2020 2020 2020 7374 6172 745f  ).        start_
-0000fc20: 706f 696e 7473 203d 205b 0a20 2020 2020  points = [.     
-0000fc30: 2020 2020 2020 206e 702e 726f 756e 6428         np.round(
-0000fc40: 7265 6769 6f6e 5f73 697a 655b 695d 202a  region_size[i] *
-0000fc50: 2028 302e 3520 2b20 6e70 2e61 7261 6e67   (0.5 + np.arang
-0000fc60: 6528 6772 6964 5f73 6861 7065 5b69 5d29  e(grid_shape[i])
-0000fc70: 2920 2f20 6772 6964 5f73 6861 7065 5b69  ) / grid_shape[i
-0000fc80: 5d20 2d20 7061 7463 685f 7369 7a65 5b69  ] - patch_size[i
-0000fc90: 5d20 2f20 3229 2e61 7374 7970 6528 696e  ] / 2).astype(in
-0000fca0: 7429 0a20 2020 2020 2020 2020 2020 2066  t).            f
-0000fcb0: 6f72 2069 2069 6e20 7261 6e67 6528 3229  or i in range(2)
-0000fcc0: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-0000fcd0: 2020 2069 6478 203d 2030 0a20 2020 2020     idx = 0.     
-0000fce0: 2020 2066 6f72 2079 5f73 7461 7274 2069     for y_start i
-0000fcf0: 6e20 7374 6172 745f 706f 696e 7473 5b31  n start_points[1
-0000fd00: 5d3a 0a20 2020 2020 2020 2020 2020 2066  ]:.            f
-0000fd10: 6f72 2078 5f73 7461 7274 2069 6e20 7374  or x_start in st
-0000fd20: 6172 745f 706f 696e 7473 5b30 5d3a 0a20  art_points[0]:. 
-0000fd30: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0000fd40: 5f65 6e64 203d 2078 5f73 7461 7274 202b  _end = x_start +
-0000fd50: 2070 6174 6368 5f73 697a 655b 305d 0a20   patch_size[0]. 
-0000fd60: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-0000fd70: 5f65 6e64 203d 2079 5f73 7461 7274 202b  _end = y_start +
-0000fd80: 2070 6174 6368 5f73 697a 655b 315d 0a20   patch_size[1]. 
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000fda0: 6c61 745f 7061 7463 685f 6772 6964 5b69  lat_patch_grid[i
-0000fdb0: 6478 5d20 3d20 7265 6769 6f6e 5b3a 2c20  dx] = region[:, 
-0000fdc0: 785f 7374 6172 743a 785f 656e 642c 2079  x_start:x_end, y
-0000fdd0: 5f73 7461 7274 3a79 5f65 6e64 5d0a 2020  _start:y_end].  
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 6964                id
-0000fdf0: 7820 2b3d 2031 0a0a 2020 2020 2020 2020  x += 1..        
-0000fe00: 7265 7475 726e 2066 6c61 745f 7061 7463  return flat_patc
-0000fe10: 685f 6772 6964 0a0a 0a40 6461 7461 636c  h_grid...@datacl
-0000fe20: 6173 730a 636c 6173 7320 4e72 7264 496d  ass.class NrrdIm
-0000fe30: 6167 653a 0a20 2020 2022 2222 436c 6173  age:.    """Clas
-0000fe40: 7320 746f 2077 7261 7020 6e72 7264 2069  s to wrap nrrd i
-0000fe50: 6d61 6765 2061 7272 6179 2061 6e64 206d  mage array and m
-0000fe60: 6574 6164 6174 6120 6865 6164 6572 2222  etadata header""
-0000fe70: 220a 0a20 2020 2061 7272 6179 3a20 6e70  "..    array: np
-0000fe80: 2e6e 6461 7272 6179 0a20 2020 2068 6561  .ndarray.    hea
-0000fe90: 6465 723a 2064 6963 740a 0a0a 4072 6571  der: dict...@req
-0000fea0: 7569 7265 5f70 6b67 2870 6b67 5f6e 616d  uire_pkg(pkg_nam
-0000feb0: 653d 226e 7272 6422 290a 636c 6173 7320  e="nrrd").class 
-0000fec0: 4e72 7264 5265 6164 6572 2849 6d61 6765  NrrdReader(Image
-0000fed0: 5265 6164 6572 293a 0a20 2020 2022 2222  Reader):.    """
-0000fee0: 0a20 2020 204c 6f61 6420 4e52 5244 2066  .    Load NRRD f
-0000fef0: 6f72 6d61 7420 696d 6167 6573 2062 6173  ormat images bas
-0000ff00: 6564 206f 6e20 7079 6e72 7264 206c 6962  ed on pynrrd lib
-0000ff10: 7261 7279 2e0a 0a20 2020 2041 7267 733a  rary...    Args:
-0000ff20: 0a20 2020 2020 2020 2063 6861 6e6e 656c  .        channel
-0000ff30: 5f64 696d 3a20 7468 6520 6368 616e 6e65  _dim: the channe
-0000ff40: 6c20 6469 6d65 6e73 696f 6e20 6f66 2074  l dimension of t
-0000ff50: 6865 2069 6e70 7574 2069 6d61 6765 2c20  he input image, 
-0000ff60: 6465 6661 756c 7420 6973 204e 6f6e 652e  default is None.
-0000ff70: 0a20 2020 2020 2020 2020 2020 2054 6869  .            Thi
-0000ff80: 7320 6973 2075 7365 6420 746f 2073 6574  s is used to set
-0000ff90: 206f 7269 6769 6e61 6c5f 6368 616e 6e65   original_channe
-0000ffa0: 6c5f 6469 6d20 696e 2074 6865 206d 6574  l_dim in the met
-0000ffb0: 6164 6174 612c 2045 6e73 7572 6543 6861  adata, EnsureCha
-0000ffc0: 6e6e 656c 4669 7273 7444 2072 6561 6473  nnelFirstD reads
-0000ffd0: 2074 6869 7320 6669 656c 642e 0a20 2020   this field..   
-0000ffe0: 2020 2020 2020 2020 2049 6620 4e6f 6e65           If None
-0000fff0: 2c20 606f 7269 6769 6e61 6c5f 6368 616e  , `original_chan
-00010000: 6e65 6c5f 6469 6d60 2077 696c 6c20 6265  nel_dim` will be
-00010010: 2065 6974 6865 7220 606e 6f5f 6368 616e   either `no_chan
-00010020: 6e65 6c60 206f 7220 6030 602e 0a20 2020  nel` or `0`..   
-00010030: 2020 2020 2020 2020 204e 5252 4420 6669           NRRD fi
-00010040: 6c65 7320 6172 6520 7573 7561 6c6c 7920  les are usually 
-00010050: 2263 6861 6e6e 656c 2066 6972 7374 222e  "channel first".
-00010060: 0a20 2020 2020 2020 2064 7479 7065 3a20  .        dtype: 
-00010070: 6474 7970 6520 6f66 2074 6865 2064 6174  dtype of the dat
-00010080: 6120 6172 7261 7920 7768 656e 206c 6f61  a array when loa
-00010090: 6469 6e67 2069 6d61 6765 2e0a 2020 2020  ding image..    
-000100a0: 2020 2020 696e 6465 785f 6f72 6465 723a      index_order:
-000100b0: 2053 7065 6369 6679 2077 6865 7468 6572   Specify whether
-000100c0: 2074 6865 2072 6574 7572 6e65 6420 6461   the returned da
-000100d0: 7461 2061 7272 6179 2073 686f 756c 6420  ta array should 
-000100e0: 6265 2069 6e20 432d 6f72 6465 7220 28e2  be in C-order (.
-000100f0: 8098 43e2 8099 2920 6f72 2046 6f72 7472  ..C...) or Fortr
-00010100: 616e 2d6f 7264 6572 2028 e280 9846 e280  an-order (...F..
-00010110: 9929 2e0a 2020 2020 2020 2020 2020 2020  .)..            
-00010120: 4e75 6d70 7920 6973 2075 7375 616c 6c79  Numpy is usually
-00010130: 2069 6e20 432d 6f72 6465 722c 2062 7574   in C-order, but
-00010140: 2064 6566 6175 6c74 206f 6e20 7468 6520   default on the 
-00010150: 4e52 5244 2068 6561 6465 7220 6973 2046  NRRD header is F
-00010160: 0a20 2020 2020 2020 2061 6666 696e 655f  .        affine_
-00010170: 6c70 735f 746f 5f72 6173 3a20 7768 6574  lps_to_ras: whet
-00010180: 6865 7220 746f 2063 6f6e 7665 7274 2074  her to convert t
-00010190: 6865 2061 6666 696e 6520 6d61 7472 6978  he affine matrix
-000101a0: 2066 726f 6d20 224c 5053 2220 746f 2022   from "LPS" to "
-000101b0: 5241 5322 2e20 4465 6661 756c 7473 2074  RAS". Defaults t
-000101c0: 6f20 6060 5472 7565 6060 2e0a 2020 2020  o ``True``..    
-000101d0: 2020 2020 2020 2020 5365 7420 746f 2060          Set to `
-000101e0: 6054 7275 6560 6020 746f 2062 6520 636f  `True`` to be co
-000101f0: 6e73 6973 7465 6e74 2077 6974 6820 6060  nsistent with ``
-00010200: 4e69 6261 6265 6c52 6561 6465 7260 602c  NibabelReader``,
-00010210: 206f 7468 6572 7769 7365 2074 6865 2061   otherwise the a
-00010220: 6666 696e 6520 6d61 7472 6978 2069 7320  ffine matrix is 
-00010230: 756e 6d6f 6469 6669 6564 2e0a 0a20 2020  unmodified...   
-00010240: 2020 2020 206b 7761 7267 733a 2061 6464       kwargs: add
-00010250: 6974 696f 6e61 6c20 6172 6773 2066 6f72  itional args for
-00010260: 2060 6e72 7264 2e72 6561 6460 2041 5049   `nrrd.read` API
-00010270: 2e20 6d6f 7265 2064 6574 6169 6c73 2061  . more details a
-00010280: 626f 7574 2061 7661 696c 6162 6c65 2061  bout available a
-00010290: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-000102a0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-000102b0: 636f 6d2f 6d68 652f 7079 6e72 7264 2f62  com/mhe/pynrrd/b
-000102c0: 6c6f 622f 6d61 7374 6572 2f6e 7272 642f  lob/master/nrrd/
-000102d0: 7265 6164 6572 2e70 790a 0a20 2020 2022  reader.py..    "
-000102e0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
-000102f0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-00010300: 6c66 2c0a 2020 2020 2020 2020 6368 616e  lf,.        chan
-00010310: 6e65 6c5f 6469 6d3a 2073 7472 207c 2069  nel_dim: str | i
-00010320: 6e74 207c 204e 6f6e 6520 3d20 4e6f 6e65  nt | None = None
-00010330: 2c0a 2020 2020 2020 2020 6474 7970 653a  ,.        dtype:
-00010340: 206e 702e 6474 7970 6520 7c20 7479 7065   np.dtype | type
-00010350: 207c 2073 7472 207c 204e 6f6e 6520 3d20   | str | None = 
-00010360: 6e70 2e66 6c6f 6174 3332 2c0a 2020 2020  np.float32,.    
-00010370: 2020 2020 696e 6465 785f 6f72 6465 723a      index_order:
-00010380: 2073 7472 203d 2022 4622 2c0a 2020 2020   str = "F",.    
-00010390: 2020 2020 6166 6669 6e65 5f6c 7073 5f74      affine_lps_t
-000103a0: 6f5f 7261 733a 2062 6f6f 6c20 3d20 5472  o_ras: bool = Tr
-000103b0: 7565 2c0a 2020 2020 2020 2020 2a2a 6b77  ue,.        **kw
-000103c0: 6172 6773 2c0a 2020 2020 293a 0a20 2020  args,.    ):.   
-000103d0: 2020 2020 2073 656c 662e 6368 616e 6e65       self.channe
-000103e0: 6c5f 6469 6d20 3d20 666c 6f61 7428 226e  l_dim = float("n
-000103f0: 616e 2229 2069 6620 6368 616e 6e65 6c5f  an") if channel_
-00010400: 6469 6d20 3d3d 2022 6e6f 5f63 6861 6e6e  dim == "no_chann
-00010410: 656c 2220 656c 7365 2063 6861 6e6e 656c  el" else channel
-00010420: 5f64 696d 0a20 2020 2020 2020 2073 656c  _dim.        sel
-00010430: 662e 6474 7970 6520 3d20 6474 7970 650a  f.dtype = dtype.
-00010440: 2020 2020 2020 2020 7365 6c66 2e69 6e64          self.ind
-00010450: 6578 5f6f 7264 6572 203d 2069 6e64 6578  ex_order = index
-00010460: 5f6f 7264 6572 0a20 2020 2020 2020 2073  _order.        s
-00010470: 656c 662e 6166 6669 6e65 5f6c 7073 5f74  elf.affine_lps_t
-00010480: 6f5f 7261 7320 3d20 6166 6669 6e65 5f6c  o_ras = affine_l
-00010490: 7073 5f74 6f5f 7261 730a 2020 2020 2020  ps_to_ras.      
-000104a0: 2020 7365 6c66 2e6b 7761 7267 7320 3d20    self.kwargs = 
-000104b0: 6b77 6172 6773 0a0a 2020 2020 6465 6620  kwargs..    def 
-000104c0: 7665 7269 6679 5f73 7566 6669 7828 7365  verify_suffix(se
-000104d0: 6c66 2c20 6669 6c65 6e61 6d65 3a20 5365  lf, filename: Se
-000104e0: 7175 656e 6365 5b50 6174 684c 696b 655d  quence[PathLike]
-000104f0: 207c 2050 6174 684c 696b 6529 202d 3e20   | PathLike) -> 
-00010500: 626f 6f6c 3a0a 2020 2020 2020 2020 2222  bool:.        ""
-00010510: 220a 2020 2020 2020 2020 5665 7269 6679  ".        Verify
-00010520: 2077 6865 7468 6572 2074 6865 2073 7065   whether the spe
-00010530: 6369 6669 6564 2060 6669 6c65 6e61 6d65  cified `filename
-00010540: 6020 6973 2073 7570 706f 7274 6564 2062  ` is supported b
-00010550: 7920 7079 6e72 7264 2072 6561 6465 722e  y pynrrd reader.
-00010560: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00010570: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00010580: 6e61 6d65 3a20 6669 6c65 206e 616d 6520  name: file name 
-00010590: 6f72 2061 206c 6973 7420 6f66 2066 696c  or a list of fil
-000105a0: 6520 6e61 6d65 7320 746f 2072 6561 642e  e names to read.
-000105b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000105c0: 2069 6620 6120 6c69 7374 206f 6620 6669   if a list of fi
-000105d0: 6c65 732c 2076 6572 6966 7920 616c 6c20  les, verify all 
-000105e0: 7468 6520 7375 6666 6978 6573 2e0a 0a20  the suffixes... 
-000105f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010600: 2020 2073 7566 6669 7865 733a 2053 6571     suffixes: Seq
-00010610: 7565 6e63 655b 7374 725d 203d 205b 226e  uence[str] = ["n
-00010620: 7272 6422 2c20 2273 6567 2e6e 7272 6422  rrd", "seg.nrrd"
-00010630: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-00010640: 2068 6173 5f6e 7272 6420 616e 6420 6973   has_nrrd and is
-00010650: 5f73 7570 706f 7274 6564 5f66 6f72 6d61  _supported_forma
-00010660: 7428 6669 6c65 6e61 6d65 2c20 7375 6666  t(filename, suff
-00010670: 6978 6573 290a 0a20 2020 2064 6566 2072  ixes)..    def r
-00010680: 6561 6428 7365 6c66 2c20 6461 7461 3a20  ead(self, data: 
-00010690: 5365 7175 656e 6365 5b50 6174 684c 696b  Sequence[PathLik
-000106a0: 655d 207c 2050 6174 684c 696b 652c 202a  e] | PathLike, *
-000106b0: 2a6b 7761 7267 7329 202d 3e20 5365 7175  *kwargs) -> Sequ
-000106c0: 656e 6365 5b41 6e79 5d20 7c20 416e 793a  ence[Any] | Any:
-000106d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000106e0: 2020 2020 2052 6561 6420 696d 6167 6520       Read image 
-000106f0: 6461 7461 2066 726f 6d20 7370 6563 6966  data from specif
-00010700: 6965 6420 6669 6c65 206f 7220 6669 6c65  ied file or file
-00010710: 732e 0a20 2020 2020 2020 204e 6f74 6520  s..        Note 
-00010720: 7468 6174 2069 7420 7265 7475 726e 7320  that it returns 
-00010730: 6120 6461 7461 206f 626a 6563 7420 6f72  a data object or
-00010740: 2061 2073 6571 7565 6e63 6520 6f66 2064   a sequence of d
-00010750: 6174 6120 6f62 6a65 6374 732e 0a0a 2020  ata objects...  
-00010760: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00010770: 2020 2020 2020 2020 6461 7461 3a20 6669          data: fi
-00010780: 6c65 206e 616d 6520 6f72 2061 206c 6973  le name or a lis
-00010790: 7420 6f66 2066 696c 6520 6e61 6d65 7320  t of file names 
-000107a0: 746f 2072 6561 642e 0a20 2020 2020 2020  to read..       
-000107b0: 2020 2020 206b 7761 7267 733a 2061 6464       kwargs: add
-000107c0: 6974 696f 6e61 6c20 6172 6773 2066 6f72  itional args for
-000107d0: 2061 6374 7561 6c20 6072 6561 6460 2041   actual `read` A
-000107e0: 5049 206f 6620 3372 6420 7061 7274 7920  PI of 3rd party 
-000107f0: 6c69 6273 2e0a 0a20 2020 2020 2020 2022  libs...        "
-00010800: 2222 0a20 2020 2020 2020 2069 6d67 5f3a  "".        img_:
-00010810: 206c 6973 7420 3d20 5b5d 0a20 2020 2020   list = [].     
-00010820: 2020 2066 696c 656e 616d 6573 3a20 5365     filenames: Se
-00010830: 7175 656e 6365 5b50 6174 684c 696b 655d  quence[PathLike]
-00010840: 203d 2065 6e73 7572 655f 7475 706c 6528   = ensure_tuple(
-00010850: 6461 7461 290a 2020 2020 2020 2020 6b77  data).        kw
-00010860: 6172 6773 5f20 3d20 7365 6c66 2e6b 7761  args_ = self.kwa
-00010870: 7267 732e 636f 7079 2829 0a20 2020 2020  rgs.copy().     
-00010880: 2020 206b 7761 7267 735f 2e75 7064 6174     kwargs_.updat
-00010890: 6528 6b77 6172 6773 290a 2020 2020 2020  e(kwargs).      
-000108a0: 2020 666f 7220 6e61 6d65 2069 6e20 6669    for name in fi
-000108b0: 6c65 6e61 6d65 733a 0a20 2020 2020 2020  lenames:.       
-000108c0: 2020 2020 206e 7272 645f 696d 6167 6520       nrrd_image 
-000108d0: 3d20 4e72 7264 496d 6167 6528 2a6e 7272  = NrrdImage(*nrr
-000108e0: 642e 7265 6164 286e 616d 652c 2069 6e64  d.read(name, ind
-000108f0: 6578 5f6f 7264 6572 3d73 656c 662e 696e  ex_order=self.in
-00010900: 6465 785f 6f72 6465 722c 202a 6b77 6172  dex_order, *kwar
-00010910: 6773 5f29 290a 2020 2020 2020 2020 2020  gs_)).          
-00010920: 2020 696d 675f 2e61 7070 656e 6428 6e72    img_.append(nr
-00010930: 7264 5f69 6d61 6765 290a 2020 2020 2020  rd_image).      
-00010940: 2020 7265 7475 726e 2069 6d67 5f20 6966    return img_ if
-00010950: 206c 656e 2866 696c 656e 616d 6573 2920   len(filenames) 
-00010960: 3e20 3120 656c 7365 2069 6d67 5f5b 305d  > 1 else img_[0]
-00010970: 0a0a 2020 2020 6465 6620 6765 745f 6461  ..    def get_da
-00010980: 7461 2873 656c 662c 2069 6d67 3a20 4e72  ta(self, img: Nr
-00010990: 7264 496d 6167 6520 7c20 6c69 7374 5b4e  rdImage | list[N
-000109a0: 7272 6449 6d61 6765 5d29 202d 3e20 7475  rrdImage]) -> tu
-000109b0: 706c 655b 6e70 2e6e 6461 7272 6179 2c20  ple[np.ndarray, 
-000109c0: 6469 6374 5d3a 0a20 2020 2020 2020 2022  dict]:.        "
-000109d0: 2222 0a20 2020 2020 2020 2045 7874 7261  "".        Extra
-000109e0: 6374 2064 6174 6120 6172 7261 7920 616e  ct data array an
-000109f0: 6420 6d65 7461 6461 7461 2066 726f 6d20  d metadata from 
-00010a00: 6c6f 6164 6564 2069 6d61 6765 2061 6e64  loaded image and
-00010a10: 2072 6574 7572 6e20 7468 656d 2e0a 2020   return them..  
-00010a20: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00010a30: 696f 6e20 6d75 7374 2072 6574 7572 6e20  ion must return 
-00010a40: 7477 6f20 6f62 6a65 6374 732c 2074 6865  two objects, the
-00010a50: 2066 6972 7374 2069 7320 6120 6e75 6d70   first is a nump
-00010a60: 7920 6172 7261 7920 6f66 2069 6d61 6765  y array of image
-00010a70: 2064 6174 612c 0a20 2020 2020 2020 2074   data,.        t
-00010a80: 6865 2073 6563 6f6e 6420 6973 2061 2064  he second is a d
-00010a90: 6963 7469 6f6e 6172 7920 6f66 206d 6574  ictionary of met
-00010aa0: 6164 6174 612e 0a0a 2020 2020 2020 2020  adata...        
-00010ab0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00010ac0: 2020 696d 673a 2061 2060 4e72 7264 496d    img: a `NrrdIm
-00010ad0: 6167 6560 206c 6f61 6465 6420 6672 6f6d  age` loaded from
-00010ae0: 2061 6e20 696d 6167 6520 6669 6c65 206f   an image file o
-00010af0: 7220 6120 6c69 7374 206f 6620 696d 6167  r a list of imag
-00010b00: 6520 6f62 6a65 6374 732e 0a0a 2020 2020  e objects...    
-00010b10: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010b20: 696d 675f 6172 7261 793a 206c 6973 745b  img_array: list[
-00010b30: 6e70 2e6e 6461 7272 6179 5d20 3d20 5b5d  np.ndarray] = []
-00010b40: 0a20 2020 2020 2020 2063 6f6d 7061 7469  .        compati
-00010b50: 626c 655f 6d65 7461 3a20 6469 6374 203d  ble_meta: dict =
-00010b60: 207b 7d0a 0a20 2020 2020 2020 2066 6f72   {}..        for
-00010b70: 2069 2069 6e20 656e 7375 7265 5f74 7570   i in ensure_tup
-00010b80: 6c65 2869 6d67 293a 0a20 2020 2020 2020  le(img):.       
-00010b90: 2020 2020 2064 6174 6120 3d20 692e 6172       data = i.ar
-00010ba0: 7261 792e 6173 7479 7065 2873 656c 662e  ray.astype(self.
-00010bb0: 6474 7970 6529 0a20 2020 2020 2020 2020  dtype).         
-00010bc0: 2020 2069 6d67 5f61 7272 6179 2e61 7070     img_array.app
-00010bd0: 656e 6428 6461 7461 290a 2020 2020 2020  end(data).      
-00010be0: 2020 2020 2020 6865 6164 6572 203d 2064        header = d
-00010bf0: 6963 7428 692e 6865 6164 6572 290a 2020  ict(i.header).  
-00010c00: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00010c10: 662e 696e 6465 785f 6f72 6465 7220 3d3d  f.index_order ==
-00010c20: 2022 4322 3a0a 2020 2020 2020 2020 2020   "C":.          
-00010c30: 2020 2020 2020 6865 6164 6572 203d 2073        header = s
-00010c40: 656c 662e 5f63 6f6e 7665 7274 5f66 5f74  elf._convert_f_t
-00010c50: 6f5f 635f 6f72 6465 7228 6865 6164 6572  o_c_order(header
-00010c60: 290a 2020 2020 2020 2020 2020 2020 6865  ).            he
-00010c70: 6164 6572 5b4d 6574 614b 6579 732e 4f52  ader[MetaKeys.OR
-00010c80: 4947 494e 414c 5f41 4646 494e 455d 203d  IGINAL_AFFINE] =
-00010c90: 2073 656c 662e 5f67 6574 5f61 6666 696e   self._get_affin
-00010ca0: 6528 6929 0a0a 2020 2020 2020 2020 2020  e(i)..          
-00010cb0: 2020 6966 2073 656c 662e 6166 6669 6e65    if self.affine
-00010cc0: 5f6c 7073 5f74 6f5f 7261 733a 0a20 2020  _lps_to_ras:.   
-00010cd0: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-00010ce0: 6465 7220 3d20 7365 6c66 2e5f 7377 6974  der = self._swit
-00010cf0: 6368 5f6c 7073 5f72 6173 2868 6561 6465  ch_lps_ras(heade
-00010d00: 7229 0a0a 2020 2020 2020 2020 2020 2020  r)..            
-00010d10: 6865 6164 6572 5b4d 6574 614b 6579 732e  header[MetaKeys.
-00010d20: 4146 4649 4e45 5d20 3d20 6865 6164 6572  AFFINE] = header
-00010d30: 5b4d 6574 614b 6579 732e 4f52 4947 494e  [MetaKeys.ORIGIN
-00010d40: 414c 5f41 4646 494e 455d 2e63 6f70 7928  AL_AFFINE].copy(
-00010d50: 290a 2020 2020 2020 2020 2020 2020 6865  ).            he
-00010d60: 6164 6572 5b4d 6574 614b 6579 732e 5350  ader[MetaKeys.SP
-00010d70: 4154 4941 4c5f 5348 4150 455d 203d 2068  ATIAL_SHAPE] = h
-00010d80: 6561 6465 725b 2273 697a 6573 225d 0a20  eader["sizes"]. 
-00010d90: 2020 2020 2020 2020 2020 205b 6865 6164             [head
-00010da0: 6572 2e70 6f70 286b 2920 666f 7220 6b20  er.pop(k) for k 
-00010db0: 696e 2028 2273 697a 6573 222c 2022 7370  in ("sizes", "sp
-00010dc0: 6163 6520 6f72 6967 696e 222c 2022 7370  ace origin", "sp
-00010dd0: 6163 6520 6469 7265 6374 696f 6e73 2229  ace directions")
-00010de0: 5d20 2023 2072 6d20 6475 706c 6963 6174  ]  # rm duplicat
-00010df0: 6564 2064 6174 6120 696e 2068 6561 6465  ed data in heade
-00010e00: 720a 0a20 2020 2020 2020 2020 2020 2069  r..            i
-00010e10: 6620 7365 6c66 2e63 6861 6e6e 656c 5f64  f self.channel_d
-00010e20: 696d 2069 7320 4e6f 6e65 3a20 2023 2064  im is None:  # d
-00010e30: 6566 6175 6c74 2074 6f20 226e 6f5f 6368  efault to "no_ch
-00010e40: 616e 6e65 6c22 206f 7220 2d31 0a20 2020  annel" or -1.   
-00010e50: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-00010e60: 6465 725b 4d65 7461 4b65 7973 2e4f 5249  der[MetaKeys.ORI
-00010e70: 4749 4e41 4c5f 4348 414e 4e45 4c5f 4449  GINAL_CHANNEL_DI
-00010e80: 4d5d 203d 2028 0a20 2020 2020 2020 2020  M] = (.         
-00010e90: 2020 2020 2020 2020 2020 2066 6c6f 6174             float
-00010ea0: 2822 6e61 6e22 2920 6966 206c 656e 2864  ("nan") if len(d
-00010eb0: 6174 612e 7368 6170 6529 203d 3d20 6c65  ata.shape) == le
-00010ec0: 6e28 6865 6164 6572 5b4d 6574 614b 6579  n(header[MetaKey
-00010ed0: 732e 5350 4154 4941 4c5f 5348 4150 455d  s.SPATIAL_SHAPE]
-00010ee0: 2920 656c 7365 2030 0a20 2020 2020 2020  ) else 0.       
-00010ef0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00010f00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00010f10: 2020 2020 2020 2020 2020 2020 2068 6561               hea
-00010f20: 6465 725b 4d65 7461 4b65 7973 2e4f 5249  der[MetaKeys.ORI
-00010f30: 4749 4e41 4c5f 4348 414e 4e45 4c5f 4449  GINAL_CHANNEL_DI
-00010f40: 4d5d 203d 2073 656c 662e 6368 616e 6e65  M] = self.channe
-00010f50: 6c5f 6469 6d0a 2020 2020 2020 2020 2020  l_dim.          
-00010f60: 2020 5f63 6f70 795f 636f 6d70 6174 6962    _copy_compatib
-00010f70: 6c65 5f64 6963 7428 6865 6164 6572 2c20  le_dict(header, 
-00010f80: 636f 6d70 6174 6962 6c65 5f6d 6574 6129  compatible_meta)
-00010f90: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00010fa0: 205f 7374 6163 6b5f 696d 6167 6573 2869   _stack_images(i
-00010fb0: 6d67 5f61 7272 6179 2c20 636f 6d70 6174  mg_array, compat
-00010fc0: 6962 6c65 5f6d 6574 6129 2c20 636f 6d70  ible_meta), comp
-00010fd0: 6174 6962 6c65 5f6d 6574 610a 0a20 2020  atible_meta..   
-00010fe0: 2064 6566 205f 6765 745f 6166 6669 6e65   def _get_affine
-00010ff0: 2873 656c 662c 2069 6d67 3a20 4e72 7264  (self, img: Nrrd
-00011000: 496d 6167 6529 202d 3e20 6e70 2e6e 6461  Image) -> np.nda
-00011010: 7272 6179 3a0a 2020 2020 2020 2020 2222  rray:.        ""
-00011020: 220a 2020 2020 2020 2020 4765 7420 7468  ".        Get th
-00011030: 6520 6166 6669 6e65 206d 6174 7269 7820  e affine matrix 
-00011040: 6f66 2074 6865 2069 6d61 6765 2c20 6974  of the image, it
-00011050: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00011060: 636f 7272 6563 740a 2020 2020 2020 2020  correct.        
-00011070: 7370 6163 696e 672c 206f 7269 656e 7461  spacing, orienta
-00011080: 7469 6f6e 206f 7220 6578 6563 7574 6520  tion or execute 
-00011090: 7370 6174 6961 6c20 7472 616e 7366 6f72  spatial transfor
-000110a0: 6d73 2e0a 0a20 2020 2020 2020 2041 7267  ms...        Arg
-000110b0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-000110c0: 6d67 3a20 4120 604e 7272 6449 6d61 6765  mg: A `NrrdImage
-000110d0: 6020 6c6f 6164 6564 2066 726f 6d20 696d  ` loaded from im
-000110e0: 6167 6520 6669 6c65 0a0a 2020 2020 2020  age file..      
-000110f0: 2020 2222 220a 2020 2020 2020 2020 6469    """.        di
-00011100: 7265 6374 696f 6e20 3d20 696d 672e 6865  rection = img.he
-00011110: 6164 6572 5b22 7370 6163 6520 6469 7265  ader["space dire
-00011120: 6374 696f 6e73 225d 0a20 2020 2020 2020  ctions"].       
-00011130: 206f 7269 6769 6e20 3d20 696d 672e 6865   origin = img.he
-00011140: 6164 6572 5b22 7370 6163 6520 6f72 6967  ader["space orig
-00011150: 696e 225d 0a0a 2020 2020 2020 2020 782c  in"]..        x,
-00011160: 2079 203d 2064 6972 6563 7469 6f6e 2e73   y = direction.s
-00011170: 6861 7065 0a20 2020 2020 2020 2061 6666  hape.        aff
-00011180: 696e 655f 6469 616d 203d 206d 696e 2878  ine_diam = min(x
-00011190: 2c20 7929 202b 2031 0a20 2020 2020 2020  , y) + 1.       
-000111a0: 2061 6666 696e 653a 206e 702e 6e64 6172   affine: np.ndar
-000111b0: 7261 7920 3d20 6e70 2e65 7965 2861 6666  ray = np.eye(aff
-000111c0: 696e 655f 6469 616d 290a 2020 2020 2020  ine_diam).      
-000111d0: 2020 6166 6669 6e65 5b3a 782c 203a 795d    affine[:x, :y]
-000111e0: 203d 2064 6972 6563 7469 6f6e 0a20 2020   = direction.   
-000111f0: 2020 2020 2061 6666 696e 655b 3a20 2861       affine[: (a
-00011200: 6666 696e 655f 6469 616d 202d 2031 292c  ffine_diam - 1),
-00011210: 202d 315d 203d 206f 7269 6769 6e20 2023   -1] = origin  #
-00011220: 206c 656e 206f 7269 6769 6e20 6973 2061   len origin is a
-00011230: 6c77 6179 7320 6166 6669 6e65 5f64 6961  lways affine_dia
-00011240: 6d20 2d20 310a 2020 2020 2020 2020 7265  m - 1.        re
-00011250: 7475 726e 2061 6666 696e 650a 0a20 2020  turn affine..   
-00011260: 2064 6566 205f 7377 6974 6368 5f6c 7073   def _switch_lps
-00011270: 5f72 6173 2873 656c 662c 2068 6561 6465  _ras(self, heade
-00011280: 723a 2064 6963 7429 202d 3e20 6469 6374  r: dict) -> dict
-00011290: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000112a0: 2020 2020 2020 466f 7220 636f 6d70 6174        For compat
-000112b0: 6962 696c 6974 7920 7769 7468 206e 6962  ibility with nib
-000112c0: 6162 656c 2c20 7377 6974 6368 2066 726f  abel, switch fro
-000112d0: 6d20 4c50 5320 746f 2052 4153 2e20 4164  m LPS to RAS. Ad
-000112e0: 6170 7420 6166 6669 6e65 206d 6174 7269  apt affine matri
-000112f0: 7820 616e 640a 2020 2020 2020 2020 6073  x and.        `s
-00011300: 7061 6365 6020 6172 6775 6d65 6e74 2069  pace` argument i
-00011310: 6e20 6865 6164 6572 2061 6363 6f72 6469  n header accordi
-00011320: 6e67 6c79 2e20 4966 206e 6f20 696e 666f  ngly. If no info
-00011330: 726d 6174 696f 6e20 6f66 2073 7061 6365  rmation of space
-00011340: 2069 7320 6769 7665 6e20 696e 2074 6865   is given in the
-00011350: 2068 6561 6465 722c 0a20 2020 2020 2020   header,.       
-00011360: 204c 5053 2069 7320 6173 7375 6d65 6420   LPS is assumed 
-00011370: 616e 6420 7468 7573 2063 6f6e 7665 7274  and thus convert
-00011380: 6564 2074 6f20 5241 532e 2049 6620 696e  ed to RAS. If in
-00011390: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
-000113a0: 7370 6163 6520 6973 2067 6976 656e 2c0a  space is given,.
-000113b0: 2020 2020 2020 2020 6275 7420 6973 206e          but is n
-000113c0: 6f74 204c 5053 2c20 7468 6520 756e 6368  ot LPS, the unch
-000113d0: 616e 6765 6420 6865 6164 6572 2069 7320  anged header is 
-000113e0: 7265 7475 726e 6564 2e0a 0a20 2020 2020  returned...     
-000113f0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00011400: 2020 2020 2068 6561 6465 723a 2054 6865       header: The
-00011410: 2069 6d61 6765 206d 6574 6164 6174 6120   image metadata 
-00011420: 6173 2064 6963 740a 0a20 2020 2020 2020  as dict..       
-00011430: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00011440: 2273 7061 6365 2220 6e6f 7420 696e 2068  "space" not in h
-00011450: 6561 6465 7220 6f72 2068 6561 6465 725b  eader or header[
-00011460: 2273 7061 6365 225d 203d 3d20 226c 6566  "space"] == "lef
-00011470: 742d 706f 7374 6572 696f 722d 7375 7065  t-posterior-supe
-00011480: 7269 6f72 223a 0a20 2020 2020 2020 2020  rior":.         
-00011490: 2020 2068 6561 6465 725b 4d65 7461 4b65     header[MetaKe
-000114a0: 7973 2e4f 5249 4749 4e41 4c5f 4146 4649  ys.ORIGINAL_AFFI
-000114b0: 4e45 5d20 3d20 6f72 6965 6e74 6174 696f  NE] = orientatio
-000114c0: 6e5f 7261 735f 6c70 7328 6865 6164 6572  n_ras_lps(header
-000114d0: 5b4d 6574 614b 6579 732e 4f52 4947 494e  [MetaKeys.ORIGIN
-000114e0: 414c 5f41 4646 494e 455d 290a 2020 2020  AL_AFFINE]).    
-000114f0: 2020 2020 2020 2020 6865 6164 6572 5b4d          header[M
-00011500: 6574 614b 6579 732e 5350 4143 455d 203d  etaKeys.SPACE] =
-00011510: 2053 7061 6365 4b65 7973 2e52 4153 0a20   SpaceKeys.RAS. 
-00011520: 2020 2020 2020 2072 6574 7572 6e20 6865         return he
-00011530: 6164 6572 0a0a 2020 2020 6465 6620 5f63  ader..    def _c
-00011540: 6f6e 7665 7274 5f66 5f74 6f5f 635f 6f72  onvert_f_to_c_or
-00011550: 6465 7228 7365 6c66 2c20 6865 6164 6572  der(self, header
-00011560: 3a20 6469 6374 2920 2d3e 2064 6963 743a  : dict) -> dict:
-00011570: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011580: 2020 2020 2041 6c6c 2068 6561 6465 7220       All header 
-00011590: 6669 656c 6473 206f 6620 6120 4e52 5244  fields of a NRRD
-000115a0: 2061 7265 2073 7065 6369 6669 6564 2069   are specified i
-000115b0: 6e20 6046 6020 2846 6f72 7472 616e 2920  n `F` (Fortran) 
-000115c0: 6f72 6465 722c 2065 7665 6e20 6966 2074  order, even if t
-000115d0: 6865 2069 6d61 6765 2077 6173 2072 6561  he image was rea
-000115e0: 6420 6173 2043 2d6f 7264 6572 6564 2061  d as C-ordered a
-000115f0: 7272 6179 2e0a 2020 2020 2020 2020 3144  rray..        1D
-00011600: 2061 7272 6179 7320 6f66 2068 6561 6465   arrays of heade
-00011610: 725b 2773 7061 6365 206f 7269 6769 6e27  r['space origin'
-00011620: 5d20 616e 6420 6865 6164 6572 5b27 7369  ] and header['si
-00011630: 7a65 7327 5d20 6265 636f 6d65 2069 6e76  zes'] become inv
-00011640: 6572 7465 642c 2065 2e67 2c20 5b31 2c32  erted, e.g, [1,2
-00011650: 2c33 5d20 2d3e 205b 332c 322c 315d 0a20  ,3] -> [3,2,1]. 
-00011660: 2020 2020 2020 2054 6865 2032 4420 4172         The 2D Ar
-00011670: 7261 7920 666f 7220 6865 6164 6572 5b27  ray for header['
-00011680: 7370 6163 6520 6469 7265 6374 696f 6e73  space directions
-00011690: 275d 2069 7320 7472 616e 7370 6f73 6564  '] is transposed
-000116a0: 3a20 5b5b 312c 302c 305d 2c5b 302c 322c  : [[1,0,0],[0,2,
-000116b0: 305d 2c5b 302c 302c 335d 5d20 2d3e 205b  0],[0,0,3]] -> [
-000116c0: 5b33 2c30 2c30 5d2c 5b30 2c32 2c30 5d2c  [3,0,0],[0,2,0],
-000116d0: 5b30 2c30 2c31 5d5d 0a20 2020 2020 2020  [0,0,1]].       
-000116e0: 2046 6f72 206d 6f72 6520 6465 7461 696c   For more detail
-000116f0: 7320 7265 6665 7220 746f 3a20 6874 7470  s refer to: http
-00011700: 733a 2f2f 7079 6e72 7264 2e72 6561 6474  s://pynrrd.readt
-00011710: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00011720: 6573 742f 7573 6572 2d67 7569 6465 2e68  est/user-guide.h
-00011730: 746d 6c23 696e 6465 782d 6f72 6465 7269  tml#index-orderi
-00011740: 6e67 0a0a 2020 2020 2020 2020 4172 6773  ng..        Args
-00011750: 3a0a 2020 2020 2020 2020 2020 2020 6865  :.            he
-00011760: 6164 6572 3a20 5468 6520 696d 6167 6520  ader: The image 
-00011770: 6d65 7461 6461 7461 2061 7320 6469 6374  metadata as dict
-00011780: 0a0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-00011790: 2020 2020 2020 2068 6561 6465 725b 2273         header["s
-000117a0: 7061 6365 2064 6972 6563 7469 6f6e 7322  pace directions"
-000117b0: 5d20 3d20 6e70 2e72 6f74 3930 286e 702e  ] = np.rot90(np.
-000117c0: 666c 6970 2868 6561 6465 725b 2273 7061  flip(header["spa
-000117d0: 6365 2064 6972 6563 7469 6f6e 7322 5d2c  ce directions"],
-000117e0: 2030 2929 0a20 2020 2020 2020 2068 6561   0)).        hea
-000117f0: 6465 725b 2273 7061 6365 206f 7269 6769  der["space origi
-00011800: 6e22 5d20 3d20 6865 6164 6572 5b22 7370  n"] = header["sp
-00011810: 6163 6520 6f72 6967 696e 225d 5b3a 3a2d  ace origin"][::-
-00011820: 315d 0a20 2020 2020 2020 2068 6561 6465  1].        heade
-00011830: 725b 2273 697a 6573 225d 203d 2068 6561  r["sizes"] = hea
-00011840: 6465 725b 2273 697a 6573 225d 5b3a 3a2d  der["sizes"][::-
-00011850: 315d 0a20 2020 2020 2020 2072 6574 7572  1].        retur
-00011860: 6e20 6865 6164 6572 0a                   n header.
+000081b0: 2020 2020 2020 7261 6973 6520 4e6f 7449        raise NotI
+000081c0: 6d70 6c65 6d65 6e74 6564 4572 726f 7228  mplementedError(
+000081d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081e0: 2020 2020 2066 2254 6f20 7265 6164 2064       f"To read d
+000081f0: 6963 6f6d 2073 6567 3a20 7b69 6d67 2e66  icom seg: {img.f
+00008200: 696c 656e 616d 657d 2c20 2753 6567 6d65  ilename}, 'Segme
+00008210: 6e74 4964 656e 7469 6669 6361 7469 6f6e  ntIdentification
+00008220: 5365 7175 656e 6365 2720 6973 2072 6571  Sequence' is req
+00008230: 7569 7265 6420 666f 7220 6561 6368 2066  uired for each f
+00008240: 7261 6d65 2e22 0a20 2020 2020 2020 2020  rame.".         
+00008250: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00008260: 2020 2020 2066 7261 6d65 5f73 6567 5f6e       frame_seg_n
+00008270: 756d 732e 6170 7065 6e64 2869 6e74 2866  ums.append(int(f
+00008280: 2e53 6567 6d65 6e74 4964 656e 7469 6669  .SegmentIdentifi
+00008290: 6361 7469 6f6e 5365 7175 656e 6365 5b30  cationSequence[0
+000082a0: 5d2e 5265 6665 7265 6e63 6564 5365 676d  ].ReferencedSegm
+000082b0: 656e 744e 756d 6265 7229 290a 0a20 2020  entNumber))..   
+000082c0: 2020 2020 2066 7261 6d65 5f73 6567 5f6e       frame_seg_n
+000082d0: 756d 735f 6172 7220 3d20 6e70 2e61 7272  ums_arr = np.arr
+000082e0: 6179 2866 7261 6d65 5f73 6567 5f6e 756d  ay(frame_seg_num
+000082f0: 7329 0a0a 2020 2020 2020 2020 7365 675f  s)..        seg_
+00008300: 6465 7363 7269 7074 696f 6e73 203d 207b  descriptions = {
+00008310: 696e 7428 662e 5365 676d 656e 744e 756d  int(f.SegmentNum
+00008320: 6265 7229 3a20 6620 666f 7220 6620 696e  ber): f for f in
+00008330: 2069 6d67 2e53 6567 6d65 6e74 5365 7175   img.SegmentSequ
+00008340: 656e 6365 7d0a 0a20 2020 2020 2020 2066  ence}..        f
+00008350: 6f72 2069 2069 6e20 6e70 2e75 6e69 7175  or i in np.uniqu
+00008360: 6528 6672 616d 655f 7365 675f 6e75 6d73  e(frame_seg_nums
+00008370: 5f61 7272 293a 0a20 2020 2020 2020 2020  _arr):.         
+00008380: 2020 2069 6e64 6963 6573 203d 206e 702e     indices = np.
+00008390: 7768 6572 6528 6672 616d 655f 7365 675f  where(frame_seg_
+000083a0: 6e75 6d73 5f61 7272 203d 3d20 6929 5b30  nums_arr == i)[0
+000083b0: 5d0a 2020 2020 2020 2020 2020 2020 7969  ].            yi
+000083c0: 656c 6420 2869 6d67 2e70 6978 656c 5f61  eld (img.pixel_a
+000083d0: 7272 6179 5b69 6e64 6963 6573 2c20 2e2e  rray[indices, ..
+000083e0: 2e5d 2c20 7365 675f 6465 7363 7269 7074  .], seg_descript
+000083f0: 696f 6e73 5b69 5d29 0a0a 2020 2020 6465  ions[i])..    de
+00008400: 6620 5f67 6574 5f73 6567 5f64 6174 6128  f _get_seg_data(
+00008410: 7365 6c66 2c20 696d 6729 3a0a 2020 2020  self, img):.    
+00008420: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008430: 4765 7420 7468 6520 6172 7261 7920 6461  Get the array da
+00008440: 7461 2061 6e64 206d 6574 6164 6174 6120  ta and metadata 
+00008450: 6f66 2074 6865 2073 6567 6d65 6e74 6174  of the segmentat
+00008460: 696f 6e20 696d 6167 652e 0a0a 2020 2020  ion image...    
+00008470: 2020 2020 4165 6773 3a0a 2020 2020 2020      Aegs:.      
+00008480: 2020 2020 2020 696d 673a 2061 2050 7964        img: a Pyd
+00008490: 6963 6f6d 2064 6174 6173 6574 206f 626a  icom dataset obj
+000084a0: 6563 7420 7468 6174 2068 6173 2061 7474  ect that has att
+000084b0: 7269 6275 7465 2022 5365 676d 656e 7453  ribute "SegmentS
+000084c0: 6571 7565 6e63 6522 2e0a 0a20 2020 2020  equence"...     
+000084d0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+000084e0: 6d65 7461 6461 7461 203d 2073 656c 662e  metadata = self.
+000084f0: 5f67 6574 5f6d 6574 615f 6469 6374 2869  _get_meta_dict(i
+00008500: 6d67 290a 2020 2020 2020 2020 6e5f 636c  mg).        n_cl
+00008510: 6173 7365 7320 3d20 6c65 6e28 696d 672e  asses = len(img.
+00008520: 5365 676d 656e 7453 6571 7565 6e63 6529  SegmentSequence)
+00008530: 0a20 2020 2020 2020 2073 7061 7469 616c  .        spatial
+00008540: 5f73 6861 7065 203d 206c 6973 7428 696d  _shape = list(im
+00008550: 672e 7069 7865 6c5f 6172 7261 792e 7368  g.pixel_array.sh
+00008560: 6170 6529 0a20 2020 2020 2020 2073 7061  ape).        spa
+00008570: 7469 616c 5f73 6861 7065 5b30 5d20 3d20  tial_shape[0] = 
+00008580: 7370 6174 6961 6c5f 7368 6170 655b 305d  spatial_shape[0]
+00008590: 202f 2f20 6e5f 636c 6173 7365 730a 0a20   // n_classes.. 
+000085a0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+000085b0: 6162 656c 5f64 6963 7420 6973 206e 6f74  abel_dict is not
+000085c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000085d0: 2020 206d 6574 6164 6174 615b 226c 6162     metadata["lab
+000085e0: 656c 7322 5d20 3d20 7365 6c66 2e6c 6162  els"] = self.lab
+000085f0: 656c 5f64 6963 740a 2020 2020 2020 2020  el_dict.        
+00008600: 2020 2020 616c 6c5f 7365 6773 203d 206e      all_segs = n
+00008610: 702e 7a65 726f 7328 5b2a 7370 6174 6961  p.zeros([*spatia
+00008620: 6c5f 7368 6170 652c 206c 656e 2873 656c  l_shape, len(sel
+00008630: 662e 6c61 6265 6c5f 6469 6374 295d 290a  f.label_dict)]).
+00008640: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00008650: 2020 2020 2020 2020 2020 6d65 7461 6461            metada
+00008660: 7461 5b22 6c61 6265 6c73 225d 203d 207b  ta["labels"] = {
+00008670: 7d0a 2020 2020 2020 2020 2020 2020 616c  }.            al
+00008680: 6c5f 7365 6773 203d 206e 702e 7a65 726f  l_segs = np.zero
+00008690: 7328 5b2a 7370 6174 6961 6c5f 7368 6170  s([*spatial_shap
+000086a0: 652c 206e 5f63 6c61 7373 6573 5d29 0a0a  e, n_classes])..
+000086b0: 2020 2020 2020 2020 666f 7220 692c 2028          for i, (
+000086c0: 6672 616d 6573 2c20 6465 7363 7269 7074  frames, descript
+000086d0: 696f 6e29 2069 6e20 656e 756d 6572 6174  ion) in enumerat
+000086e0: 6528 7365 6c66 2e5f 6765 745f 6672 616d  e(self._get_fram
+000086f0: 655f 6461 7461 2869 6d67 2929 3a0a 2020  e_data(img)):.  
+00008700: 2020 2020 2020 2020 2020 636c 6173 735f            class_
+00008710: 6e61 6d65 203d 2064 6573 6372 6970 7469  name = descripti
+00008720: 6f6e 2e53 6567 6d65 6e74 4465 7363 7269  on.SegmentDescri
+00008730: 7074 696f 6e0a 2020 2020 2020 2020 2020  ption.          
+00008740: 2020 6966 2063 6c61 7373 5f6e 616d 6520    if class_name 
+00008750: 6e6f 7420 696e 206d 6574 6164 6174 615b  not in metadata[
+00008760: 226c 6162 656c 7322 5d2e 6b65 7973 2829  "labels"].keys()
+00008770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00008780: 2020 6d65 7461 6461 7461 5b22 6c61 6265    metadata["labe
+00008790: 6c73 225d 5b63 6c61 7373 5f6e 616d 655d  ls"][class_name]
+000087a0: 203d 2069 0a20 2020 2020 2020 2020 2020   = i.           
+000087b0: 2063 6c61 7373 5f6e 756d 203d 206d 6574   class_num = met
+000087c0: 6164 6174 615b 226c 6162 656c 7322 5d5b  adata["labels"][
+000087d0: 636c 6173 735f 6e61 6d65 5d0a 2020 2020  class_name].    
+000087e0: 2020 2020 2020 2020 616c 6c5f 7365 6773          all_segs
+000087f0: 5b2e 2e2e 2c20 636c 6173 735f 6e75 6d5d  [..., class_num]
+00008800: 203d 2066 7261 6d65 730a 0a20 2020 2020   = frames..     
+00008810: 2020 2061 6c6c 5f73 6567 7320 3d20 616c     all_segs = al
+00008820: 6c5f 7365 6773 2e74 7261 6e73 706f 7365  l_segs.transpose
+00008830: 285b 312c 2032 2c20 302c 2033 5d29 0a20  ([1, 2, 0, 3]). 
+00008840: 2020 2020 2020 206d 6574 6164 6174 615b         metadata[
+00008850: 4d65 7461 4b65 7973 2e53 5041 5449 414c  MetaKeys.SPATIAL
+00008860: 5f53 4841 5045 5d20 3d20 616c 6c5f 7365  _SHAPE] = all_se
+00008870: 6773 2e73 6861 7065 5b3a 2d31 5d0a 0a20  gs.shape[:-1].. 
+00008880: 2020 2020 2020 2069 6620 2235 3230 3039         if "52009
+00008890: 3232 3922 2069 6e20 6d65 7461 6461 7461  229" in metadata
+000088a0: 2e6b 6579 7328 293a 0a20 2020 2020 2020  .keys():.       
+000088b0: 2020 2020 2073 6861 7265 645f 6675 6e63       shared_func
+000088c0: 5f67 726f 7570 5f73 6571 203d 206d 6574  _group_seq = met
+000088d0: 6164 6174 615b 2235 3230 3039 3232 3922  adata["52009229"
+000088e0: 5d5b 2256 616c 7565 225d 5b30 5d0a 0a20  ]["Value"][0].. 
+000088f0: 2020 2020 2020 2020 2020 2023 2067 6574             # get
+00008900: 2060 496d 6167 654f 7269 656e 7461 7469   `ImageOrientati
+00008910: 6f6e 5061 7469 656e 7460 0a20 2020 2020  onPatient`.     
+00008920: 2020 2020 2020 2069 6620 2230 3032 3039         if "00209
+00008930: 3131 3622 2069 6e20 7368 6172 6564 5f66  116" in shared_f
+00008940: 756e 635f 6772 6f75 705f 7365 712e 6b65  unc_group_seq.ke
+00008950: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00008960: 2020 2020 2020 706c 616e 655f 6f72 6965        plane_orie
+00008970: 6e74 5f73 6571 203d 2073 6861 7265 645f  nt_seq = shared_
+00008980: 6675 6e63 5f67 726f 7570 5f73 6571 5b22  func_group_seq["
+00008990: 3030 3230 3931 3136 225d 5b22 5661 6c75  00209116"]["Valu
+000089a0: 6522 5d5b 305d 0a20 2020 2020 2020 2020  e"][0].         
+000089b0: 2020 2020 2020 2069 6620 2230 3032 3030         if "00200
+000089c0: 3033 3722 2069 6e20 706c 616e 655f 6f72  037" in plane_or
+000089d0: 6965 6e74 5f73 6571 2e6b 6579 7328 293a  ient_seq.keys():
+000089e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000089f0: 2020 2020 206d 6574 6164 6174 615b 2230       metadata["0
+00008a00: 3032 3030 3033 3722 5d20 3d20 706c 616e  0200037"] = plan
+00008a10: 655f 6f72 6965 6e74 5f73 6571 5b22 3030  e_orient_seq["00
+00008a20: 3230 3030 3337 225d 0a0a 2020 2020 2020  200037"]..      
+00008a30: 2020 2020 2020 2320 6765 7420 6050 6978        # get `Pix
+00008a40: 656c 5370 6163 696e 6760 0a20 2020 2020  elSpacing`.     
+00008a50: 2020 2020 2020 2069 6620 2230 3032 3839         if "00289
+00008a60: 3131 3022 2069 6e20 7368 6172 6564 5f66  110" in shared_f
+00008a70: 756e 635f 6772 6f75 705f 7365 712e 6b65  unc_group_seq.ke
+00008a80: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00008a90: 2020 2020 2020 7069 7865 6c5f 6d65 6173        pixel_meas
+00008aa0: 7572 655f 7365 7120 3d20 7368 6172 6564  ure_seq = shared
+00008ab0: 5f66 756e 635f 6772 6f75 705f 7365 715b  _func_group_seq[
+00008ac0: 2230 3032 3839 3131 3022 5d5b 2256 616c  "00289110"]["Val
+00008ad0: 7565 225d 5b30 5d0a 0a20 2020 2020 2020  ue"][0]..       
+00008ae0: 2020 2020 2020 2020 2069 6620 2230 3032           if "002
+00008af0: 3830 3033 3022 2069 6e20 7069 7865 6c5f  80030" in pixel_
+00008b00: 6d65 6173 7572 655f 7365 712e 6b65 7973  measure_seq.keys
+00008b10: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00008b20: 2020 2020 2020 2020 7069 7865 6c5f 7370          pixel_sp
+00008b30: 6163 696e 6720 3d20 7069 7865 6c5f 6d65  acing = pixel_me
+00008b40: 6173 7572 655f 7365 715b 2230 3032 3830  asure_seq["00280
+00008b50: 3033 3022 5d5b 2256 616c 7565 225d 0a20  030"]["Value"]. 
+00008b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b70: 2020 206d 6574 6164 6174 615b 2273 7061     metadata["spa
+00008b80: 6369 6e67 225d 203d 2070 6978 656c 5f73  cing"] = pixel_s
+00008b90: 7061 6369 6e67 0a20 2020 2020 2020 2020  pacing.         
+00008ba0: 2020 2020 2020 2020 2020 2069 6620 2230             if "0
+00008bb0: 3031 3830 3035 3022 2069 6e20 7069 7865  0180050" in pixe
+00008bc0: 6c5f 6d65 6173 7572 655f 7365 712e 6b65  l_measure_seq.ke
+00008bd0: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+00008be0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00008bf0: 7461 6461 7461 5b22 7370 6163 696e 6722  tadata["spacing"
+00008c00: 5d20 2b3d 2070 6978 656c 5f6d 6561 7375  ] += pixel_measu
+00008c10: 7265 5f73 6571 5b22 3030 3138 3030 3530  re_seq["00180050
+00008c20: 225d 5b22 5661 6c75 6522 5d0a 0a20 2020  "]["Value"]..   
+00008c30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00008c40: 2e70 7275 6e65 5f6d 6574 6164 6174 613a  .prune_metadata:
+00008c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c60: 206d 6574 6164 6174 612e 706f 7028 2235   metadata.pop("5
+00008c70: 3230 3039 3232 3922 290a 0a20 2020 2020  2009229")..     
+00008c80: 2020 2023 2067 6574 2060 496d 6167 6550     # get `ImageP
+00008c90: 6f73 6974 696f 6e50 6174 6965 6e74 600a  ositionPatient`.
+00008ca0: 2020 2020 2020 2020 6966 2022 3532 3030          if "5200
+00008cb0: 3932 3330 2220 696e 206d 6574 6164 6174  9230" in metadat
+00008cc0: 612e 6b65 7973 2829 3a0a 2020 2020 2020  a.keys():.      
+00008cd0: 2020 2020 2020 6669 7273 745f 6672 616d        first_fram
+00008ce0: 655f 6675 6e63 5f67 726f 7570 5f73 6571  e_func_group_seq
+00008cf0: 203d 206d 6574 6164 6174 615b 2235 3230   = metadata["520
+00008d00: 3039 3233 3022 5d5b 2256 616c 7565 225d  09230"]["Value"]
+00008d10: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00008d20: 6966 2022 3030 3230 3931 3133 2220 696e  if "00209113" in
+00008d30: 2066 6972 7374 5f66 7261 6d65 5f66 756e   first_frame_fun
+00008d40: 635f 6772 6f75 705f 7365 712e 6b65 7973  c_group_seq.keys
+00008d50: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00008d60: 2020 2020 706c 616e 655f 706f 7369 7469      plane_positi
+00008d70: 6f6e 5f73 6571 203d 2066 6972 7374 5f66  on_seq = first_f
+00008d80: 7261 6d65 5f66 756e 635f 6772 6f75 705f  rame_func_group_
+00008d90: 7365 715b 2230 3032 3039 3131 3322 5d5b  seq["00209113"][
+00008da0: 2256 616c 7565 225d 5b30 5d0a 2020 2020  "Value"][0].    
+00008db0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00008dc0: 3030 3230 3030 3332 2220 696e 2070 6c61  00200032" in pla
+00008dd0: 6e65 5f70 6f73 6974 696f 6e5f 7365 712e  ne_position_seq.
+00008de0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
+00008df0: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
+00008e00: 6461 7461 5b22 3030 3230 3030 3332 225d  data["00200032"]
+00008e10: 203d 2070 6c61 6e65 5f70 6f73 6974 696f   = plane_positio
+00008e20: 6e5f 7365 715b 2230 3032 3030 3033 3222  n_seq["00200032"
+00008e30: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00008e40: 2020 2020 2020 6d65 7461 6461 7461 5b22        metadata["
+00008e50: 6c61 7374 496d 6167 6550 6f73 6974 696f  lastImagePositio
+00008e60: 6e50 6174 6965 6e74 225d 203d 206d 6574  nPatient"] = met
+00008e70: 6164 6174 615b 2235 3230 3039 3233 3022  adata["52009230"
+00008e80: 5d5b 2256 616c 7565 225d 5b2d 315d 5b22  ]["Value"][-1]["
+00008e90: 3030 3230 3931 3133 225d 5b22 5661 6c75  00209113"]["Valu
+00008ea0: 6522 5d5b 305d 5b0a 2020 2020 2020 2020  e"][0][.        
+00008eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ec0: 2230 3032 3030 3033 3222 0a20 2020 2020  "00200032".     
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00008ee0: 5b22 5661 6c75 6522 5d0a 2020 2020 2020  ["Value"].      
+00008ef0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
+00008f00: 756e 655f 6d65 7461 6461 7461 3a0a 2020  une_metadata:.  
+00008f10: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+00008f20: 7461 6461 7461 2e70 6f70 2822 3532 3030  tadata.pop("5200
+00008f30: 3932 3330 2229 0a0a 2020 2020 2020 2020  9230")..        
+00008f40: 7265 7475 726e 2061 6c6c 5f73 6567 732c  return all_segs,
+00008f50: 206d 6574 6164 6174 610a 0a20 2020 2064   metadata..    d
+00008f60: 6566 205f 6765 745f 6172 7261 795f 6461  ef _get_array_da
+00008f70: 7461 2873 656c 662c 2069 6d67 293a 0a20  ta(self, img):. 
+00008f80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008f90: 2020 2047 6574 2074 6865 2061 7272 6179     Get the array
+00008fa0: 2064 6174 6120 6f66 2074 6865 2069 6d61   data of the ima
+00008fb0: 6765 2e20 4966 2060 5265 7363 616c 6553  ge. If `RescaleS
+00008fc0: 6c6f 7065 6020 616e 6420 6052 6573 6361  lope` and `Resca
+00008fd0: 6c65 496e 7465 7263 6570 7460 2061 7265  leIntercept` are
+00008fe0: 2061 7661 696c 6162 6c65 2c20 7468 6520   available, the 
+00008ff0: 7261 7720 6172 7261 7920 6461 7461 0a20  raw array data. 
+00009000: 2020 2020 2020 2077 696c 6c20 6265 2072         will be r
+00009010: 6573 6361 6c65 642e 2054 6865 206f 7574  escaled. The out
+00009020: 7075 7420 6461 7461 2068 6173 2074 6865  put data has the
+00009030: 2064 7479 7065 206e 702e 666c 6f61 7433   dtype np.float3
+00009040: 3220 6966 2074 6865 2072 6573 6361 6c69  2 if the rescali
+00009050: 6e67 2069 7320 6170 706c 6965 642e 0a0a  ng is applied...
+00009060: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00009070: 2020 2020 2020 2020 2020 696d 673a 2061            img: a
+00009080: 2050 7964 6963 6f6d 2064 6174 6173 6574   Pydicom dataset
+00009090: 206f 626a 6563 742e 0a0a 2020 2020 2020   object...      
+000090a0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+000090b0: 7072 6f63 6573 7320 4469 636f 6d20 7365  process Dicom se
+000090c0: 7269 6573 0a20 2020 2020 2020 2069 6620  ries.        if 
+000090d0: 6e6f 7420 6861 7361 7474 7228 696d 672c  not hasattr(img,
+000090e0: 2022 7069 7865 6c5f 6172 7261 7922 293a   "pixel_array"):
+000090f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00009100: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
+00009110: 6469 636f 6d20 6461 7461 3a20 7b69 6d67  dicom data: {img
+00009120: 2e66 696c 656e 616d 657d 2064 6f65 7320  .filename} does 
+00009130: 6e6f 7420 6861 7665 2070 6978 656c 5f61  not have pixel_a
+00009140: 7272 6179 2e22 290a 2020 2020 2020 2020  rray.").        
+00009150: 6461 7461 203d 2069 6d67 2e70 6978 656c  data = img.pixel
+00009160: 5f61 7272 6179 0a0a 2020 2020 2020 2020  _array..        
+00009170: 736c 6f70 652c 206f 6666 7365 7420 3d20  slope, offset = 
+00009180: 312e 302c 2030 2e30 0a20 2020 2020 2020  1.0, 0.0.       
+00009190: 2072 6573 6361 6c65 5f66 6c61 6720 3d20   rescale_flag = 
+000091a0: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
+000091b0: 2068 6173 6174 7472 2869 6d67 2c20 2252   hasattr(img, "R
+000091c0: 6573 6361 6c65 536c 6f70 6522 293a 0a20  escaleSlope"):. 
+000091d0: 2020 2020 2020 2020 2020 2073 6c6f 7065             slope
+000091e0: 203d 2069 6d67 2e52 6573 6361 6c65 536c   = img.RescaleSl
+000091f0: 6f70 650a 2020 2020 2020 2020 2020 2020  ope.            
+00009200: 7265 7363 616c 655f 666c 6167 203d 2054  rescale_flag = T
+00009210: 7275 650a 2020 2020 2020 2020 6966 2068  rue.        if h
+00009220: 6173 6174 7472 2869 6d67 2c20 2252 6573  asattr(img, "Res
+00009230: 6361 6c65 496e 7465 7263 6570 7422 293a  caleIntercept"):
+00009240: 0a20 2020 2020 2020 2020 2020 206f 6666  .            off
+00009250: 7365 7420 3d20 696d 672e 5265 7363 616c  set = img.Rescal
+00009260: 6549 6e74 6572 6365 7074 0a20 2020 2020  eIntercept.     
+00009270: 2020 2020 2020 2072 6573 6361 6c65 5f66         rescale_f
+00009280: 6c61 6720 3d20 5472 7565 0a20 2020 2020  lag = True.     
+00009290: 2020 2069 6620 7265 7363 616c 655f 666c     if rescale_fl
+000092a0: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+000092b0: 6461 7461 203d 2064 6174 612e 6173 7479  data = data.asty
+000092c0: 7065 286e 702e 666c 6f61 7433 3229 202a  pe(np.float32) *
+000092d0: 2073 6c6f 7065 202b 206f 6666 7365 740a   slope + offset.
+000092e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000092f0: 6461 7461 0a0a 0a40 7265 7175 6972 655f  data...@require_
+00009300: 706b 6728 706b 675f 6e61 6d65 3d22 6e69  pkg(pkg_name="ni
+00009310: 6261 6265 6c22 290a 636c 6173 7320 4e69  babel").class Ni
+00009320: 6261 6265 6c52 6561 6465 7228 496d 6167  babelReader(Imag
+00009330: 6552 6561 6465 7229 3a0a 2020 2020 2222  eReader):.    ""
+00009340: 220a 2020 2020 4c6f 6164 204e 4966 5449  ".    Load NIfTI
+00009350: 2066 6f72 6d61 7420 696d 6167 6573 2062   format images b
+00009360: 6173 6564 206f 6e20 4e69 6261 6265 6c20  ased on Nibabel 
+00009370: 6c69 6272 6172 792e 0a0a 2020 2020 4172  library...    Ar
+00009380: 6773 3a0a 2020 2020 2020 2020 6173 5f63  gs:.        as_c
+00009390: 6c6f 7365 7374 5f63 616e 6f6e 6963 616c  losest_canonical
+000093a0: 3a20 6966 2054 7275 652c 206c 6f61 6420  : if True, load 
+000093b0: 7468 6520 696d 6167 6520 6173 2063 6c6f  the image as clo
+000093c0: 7365 7374 2074 6f20 6361 6e6f 6e69 6361  sest to canonica
+000093d0: 6c20 6178 6973 2066 6f72 6d61 742e 0a20  l axis format.. 
+000093e0: 2020 2020 2020 2073 7175 6565 7a65 5f6e         squeeze_n
+000093f0: 6f6e 5f73 7061 7469 616c 5f64 696d 733a  on_spatial_dims:
+00009400: 2069 6620 5472 7565 2c20 6e6f 6e2d 7370   if True, non-sp
+00009410: 6174 6961 6c20 7369 6e67 6c65 746f 6e73  atial singletons
+00009420: 2077 696c 6c20 6265 2073 7175 6565 7a65   will be squeeze
+00009430: 642c 2065 2e67 2e20 2832 3536 2c32 3536  d, e.g. (256,256
+00009440: 2c31 2c33 2920 2d3e 2028 3235 362c 3235  ,1,3) -> (256,25
+00009450: 362c 3329 0a20 2020 2020 2020 2063 6861  6,3).        cha
+00009460: 6e6e 656c 5f64 696d 3a20 7468 6520 6368  nnel_dim: the ch
+00009470: 616e 6e65 6c20 6469 6d65 6e73 696f 6e20  annel dimension 
+00009480: 6f66 2074 6865 2069 6e70 7574 2069 6d61  of the input ima
+00009490: 6765 2c20 6465 6661 756c 7420 6973 204e  ge, default is N
+000094a0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+000094b0: 2074 6869 7320 6973 2075 7365 6420 746f   this is used to
+000094c0: 2073 6574 206f 7269 6769 6e61 6c5f 6368   set original_ch
+000094d0: 616e 6e65 6c5f 6469 6d20 696e 2074 6865  annel_dim in the
+000094e0: 206d 6574 6164 6174 612c 2045 6e73 7572   metadata, Ensur
+000094f0: 6543 6861 6e6e 656c 4669 7273 7444 2072  eChannelFirstD r
+00009500: 6561 6473 2074 6869 7320 6669 656c 642e  eads this field.
+00009510: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009520: 4e6f 6e65 2c20 606f 7269 6769 6e61 6c5f  None, `original_
+00009530: 6368 616e 6e65 6c5f 6469 6d60 2077 696c  channel_dim` wil
+00009540: 6c20 6265 2065 6974 6865 7220 606e 6f5f  l be either `no_
+00009550: 6368 616e 6e65 6c60 206f 7220 602d 3160  channel` or `-1`
+00009560: 2e0a 2020 2020 2020 2020 2020 2020 6d6f  ..            mo
+00009570: 7374 204e 6966 7469 2066 696c 6573 2061  st Nifti files a
+00009580: 7265 2075 7375 616c 6c79 2022 6368 616e  re usually "chan
+00009590: 6e65 6c20 6c61 7374 222c 206e 6f20 6e65  nel last", no ne
+000095a0: 6564 2074 6f20 7370 6563 6966 7920 7468  ed to specify th
+000095b0: 6973 2061 7267 756d 656e 7420 666f 7220  is argument for 
+000095c0: 7468 656d 2e0a 2020 2020 2020 2020 6b77  them..        kw
+000095d0: 6172 6773 3a20 6164 6469 7469 6f6e 616c  args: additional
+000095e0: 2061 7267 7320 666f 7220 606e 6962 6162   args for `nibab
+000095f0: 656c 2e6c 6f61 6460 2041 5049 2e20 6d6f  el.load` API. mo
+00009600: 7265 2064 6574 6169 6c73 2061 626f 7574  re details about
+00009610: 2061 7661 696c 6162 6c65 2061 7267 733a   available args:
+00009620: 0a20 2020 2020 2020 2020 2020 2068 7474  .            htt
+00009630: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00009640: 6e69 7079 2f6e 6962 6162 656c 2f62 6c6f  nipy/nibabel/blo
+00009650: 622f 6d61 7374 6572 2f6e 6962 6162 656c  b/master/nibabel
+00009660: 2f6c 6f61 6473 6176 652e 7079 0a0a 2020  /loadsave.py..  
+00009670: 2020 2222 220a 0a20 2020 2040 6465 7072    """..    @depr
+00009680: 6563 6174 6564 5f61 7267 2822 6474 7970  ecated_arg("dtyp
+00009690: 6522 2c20 7369 6e63 653d 2231 2e30 222c  e", since="1.0",
+000096a0: 206d 7367 5f73 7566 6669 783d 2270 6c65   msg_suffix="ple
+000096b0: 6173 6520 6d6f 6469 6679 2064 7479 7065  ase modify dtype
+000096c0: 206f 6620 7468 6520 7265 7475 726e 6564   of the returned
+000096d0: 2062 7920 6060 6765 745f 6461 7461 6060   by ``get_data``
+000096e0: 2069 6e73 7465 6164 2e22 290a 2020 2020   instead.").    
+000096f0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+00009700: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00009710: 2020 2020 6368 616e 6e65 6c5f 6469 6d3a      channel_dim:
+00009720: 2073 7472 207c 2069 6e74 207c 204e 6f6e   str | int | Non
+00009730: 6520 3d20 4e6f 6e65 2c0a 2020 2020 2020  e = None,.      
+00009740: 2020 6173 5f63 6c6f 7365 7374 5f63 616e    as_closest_can
+00009750: 6f6e 6963 616c 3a20 626f 6f6c 203d 2046  onical: bool = F
+00009760: 616c 7365 2c0a 2020 2020 2020 2020 7371  alse,.        sq
+00009770: 7565 657a 655f 6e6f 6e5f 7370 6174 6961  ueeze_non_spatia
+00009780: 6c5f 6469 6d73 3a20 626f 6f6c 203d 2046  l_dims: bool = F
+00009790: 616c 7365 2c0a 2020 2020 2020 2020 6474  alse,.        dt
+000097a0: 7970 653a 2044 7479 7065 4c69 6b65 203d  ype: DtypeLike =
+000097b0: 206e 702e 666c 6f61 7433 322c 0a20 2020   np.float32,.   
+000097c0: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
+000097d0: 2020 2029 3a0a 2020 2020 2020 2020 7375     ):.        su
+000097e0: 7065 7228 292e 5f5f 696e 6974 5f5f 2829  per().__init__()
+000097f0: 0a20 2020 2020 2020 2073 656c 662e 6368  .        self.ch
+00009800: 616e 6e65 6c5f 6469 6d20 3d20 666c 6f61  annel_dim = floa
+00009810: 7428 226e 616e 2229 2069 6620 6368 616e  t("nan") if chan
+00009820: 6e65 6c5f 6469 6d20 3d3d 2022 6e6f 5f63  nel_dim == "no_c
+00009830: 6861 6e6e 656c 2220 656c 7365 2063 6861  hannel" else cha
+00009840: 6e6e 656c 5f64 696d 0a20 2020 2020 2020  nnel_dim.       
+00009850: 2073 656c 662e 6173 5f63 6c6f 7365 7374   self.as_closest
+00009860: 5f63 616e 6f6e 6963 616c 203d 2061 735f  _canonical = as_
+00009870: 636c 6f73 6573 745f 6361 6e6f 6e69 6361  closest_canonica
+00009880: 6c0a 2020 2020 2020 2020 7365 6c66 2e73  l.        self.s
+00009890: 7175 6565 7a65 5f6e 6f6e 5f73 7061 7469  queeze_non_spati
+000098a0: 616c 5f64 696d 7320 3d20 7371 7565 657a  al_dims = squeez
+000098b0: 655f 6e6f 6e5f 7370 6174 6961 6c5f 6469  e_non_spatial_di
+000098c0: 6d73 0a20 2020 2020 2020 2073 656c 662e  ms.        self.
+000098d0: 6474 7970 6520 3d20 6474 7970 6520 2023  dtype = dtype  #
+000098e0: 2064 6570 7265 6361 7465 640a 2020 2020   deprecated.    
+000098f0: 2020 2020 7365 6c66 2e6b 7761 7267 7320      self.kwargs 
+00009900: 3d20 6b77 6172 6773 0a0a 2020 2020 6465  = kwargs..    de
+00009910: 6620 7665 7269 6679 5f73 7566 6669 7828  f verify_suffix(
+00009920: 7365 6c66 2c20 6669 6c65 6e61 6d65 3a20  self, filename: 
+00009930: 5365 7175 656e 6365 5b50 6174 684c 696b  Sequence[PathLik
+00009940: 655d 207c 2050 6174 684c 696b 6529 202d  e] | PathLike) -
+00009950: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+00009960: 2222 220a 2020 2020 2020 2020 5665 7269  """.        Veri
+00009970: 6679 2077 6865 7468 6572 2074 6865 2073  fy whether the s
+00009980: 7065 6369 6669 6564 2066 696c 6520 6f72  pecified file or
+00009990: 2066 696c 6573 2066 6f72 6d61 7420 6973   files format is
+000099a0: 2073 7570 706f 7274 6564 2062 7920 4e69   supported by Ni
+000099b0: 6261 6265 6c20 7265 6164 6572 2e0a 0a20  babel reader... 
+000099c0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000099d0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+000099e0: 653a 2066 696c 6520 6e61 6d65 206f 7220  e: file name or 
+000099f0: 6120 6c69 7374 206f 6620 6669 6c65 206e  a list of file n
+00009a00: 616d 6573 2074 6f20 7265 6164 2e0a 2020  ames to read..  
+00009a10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00009a20: 2061 206c 6973 7420 6f66 2066 696c 6573   a list of files
+00009a30: 2c20 7665 7269 6679 2061 6c6c 2074 6865  , verify all the
+00009a40: 2073 7566 6669 7865 732e 0a0a 2020 2020   suffixes...    
+00009a50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00009a60: 7375 6666 6978 6573 3a20 5365 7175 656e  suffixes: Sequen
+00009a70: 6365 5b73 7472 5d20 3d20 5b22 6e69 6922  ce[str] = ["nii"
+00009a80: 2c20 226e 6969 2e67 7a22 5d0a 2020 2020  , "nii.gz"].    
+00009a90: 2020 2020 7265 7475 726e 2068 6173 5f6e      return has_n
+00009aa0: 6962 2061 6e64 2069 735f 7375 7070 6f72  ib and is_suppor
+00009ab0: 7465 645f 666f 726d 6174 2866 696c 656e  ted_format(filen
+00009ac0: 616d 652c 2073 7566 6669 7865 7329 0a0a  ame, suffixes)..
+00009ad0: 2020 2020 6465 6620 7265 6164 2873 656c      def read(sel
+00009ae0: 662c 2064 6174 613a 2053 6571 7565 6e63  f, data: Sequenc
+00009af0: 655b 5061 7468 4c69 6b65 5d20 7c20 5061  e[PathLike] | Pa
+00009b00: 7468 4c69 6b65 2c20 2a2a 6b77 6172 6773  thLike, **kwargs
+00009b10: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00009b20: 2020 2020 2020 2052 6561 6420 696d 6167         Read imag
+00009b30: 6520 6461 7461 2066 726f 6d20 7370 6563  e data from spec
+00009b40: 6966 6965 6420 6669 6c65 206f 7220 6669  ified file or fi
+00009b50: 6c65 732c 2069 7420 6361 6e20 7265 6164  les, it can read
+00009b60: 2061 206c 6973 7420 6f66 2069 6d61 6765   a list of image
+00009b70: 730a 2020 2020 2020 2020 616e 6420 7374  s.        and st
+00009b80: 6163 6b20 7468 656d 2074 6f67 6574 6865  ack them togethe
+00009b90: 7220 6173 206d 756c 7469 2d63 6861 6e6e  r as multi-chann
+00009ba0: 656c 2064 6174 6120 696e 2060 6765 745f  el data in `get_
+00009bb0: 6461 7461 2829 602e 0a20 2020 2020 2020  data()`..       
+00009bc0: 204e 6f74 6520 7468 6174 2074 6865 2072   Note that the r
+00009bd0: 6574 7572 6e65 6420 6f62 6a65 6374 2069  eturned object i
+00009be0: 7320 4e69 6261 6265 6c20 696d 6167 6520  s Nibabel image 
+00009bf0: 6f62 6a65 6374 206f 7220 6c69 7374 206f  object or list o
+00009c00: 6620 4e69 6261 6265 6c20 696d 6167 6520  f Nibabel image 
+00009c10: 6f62 6a65 6374 732e 0a0a 2020 2020 2020  objects...      
+00009c20: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00009c30: 2020 2020 6461 7461 3a20 6669 6c65 206e      data: file n
+00009c40: 616d 6520 6f72 2061 206c 6973 7420 6f66  ame or a list of
+00009c50: 2066 696c 6520 6e61 6d65 7320 746f 2072   file names to r
+00009c60: 6561 642e 0a20 2020 2020 2020 2020 2020  ead..           
+00009c70: 206b 7761 7267 733a 2061 6464 6974 696f   kwargs: additio
+00009c80: 6e61 6c20 6172 6773 2066 6f72 2060 6e69  nal args for `ni
+00009c90: 6261 6265 6c2e 6c6f 6164 6020 4150 492c  babel.load` API,
+00009ca0: 2077 696c 6c20 6f76 6572 7269 6465 2060   will override `
+00009cb0: 7365 6c66 2e6b 7761 7267 7360 2066 6f72  self.kwargs` for
+00009cc0: 2065 7869 7374 696e 6720 6b65 7973 2e0a   existing keys..
+00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ce0: 4d6f 7265 2064 6574 6169 6c73 2061 626f  More details abo
+00009cf0: 7574 2061 7661 696c 6162 6c65 2061 7267  ut available arg
+00009d00: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00009d10: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
+00009d20: 622e 636f 6d2f 6e69 7079 2f6e 6962 6162  b.com/nipy/nibab
+00009d30: 656c 2f62 6c6f 622f 6d61 7374 6572 2f6e  el/blob/master/n
+00009d40: 6962 6162 656c 2f6c 6f61 6473 6176 652e  ibabel/loadsave.
+00009d50: 7079 0a0a 2020 2020 2020 2020 2222 220a  py..        """.
+00009d60: 2020 2020 2020 2020 696d 675f 3a20 6c69          img_: li
+00009d70: 7374 5b4e 6966 7469 3149 6d61 6765 5d20  st[Nifti1Image] 
+00009d80: 3d20 5b5d 0a0a 2020 2020 2020 2020 6669  = []..        fi
+00009d90: 6c65 6e61 6d65 733a 2053 6571 7565 6e63  lenames: Sequenc
+00009da0: 655b 5061 7468 4c69 6b65 5d20 3d20 656e  e[PathLike] = en
+00009db0: 7375 7265 5f74 7570 6c65 2864 6174 6129  sure_tuple(data)
+00009dc0: 0a20 2020 2020 2020 206b 7761 7267 735f  .        kwargs_
+00009dd0: 203d 2073 656c 662e 6b77 6172 6773 2e63   = self.kwargs.c
+00009de0: 6f70 7928 290a 2020 2020 2020 2020 6b77  opy().        kw
+00009df0: 6172 6773 5f2e 7570 6461 7465 286b 7761  args_.update(kwa
+00009e00: 7267 7329 0a20 2020 2020 2020 2066 6f72  rgs).        for
+00009e10: 206e 616d 6520 696e 2066 696c 656e 616d   name in filenam
+00009e20: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+00009e30: 696d 6720 3d20 6e69 622e 6c6f 6164 286e  img = nib.load(n
+00009e40: 616d 652c 202a 2a6b 7761 7267 735f 290a  ame, **kwargs_).
+00009e50: 2020 2020 2020 2020 2020 2020 696d 6720              img 
+00009e60: 3d20 636f 7272 6563 745f 6e69 6674 695f  = correct_nifti_
+00009e70: 6865 6164 6572 5f69 665f 6e65 6365 7373  header_if_necess
+00009e80: 6172 7928 696d 6729 0a20 2020 2020 2020  ary(img).       
+00009e90: 2020 2020 2069 6d67 5f2e 6170 7065 6e64       img_.append
+00009ea0: 2869 6d67 2920 2023 2074 7970 653a 2069  (img)  # type: i
+00009eb0: 676e 6f72 650a 2020 2020 2020 2020 7265  gnore.        re
+00009ec0: 7475 726e 2069 6d67 5f20 6966 206c 656e  turn img_ if len
+00009ed0: 2866 696c 656e 616d 6573 2920 3e20 3120  (filenames) > 1 
+00009ee0: 656c 7365 2069 6d67 5f5b 305d 0a0a 2020  else img_[0]..  
+00009ef0: 2020 6465 6620 6765 745f 6461 7461 2873    def get_data(s
+00009f00: 656c 662c 2069 6d67 2920 2d3e 2074 7570  elf, img) -> tup
+00009f10: 6c65 5b6e 702e 6e64 6172 7261 792c 2064  le[np.ndarray, d
+00009f20: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
+00009f30: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
+00009f40: 7420 6461 7461 2061 7272 6179 2061 6e64  t data array and
+00009f50: 206d 6574 6164 6174 6120 6672 6f6d 206c   metadata from l
+00009f60: 6f61 6465 6420 696d 6167 6520 616e 6420  oaded image and 
+00009f70: 7265 7475 726e 2074 6865 6d2e 0a20 2020  return them..   
+00009f80: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+00009f90: 6f6e 2072 6574 7572 6e73 2074 776f 206f  on returns two o
+00009fa0: 626a 6563 7473 2c20 6669 7273 7420 6973  bjects, first is
+00009fb0: 206e 756d 7079 2061 7272 6179 206f 6620   numpy array of 
+00009fc0: 696d 6167 6520 6461 7461 2c20 7365 636f  image data, seco
+00009fd0: 6e64 2069 7320 6469 6374 206f 6620 6d65  nd is dict of me
+00009fe0: 7461 6461 7461 2e0a 2020 2020 2020 2020  tadata..        
+00009ff0: 4974 2063 6f6e 7374 7275 6374 7320 6061  It constructs `a
+0000a000: 6666 696e 6560 2c20 606f 7269 6769 6e61  ffine`, `origina
+0000a010: 6c5f 6166 6669 6e65 602c 2061 6e64 2060  l_affine`, and `
+0000a020: 7370 6174 6961 6c5f 7368 6170 6560 2061  spatial_shape` a
+0000a030: 6e64 2073 746f 7265 7320 7468 656d 2069  nd stores them i
+0000a040: 6e20 6d65 7461 2064 6963 742e 0a20 2020  n meta dict..   
+0000a050: 2020 2020 2057 6865 6e20 6c6f 6164 696e       When loadin
+0000a060: 6720 6120 6c69 7374 206f 6620 6669 6c65  g a list of file
+0000a070: 732c 2074 6865 7920 6172 6520 7374 6163  s, they are stac
+0000a080: 6b65 6420 746f 6765 7468 6572 2061 7420  ked together at 
+0000a090: 6120 6e65 7720 6469 6d65 6e73 696f 6e20  a new dimension 
+0000a0a0: 6173 2074 6865 2066 6972 7374 2064 696d  as the first dim
+0000a0b0: 656e 7369 6f6e 2c0a 2020 2020 2020 2020  ension,.        
+0000a0c0: 616e 6420 7468 6520 6d65 7461 6461 7461  and the metadata
+0000a0d0: 206f 6620 7468 6520 6669 7273 7420 696d   of the first im
+0000a0e0: 6167 6520 6973 2075 7365 6420 746f 2070  age is used to p
+0000a0f0: 7265 7365 6e74 2074 6865 206f 7574 7075  resent the outpu
+0000a100: 7420 6d65 7461 6461 7461 2e0a 0a20 2020  t metadata...   
+0000a110: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000a120: 2020 2020 2020 2069 6d67 3a20 6120 4e69         img: a Ni
+0000a130: 6261 6265 6c20 696d 6167 6520 6f62 6a65  babel image obje
+0000a140: 6374 206c 6f61 6465 6420 6672 6f6d 2061  ct loaded from a
+0000a150: 6e20 696d 6167 6520 6669 6c65 206f 7220  n image file or 
+0000a160: 6120 6c69 7374 206f 6620 4e69 6261 6265  a list of Nibabe
+0000a170: 6c20 696d 6167 6520 6f62 6a65 6374 732e  l image objects.
+0000a180: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000a190: 2020 2020 2020 696d 675f 6172 7261 793a        img_array:
+0000a1a0: 206c 6973 745b 6e70 2e6e 6461 7272 6179   list[np.ndarray
+0000a1b0: 5d20 3d20 5b5d 0a20 2020 2020 2020 2063  ] = [].        c
+0000a1c0: 6f6d 7061 7469 626c 655f 6d65 7461 3a20  ompatible_meta: 
+0000a1d0: 6469 6374 203d 207b 7d0a 0a20 2020 2020  dict = {}..     
+0000a1e0: 2020 2066 6f72 2069 2069 6e20 656e 7375     for i in ensu
+0000a1f0: 7265 5f74 7570 6c65 2869 6d67 293a 0a20  re_tuple(img):. 
+0000a200: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+0000a210: 7220 3d20 7365 6c66 2e5f 6765 745f 6d65  r = self._get_me
+0000a220: 7461 5f64 6963 7428 6929 0a20 2020 2020  ta_dict(i).     
+0000a230: 2020 2020 2020 2068 6561 6465 725b 4d65         header[Me
+0000a240: 7461 4b65 7973 2e41 4646 494e 455d 203d  taKeys.AFFINE] =
+0000a250: 2073 656c 662e 5f67 6574 5f61 6666 696e   self._get_affin
+0000a260: 6528 6929 0a20 2020 2020 2020 2020 2020  e(i).           
+0000a270: 2068 6561 6465 725b 4d65 7461 4b65 7973   header[MetaKeys
+0000a280: 2e4f 5249 4749 4e41 4c5f 4146 4649 4e45  .ORIGINAL_AFFINE
+0000a290: 5d20 3d20 7365 6c66 2e5f 6765 745f 6166  ] = self._get_af
+0000a2a0: 6669 6e65 2869 290a 2020 2020 2020 2020  fine(i).        
+0000a2b0: 2020 2020 6865 6164 6572 5b22 6173 5f63      header["as_c
+0000a2c0: 6c6f 7365 7374 5f63 616e 6f6e 6963 616c  losest_canonical
+0000a2d0: 225d 203d 2073 656c 662e 6173 5f63 6c6f  "] = self.as_clo
+0000a2e0: 7365 7374 5f63 616e 6f6e 6963 616c 0a20  sest_canonical. 
+0000a2f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000a300: 6c66 2e61 735f 636c 6f73 6573 745f 6361  lf.as_closest_ca
+0000a310: 6e6f 6e69 6361 6c3a 0a20 2020 2020 2020  nonical:.       
+0000a320: 2020 2020 2020 2020 2069 203d 206e 6962           i = nib
+0000a330: 2e61 735f 636c 6f73 6573 745f 6361 6e6f  .as_closest_cano
+0000a340: 6e69 6361 6c28 6929 0a20 2020 2020 2020  nical(i).       
+0000a350: 2020 2020 2020 2020 2068 6561 6465 725b           header[
+0000a360: 4d65 7461 4b65 7973 2e41 4646 494e 455d  MetaKeys.AFFINE]
+0000a370: 203d 2073 656c 662e 5f67 6574 5f61 6666   = self._get_aff
+0000a380: 696e 6528 6929 0a20 2020 2020 2020 2020  ine(i).         
+0000a390: 2020 2068 6561 6465 725b 4d65 7461 4b65     header[MetaKe
+0000a3a0: 7973 2e53 5041 5449 414c 5f53 4841 5045  ys.SPATIAL_SHAPE
+0000a3b0: 5d20 3d20 7365 6c66 2e5f 6765 745f 7370  ] = self._get_sp
+0000a3c0: 6174 6961 6c5f 7368 6170 6528 6929 0a20  atial_shape(i). 
+0000a3d0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+0000a3e0: 725b 4d65 7461 4b65 7973 2e53 5041 4345  r[MetaKeys.SPACE
+0000a3f0: 5d20 3d20 5370 6163 654b 6579 732e 5241  ] = SpaceKeys.RA
+0000a400: 530a 2020 2020 2020 2020 2020 2020 6461  S.            da
+0000a410: 7461 203d 2073 656c 662e 5f67 6574 5f61  ta = self._get_a
+0000a420: 7272 6179 5f64 6174 6128 6929 0a20 2020  rray_data(i).   
+0000a430: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0000a440: 2e73 7175 6565 7a65 5f6e 6f6e 5f73 7061  .squeeze_non_spa
+0000a450: 7469 616c 5f64 696d 733a 0a20 2020 2020  tial_dims:.     
+0000a460: 2020 2020 2020 2020 2020 2066 6f72 2064             for d
+0000a470: 2069 6e20 7261 6e67 6528 6c65 6e28 6461   in range(len(da
+0000a480: 7461 2e73 6861 7065 292c 206c 656e 2868  ta.shape), len(h
+0000a490: 6561 6465 725b 4d65 7461 4b65 7973 2e53  eader[MetaKeys.S
+0000a4a0: 5041 5449 414c 5f53 4841 5045 5d29 2c20  PATIAL_SHAPE]), 
+0000a4b0: 2d31 293a 0a20 2020 2020 2020 2020 2020  -1):.           
+0000a4c0: 2020 2020 2020 2020 2069 6620 6461 7461           if data
+0000a4d0: 2e73 6861 7065 5b64 202d 2031 5d20 3d3d  .shape[d - 1] ==
+0000a4e0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000a4f0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000a500: 203d 2064 6174 612e 7371 7565 657a 6528   = data.squeeze(
+0000a510: 6178 6973 3d64 202d 2031 290a 2020 2020  axis=d - 1).    
+0000a520: 2020 2020 2020 2020 696d 675f 6172 7261          img_arra
+0000a530: 792e 6170 7065 6e64 2864 6174 6129 0a20  y.append(data). 
+0000a540: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0000a550: 6c66 2e63 6861 6e6e 656c 5f64 696d 2069  lf.channel_dim i
+0000a560: 7320 4e6f 6e65 3a20 2023 2064 6566 6175  s None:  # defau
+0000a570: 6c74 2074 6f20 226e 6f5f 6368 616e 6e65  lt to "no_channe
+0000a580: 6c22 206f 7220 2d31 0a20 2020 2020 2020  l" or -1.       
+0000a590: 2020 2020 2020 2020 2068 6561 6465 725b           header[
+0000a5a0: 4d65 7461 4b65 7973 2e4f 5249 4749 4e41  MetaKeys.ORIGINA
+0000a5b0: 4c5f 4348 414e 4e45 4c5f 4449 4d5d 203d  L_CHANNEL_DIM] =
+0000a5c0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000a5d0: 2020 2020 2020 2066 6c6f 6174 2822 6e61         float("na
+0000a5e0: 6e22 2920 6966 206c 656e 2864 6174 612e  n") if len(data.
+0000a5f0: 7368 6170 6529 203d 3d20 6c65 6e28 6865  shape) == len(he
+0000a600: 6164 6572 5b4d 6574 614b 6579 732e 5350  ader[MetaKeys.SP
+0000a610: 4154 4941 4c5f 5348 4150 455d 2920 656c  ATIAL_SHAPE]) el
+0000a620: 7365 202d 310a 2020 2020 2020 2020 2020  se -1.          
+0000a630: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000a640: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a650: 2020 2020 2020 2020 2020 6865 6164 6572            header
+0000a660: 5b4d 6574 614b 6579 732e 4f52 4947 494e  [MetaKeys.ORIGIN
+0000a670: 414c 5f43 4841 4e4e 454c 5f44 494d 5d20  AL_CHANNEL_DIM] 
+0000a680: 3d20 7365 6c66 2e63 6861 6e6e 656c 5f64  = self.channel_d
+0000a690: 696d 0a20 2020 2020 2020 2020 2020 205f  im.            _
+0000a6a0: 636f 7079 5f63 6f6d 7061 7469 626c 655f  copy_compatible_
+0000a6b0: 6469 6374 2868 6561 6465 722c 2063 6f6d  dict(header, com
+0000a6c0: 7061 7469 626c 655f 6d65 7461 290a 0a20  patible_meta).. 
+0000a6d0: 2020 2020 2020 2072 6574 7572 6e20 5f73         return _s
+0000a6e0: 7461 636b 5f69 6d61 6765 7328 696d 675f  tack_images(img_
+0000a6f0: 6172 7261 792c 2063 6f6d 7061 7469 626c  array, compatibl
+0000a700: 655f 6d65 7461 292c 2063 6f6d 7061 7469  e_meta), compati
+0000a710: 626c 655f 6d65 7461 0a0a 2020 2020 6465  ble_meta..    de
+0000a720: 6620 5f67 6574 5f6d 6574 615f 6469 6374  f _get_meta_dict
+0000a730: 2873 656c 662c 2069 6d67 2920 2d3e 2064  (self, img) -> d
+0000a740: 6963 743a 0a20 2020 2020 2020 2022 2222  ict:.        """
+0000a750: 0a20 2020 2020 2020 2047 6574 2074 6865  .        Get the
+0000a760: 2061 6c6c 2074 6865 206d 6574 6164 6174   all the metadat
+0000a770: 6120 6f66 2074 6865 2069 6d61 6765 2061  a of the image a
+0000a780: 6e64 2063 6f6e 7665 7274 2074 6f20 6469  nd convert to di
+0000a790: 6374 2074 7970 652e 0a0a 2020 2020 2020  ct type...      
+0000a7a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000a7b0: 2020 2020 696d 673a 2061 204e 6962 6162      img: a Nibab
+0000a7c0: 656c 2069 6d61 6765 206f 626a 6563 7420  el image object 
+0000a7d0: 6c6f 6164 6564 2066 726f 6d20 616e 2069  loaded from an i
+0000a7e0: 6d61 6765 2066 696c 652e 0a0a 2020 2020  mage file...    
+0000a7f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000a800: 2320 7377 6170 2074 6f20 6c69 7474 6c65  # swap to little
+0000a810: 2065 6e64 6961 6e20 6173 2050 7954 6f72   endian as PyTor
+0000a820: 6368 2064 6f65 736e 2774 2073 7570 706f  ch doesn't suppo
+0000a830: 7274 2062 6967 2065 6e64 6961 6e0a 2020  rt big endian.  
+0000a840: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0000a850: 2020 2020 2020 2068 6561 6465 7220 3d20         header = 
+0000a860: 696d 672e 6865 6164 6572 2e61 735f 6279  img.header.as_by
+0000a870: 7465 7377 6170 7065 6428 223c 2229 0a20  teswapped("<"). 
+0000a880: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
+0000a890: 6c75 6545 7272 6f72 3a0a 2020 2020 2020  lueError:.      
+0000a8a0: 2020 2020 2020 6865 6164 6572 203d 2069        header = i
+0000a8b0: 6d67 2e68 6561 6465 720a 2020 2020 2020  mg.header.      
+0000a8c0: 2020 7265 7475 726e 2064 6963 7428 6865    return dict(he
+0000a8d0: 6164 6572 290a 0a20 2020 2064 6566 205f  ader)..    def _
+0000a8e0: 6765 745f 6166 6669 6e65 2873 656c 662c  get_affine(self,
+0000a8f0: 2069 6d67 293a 0a20 2020 2020 2020 2022   img):.        "
+0000a900: 2222 0a20 2020 2020 2020 2047 6574 2074  "".        Get t
+0000a910: 6865 2061 6666 696e 6520 6d61 7472 6978  he affine matrix
+0000a920: 206f 6620 7468 6520 696d 6167 652c 2069   of the image, i
+0000a930: 7420 6361 6e20 6265 2075 7365 6420 746f  t can be used to
+0000a940: 2063 6f72 7265 6374 0a20 2020 2020 2020   correct.       
+0000a950: 2073 7061 6369 6e67 2c20 6f72 6965 6e74   spacing, orient
+0000a960: 6174 696f 6e20 6f72 2065 7865 6375 7465  ation or execute
+0000a970: 2073 7061 7469 616c 2074 7261 6e73 666f   spatial transfo
+0000a980: 726d 732e 0a0a 2020 2020 2020 2020 4172  rms...        Ar
+0000a990: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000a9a0: 696d 673a 2061 204e 6962 6162 656c 2069  img: a Nibabel i
+0000a9b0: 6d61 6765 206f 626a 6563 7420 6c6f 6164  mage object load
+0000a9c0: 6564 2066 726f 6d20 616e 2069 6d61 6765  ed from an image
+0000a9d0: 2066 696c 652e 0a0a 2020 2020 2020 2020   file...        
+0000a9e0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000a9f0: 726e 206e 702e 6172 7261 7928 696d 672e  rn np.array(img.
+0000aa00: 6166 6669 6e65 2c20 636f 7079 3d54 7275  affine, copy=Tru
+0000aa10: 6529 0a0a 2020 2020 6465 6620 5f67 6574  e)..    def _get
+0000aa20: 5f73 7061 7469 616c 5f73 6861 7065 2873  _spatial_shape(s
+0000aa30: 656c 662c 2069 6d67 293a 0a20 2020 2020  elf, img):.     
+0000aa40: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+0000aa50: 6574 2074 6865 2073 7061 7469 616c 2073  et the spatial s
+0000aa60: 6861 7065 206f 6620 696d 6167 6520 6461  hape of image da
+0000aa70: 7461 2c20 6974 2064 6f65 736e 2774 2063  ta, it doesn't c
+0000aa80: 6f6e 7461 696e 2074 6865 2063 6861 6e6e  ontain the chann
+0000aa90: 656c 2064 696d 2e0a 0a20 2020 2020 2020  el dim...       
+0000aaa0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000aab0: 2020 2069 6d67 3a20 6120 4e69 6261 6265     img: a Nibabe
+0000aac0: 6c20 696d 6167 6520 6f62 6a65 6374 206c  l image object l
+0000aad0: 6f61 6465 6420 6672 6f6d 2061 6e20 696d  oaded from an im
+0000aae0: 6167 6520 6669 6c65 2e0a 0a20 2020 2020  age file...     
+0000aaf0: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+0000ab00: 2073 7761 7020 746f 206c 6974 746c 6520   swap to little 
+0000ab10: 656e 6469 616e 2061 7320 5079 546f 7263  endian as PyTorc
+0000ab20: 6820 646f 6573 6e27 7420 7375 7070 6f72  h doesn't suppor
+0000ab30: 7420 6269 6720 656e 6469 616e 0a20 2020  t big endian.   
+0000ab40: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000ab50: 2020 2020 2020 6865 6164 6572 203d 2069        header = i
+0000ab60: 6d67 2e68 6561 6465 722e 6173 5f62 7974  mg.header.as_byt
+0000ab70: 6573 7761 7070 6564 2822 3c22 290a 2020  eswapped("<").  
+0000ab80: 2020 2020 2020 6578 6365 7074 2056 616c        except Val
+0000ab90: 7565 4572 726f 723a 0a20 2020 2020 2020  ueError:.       
+0000aba0: 2020 2020 2068 6561 6465 7220 3d20 696d       header = im
+0000abb0: 672e 6865 6164 6572 0a20 2020 2020 2020  g.header.       
+0000abc0: 2064 696d 203d 2068 6561 6465 722e 6765   dim = header.ge
+0000abd0: 7428 2264 696d 222c 204e 6f6e 6529 0a20  t("dim", None). 
+0000abe0: 2020 2020 2020 2069 6620 6469 6d20 6973         if dim is
+0000abf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0000ac00: 2020 2064 696d 203d 2068 6561 6465 722e     dim = header.
+0000ac10: 6765 7428 2264 696d 7322 2920 2023 206d  get("dims")  # m
+0000ac20: 6768 2066 6f72 6d61 743f 0a20 2020 2020  gh format?.     
+0000ac30: 2020 2020 2020 2064 696d 203d 206e 702e         dim = np.
+0000ac40: 696e 7365 7274 2864 696d 2c20 302c 2033  insert(dim, 0, 3
+0000ac50: 290a 2020 2020 2020 2020 6e64 696d 203d  ).        ndim =
+0000ac60: 2064 696d 5b30 5d0a 2020 2020 2020 2020   dim[0].        
+0000ac70: 7369 7a65 203d 206c 6973 7428 6469 6d5b  size = list(dim[
+0000ac80: 313a 5d29 0a20 2020 2020 2020 2069 6620  1:]).        if 
+0000ac90: 6e6f 7420 6973 5f6e 6f5f 6368 616e 6e65  not is_no_channe
+0000aca0: 6c28 7365 6c66 2e63 6861 6e6e 656c 5f64  l(self.channel_d
+0000acb0: 696d 293a 0a20 2020 2020 2020 2020 2020  im):.           
+0000acc0: 2073 697a 652e 706f 7028 696e 7428 7365   size.pop(int(se
+0000acd0: 6c66 2e63 6861 6e6e 656c 5f64 696d 2929  lf.channel_dim))
+0000ace0: 2020 2320 7479 7065 3a20 6967 6e6f 7265    # type: ignore
+0000acf0: 0a20 2020 2020 2020 2073 7061 7469 616c  .        spatial
+0000ad00: 5f72 616e 6b20 3d20 6d61 7828 6d69 6e28  _rank = max(min(
+0000ad10: 6e64 696d 2c20 3329 2c20 3129 0a20 2020  ndim, 3), 1).   
+0000ad20: 2020 2020 2072 6574 7572 6e20 6e70 2e61       return np.a
+0000ad30: 7361 7272 6179 2873 697a 655b 3a73 7061  sarray(size[:spa
+0000ad40: 7469 616c 5f72 616e 6b5d 290a 0a20 2020  tial_rank])..   
+0000ad50: 2064 6566 205f 6765 745f 6172 7261 795f   def _get_array_
+0000ad60: 6461 7461 2873 656c 662c 2069 6d67 293a  data(self, img):
+0000ad70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ad80: 2020 2020 2047 6574 2074 6865 2072 6177       Get the raw
+0000ad90: 2061 7272 6179 2064 6174 6120 6f66 2074   array data of t
+0000ada0: 6865 2069 6d61 6765 2c20 636f 6e76 6572  he image, conver
+0000adb0: 7465 6420 746f 204e 756d 7079 2061 7272  ted to Numpy arr
+0000adc0: 6179 2e0a 0a20 2020 2020 2020 2041 7267  ay...        Arg
+0000add0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+0000ade0: 6d67 3a20 6120 4e69 6261 6265 6c20 696d  mg: a Nibabel im
+0000adf0: 6167 6520 6f62 6a65 6374 206c 6f61 6465  age object loade
+0000ae00: 6420 6672 6f6d 2061 6e20 696d 6167 6520  d from an image 
+0000ae10: 6669 6c65 2e0a 0a20 2020 2020 2020 2022  file...        "
+0000ae20: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
+0000ae30: 6e20 6e70 2e61 7361 6e79 6172 7261 7928  n np.asanyarray(
+0000ae40: 696d 672e 6461 7461 6f62 6a2c 206f 7264  img.dataobj, ord
+0000ae50: 6572 3d22 4322 290a 0a0a 636c 6173 7320  er="C")...class 
+0000ae60: 4e75 6d70 7952 6561 6465 7228 496d 6167  NumpyReader(Imag
+0000ae70: 6552 6561 6465 7229 3a0a 2020 2020 2222  eReader):.    ""
+0000ae80: 220a 2020 2020 4c6f 6164 204e 5059 206f  ".    Load NPY o
+0000ae90: 7220 4e50 5a20 666f 726d 6174 2064 6174  r NPZ format dat
+0000aea0: 6120 6261 7365 6420 6f6e 204e 756d 7079  a based on Numpy
+0000aeb0: 206c 6962 7261 7279 2c20 7468 6579 2063   library, they c
+0000aec0: 616e 2062 6520 6172 7261 7973 206f 7220  an be arrays or 
+0000aed0: 7069 636b 6c65 6420 6f62 6a65 6374 732e  pickled objects.
+0000aee0: 0a20 2020 2041 2074 7970 6963 616c 2075  .    A typical u
+0000aef0: 7361 6765 2069 7320 746f 206c 6f61 6420  sage is to load 
+0000af00: 7468 6520 606d 6173 6b60 2064 6174 6120  the `mask` data 
+0000af10: 666f 7220 636c 6173 7369 6669 6361 7469  for classificati
+0000af20: 6f6e 2074 6173 6b2e 0a20 2020 2049 7420  on task..    It 
+0000af30: 6361 6e20 6c6f 6164 2070 6172 7420 6f66  can load part of
+0000af40: 2074 6865 206e 707a 2066 696c 6520 7769   the npz file wi
+0000af50: 7468 2073 7065 6369 6669 6564 2060 6e70  th specified `np
+0000af60: 7a5f 6b65 7973 602e 0a0a 2020 2020 4172  z_keys`...    Ar
+0000af70: 6773 3a0a 2020 2020 2020 2020 6e70 7a5f  gs:.        npz_
+0000af80: 6b65 7973 3a20 6966 206c 6f61 6469 6e67  keys: if loading
+0000af90: 206e 707a 2066 696c 652c 206f 6e6c 7920   npz file, only 
+0000afa0: 6c6f 6164 2074 6865 2073 7065 6369 6669  load the specifi
+0000afb0: 6564 206b 6579 732c 2069 6620 4e6f 6e65  ed keys, if None
+0000afc0: 2c20 6c6f 6164 2061 6c6c 2074 6865 2069  , load all the i
+0000afd0: 7465 6d73 2e0a 2020 2020 2020 2020 2020  tems..          
+0000afe0: 2020 7374 6163 6b20 7468 6520 6c6f 6164    stack the load
+0000aff0: 6564 2069 7465 6d73 2074 6f67 6574 6865  ed items togethe
+0000b000: 7220 746f 2063 6f6e 7374 7275 6374 2061  r to construct a
+0000b010: 206e 6577 2066 6972 7374 2064 696d 656e   new first dimen
+0000b020: 7369 6f6e 2e0a 2020 2020 2020 2020 6368  sion..        ch
+0000b030: 616e 6e65 6c5f 6469 6d3a 2069 6620 6e6f  annel_dim: if no
+0000b040: 7420 4e6f 6e65 2c20 6578 706c 6963 6974  t None, explicit
+0000b050: 6c79 2073 7065 6369 6679 2074 6865 2063  ly specify the c
+0000b060: 6861 6e6e 656c 2064 696d 2c20 6f74 6865  hannel dim, othe
+0000b070: 7277 6973 652c 2074 7265 6174 2074 6865  rwise, treat the
+0000b080: 2061 7272 6179 2061 7320 6e6f 2063 6861   array as no cha
+0000b090: 6e6e 656c 2e0a 2020 2020 2020 2020 6b77  nnel..        kw
+0000b0a0: 6172 6773 3a20 6164 6469 7469 6f6e 616c  args: additional
+0000b0b0: 2061 7267 7320 666f 7220 606e 756d 7079   args for `numpy
+0000b0c0: 2e6c 6f61 6460 2041 5049 2065 7863 6570  .load` API excep
+0000b0d0: 7420 6061 6c6c 6f77 5f70 6963 6b6c 6560  t `allow_pickle`
+0000b0e0: 2e20 6d6f 7265 2064 6574 6169 6c73 2061  . more details a
+0000b0f0: 626f 7574 2061 7661 696c 6162 6c65 2061  bout available a
+0000b100: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000b110: 2068 7474 7073 3a2f 2f6e 756d 7079 2e6f   https://numpy.o
+0000b120: 7267 2f64 6f63 2f73 7461 626c 652f 7265  rg/doc/stable/re
+0000b130: 6665 7265 6e63 652f 6765 6e65 7261 7465  ference/generate
+0000b140: 642f 6e75 6d70 792e 6c6f 6164 2e68 746d  d/numpy.load.htm
+0000b150: 6c0a 0a20 2020 2022 2222 0a0a 2020 2020  l..    """..    
+0000b160: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000b170: 662c 206e 707a 5f6b 6579 733a 204b 6579  f, npz_keys: Key
+0000b180: 7343 6f6c 6c65 6374 696f 6e20 7c20 4e6f  sCollection | No
+0000b190: 6e65 203d 204e 6f6e 652c 2063 6861 6e6e  ne = None, chann
+0000b1a0: 656c 5f64 696d 3a20 7374 7220 7c20 696e  el_dim: str | in
+0000b1b0: 7420 7c20 4e6f 6e65 203d 204e 6f6e 652c  t | None = None,
+0000b1c0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+0000b1d0: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
+0000b1e0: 6974 5f5f 2829 0a20 2020 2020 2020 2069  it__().        i
+0000b1f0: 6620 6e70 7a5f 6b65 7973 2069 7320 6e6f  f npz_keys is no
+0000b200: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000b210: 2020 2020 6e70 7a5f 6b65 7973 203d 2065      npz_keys = e
+0000b220: 6e73 7572 655f 7475 706c 6528 6e70 7a5f  nsure_tuple(npz_
+0000b230: 6b65 7973 290a 2020 2020 2020 2020 7365  keys).        se
+0000b240: 6c66 2e6e 707a 5f6b 6579 7320 3d20 6e70  lf.npz_keys = np
+0000b250: 7a5f 6b65 7973 0a20 2020 2020 2020 2073  z_keys.        s
+0000b260: 656c 662e 6368 616e 6e65 6c5f 6469 6d20  elf.channel_dim 
+0000b270: 3d20 666c 6f61 7428 226e 616e 2229 2069  = float("nan") i
+0000b280: 6620 6368 616e 6e65 6c5f 6469 6d20 3d3d  f channel_dim ==
+0000b290: 2022 6e6f 5f63 6861 6e6e 656c 2220 656c   "no_channel" el
+0000b2a0: 7365 2063 6861 6e6e 656c 5f64 696d 0a20  se channel_dim. 
+0000b2b0: 2020 2020 2020 2073 656c 662e 6b77 6172         self.kwar
+0000b2c0: 6773 203d 206b 7761 7267 730a 0a20 2020  gs = kwargs..   
+0000b2d0: 2064 6566 2076 6572 6966 795f 7375 6666   def verify_suff
+0000b2e0: 6978 2873 656c 662c 2066 696c 656e 616d  ix(self, filenam
+0000b2f0: 653a 2053 6571 7565 6e63 655b 5061 7468  e: Sequence[Path
+0000b300: 4c69 6b65 5d20 7c20 5061 7468 4c69 6b65  Like] | PathLike
+0000b310: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+0000b320: 2020 2022 2222 0a20 2020 2020 2020 2056     """.        V
+0000b330: 6572 6966 7920 7768 6574 6865 7220 7468  erify whether th
+0000b340: 6520 7370 6563 6966 6965 6420 6669 6c65  e specified file
+0000b350: 206f 7220 6669 6c65 7320 666f 726d 6174   or files format
+0000b360: 2069 7320 7375 7070 6f72 7465 6420 6279   is supported by
+0000b370: 204e 756d 7079 2072 6561 6465 722e 0a0a   Numpy reader...
+0000b380: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000b390: 2020 2020 2020 2020 2020 6669 6c65 6e61            filena
+0000b3a0: 6d65 3a20 6669 6c65 206e 616d 6520 6f72  me: file name or
+0000b3b0: 2061 206c 6973 7420 6f66 2066 696c 6520   a list of file 
+0000b3c0: 6e61 6d65 7320 746f 2072 6561 642e 0a20  names to read.. 
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000b3e0: 6620 6120 6c69 7374 206f 6620 6669 6c65  f a list of file
+0000b3f0: 732c 2076 6572 6966 7920 616c 6c20 7468  s, verify all th
+0000b400: 6520 7375 6666 6978 6573 2e0a 2020 2020  e suffixes..    
+0000b410: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000b420: 7375 6666 6978 6573 3a20 5365 7175 656e  suffixes: Sequen
+0000b430: 6365 5b73 7472 5d20 3d20 5b22 6e70 7a22  ce[str] = ["npz"
+0000b440: 2c20 226e 7079 225d 0a20 2020 2020 2020  , "npy"].       
+0000b450: 2072 6574 7572 6e20 6973 5f73 7570 706f   return is_suppo
+0000b460: 7274 6564 5f66 6f72 6d61 7428 6669 6c65  rted_format(file
+0000b470: 6e61 6d65 2c20 7375 6666 6978 6573 290a  name, suffixes).
+0000b480: 0a20 2020 2064 6566 2072 6561 6428 7365  .    def read(se
+0000b490: 6c66 2c20 6461 7461 3a20 5365 7175 656e  lf, data: Sequen
+0000b4a0: 6365 5b50 6174 684c 696b 655d 207c 2050  ce[PathLike] | P
+0000b4b0: 6174 684c 696b 652c 202a 2a6b 7761 7267  athLike, **kwarg
+0000b4c0: 7329 3a0a 2020 2020 2020 2020 2222 220a  s):.        """.
+0000b4d0: 2020 2020 2020 2020 5265 6164 2069 6d61          Read ima
+0000b4e0: 6765 2064 6174 6120 6672 6f6d 2073 7065  ge data from spe
+0000b4f0: 6369 6669 6564 2066 696c 6520 6f72 2066  cified file or f
+0000b500: 696c 6573 2c20 6974 2063 616e 2072 6561  iles, it can rea
+0000b510: 6420 6120 6c69 7374 206f 6620 6461 7461  d a list of data
+0000b520: 2066 696c 6573 0a20 2020 2020 2020 2061   files.        a
+0000b530: 6e64 2073 7461 636b 2074 6865 6d20 746f  nd stack them to
+0000b540: 6765 7468 6572 2061 7320 6d75 6c74 692d  gether as multi-
+0000b550: 6368 616e 6e65 6c20 6461 7461 2069 6e20  channel data in 
+0000b560: 6067 6574 5f64 6174 6128 2960 2e0a 2020  `get_data()`..  
+0000b570: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
+0000b580: 7468 6520 7265 7475 726e 6564 206f 626a  the returned obj
+0000b590: 6563 7420 6973 204e 756d 7079 2061 7272  ect is Numpy arr
+0000b5a0: 6179 206f 7220 6c69 7374 206f 6620 4e75  ay or list of Nu
+0000b5b0: 6d70 7920 6172 7261 7973 2e0a 0a20 2020  mpy arrays...   
+0000b5c0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000b5d0: 2020 2020 2020 2064 6174 613a 2066 696c         data: fil
+0000b5e0: 6520 6e61 6d65 206f 7220 6120 6c69 7374  e name or a list
+0000b5f0: 206f 6620 6669 6c65 206e 616d 6573 2074   of file names t
+0000b600: 6f20 7265 6164 2e0a 2020 2020 2020 2020  o read..        
+0000b610: 2020 2020 6b77 6172 6773 3a20 6164 6469      kwargs: addi
+0000b620: 7469 6f6e 616c 2061 7267 7320 666f 7220  tional args for 
+0000b630: 606e 756d 7079 2e6c 6f61 6460 2041 5049  `numpy.load` API
+0000b640: 2065 7863 6570 7420 6061 6c6c 6f77 5f70   except `allow_p
+0000b650: 6963 6b6c 6560 2c20 7769 6c6c 206f 7665  ickle`, will ove
+0000b660: 7272 6964 6520 6073 656c 662e 6b77 6172  rride `self.kwar
+0000b670: 6773 6020 666f 7220 6578 6973 7469 6e67  gs` for existing
+0000b680: 206b 6579 732e 0a20 2020 2020 2020 2020   keys..         
+0000b690: 2020 2020 2020 204d 6f72 6520 6465 7461         More deta
+0000b6a0: 696c 7320 6162 6f75 7420 6176 6169 6c61  ils about availa
+0000b6b0: 626c 6520 6172 6773 3a0a 2020 2020 2020  ble args:.      
+0000b6c0: 2020 2020 2020 2020 2020 6874 7470 733a            https:
+0000b6d0: 2f2f 6e75 6d70 792e 6f72 672f 646f 632f  //numpy.org/doc/
+0000b6e0: 7374 6162 6c65 2f72 6566 6572 656e 6365  stable/reference
+0000b6f0: 2f67 656e 6572 6174 6564 2f6e 756d 7079  /generated/numpy
+0000b700: 2e6c 6f61 642e 6874 6d6c 0a0a 2020 2020  .load.html..    
+0000b710: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000b720: 696d 675f 3a20 6c69 7374 5b4e 6966 7469  img_: list[Nifti
+0000b730: 3149 6d61 6765 5d20 3d20 5b5d 0a0a 2020  1Image] = []..  
+0000b740: 2020 2020 2020 6669 6c65 6e61 6d65 733a        filenames:
+0000b750: 2053 6571 7565 6e63 655b 5061 7468 4c69   Sequence[PathLi
+0000b760: 6b65 5d20 3d20 656e 7375 7265 5f74 7570  ke] = ensure_tup
+0000b770: 6c65 2864 6174 6129 0a20 2020 2020 2020  le(data).       
+0000b780: 206b 7761 7267 735f 203d 2073 656c 662e   kwargs_ = self.
+0000b790: 6b77 6172 6773 2e63 6f70 7928 290a 2020  kwargs.copy().  
+0000b7a0: 2020 2020 2020 6b77 6172 6773 5f2e 7570        kwargs_.up
+0000b7b0: 6461 7465 286b 7761 7267 7329 0a20 2020  date(kwargs).   
+0000b7c0: 2020 2020 2066 6f72 206e 616d 6520 696e       for name in
+0000b7d0: 2066 696c 656e 616d 6573 3a0a 2020 2020   filenames:.    
+0000b7e0: 2020 2020 2020 2020 696d 6720 3d20 6e70          img = np
+0000b7f0: 2e6c 6f61 6428 6e61 6d65 2c20 616c 6c6f  .load(name, allo
+0000b800: 775f 7069 636b 6c65 3d54 7275 652c 202a  w_pickle=True, *
+0000b810: 2a6b 7761 7267 735f 290a 2020 2020 2020  *kwargs_).      
+0000b820: 2020 2020 2020 6966 2050 6174 6828 6e61        if Path(na
+0000b830: 6d65 292e 6e61 6d65 2e65 6e64 7377 6974  me).name.endswit
+0000b840: 6828 222e 6e70 7a22 293a 0a20 2020 2020  h(".npz"):.     
+0000b850: 2020 2020 2020 2020 2020 2023 206c 6f61             # loa
+0000b860: 6420 6578 7065 6374 6564 2069 7465 6d73  d expected items
+0000b870: 2066 726f 6d20 4e50 5a20 6669 6c65 0a20   from NPZ file. 
+0000b880: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000b890: 707a 5f6b 6579 7320 3d20 5b66 2261 7272  pz_keys = [f"arr
+0000b8a0: 5f7b 697d 2220 666f 7220 6920 696e 2072  _{i}" for i in r
+0000b8b0: 616e 6765 286c 656e 2869 6d67 2929 5d20  ange(len(img))] 
+0000b8c0: 6966 2073 656c 662e 6e70 7a5f 6b65 7973  if self.npz_keys
+0000b8d0: 2069 7320 4e6f 6e65 2065 6c73 6520 7365   is None else se
+0000b8e0: 6c66 2e6e 707a 5f6b 6579 730a 2020 2020  lf.npz_keys.    
+0000b8f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000b900: 6b20 696e 206e 707a 5f6b 6579 733a 0a20  k in npz_keys:. 
+0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b920: 2020 2069 6d67 5f2e 6170 7065 6e64 2869     img_.append(i
+0000b930: 6d67 5b6b 5d29 0a20 2020 2020 2020 2020  mg[k]).         
+0000b940: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000b950: 2020 2020 2020 2020 2069 6d67 5f2e 6170           img_.ap
+0000b960: 7065 6e64 2869 6d67 290a 0a20 2020 2020  pend(img)..     
+0000b970: 2020 2072 6574 7572 6e20 696d 675f 2069     return img_ i
+0000b980: 6620 6c65 6e28 696d 675f 2920 3e20 3120  f len(img_) > 1 
+0000b990: 656c 7365 2069 6d67 5f5b 305d 0a0a 2020  else img_[0]..  
+0000b9a0: 2020 6465 6620 6765 745f 6461 7461 2873    def get_data(s
+0000b9b0: 656c 662c 2069 6d67 2920 2d3e 2074 7570  elf, img) -> tup
+0000b9c0: 6c65 5b6e 702e 6e64 6172 7261 792c 2064  le[np.ndarray, d
+0000b9d0: 6963 745d 3a0a 2020 2020 2020 2020 2222  ict]:.        ""
+0000b9e0: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
+0000b9f0: 7420 6461 7461 2061 7272 6179 2061 6e64  t data array and
+0000ba00: 206d 6574 6164 6174 6120 6672 6f6d 206c   metadata from l
+0000ba10: 6f61 6465 6420 696d 6167 6520 616e 6420  oaded image and 
+0000ba20: 7265 7475 726e 2074 6865 6d2e 0a20 2020  return them..   
+0000ba30: 2020 2020 2054 6869 7320 6675 6e63 7469       This functi
+0000ba40: 6f6e 2072 6574 7572 6e73 2074 776f 206f  on returns two o
+0000ba50: 626a 6563 7473 2c20 6669 7273 7420 6973  bjects, first is
+0000ba60: 206e 756d 7079 2061 7272 6179 206f 6620   numpy array of 
+0000ba70: 696d 6167 6520 6461 7461 2c20 7365 636f  image data, seco
+0000ba80: 6e64 2069 7320 6469 6374 206f 6620 6d65  nd is dict of me
+0000ba90: 7461 6461 7461 2e0a 2020 2020 2020 2020  tadata..        
+0000baa0: 4974 2063 6f6e 7374 7275 6374 7320 6061  It constructs `a
+0000bab0: 6666 696e 6560 2c20 606f 7269 6769 6e61  ffine`, `origina
+0000bac0: 6c5f 6166 6669 6e65 602c 2061 6e64 2060  l_affine`, and `
+0000bad0: 7370 6174 6961 6c5f 7368 6170 6560 2061  spatial_shape` a
+0000bae0: 6e64 2073 746f 7265 7320 7468 656d 2069  nd stores them i
+0000baf0: 6e20 6d65 7461 2064 6963 742e 0a20 2020  n meta dict..   
+0000bb00: 2020 2020 2057 6865 6e20 6c6f 6164 696e       When loadin
+0000bb10: 6720 6120 6c69 7374 206f 6620 6669 6c65  g a list of file
+0000bb20: 732c 2074 6865 7920 6172 6520 7374 6163  s, they are stac
+0000bb30: 6b65 6420 746f 6765 7468 6572 2061 7420  ked together at 
+0000bb40: 6120 6e65 7720 6469 6d65 6e73 696f 6e20  a new dimension 
+0000bb50: 6173 2074 6865 2066 6972 7374 2064 696d  as the first dim
+0000bb60: 656e 7369 6f6e 2c0a 2020 2020 2020 2020  ension,.        
+0000bb70: 616e 6420 7468 6520 6d65 7461 6461 7461  and the metadata
+0000bb80: 206f 6620 7468 6520 6669 7273 7420 696d   of the first im
+0000bb90: 6167 6520 6973 2075 7365 6420 746f 2072  age is used to r
+0000bba0: 6570 7265 7365 6e74 2074 6865 206f 7574  epresent the out
+0000bbb0: 7075 7420 6d65 7461 6461 7461 2e0a 0a20  put metadata... 
+0000bbc0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000bbd0: 2020 2020 2020 2020 2069 6d67 3a20 6120           img: a 
+0000bbe0: 4e75 6d70 7920 6172 7261 7920 6c6f 6164  Numpy array load
+0000bbf0: 6564 2066 726f 6d20 6120 6669 6c65 206f  ed from a file o
+0000bc00: 7220 6120 6c69 7374 206f 6620 4e75 6d70  r a list of Nump
+0000bc10: 7920 6172 7261 7973 2e0a 0a20 2020 2020  y arrays...     
+0000bc20: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000bc30: 6d67 5f61 7272 6179 3a20 6c69 7374 5b6e  mg_array: list[n
+0000bc40: 702e 6e64 6172 7261 795d 203d 205b 5d0a  p.ndarray] = [].
+0000bc50: 2020 2020 2020 2020 636f 6d70 6174 6962          compatib
+0000bc60: 6c65 5f6d 6574 613a 2064 6963 7420 3d20  le_meta: dict = 
+0000bc70: 7b7d 0a20 2020 2020 2020 2069 6620 6973  {}.        if is
+0000bc80: 696e 7374 616e 6365 2869 6d67 2c20 6e70  instance(img, np
+0000bc90: 2e6e 6461 7272 6179 293a 0a20 2020 2020  .ndarray):.     
+0000bca0: 2020 2020 2020 2069 6d67 203d 2028 696d         img = (im
+0000bcb0: 672c 290a 0a20 2020 2020 2020 2066 6f72  g,)..        for
+0000bcc0: 2069 2069 6e20 656e 7375 7265 5f74 7570   i in ensure_tup
+0000bcd0: 6c65 2869 6d67 293a 0a20 2020 2020 2020  le(img):.       
+0000bce0: 2020 2020 2068 6561 6465 723a 2064 6963       header: dic
+0000bcf0: 745b 4d65 7461 4b65 7973 2c20 416e 795d  t[MetaKeys, Any]
+0000bd00: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+0000bd10: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000bd20: 692c 206e 702e 6e64 6172 7261 7929 3a0a  i, np.ndarray):.
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd40: 2320 6966 2060 6368 616e 6e65 6c5f 6469  # if `channel_di
+0000bd50: 6d60 2069 7320 4e6f 6e65 2c20 6361 6e20  m` is None, can 
+0000bd60: 6e6f 7420 6465 7465 6374 2074 6865 2063  not detect the c
+0000bd70: 6861 6e6e 656c 2064 696d 2c20 7573 6520  hannel dim, use 
+0000bd80: 616c 6c20 7468 6520 6469 6d73 2061 7320  all the dims as 
+0000bd90: 7370 6174 6961 6c5f 7368 6170 650a 2020  spatial_shape.  
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 7370                sp
+0000bdb0: 6174 6961 6c5f 7368 6170 6520 3d20 6e70  atial_shape = np
+0000bdc0: 2e61 7361 7272 6179 2869 2e73 6861 7065  .asarray(i.shape
+0000bdd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000bde0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000bdf0: 7365 6c66 2e63 6861 6e6e 656c 5f64 696d  self.channel_dim
+0000be00: 2c20 696e 7429 3a0a 2020 2020 2020 2020  , int):.        
+0000be10: 2020 2020 2020 2020 2020 2020 7370 6174              spat
+0000be20: 6961 6c5f 7368 6170 6520 3d20 6e70 2e64  ial_shape = np.d
+0000be30: 656c 6574 6528 7370 6174 6961 6c5f 7368  elete(spatial_sh
+0000be40: 6170 652c 2073 656c 662e 6368 616e 6e65  ape, self.channe
+0000be50: 6c5f 6469 6d29 0a20 2020 2020 2020 2020  l_dim).         
+0000be60: 2020 2020 2020 2068 6561 6465 725b 4d65         header[Me
+0000be70: 7461 4b65 7973 2e53 5041 5449 414c 5f53  taKeys.SPATIAL_S
+0000be80: 4841 5045 5d20 3d20 7370 6174 6961 6c5f  HAPE] = spatial_
+0000be90: 7368 6170 650a 2020 2020 2020 2020 2020  shape.          
+0000bea0: 2020 2020 2020 6865 6164 6572 5b4d 6574        header[Met
+0000beb0: 614b 6579 732e 5350 4143 455d 203d 2053  aKeys.SPACE] = S
+0000bec0: 7061 6365 4b65 7973 2e52 4153 0a20 2020  paceKeys.RAS.   
+0000bed0: 2020 2020 2020 2020 2069 6d67 5f61 7272           img_arr
+0000bee0: 6179 2e61 7070 656e 6428 6929 0a20 2020  ay.append(i).   
+0000bef0: 2020 2020 2020 2020 2068 6561 6465 725b           header[
+0000bf00: 4d65 7461 4b65 7973 2e4f 5249 4749 4e41  MetaKeys.ORIGINA
+0000bf10: 4c5f 4348 414e 4e45 4c5f 4449 4d5d 203d  L_CHANNEL_DIM] =
+0000bf20: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000bf30: 2020 2073 656c 662e 6368 616e 6e65 6c5f     self.channel_
+0000bf40: 6469 6d20 6966 2069 7369 6e73 7461 6e63  dim if isinstanc
+0000bf50: 6528 7365 6c66 2e63 6861 6e6e 656c 5f64  e(self.channel_d
+0000bf60: 696d 2c20 696e 7429 2065 6c73 6520 666c  im, int) else fl
+0000bf70: 6f61 7428 226e 616e 2229 0a20 2020 2020  oat("nan").     
+0000bf80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000bf90: 2020 2020 205f 636f 7079 5f63 6f6d 7061       _copy_compa
+0000bfa0: 7469 626c 655f 6469 6374 2868 6561 6465  tible_dict(heade
+0000bfb0: 722c 2063 6f6d 7061 7469 626c 655f 6d65  r, compatible_me
+0000bfc0: 7461 290a 0a20 2020 2020 2020 2072 6574  ta)..        ret
+0000bfd0: 7572 6e20 5f73 7461 636b 5f69 6d61 6765  urn _stack_image
+0000bfe0: 7328 696d 675f 6172 7261 792c 2063 6f6d  s(img_array, com
+0000bff0: 7061 7469 626c 655f 6d65 7461 292c 2063  patible_meta), c
+0000c000: 6f6d 7061 7469 626c 655f 6d65 7461 0a0a  ompatible_meta..
+0000c010: 0a40 7265 7175 6972 655f 706b 6728 706b  .@require_pkg(pk
+0000c020: 675f 6e61 6d65 3d22 5049 4c22 290a 636c  g_name="PIL").cl
+0000c030: 6173 7320 5049 4c52 6561 6465 7228 496d  ass PILReader(Im
+0000c040: 6167 6552 6561 6465 7229 3a0a 2020 2020  ageReader):.    
+0000c050: 2222 220a 2020 2020 4c6f 6164 2063 6f6d  """.    Load com
+0000c060: 6d6f 6e20 3244 2069 6d61 6765 2066 6f72  mon 2D image for
+0000c070: 6d61 7420 2873 7570 706f 7274 7320 504e  mat (supports PN
+0000c080: 472c 204a 5047 2c20 424d 5029 2066 696c  G, JPG, BMP) fil
+0000c090: 6520 6f72 2066 696c 6573 2066 726f 6d20  e or files from 
+0000c0a0: 7072 6f76 6964 6564 2070 6174 682e 0a0a  provided path...
+0000c0b0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000c0c0: 2020 636f 6e76 6572 7465 723a 2061 6464    converter: add
+0000c0d0: 6974 696f 6e61 6c20 6675 6e63 7469 6f6e  itional function
+0000c0e0: 2074 6f20 636f 6e76 6572 7420 7468 6520   to convert the 
+0000c0f0: 696d 6167 6520 6461 7461 2061 6674 6572  image data after
+0000c100: 2060 7265 6164 2829 602e 0a20 2020 2020   `read()`..     
+0000c110: 2020 2020 2020 2066 6f72 2065 7861 6d70         for examp
+0000c120: 6c65 2c20 7573 6520 6063 6f6e 7665 7274  le, use `convert
+0000c130: 6572 3d6c 616d 6264 6120 696d 6167 653a  er=lambda image:
+0000c140: 2069 6d61 6765 2e63 6f6e 7665 7274 2822   image.convert("
+0000c150: 4c41 2229 6020 746f 2063 6f6e 7665 7274  LA")` to convert
+0000c160: 2069 6d61 6765 2066 6f72 6d61 742e 0a20   image format.. 
+0000c170: 2020 2020 2020 2072 6576 6572 7365 5f69         reverse_i
+0000c180: 6e64 6578 696e 673a 2077 6865 7468 6572  ndexing: whether
+0000c190: 2074 6f20 7377 6170 2061 7869 7320 3020   to swap axis 0 
+0000c1a0: 616e 6420 3120 6166 7465 7220 6c6f 6164  and 1 after load
+0000c1b0: 696e 6720 7468 6520 6172 7261 792c 2074  ing the array, t
+0000c1c0: 6869 7320 6973 2065 6e61 626c 6564 2062  his is enabled b
+0000c1d0: 7920 6465 6661 756c 742c 0a20 2020 2020  y default,.     
+0000c1e0: 2020 2020 2020 2073 6f20 7468 6174 206f         so that o
+0000c1f0: 7574 7075 7420 6f66 2074 6865 2072 6561  utput of the rea
+0000c200: 6465 7220 6973 2063 6f6e 7369 7374 656e  der is consisten
+0000c210: 7420 7769 7468 2074 6865 206f 7468 6572  t with the other
+0000c220: 2072 6561 6465 7273 2e20 5365 7420 7468   readers. Set th
+0000c230: 6973 206f 7074 696f 6e20 746f 2060 6046  is option to ``F
+0000c240: 616c 7365 6060 2074 6f20 7573 650a 2020  alse`` to use.  
+0000c250: 2020 2020 2020 2020 2020 7468 6520 5049            the PI
+0000c260: 4c20 6261 636b 656e 6427 7320 6f72 6967  L backend's orig
+0000c270: 696e 616c 2073 7061 7469 616c 2061 7865  inal spatial axe
+0000c280: 7320 636f 6e76 656e 7469 6f6e 2e0a 2020  s convention..  
+0000c290: 2020 2020 2020 6b77 6172 6773 3a20 6164        kwargs: ad
+0000c2a0: 6469 7469 6f6e 616c 2061 7267 7320 666f  ditional args fo
+0000c2b0: 7220 6049 6d61 6765 2e6f 7065 6e60 2041  r `Image.open` A
+0000c2c0: 5049 2069 6e20 6072 6561 6428 2960 2c20  PI in `read()`, 
+0000c2d0: 6d6f 6465 2064 6574 6169 6c73 2061 626f  mode details abo
+0000c2e0: 7574 2061 7661 696c 6162 6c65 2061 7267  ut available arg
+0000c2f0: 733a 0a20 2020 2020 2020 2020 2020 2068  s:.            h
+0000c300: 7474 7073 3a2f 2f70 696c 6c6f 772e 7265  ttps://pillow.re
+0000c310: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+0000c320: 7374 6162 6c65 2f72 6566 6572 656e 6365  stable/reference
+0000c330: 2f49 6d61 6765 2e68 746d 6c23 5049 4c2e  /Image.html#PIL.
+0000c340: 496d 6167 652e 6f70 656e 0a20 2020 2022  Image.open.    "
+0000c350: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+0000c360: 6974 5f5f 2873 656c 662c 2063 6f6e 7665  it__(self, conve
+0000c370: 7274 6572 3a20 4361 6c6c 6162 6c65 207c  rter: Callable |
+0000c380: 204e 6f6e 6520 3d20 4e6f 6e65 2c20 7265   None = None, re
+0000c390: 7665 7273 655f 696e 6465 7869 6e67 3a20  verse_indexing: 
+0000c3a0: 626f 6f6c 203d 2054 7275 652c 202a 2a6b  bool = True, **k
+0000c3b0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+0000c3c0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+0000c3d0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000c3e0: 636f 6e76 6572 7465 7220 3d20 636f 6e76  converter = conv
+0000c3f0: 6572 7465 720a 2020 2020 2020 2020 7365  erter.        se
+0000c400: 6c66 2e72 6576 6572 7365 5f69 6e64 6578  lf.reverse_index
+0000c410: 696e 6720 3d20 7265 7665 7273 655f 696e  ing = reverse_in
+0000c420: 6465 7869 6e67 0a20 2020 2020 2020 2073  dexing.        s
+0000c430: 656c 662e 6b77 6172 6773 203d 206b 7761  elf.kwargs = kwa
+0000c440: 7267 730a 0a20 2020 2064 6566 2076 6572  rgs..    def ver
+0000c450: 6966 795f 7375 6666 6978 2873 656c 662c  ify_suffix(self,
+0000c460: 2066 696c 656e 616d 653a 2053 6571 7565   filename: Seque
+0000c470: 6e63 655b 5061 7468 4c69 6b65 5d20 7c20  nce[PathLike] | 
+0000c480: 5061 7468 4c69 6b65 2920 2d3e 2062 6f6f  PathLike) -> boo
+0000c490: 6c3a 0a20 2020 2020 2020 2022 2222 0a20  l:.        """. 
+0000c4a0: 2020 2020 2020 2056 6572 6966 7920 7768         Verify wh
+0000c4b0: 6574 6865 7220 7468 6520 7370 6563 6966  ether the specif
+0000c4c0: 6965 6420 6669 6c65 206f 7220 6669 6c65  ied file or file
+0000c4d0: 7320 666f 726d 6174 2069 7320 7375 7070  s format is supp
+0000c4e0: 6f72 7465 6420 6279 2050 494c 2072 6561  orted by PIL rea
+0000c4f0: 6465 722e 0a0a 2020 2020 2020 2020 4172  der...        Ar
+0000c500: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000c510: 6669 6c65 6e61 6d65 3a20 6669 6c65 206e  filename: file n
+0000c520: 616d 6520 6f72 2061 206c 6973 7420 6f66  ame or a list of
+0000c530: 2066 696c 6520 6e61 6d65 7320 746f 2072   file names to r
+0000c540: 6561 642e 0a20 2020 2020 2020 2020 2020  ead..           
+0000c550: 2020 2020 2069 6620 6120 6c69 7374 206f       if a list o
+0000c560: 6620 6669 6c65 732c 2076 6572 6966 7920  f files, verify 
+0000c570: 616c 6c20 7468 6520 7375 6666 6978 6573  all the suffixes
+0000c580: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000c590: 2020 2020 2020 7375 6666 6978 6573 3a20        suffixes: 
+0000c5a0: 5365 7175 656e 6365 5b73 7472 5d20 3d20  Sequence[str] = 
+0000c5b0: 5b22 706e 6722 2c20 226a 7067 222c 2022  ["png", "jpg", "
+0000c5c0: 6a70 6567 222c 2022 626d 7022 5d0a 2020  jpeg", "bmp"].  
+0000c5d0: 2020 2020 2020 7265 7475 726e 2068 6173        return has
+0000c5e0: 5f70 696c 2061 6e64 2069 735f 7375 7070  _pil and is_supp
+0000c5f0: 6f72 7465 645f 666f 726d 6174 2866 696c  orted_format(fil
+0000c600: 656e 616d 652c 2073 7566 6669 7865 7329  ename, suffixes)
+0000c610: 0a0a 2020 2020 6465 6620 7265 6164 2873  ..    def read(s
+0000c620: 656c 662c 2064 6174 613a 2053 6571 7565  elf, data: Seque
+0000c630: 6e63 655b 5061 7468 4c69 6b65 5d20 7c20  nce[PathLike] | 
+0000c640: 5061 7468 4c69 6b65 207c 206e 702e 6e64  PathLike | np.nd
+0000c650: 6172 7261 792c 202a 2a6b 7761 7267 7329  array, **kwargs)
+0000c660: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000c670: 2020 2020 2020 5265 6164 2069 6d61 6765        Read image
+0000c680: 2064 6174 6120 6672 6f6d 2073 7065 6369   data from speci
+0000c690: 6669 6564 2066 696c 6520 6f72 2066 696c  fied file or fil
+0000c6a0: 6573 2c20 6974 2063 616e 2072 6561 6420  es, it can read 
+0000c6b0: 6120 6c69 7374 206f 6620 696d 6167 6573  a list of images
+0000c6c0: 0a20 2020 2020 2020 2061 6e64 2073 7461  .        and sta
+0000c6d0: 636b 2074 6865 6d20 746f 6765 7468 6572  ck them together
+0000c6e0: 2061 7320 6d75 6c74 692d 6368 616e 6e65   as multi-channe
+0000c6f0: 6c20 6461 7461 2069 6e20 6067 6574 5f64  l data in `get_d
+0000c700: 6174 6128 2960 2e0a 2020 2020 2020 2020  ata()`..        
+0000c710: 4e6f 7465 2074 6861 7420 7468 6520 7265  Note that the re
+0000c720: 7475 726e 6564 206f 626a 6563 7420 6973  turned object is
+0000c730: 2050 494c 2069 6d61 6765 206f 7220 6c69   PIL image or li
+0000c740: 7374 206f 6620 5049 4c20 696d 6167 652e  st of PIL image.
+0000c750: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000c760: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000c770: 3a20 6669 6c65 206e 616d 6520 6f72 2061  : file name or a
+0000c780: 206c 6973 7420 6f66 2066 696c 6520 6e61   list of file na
+0000c790: 6d65 7320 746f 2072 6561 642e 0a20 2020  mes to read..   
+0000c7a0: 2020 2020 2020 2020 206b 7761 7267 733a           kwargs:
+0000c7b0: 2061 6464 6974 696f 6e61 6c20 6172 6773   additional args
+0000c7c0: 2066 6f72 2060 496d 6167 652e 6f70 656e   for `Image.open
+0000c7d0: 6020 4150 4920 696e 2060 7265 6164 2829  ` API in `read()
+0000c7e0: 602c 2077 696c 6c20 6f76 6572 7269 6465  `, will override
+0000c7f0: 2060 7365 6c66 2e6b 7761 7267 7360 2066   `self.kwargs` f
+0000c800: 6f72 2065 7869 7374 696e 6720 6b65 7973  or existing keys
+0000c810: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000c820: 2020 4d6f 6465 2064 6574 6169 6c73 2061    Mode details a
+0000c830: 626f 7574 2061 7661 696c 6162 6c65 2061  bout available a
+0000c840: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000c850: 2020 2020 2068 7474 7073 3a2f 2f70 696c       https://pil
+0000c860: 6c6f 772e 7265 6164 7468 6564 6f63 732e  low.readthedocs.
+0000c870: 696f 2f65 6e2f 7374 6162 6c65 2f72 6566  io/en/stable/ref
+0000c880: 6572 656e 6365 2f49 6d61 6765 2e68 746d  erence/Image.htm
+0000c890: 6c23 5049 4c2e 496d 6167 652e 6f70 656e  l#PIL.Image.open
+0000c8a0: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000c8b0: 2020 2020 2020 696d 675f 3a20 6c69 7374        img_: list
+0000c8c0: 5b50 494c 496d 6167 652e 496d 6167 655d  [PILImage.Image]
+0000c8d0: 203d 205b 5d0a 0a20 2020 2020 2020 2066   = []..        f
+0000c8e0: 696c 656e 616d 6573 3a20 5365 7175 656e  ilenames: Sequen
+0000c8f0: 6365 5b50 6174 684c 696b 655d 203d 2065  ce[PathLike] = e
+0000c900: 6e73 7572 655f 7475 706c 6528 6461 7461  nsure_tuple(data
+0000c910: 290a 2020 2020 2020 2020 6b77 6172 6773  ).        kwargs
+0000c920: 5f20 3d20 7365 6c66 2e6b 7761 7267 732e  _ = self.kwargs.
+0000c930: 636f 7079 2829 0a20 2020 2020 2020 206b  copy().        k
+0000c940: 7761 7267 735f 2e75 7064 6174 6528 6b77  wargs_.update(kw
+0000c950: 6172 6773 290a 2020 2020 2020 2020 666f  args).        fo
+0000c960: 7220 6e61 6d65 2069 6e20 6669 6c65 6e61  r name in filena
+0000c970: 6d65 733a 0a20 2020 2020 2020 2020 2020  mes:.           
+0000c980: 2069 6d67 203d 2050 494c 496d 6167 652e   img = PILImage.
+0000c990: 6f70 656e 286e 616d 652c 202a 2a6b 7761  open(name, **kwa
+0000c9a0: 7267 735f 290a 2020 2020 2020 2020 2020  rgs_).          
+0000c9b0: 2020 6966 2063 616c 6c61 626c 6528 7365    if callable(se
+0000c9c0: 6c66 2e63 6f6e 7665 7274 6572 293a 0a20  lf.converter):. 
+0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c9e0: 6d67 203d 2073 656c 662e 636f 6e76 6572  mg = self.conver
+0000c9f0: 7465 7228 696d 6729 0a20 2020 2020 2020  ter(img).       
+0000ca00: 2020 2020 2069 6d67 5f2e 6170 7065 6e64       img_.append
+0000ca10: 2869 6d67 290a 0a20 2020 2020 2020 2072  (img)..        r
+0000ca20: 6574 7572 6e20 696d 675f 2069 6620 6c65  eturn img_ if le
+0000ca30: 6e28 6669 6c65 6e61 6d65 7329 203e 2031  n(filenames) > 1
+0000ca40: 2065 6c73 6520 696d 675f 5b30 5d0a 0a20   else img_[0].. 
+0000ca50: 2020 2064 6566 2067 6574 5f64 6174 6128     def get_data(
+0000ca60: 7365 6c66 2c20 696d 6729 202d 3e20 7475  self, img) -> tu
+0000ca70: 706c 655b 6e70 2e6e 6461 7272 6179 2c20  ple[np.ndarray, 
+0000ca80: 6469 6374 5d3a 0a20 2020 2020 2020 2022  dict]:.        "
+0000ca90: 2222 0a20 2020 2020 2020 2045 7874 7261  "".        Extra
+0000caa0: 6374 2064 6174 6120 6172 7261 7920 616e  ct data array an
+0000cab0: 6420 6d65 7461 6461 7461 2066 726f 6d20  d metadata from 
+0000cac0: 6c6f 6164 6564 2069 6d61 6765 2061 6e64  loaded image and
+0000cad0: 2072 6574 7572 6e20 7468 656d 2e0a 2020   return them..  
+0000cae0: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
+0000caf0: 696f 6e20 7265 7475 726e 7320 7477 6f20  ion returns two 
+0000cb00: 6f62 6a65 6374 732c 2066 6972 7374 2069  objects, first i
+0000cb10: 7320 6e75 6d70 7920 6172 7261 7920 6f66  s numpy array of
+0000cb20: 2069 6d61 6765 2064 6174 612c 2073 6563   image data, sec
+0000cb30: 6f6e 6420 6973 2064 6963 7420 6f66 206d  ond is dict of m
+0000cb40: 6574 6164 6174 612e 0a20 2020 2020 2020  etadata..       
+0000cb50: 2049 7420 636f 6d70 7574 6573 2060 7370   It computes `sp
+0000cb60: 6174 6961 6c5f 7368 6170 6560 2061 6e64  atial_shape` and
+0000cb70: 2073 746f 7265 7320 6974 2069 6e20 6d65   stores it in me
+0000cb80: 7461 2064 6963 742e 0a20 2020 2020 2020  ta dict..       
+0000cb90: 2057 6865 6e20 6c6f 6164 696e 6720 6120   When loading a 
+0000cba0: 6c69 7374 206f 6620 6669 6c65 732c 2074  list of files, t
+0000cbb0: 6865 7920 6172 6520 7374 6163 6b65 6420  hey are stacked 
+0000cbc0: 746f 6765 7468 6572 2061 7420 6120 6e65  together at a ne
+0000cbd0: 7720 6469 6d65 6e73 696f 6e20 6173 2074  w dimension as t
+0000cbe0: 6865 2066 6972 7374 2064 696d 656e 7369  he first dimensi
+0000cbf0: 6f6e 2c0a 2020 2020 2020 2020 616e 6420  on,.        and 
+0000cc00: 7468 6520 6d65 7461 6461 7461 206f 6620  the metadata of 
+0000cc10: 7468 6520 6669 7273 7420 696d 6167 6520  the first image 
+0000cc20: 6973 2075 7365 6420 746f 2072 6570 7265  is used to repre
+0000cc30: 7365 6e74 2074 6865 206f 7574 7075 7420  sent the output 
+0000cc40: 6d65 7461 6461 7461 2e0a 2020 2020 2020  metadata..      
+0000cc50: 2020 4e6f 7465 2074 6861 7420 6279 2064    Note that by d
+0000cc60: 6566 6175 6c74 2060 7365 6c66 2e72 6576  efault `self.rev
+0000cc70: 6572 7365 5f69 6e64 6578 696e 6760 2069  erse_indexing` i
+0000cc80: 7320 7365 7420 746f 2060 6054 7275 6560  s set to ``True`
+0000cc90: 602c 2077 6869 6368 2073 7761 7073 2061  `, which swaps a
+0000cca0: 7869 7320 3020 616e 6420 3120 6166 7465  xis 0 and 1 afte
+0000ccb0: 7220 6c6f 6164 696e 670a 2020 2020 2020  r loading.      
+0000ccc0: 2020 7468 6520 6172 7261 7920 6265 6361    the array beca
+0000ccd0: 7573 6520 7468 6520 7370 6174 6961 6c20  use the spatial 
+0000cce0: 6178 6573 2064 6566 696e 6974 696f 6e20  axes definition 
+0000ccf0: 696e 2050 494c 2069 7320 6469 6666 6572  in PIL is differ
+0000cd00: 656e 7420 6672 6f6d 206f 7468 6572 2063  ent from other c
+0000cd10: 6f6d 6d6f 6e20 6d65 6469 6361 6c20 7061  ommon medical pa
+0000cd20: 636b 6167 6573 2e0a 0a20 2020 2020 2020  ckages...       
+0000cd30: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000cd40: 2020 2069 6d67 3a20 6120 5049 4c20 496d     img: a PIL Im
+0000cd50: 6167 6520 6f62 6a65 6374 206c 6f61 6465  age object loade
+0000cd60: 6420 6672 6f6d 2061 2066 696c 6520 6f72  d from a file or
+0000cd70: 2061 206c 6973 7420 6f66 2050 494c 2049   a list of PIL I
+0000cd80: 6d61 6765 206f 626a 6563 7473 2e0a 0a20  mage objects... 
+0000cd90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000cda0: 2020 2069 6d67 5f61 7272 6179 3a20 6c69     img_array: li
+0000cdb0: 7374 5b6e 702e 6e64 6172 7261 795d 203d  st[np.ndarray] =
+0000cdc0: 205b 5d0a 2020 2020 2020 2020 636f 6d70   [].        comp
+0000cdd0: 6174 6962 6c65 5f6d 6574 613a 2064 6963  atible_meta: dic
+0000cde0: 7420 3d20 7b7d 0a0a 2020 2020 2020 2020  t = {}..        
+0000cdf0: 666f 7220 6920 696e 2065 6e73 7572 655f  for i in ensure_
+0000ce00: 7475 706c 6528 696d 6729 3a0a 2020 2020  tuple(img):.    
+0000ce10: 2020 2020 2020 2020 6865 6164 6572 203d          header =
+0000ce20: 2073 656c 662e 5f67 6574 5f6d 6574 615f   self._get_meta_
+0000ce30: 6469 6374 2869 290a 2020 2020 2020 2020  dict(i).        
+0000ce40: 2020 2020 6865 6164 6572 5b4d 6574 614b      header[MetaK
+0000ce50: 6579 732e 5350 4154 4941 4c5f 5348 4150  eys.SPATIAL_SHAP
+0000ce60: 455d 203d 2073 656c 662e 5f67 6574 5f73  E] = self._get_s
+0000ce70: 7061 7469 616c 5f73 6861 7065 2869 290a  patial_shape(i).
+0000ce80: 2020 2020 2020 2020 2020 2020 6461 7461              data
+0000ce90: 203d 206e 702e 6d6f 7665 6178 6973 286e   = np.moveaxis(n
+0000cea0: 702e 6173 6172 7261 7928 6929 2c20 302c  p.asarray(i), 0,
+0000ceb0: 2031 2920 6966 2073 656c 662e 7265 7665   1) if self.reve
+0000cec0: 7273 655f 696e 6465 7869 6e67 2065 6c73  rse_indexing els
+0000ced0: 6520 6e70 2e61 7361 7272 6179 2869 290a  e np.asarray(i).
+0000cee0: 2020 2020 2020 2020 2020 2020 696d 675f              img_
+0000cef0: 6172 7261 792e 6170 7065 6e64 2864 6174  array.append(dat
+0000cf00: 6129 0a20 2020 2020 2020 2020 2020 2068  a).            h
+0000cf10: 6561 6465 725b 4d65 7461 4b65 7973 2e4f  eader[MetaKeys.O
+0000cf20: 5249 4749 4e41 4c5f 4348 414e 4e45 4c5f  RIGINAL_CHANNEL_
+0000cf30: 4449 4d5d 203d 2028 0a20 2020 2020 2020  DIM] = (.       
+0000cf40: 2020 2020 2020 2020 2066 6c6f 6174 2822           float("
+0000cf50: 6e61 6e22 2920 6966 206c 656e 2864 6174  nan") if len(dat
+0000cf60: 612e 7368 6170 6529 203d 3d20 6c65 6e28  a.shape) == len(
+0000cf70: 6865 6164 6572 5b4d 6574 614b 6579 732e  header[MetaKeys.
+0000cf80: 5350 4154 4941 4c5f 5348 4150 455d 2920  SPATIAL_SHAPE]) 
+0000cf90: 656c 7365 202d 310a 2020 2020 2020 2020  else -1.        
+0000cfa0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000cfb0: 2020 5f63 6f70 795f 636f 6d70 6174 6962    _copy_compatib
+0000cfc0: 6c65 5f64 6963 7428 6865 6164 6572 2c20  le_dict(header, 
+0000cfd0: 636f 6d70 6174 6962 6c65 5f6d 6574 6129  compatible_meta)
+0000cfe0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000cff0: 205f 7374 6163 6b5f 696d 6167 6573 2869   _stack_images(i
+0000d000: 6d67 5f61 7272 6179 2c20 636f 6d70 6174  mg_array, compat
+0000d010: 6962 6c65 5f6d 6574 6129 2c20 636f 6d70  ible_meta), comp
+0000d020: 6174 6962 6c65 5f6d 6574 610a 0a20 2020  atible_meta..   
+0000d030: 2064 6566 205f 6765 745f 6d65 7461 5f64   def _get_meta_d
+0000d040: 6963 7428 7365 6c66 2c20 696d 6729 202d  ict(self, img) -
+0000d050: 3e20 6469 6374 3a0a 2020 2020 2020 2020  > dict:.        
+0000d060: 2222 220a 2020 2020 2020 2020 4765 7420  """.        Get 
+0000d070: 7468 6520 616c 6c20 7468 6520 6d65 7461  the all the meta
+0000d080: 6461 7461 206f 6620 7468 6520 696d 6167  data of the imag
+0000d090: 6520 616e 6420 636f 6e76 6572 7420 746f  e and convert to
+0000d0a0: 2064 6963 7420 7479 7065 2e0a 2020 2020   dict type..    
+0000d0b0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000d0c0: 2020 2020 2020 696d 673a 2061 2050 494c        img: a PIL
+0000d0d0: 2049 6d61 6765 206f 626a 6563 7420 6c6f   Image object lo
+0000d0e0: 6164 6564 2066 726f 6d20 616e 2069 6d61  aded from an ima
+0000d0f0: 6765 2066 696c 652e 0a0a 2020 2020 2020  ge file...      
+0000d100: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000d110: 7475 726e 207b 2266 6f72 6d61 7422 3a20  turn {"format": 
+0000d120: 696d 672e 666f 726d 6174 2c20 226d 6f64  img.format, "mod
+0000d130: 6522 3a20 696d 672e 6d6f 6465 2c20 2277  e": img.mode, "w
+0000d140: 6964 7468 223a 2069 6d67 2e77 6964 7468  idth": img.width
+0000d150: 2c20 2268 6569 6768 7422 3a20 696d 672e  , "height": img.
+0000d160: 6865 6967 6874 7d0a 0a20 2020 2064 6566  height}..    def
+0000d170: 205f 6765 745f 7370 6174 6961 6c5f 7368   _get_spatial_sh
+0000d180: 6170 6528 7365 6c66 2c20 696d 6729 3a0a  ape(self, img):.
+0000d190: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000d1a0: 2020 2020 4765 7420 7468 6520 7370 6174      Get the spat
+0000d1b0: 6961 6c20 7368 6170 6520 6f66 2069 6d61  ial shape of ima
+0000d1c0: 6765 2064 6174 612c 2069 7420 646f 6573  ge data, it does
+0000d1d0: 6e27 7420 636f 6e74 6169 6e20 7468 6520  n't contain the 
+0000d1e0: 6368 616e 6e65 6c20 6469 6d2e 0a20 2020  channel dim..   
+0000d1f0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000d200: 2020 2020 2020 2069 6d67 3a20 6120 5049         img: a PI
+0000d210: 4c20 496d 6167 6520 6f62 6a65 6374 206c  L Image object l
+0000d220: 6f61 6465 6420 6672 6f6d 2061 6e20 696d  oaded from an im
+0000d230: 6167 6520 6669 6c65 2e0a 2020 2020 2020  age file..      
+0000d240: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000d250: 7475 726e 206e 702e 6173 6172 7261 7928  turn np.asarray(
+0000d260: 2869 6d67 2e77 6964 7468 2c20 696d 672e  (img.width, img.
+0000d270: 6865 6967 6874 2929 0a0a 0a40 6461 7461  height))...@data
+0000d280: 636c 6173 730a 636c 6173 7320 4e72 7264  class.class Nrrd
+0000d290: 496d 6167 653a 0a20 2020 2022 2222 436c  Image:.    """Cl
+0000d2a0: 6173 7320 746f 2077 7261 7020 6e72 7264  ass to wrap nrrd
+0000d2b0: 2069 6d61 6765 2061 7272 6179 2061 6e64   image array and
+0000d2c0: 206d 6574 6164 6174 6120 6865 6164 6572   metadata header
+0000d2d0: 2222 220a 0a20 2020 2061 7272 6179 3a20  """..    array: 
+0000d2e0: 6e70 2e6e 6461 7272 6179 0a20 2020 2068  np.ndarray.    h
+0000d2f0: 6561 6465 723a 2064 6963 740a 0a0a 4072  eader: dict...@r
+0000d300: 6571 7569 7265 5f70 6b67 2870 6b67 5f6e  equire_pkg(pkg_n
+0000d310: 616d 653d 226e 7272 6422 290a 636c 6173  ame="nrrd").clas
+0000d320: 7320 4e72 7264 5265 6164 6572 2849 6d61  s NrrdReader(Ima
+0000d330: 6765 5265 6164 6572 293a 0a20 2020 2022  geReader):.    "
+0000d340: 2222 0a20 2020 204c 6f61 6420 4e52 5244  "".    Load NRRD
+0000d350: 2066 6f72 6d61 7420 696d 6167 6573 2062   format images b
+0000d360: 6173 6564 206f 6e20 7079 6e72 7264 206c  ased on pynrrd l
+0000d370: 6962 7261 7279 2e0a 0a20 2020 2041 7267  ibrary...    Arg
+0000d380: 733a 0a20 2020 2020 2020 2063 6861 6e6e  s:.        chann
+0000d390: 656c 5f64 696d 3a20 7468 6520 6368 616e  el_dim: the chan
+0000d3a0: 6e65 6c20 6469 6d65 6e73 696f 6e20 6f66  nel dimension of
+0000d3b0: 2074 6865 2069 6e70 7574 2069 6d61 6765   the input image
+0000d3c0: 2c20 6465 6661 756c 7420 6973 204e 6f6e  , default is Non
+0000d3d0: 652e 0a20 2020 2020 2020 2020 2020 2054  e..            T
+0000d3e0: 6869 7320 6973 2075 7365 6420 746f 2073  his is used to s
+0000d3f0: 6574 206f 7269 6769 6e61 6c5f 6368 616e  et original_chan
+0000d400: 6e65 6c5f 6469 6d20 696e 2074 6865 206d  nel_dim in the m
+0000d410: 6574 6164 6174 612c 2045 6e73 7572 6543  etadata, EnsureC
+0000d420: 6861 6e6e 656c 4669 7273 7444 2072 6561  hannelFirstD rea
+0000d430: 6473 2074 6869 7320 6669 656c 642e 0a20  ds this field.. 
+0000d440: 2020 2020 2020 2020 2020 2049 6620 4e6f             If No
+0000d450: 6e65 2c20 606f 7269 6769 6e61 6c5f 6368  ne, `original_ch
+0000d460: 616e 6e65 6c5f 6469 6d60 2077 696c 6c20  annel_dim` will 
+0000d470: 6265 2065 6974 6865 7220 606e 6f5f 6368  be either `no_ch
+0000d480: 616e 6e65 6c60 206f 7220 6030 602e 0a20  annel` or `0`.. 
+0000d490: 2020 2020 2020 2020 2020 204e 5252 4420             NRRD 
+0000d4a0: 6669 6c65 7320 6172 6520 7573 7561 6c6c  files are usuall
+0000d4b0: 7920 2263 6861 6e6e 656c 2066 6972 7374  y "channel first
+0000d4c0: 222e 0a20 2020 2020 2020 2064 7479 7065  "..        dtype
+0000d4d0: 3a20 6474 7970 6520 6f66 2074 6865 2064  : dtype of the d
+0000d4e0: 6174 6120 6172 7261 7920 7768 656e 206c  ata array when l
+0000d4f0: 6f61 6469 6e67 2069 6d61 6765 2e0a 2020  oading image..  
+0000d500: 2020 2020 2020 696e 6465 785f 6f72 6465        index_orde
+0000d510: 723a 2053 7065 6369 6679 2077 6865 7468  r: Specify wheth
+0000d520: 6572 2074 6865 2072 6574 7572 6e65 6420  er the returned 
+0000d530: 6461 7461 2061 7272 6179 2073 686f 756c  data array shoul
+0000d540: 6420 6265 2069 6e20 432d 6f72 6465 7220  d be in C-order 
+0000d550: 28e2 8098 43e2 8099 2920 6f72 2046 6f72  (...C...) or For
+0000d560: 7472 616e 2d6f 7264 6572 2028 e280 9846  tran-order (...F
+0000d570: e280 9929 2e0a 2020 2020 2020 2020 2020  ...)..          
+0000d580: 2020 4e75 6d70 7920 6973 2075 7375 616c    Numpy is usual
+0000d590: 6c79 2069 6e20 432d 6f72 6465 722c 2062  ly in C-order, b
+0000d5a0: 7574 2064 6566 6175 6c74 206f 6e20 7468  ut default on th
+0000d5b0: 6520 4e52 5244 2068 6561 6465 7220 6973  e NRRD header is
+0000d5c0: 2046 0a20 2020 2020 2020 2061 6666 696e   F.        affin
+0000d5d0: 655f 6c70 735f 746f 5f72 6173 3a20 7768  e_lps_to_ras: wh
+0000d5e0: 6574 6865 7220 746f 2063 6f6e 7665 7274  ether to convert
+0000d5f0: 2074 6865 2061 6666 696e 6520 6d61 7472   the affine matr
+0000d600: 6978 2066 726f 6d20 224c 5053 2220 746f  ix from "LPS" to
+0000d610: 2022 5241 5322 2e20 4465 6661 756c 7473   "RAS". Defaults
+0000d620: 2074 6f20 6060 5472 7565 6060 2e0a 2020   to ``True``..  
+0000d630: 2020 2020 2020 2020 2020 5365 7420 746f            Set to
+0000d640: 2060 6054 7275 6560 6020 746f 2062 6520   ``True`` to be 
+0000d650: 636f 6e73 6973 7465 6e74 2077 6974 6820  consistent with 
+0000d660: 6060 4e69 6261 6265 6c52 6561 6465 7260  ``NibabelReader`
+0000d670: 602c 206f 7468 6572 7769 7365 2074 6865  `, otherwise the
+0000d680: 2061 6666 696e 6520 6d61 7472 6978 2069   affine matrix i
+0000d690: 7320 756e 6d6f 6469 6669 6564 2e0a 0a20  s unmodified... 
+0000d6a0: 2020 2020 2020 206b 7761 7267 733a 2061         kwargs: a
+0000d6b0: 6464 6974 696f 6e61 6c20 6172 6773 2066  dditional args f
+0000d6c0: 6f72 2060 6e72 7264 2e72 6561 6460 2041  or `nrrd.read` A
+0000d6d0: 5049 2e20 6d6f 7265 2064 6574 6169 6c73  PI. more details
+0000d6e0: 2061 626f 7574 2061 7661 696c 6162 6c65   about available
+0000d6f0: 2061 7267 733a 0a20 2020 2020 2020 2020   args:.         
+0000d700: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
+0000d710: 622e 636f 6d2f 6d68 652f 7079 6e72 7264  b.com/mhe/pynrrd
+0000d720: 2f62 6c6f 622f 6d61 7374 6572 2f6e 7272  /blob/master/nrr
+0000d730: 642f 7265 6164 6572 2e70 790a 0a20 2020  d/reader.py..   
+0000d740: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+0000d750: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0000d760: 7365 6c66 2c0a 2020 2020 2020 2020 6368  self,.        ch
+0000d770: 616e 6e65 6c5f 6469 6d3a 2073 7472 207c  annel_dim: str |
+0000d780: 2069 6e74 207c 204e 6f6e 6520 3d20 4e6f   int | None = No
+0000d790: 6e65 2c0a 2020 2020 2020 2020 6474 7970  ne,.        dtyp
+0000d7a0: 653a 206e 702e 6474 7970 6520 7c20 7479  e: np.dtype | ty
+0000d7b0: 7065 207c 2073 7472 207c 204e 6f6e 6520  pe | str | None 
+0000d7c0: 3d20 6e70 2e66 6c6f 6174 3332 2c0a 2020  = np.float32,.  
+0000d7d0: 2020 2020 2020 696e 6465 785f 6f72 6465        index_orde
+0000d7e0: 723a 2073 7472 203d 2022 4622 2c0a 2020  r: str = "F",.  
+0000d7f0: 2020 2020 2020 6166 6669 6e65 5f6c 7073        affine_lps
+0000d800: 5f74 6f5f 7261 733a 2062 6f6f 6c20 3d20  _to_ras: bool = 
+0000d810: 5472 7565 2c0a 2020 2020 2020 2020 2a2a  True,.        **
+0000d820: 6b77 6172 6773 2c0a 2020 2020 293a 0a20  kwargs,.    ):. 
+0000d830: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
+0000d840: 6e65 6c5f 6469 6d20 3d20 666c 6f61 7428  nel_dim = float(
+0000d850: 226e 616e 2229 2069 6620 6368 616e 6e65  "nan") if channe
+0000d860: 6c5f 6469 6d20 3d3d 2022 6e6f 5f63 6861  l_dim == "no_cha
+0000d870: 6e6e 656c 2220 656c 7365 2063 6861 6e6e  nnel" else chann
+0000d880: 656c 5f64 696d 0a20 2020 2020 2020 2073  el_dim.        s
+0000d890: 656c 662e 6474 7970 6520 3d20 6474 7970  elf.dtype = dtyp
+0000d8a0: 650a 2020 2020 2020 2020 7365 6c66 2e69  e.        self.i
+0000d8b0: 6e64 6578 5f6f 7264 6572 203d 2069 6e64  ndex_order = ind
+0000d8c0: 6578 5f6f 7264 6572 0a20 2020 2020 2020  ex_order.       
+0000d8d0: 2073 656c 662e 6166 6669 6e65 5f6c 7073   self.affine_lps
+0000d8e0: 5f74 6f5f 7261 7320 3d20 6166 6669 6e65  _to_ras = affine
+0000d8f0: 5f6c 7073 5f74 6f5f 7261 730a 2020 2020  _lps_to_ras.    
+0000d900: 2020 2020 7365 6c66 2e6b 7761 7267 7320      self.kwargs 
+0000d910: 3d20 6b77 6172 6773 0a0a 2020 2020 6465  = kwargs..    de
+0000d920: 6620 7665 7269 6679 5f73 7566 6669 7828  f verify_suffix(
+0000d930: 7365 6c66 2c20 6669 6c65 6e61 6d65 3a20  self, filename: 
+0000d940: 5365 7175 656e 6365 5b50 6174 684c 696b  Sequence[PathLik
+0000d950: 655d 207c 2050 6174 684c 696b 6529 202d  e] | PathLike) -
+0000d960: 3e20 626f 6f6c 3a0a 2020 2020 2020 2020  > bool:.        
+0000d970: 2222 220a 2020 2020 2020 2020 5665 7269  """.        Veri
+0000d980: 6679 2077 6865 7468 6572 2074 6865 2073  fy whether the s
+0000d990: 7065 6369 6669 6564 2060 6669 6c65 6e61  pecified `filena
+0000d9a0: 6d65 6020 6973 2073 7570 706f 7274 6564  me` is supported
+0000d9b0: 2062 7920 7079 6e72 7264 2072 6561 6465   by pynrrd reade
+0000d9c0: 722e 0a0a 2020 2020 2020 2020 4172 6773  r...        Args
+0000d9d0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+0000d9e0: 6c65 6e61 6d65 3a20 6669 6c65 206e 616d  lename: file nam
+0000d9f0: 6520 6f72 2061 206c 6973 7420 6f66 2066  e or a list of f
+0000da00: 696c 6520 6e61 6d65 7320 746f 2072 6561  ile names to rea
+0000da10: 642e 0a20 2020 2020 2020 2020 2020 2020  d..             
+0000da20: 2020 2069 6620 6120 6c69 7374 206f 6620     if a list of 
+0000da30: 6669 6c65 732c 2076 6572 6966 7920 616c  files, verify al
+0000da40: 6c20 7468 6520 7375 6666 6978 6573 2e0a  l the suffixes..
+0000da50: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000da60: 2020 2020 2073 7566 6669 7865 733a 2053       suffixes: S
+0000da70: 6571 7565 6e63 655b 7374 725d 203d 205b  equence[str] = [
+0000da80: 226e 7272 6422 2c20 2273 6567 2e6e 7272  "nrrd", "seg.nrr
+0000da90: 6422 5d0a 2020 2020 2020 2020 7265 7475  d"].        retu
+0000daa0: 726e 2068 6173 5f6e 7272 6420 616e 6420  rn has_nrrd and 
+0000dab0: 6973 5f73 7570 706f 7274 6564 5f66 6f72  is_supported_for
+0000dac0: 6d61 7428 6669 6c65 6e61 6d65 2c20 7375  mat(filename, su
+0000dad0: 6666 6978 6573 290a 0a20 2020 2064 6566  ffixes)..    def
+0000dae0: 2072 6561 6428 7365 6c66 2c20 6461 7461   read(self, data
+0000daf0: 3a20 5365 7175 656e 6365 5b50 6174 684c  : Sequence[PathL
+0000db00: 696b 655d 207c 2050 6174 684c 696b 652c  ike] | PathLike,
+0000db10: 202a 2a6b 7761 7267 7329 202d 3e20 5365   **kwargs) -> Se
+0000db20: 7175 656e 6365 5b41 6e79 5d20 7c20 416e  quence[Any] | An
+0000db30: 793a 0a20 2020 2020 2020 2022 2222 0a20  y:.        """. 
+0000db40: 2020 2020 2020 2052 6561 6420 696d 6167         Read imag
+0000db50: 6520 6461 7461 2066 726f 6d20 7370 6563  e data from spec
+0000db60: 6966 6965 6420 6669 6c65 206f 7220 6669  ified file or fi
+0000db70: 6c65 732e 0a20 2020 2020 2020 204e 6f74  les..        Not
+0000db80: 6520 7468 6174 2069 7420 7265 7475 726e  e that it return
+0000db90: 7320 6120 6461 7461 206f 626a 6563 7420  s a data object 
+0000dba0: 6f72 2061 2073 6571 7565 6e63 6520 6f66  or a sequence of
+0000dbb0: 2064 6174 6120 6f62 6a65 6374 732e 0a0a   data objects...
+0000dbc0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000dbd0: 2020 2020 2020 2020 2020 6461 7461 3a20            data: 
+0000dbe0: 6669 6c65 206e 616d 6520 6f72 2061 206c  file name or a l
+0000dbf0: 6973 7420 6f66 2066 696c 6520 6e61 6d65  ist of file name
+0000dc00: 7320 746f 2072 6561 642e 0a20 2020 2020  s to read..     
+0000dc10: 2020 2020 2020 206b 7761 7267 733a 2061         kwargs: a
+0000dc20: 6464 6974 696f 6e61 6c20 6172 6773 2066  dditional args f
+0000dc30: 6f72 2061 6374 7561 6c20 6072 6561 6460  or actual `read`
+0000dc40: 2041 5049 206f 6620 3372 6420 7061 7274   API of 3rd part
+0000dc50: 7920 6c69 6273 2e0a 0a20 2020 2020 2020  y libs...       
+0000dc60: 2022 2222 0a20 2020 2020 2020 2069 6d67   """.        img
+0000dc70: 5f3a 206c 6973 7420 3d20 5b5d 0a20 2020  _: list = [].   
+0000dc80: 2020 2020 2066 696c 656e 616d 6573 3a20       filenames: 
+0000dc90: 5365 7175 656e 6365 5b50 6174 684c 696b  Sequence[PathLik
+0000dca0: 655d 203d 2065 6e73 7572 655f 7475 706c  e] = ensure_tupl
+0000dcb0: 6528 6461 7461 290a 2020 2020 2020 2020  e(data).        
+0000dcc0: 6b77 6172 6773 5f20 3d20 7365 6c66 2e6b  kwargs_ = self.k
+0000dcd0: 7761 7267 732e 636f 7079 2829 0a20 2020  wargs.copy().   
+0000dce0: 2020 2020 206b 7761 7267 735f 2e75 7064       kwargs_.upd
+0000dcf0: 6174 6528 6b77 6172 6773 290a 2020 2020  ate(kwargs).    
+0000dd00: 2020 2020 666f 7220 6e61 6d65 2069 6e20      for name in 
+0000dd10: 6669 6c65 6e61 6d65 733a 0a20 2020 2020  filenames:.     
+0000dd20: 2020 2020 2020 206e 7272 645f 696d 6167         nrrd_imag
+0000dd30: 6520 3d20 4e72 7264 496d 6167 6528 2a6e  e = NrrdImage(*n
+0000dd40: 7272 642e 7265 6164 286e 616d 652c 2069  rrd.read(name, i
+0000dd50: 6e64 6578 5f6f 7264 6572 3d73 656c 662e  ndex_order=self.
+0000dd60: 696e 6465 785f 6f72 6465 722c 202a 6b77  index_order, *kw
+0000dd70: 6172 6773 5f29 290a 2020 2020 2020 2020  args_)).        
+0000dd80: 2020 2020 696d 675f 2e61 7070 656e 6428      img_.append(
+0000dd90: 6e72 7264 5f69 6d61 6765 290a 2020 2020  nrrd_image).    
+0000dda0: 2020 2020 7265 7475 726e 2069 6d67 5f20      return img_ 
+0000ddb0: 6966 206c 656e 2866 696c 656e 616d 6573  if len(filenames
+0000ddc0: 2920 3e20 3120 656c 7365 2069 6d67 5f5b  ) > 1 else img_[
+0000ddd0: 305d 0a0a 2020 2020 6465 6620 6765 745f  0]..    def get_
+0000dde0: 6461 7461 2873 656c 662c 2069 6d67 3a20  data(self, img: 
+0000ddf0: 4e72 7264 496d 6167 6520 7c20 6c69 7374  NrrdImage | list
+0000de00: 5b4e 7272 6449 6d61 6765 5d29 202d 3e20  [NrrdImage]) -> 
+0000de10: 7475 706c 655b 6e70 2e6e 6461 7272 6179  tuple[np.ndarray
+0000de20: 2c20 6469 6374 5d3a 0a20 2020 2020 2020  , dict]:.       
+0000de30: 2022 2222 0a20 2020 2020 2020 2045 7874   """.        Ext
+0000de40: 7261 6374 2064 6174 6120 6172 7261 7920  ract data array 
+0000de50: 616e 6420 6d65 7461 6461 7461 2066 726f  and metadata fro
+0000de60: 6d20 6c6f 6164 6564 2069 6d61 6765 2061  m loaded image a
+0000de70: 6e64 2072 6574 7572 6e20 7468 656d 2e0a  nd return them..
+0000de80: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
+0000de90: 6374 696f 6e20 6d75 7374 2072 6574 7572  ction must retur
+0000dea0: 6e20 7477 6f20 6f62 6a65 6374 732c 2074  n two objects, t
+0000deb0: 6865 2066 6972 7374 2069 7320 6120 6e75  he first is a nu
+0000dec0: 6d70 7920 6172 7261 7920 6f66 2069 6d61  mpy array of ima
+0000ded0: 6765 2064 6174 612c 0a20 2020 2020 2020  ge data,.       
+0000dee0: 2074 6865 2073 6563 6f6e 6420 6973 2061   the second is a
+0000def0: 2064 6963 7469 6f6e 6172 7920 6f66 206d   dictionary of m
+0000df00: 6574 6164 6174 612e 0a0a 2020 2020 2020  etadata...      
+0000df10: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000df20: 2020 2020 696d 673a 2061 2060 4e72 7264      img: a `Nrrd
+0000df30: 496d 6167 6560 206c 6f61 6465 6420 6672  Image` loaded fr
+0000df40: 6f6d 2061 6e20 696d 6167 6520 6669 6c65  om an image file
+0000df50: 206f 7220 6120 6c69 7374 206f 6620 696d   or a list of im
+0000df60: 6167 6520 6f62 6a65 6374 732e 0a0a 2020  age objects...  
+0000df70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000df80: 2020 696d 675f 6172 7261 793a 206c 6973    img_array: lis
+0000df90: 745b 6e70 2e6e 6461 7272 6179 5d20 3d20  t[np.ndarray] = 
+0000dfa0: 5b5d 0a20 2020 2020 2020 2063 6f6d 7061  [].        compa
+0000dfb0: 7469 626c 655f 6d65 7461 3a20 6469 6374  tible_meta: dict
+0000dfc0: 203d 207b 7d0a 0a20 2020 2020 2020 2066   = {}..        f
+0000dfd0: 6f72 2069 2069 6e20 656e 7375 7265 5f74  or i in ensure_t
+0000dfe0: 7570 6c65 2869 6d67 293a 0a20 2020 2020  uple(img):.     
+0000dff0: 2020 2020 2020 2064 6174 6120 3d20 692e         data = i.
+0000e000: 6172 7261 792e 6173 7479 7065 2873 656c  array.astype(sel
+0000e010: 662e 6474 7970 6529 0a20 2020 2020 2020  f.dtype).       
+0000e020: 2020 2020 2069 6d67 5f61 7272 6179 2e61       img_array.a
+0000e030: 7070 656e 6428 6461 7461 290a 2020 2020  ppend(data).    
+0000e040: 2020 2020 2020 2020 6865 6164 6572 203d          header =
+0000e050: 2064 6963 7428 692e 6865 6164 6572 290a   dict(i.header).
+0000e060: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000e070: 656c 662e 696e 6465 785f 6f72 6465 7220  elf.index_order 
+0000e080: 3d3d 2022 4322 3a0a 2020 2020 2020 2020  == "C":.        
+0000e090: 2020 2020 2020 2020 6865 6164 6572 203d          header =
+0000e0a0: 2073 656c 662e 5f63 6f6e 7665 7274 5f66   self._convert_f
+0000e0b0: 5f74 6f5f 635f 6f72 6465 7228 6865 6164  _to_c_order(head
+0000e0c0: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
+0000e0d0: 6865 6164 6572 5b4d 6574 614b 6579 732e  header[MetaKeys.
+0000e0e0: 4f52 4947 494e 414c 5f41 4646 494e 455d  ORIGINAL_AFFINE]
+0000e0f0: 203d 2073 656c 662e 5f67 6574 5f61 6666   = self._get_aff
+0000e100: 696e 6528 6929 0a0a 2020 2020 2020 2020  ine(i)..        
+0000e110: 2020 2020 6966 2073 656c 662e 6166 6669      if self.affi
+0000e120: 6e65 5f6c 7073 5f74 6f5f 7261 733a 0a20  ne_lps_to_ras:. 
+0000e130: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000e140: 6561 6465 7220 3d20 7365 6c66 2e5f 7377  eader = self._sw
+0000e150: 6974 6368 5f6c 7073 5f72 6173 2868 6561  itch_lps_ras(hea
+0000e160: 6465 7229 0a0a 2020 2020 2020 2020 2020  der)..          
+0000e170: 2020 6865 6164 6572 5b4d 6574 614b 6579    header[MetaKey
+0000e180: 732e 4146 4649 4e45 5d20 3d20 6865 6164  s.AFFINE] = head
+0000e190: 6572 5b4d 6574 614b 6579 732e 4f52 4947  er[MetaKeys.ORIG
+0000e1a0: 494e 414c 5f41 4646 494e 455d 2e63 6f70  INAL_AFFINE].cop
+0000e1b0: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+0000e1c0: 6865 6164 6572 5b4d 6574 614b 6579 732e  header[MetaKeys.
+0000e1d0: 5350 4154 4941 4c5f 5348 4150 455d 203d  SPATIAL_SHAPE] =
+0000e1e0: 2068 6561 6465 725b 2273 697a 6573 225d   header["sizes"]
+0000e1f0: 0a20 2020 2020 2020 2020 2020 205b 6865  .            [he
+0000e200: 6164 6572 2e70 6f70 286b 2920 666f 7220  ader.pop(k) for 
+0000e210: 6b20 696e 2028 2273 697a 6573 222c 2022  k in ("sizes", "
+0000e220: 7370 6163 6520 6f72 6967 696e 222c 2022  space origin", "
+0000e230: 7370 6163 6520 6469 7265 6374 696f 6e73  space directions
+0000e240: 2229 5d20 2023 2072 6d20 6475 706c 6963  ")]  # rm duplic
+0000e250: 6174 6564 2064 6174 6120 696e 2068 6561  ated data in hea
+0000e260: 6465 720a 0a20 2020 2020 2020 2020 2020  der..           
+0000e270: 2069 6620 7365 6c66 2e63 6861 6e6e 656c   if self.channel
+0000e280: 5f64 696d 2069 7320 4e6f 6e65 3a20 2023  _dim is None:  #
+0000e290: 2064 6566 6175 6c74 2074 6f20 226e 6f5f   default to "no_
+0000e2a0: 6368 616e 6e65 6c22 206f 7220 2d31 0a20  channel" or -1. 
+0000e2b0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000e2c0: 6561 6465 725b 4d65 7461 4b65 7973 2e4f  eader[MetaKeys.O
+0000e2d0: 5249 4749 4e41 4c5f 4348 414e 4e45 4c5f  RIGINAL_CHANNEL_
+0000e2e0: 4449 4d5d 203d 2028 0a20 2020 2020 2020  DIM] = (.       
+0000e2f0: 2020 2020 2020 2020 2020 2020 2066 6c6f               flo
+0000e300: 6174 2822 6e61 6e22 2920 6966 206c 656e  at("nan") if len
+0000e310: 2864 6174 612e 7368 6170 6529 203d 3d20  (data.shape) == 
+0000e320: 6c65 6e28 6865 6164 6572 5b4d 6574 614b  len(header[MetaK
+0000e330: 6579 732e 5350 4154 4941 4c5f 5348 4150  eys.SPATIAL_SHAP
+0000e340: 455d 2920 656c 7365 2030 0a20 2020 2020  E]) else 0.     
+0000e350: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000e360: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000e370: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000e380: 6561 6465 725b 4d65 7461 4b65 7973 2e4f  eader[MetaKeys.O
+0000e390: 5249 4749 4e41 4c5f 4348 414e 4e45 4c5f  RIGINAL_CHANNEL_
+0000e3a0: 4449 4d5d 203d 2073 656c 662e 6368 616e  DIM] = self.chan
+0000e3b0: 6e65 6c5f 6469 6d0a 2020 2020 2020 2020  nel_dim.        
+0000e3c0: 2020 2020 5f63 6f70 795f 636f 6d70 6174      _copy_compat
+0000e3d0: 6962 6c65 5f64 6963 7428 6865 6164 6572  ible_dict(header
+0000e3e0: 2c20 636f 6d70 6174 6962 6c65 5f6d 6574  , compatible_met
+0000e3f0: 6129 0a0a 2020 2020 2020 2020 7265 7475  a)..        retu
+0000e400: 726e 205f 7374 6163 6b5f 696d 6167 6573  rn _stack_images
+0000e410: 2869 6d67 5f61 7272 6179 2c20 636f 6d70  (img_array, comp
+0000e420: 6174 6962 6c65 5f6d 6574 6129 2c20 636f  atible_meta), co
+0000e430: 6d70 6174 6962 6c65 5f6d 6574 610a 0a20  mpatible_meta.. 
+0000e440: 2020 2064 6566 205f 6765 745f 6166 6669     def _get_affi
+0000e450: 6e65 2873 656c 662c 2069 6d67 3a20 4e72  ne(self, img: Nr
+0000e460: 7264 496d 6167 6529 202d 3e20 6e70 2e6e  rdImage) -> np.n
+0000e470: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
+0000e480: 2222 220a 2020 2020 2020 2020 4765 7420  """.        Get 
+0000e490: 7468 6520 6166 6669 6e65 206d 6174 7269  the affine matri
+0000e4a0: 7820 6f66 2074 6865 2069 6d61 6765 2c20  x of the image, 
+0000e4b0: 6974 2063 616e 2062 6520 7573 6564 2074  it can be used t
+0000e4c0: 6f20 636f 7272 6563 740a 2020 2020 2020  o correct.      
+0000e4d0: 2020 7370 6163 696e 672c 206f 7269 656e    spacing, orien
+0000e4e0: 7461 7469 6f6e 206f 7220 6578 6563 7574  tation or execut
+0000e4f0: 6520 7370 6174 6961 6c20 7472 616e 7366  e spatial transf
+0000e500: 6f72 6d73 2e0a 0a20 2020 2020 2020 2041  orms...        A
+0000e510: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000e520: 2069 6d67 3a20 4120 604e 7272 6449 6d61   img: A `NrrdIma
+0000e530: 6765 6020 6c6f 6164 6564 2066 726f 6d20  ge` loaded from 
+0000e540: 696d 6167 6520 6669 6c65 0a0a 2020 2020  image file..    
+0000e550: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000e560: 6469 7265 6374 696f 6e20 3d20 696d 672e  direction = img.
+0000e570: 6865 6164 6572 5b22 7370 6163 6520 6469  header["space di
+0000e580: 7265 6374 696f 6e73 225d 0a20 2020 2020  rections"].     
+0000e590: 2020 206f 7269 6769 6e20 3d20 696d 672e     origin = img.
+0000e5a0: 6865 6164 6572 5b22 7370 6163 6520 6f72  header["space or
+0000e5b0: 6967 696e 225d 0a0a 2020 2020 2020 2020  igin"]..        
+0000e5c0: 782c 2079 203d 2064 6972 6563 7469 6f6e  x, y = direction
+0000e5d0: 2e73 6861 7065 0a20 2020 2020 2020 2061  .shape.        a
+0000e5e0: 6666 696e 655f 6469 616d 203d 206d 696e  ffine_diam = min
+0000e5f0: 2878 2c20 7929 202b 2031 0a20 2020 2020  (x, y) + 1.     
+0000e600: 2020 2061 6666 696e 653a 206e 702e 6e64     affine: np.nd
+0000e610: 6172 7261 7920 3d20 6e70 2e65 7965 2861  array = np.eye(a
+0000e620: 6666 696e 655f 6469 616d 290a 2020 2020  ffine_diam).    
+0000e630: 2020 2020 6166 6669 6e65 5b3a 782c 203a      affine[:x, :
+0000e640: 795d 203d 2064 6972 6563 7469 6f6e 0a20  y] = direction. 
+0000e650: 2020 2020 2020 2061 6666 696e 655b 3a20         affine[: 
+0000e660: 2861 6666 696e 655f 6469 616d 202d 2031  (affine_diam - 1
+0000e670: 292c 202d 315d 203d 206f 7269 6769 6e20  ), -1] = origin 
+0000e680: 2023 206c 656e 206f 7269 6769 6e20 6973   # len origin is
+0000e690: 2061 6c77 6179 7320 6166 6669 6e65 5f64   always affine_d
+0000e6a0: 6961 6d20 2d20 310a 2020 2020 2020 2020  iam - 1.        
+0000e6b0: 7265 7475 726e 2061 6666 696e 650a 0a20  return affine.. 
+0000e6c0: 2020 2064 6566 205f 7377 6974 6368 5f6c     def _switch_l
+0000e6d0: 7073 5f72 6173 2873 656c 662c 2068 6561  ps_ras(self, hea
+0000e6e0: 6465 723a 2064 6963 7429 202d 3e20 6469  der: dict) -> di
+0000e6f0: 6374 3a0a 2020 2020 2020 2020 2222 220a  ct:.        """.
+0000e700: 2020 2020 2020 2020 466f 7220 636f 6d70          For comp
+0000e710: 6174 6962 696c 6974 7920 7769 7468 206e  atibility with n
+0000e720: 6962 6162 656c 2c20 7377 6974 6368 2066  ibabel, switch f
+0000e730: 726f 6d20 4c50 5320 746f 2052 4153 2e20  rom LPS to RAS. 
+0000e740: 4164 6170 7420 6166 6669 6e65 206d 6174  Adapt affine mat
+0000e750: 7269 7820 616e 640a 2020 2020 2020 2020  rix and.        
+0000e760: 6073 7061 6365 6020 6172 6775 6d65 6e74  `space` argument
+0000e770: 2069 6e20 6865 6164 6572 2061 6363 6f72   in header accor
+0000e780: 6469 6e67 6c79 2e20 4966 206e 6f20 696e  dingly. If no in
+0000e790: 666f 726d 6174 696f 6e20 6f66 2073 7061  formation of spa
+0000e7a0: 6365 2069 7320 6769 7665 6e20 696e 2074  ce is given in t
+0000e7b0: 6865 2068 6561 6465 722c 0a20 2020 2020  he header,.     
+0000e7c0: 2020 204c 5053 2069 7320 6173 7375 6d65     LPS is assume
+0000e7d0: 6420 616e 6420 7468 7573 2063 6f6e 7665  d and thus conve
+0000e7e0: 7274 6564 2074 6f20 5241 532e 2049 6620  rted to RAS. If 
+0000e7f0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+0000e800: 7420 7370 6163 6520 6973 2067 6976 656e  t space is given
+0000e810: 2c0a 2020 2020 2020 2020 6275 7420 6973  ,.        but is
+0000e820: 206e 6f74 204c 5053 2c20 7468 6520 756e   not LPS, the un
+0000e830: 6368 616e 6765 6420 6865 6164 6572 2069  changed header i
+0000e840: 7320 7265 7475 726e 6564 2e0a 0a20 2020  s returned...   
+0000e850: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000e860: 2020 2020 2020 2068 6561 6465 723a 2054         header: T
+0000e870: 6865 2069 6d61 6765 206d 6574 6164 6174  he image metadat
+0000e880: 6120 6173 2064 6963 740a 0a20 2020 2020  a as dict..     
+0000e890: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000e8a0: 6620 2273 7061 6365 2220 6e6f 7420 696e  f "space" not in
+0000e8b0: 2068 6561 6465 7220 6f72 2068 6561 6465   header or heade
+0000e8c0: 725b 2273 7061 6365 225d 203d 3d20 226c  r["space"] == "l
+0000e8d0: 6566 742d 706f 7374 6572 696f 722d 7375  eft-posterior-su
+0000e8e0: 7065 7269 6f72 223a 0a20 2020 2020 2020  perior":.       
+0000e8f0: 2020 2020 2068 6561 6465 725b 4d65 7461       header[Meta
+0000e900: 4b65 7973 2e4f 5249 4749 4e41 4c5f 4146  Keys.ORIGINAL_AF
+0000e910: 4649 4e45 5d20 3d20 6f72 6965 6e74 6174  FINE] = orientat
+0000e920: 696f 6e5f 7261 735f 6c70 7328 6865 6164  ion_ras_lps(head
+0000e930: 6572 5b4d 6574 614b 6579 732e 4f52 4947  er[MetaKeys.ORIG
+0000e940: 494e 414c 5f41 4646 494e 455d 290a 2020  INAL_AFFINE]).  
+0000e950: 2020 2020 2020 2020 2020 6865 6164 6572            header
+0000e960: 5b4d 6574 614b 6579 732e 5350 4143 455d  [MetaKeys.SPACE]
+0000e970: 203d 2053 7061 6365 4b65 7973 2e52 4153   = SpaceKeys.RAS
+0000e980: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000e990: 6865 6164 6572 0a0a 2020 2020 6465 6620  header..    def 
+0000e9a0: 5f63 6f6e 7665 7274 5f66 5f74 6f5f 635f  _convert_f_to_c_
+0000e9b0: 6f72 6465 7228 7365 6c66 2c20 6865 6164  order(self, head
+0000e9c0: 6572 3a20 6469 6374 2920 2d3e 2064 6963  er: dict) -> dic
+0000e9d0: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+0000e9e0: 2020 2020 2020 2041 6c6c 2068 6561 6465         All heade
+0000e9f0: 7220 6669 656c 6473 206f 6620 6120 4e52  r fields of a NR
+0000ea00: 5244 2061 7265 2073 7065 6369 6669 6564  RD are specified
+0000ea10: 2069 6e20 6046 6020 2846 6f72 7472 616e   in `F` (Fortran
+0000ea20: 2920 6f72 6465 722c 2065 7665 6e20 6966  ) order, even if
+0000ea30: 2074 6865 2069 6d61 6765 2077 6173 2072   the image was r
+0000ea40: 6561 6420 6173 2043 2d6f 7264 6572 6564  ead as C-ordered
+0000ea50: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
+0000ea60: 3144 2061 7272 6179 7320 6f66 2068 6561  1D arrays of hea
+0000ea70: 6465 725b 2773 7061 6365 206f 7269 6769  der['space origi
+0000ea80: 6e27 5d20 616e 6420 6865 6164 6572 5b27  n'] and header['
+0000ea90: 7369 7a65 7327 5d20 6265 636f 6d65 2069  sizes'] become i
+0000eaa0: 6e76 6572 7465 642c 2065 2e67 2c20 5b31  nverted, e.g, [1
+0000eab0: 2c32 2c33 5d20 2d3e 205b 332c 322c 315d  ,2,3] -> [3,2,1]
+0000eac0: 0a20 2020 2020 2020 2054 6865 2032 4420  .        The 2D 
+0000ead0: 4172 7261 7920 666f 7220 6865 6164 6572  Array for header
+0000eae0: 5b27 7370 6163 6520 6469 7265 6374 696f  ['space directio
+0000eaf0: 6e73 275d 2069 7320 7472 616e 7370 6f73  ns'] is transpos
+0000eb00: 6564 3a20 5b5b 312c 302c 305d 2c5b 302c  ed: [[1,0,0],[0,
+0000eb10: 322c 305d 2c5b 302c 302c 335d 5d20 2d3e  2,0],[0,0,3]] ->
+0000eb20: 205b 5b33 2c30 2c30 5d2c 5b30 2c32 2c30   [[3,0,0],[0,2,0
+0000eb30: 5d2c 5b30 2c30 2c31 5d5d 0a20 2020 2020  ],[0,0,1]].     
+0000eb40: 2020 2046 6f72 206d 6f72 6520 6465 7461     For more deta
+0000eb50: 696c 7320 7265 6665 7220 746f 3a20 6874  ils refer to: ht
+0000eb60: 7470 733a 2f2f 7079 6e72 7264 2e72 6561  tps://pynrrd.rea
+0000eb70: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+0000eb80: 6174 6573 742f 7573 6572 2d67 7569 6465  atest/user-guide
+0000eb90: 2e68 746d 6c23 696e 6465 782d 6f72 6465  .html#index-orde
+0000eba0: 7269 6e67 0a0a 2020 2020 2020 2020 4172  ring..        Ar
+0000ebb0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000ebc0: 6865 6164 6572 3a20 5468 6520 696d 6167  header: The imag
+0000ebd0: 6520 6d65 7461 6461 7461 2061 7320 6469  e metadata as di
+0000ebe0: 6374 0a0a 2020 2020 2020 2020 2222 220a  ct..        """.
+0000ebf0: 0a20 2020 2020 2020 2068 6561 6465 725b  .        header[
+0000ec00: 2273 7061 6365 2064 6972 6563 7469 6f6e  "space direction
+0000ec10: 7322 5d20 3d20 6e70 2e72 6f74 3930 286e  s"] = np.rot90(n
+0000ec20: 702e 666c 6970 2868 6561 6465 725b 2273  p.flip(header["s
+0000ec30: 7061 6365 2064 6972 6563 7469 6f6e 7322  pace directions"
+0000ec40: 5d2c 2030 2929 0a20 2020 2020 2020 2068  ], 0)).        h
+0000ec50: 6561 6465 725b 2273 7061 6365 206f 7269  eader["space ori
+0000ec60: 6769 6e22 5d20 3d20 6865 6164 6572 5b22  gin"] = header["
+0000ec70: 7370 6163 6520 6f72 6967 696e 225d 5b3a  space origin"][:
+0000ec80: 3a2d 315d 0a20 2020 2020 2020 2068 6561  :-1].        hea
+0000ec90: 6465 725b 2273 697a 6573 225d 203d 2068  der["sizes"] = h
+0000eca0: 6561 6465 725b 2273 697a 6573 225d 5b3a  eader["sizes"][:
+0000ecb0: 3a2d 315d 0a20 2020 2020 2020 2072 6574  :-1].        ret
+0000ecc0: 7572 6e20 6865 6164 6572 0a              urn header.
```

## monai/data/meta_tensor.py

```diff
@@ -506,17 +506,24 @@
         See:
             - https://pytorch.org/docs/stable/generated/torch.Tensor.new_empty.html#torch-tensor-new-empty
         """
         return type(self)(
             self.as_tensor().new_empty(size=size, dtype=dtype, device=device, requires_grad=requires_grad)
         )
 
-    def clone(self):
-        """returns a copy of the MetaTensor instance."""
-        new_inst = MetaTensor(self.as_tensor().clone())
+    def clone(self, **kwargs):
+        """
+        Returns a copy of the MetaTensor instance.
+
+        Args:
+            kwargs: additional keyword arguments to `torch.clone`.
+
+        See also: https://pytorch.org/docs/stable/generated/torch.clone.html
+        """
+        new_inst = MetaTensor(self.as_tensor().clone(**kwargs))
         new_inst.__dict__ = deepcopy(self.__dict__)
         return new_inst
 
     @staticmethod
     def ensure_torch_and_prune_meta(
         im: NdarrayTensor, meta: dict | None, simple_keys: bool = False, pattern: str | None = None, sep: str = "."
     ):
```

## monai/data/utils.py

```diff
@@ -13,15 +13,14 @@
 
 import hashlib
 import json
 import logging
 import math
 import os
 import pickle
-import warnings
 from collections import abc, defaultdict
 from collections.abc import Generator, Iterable, Mapping, Sequence, Sized
 from copy import deepcopy
 from functools import reduce
 from itertools import product, starmap, zip_longest
 from pathlib import PurePath
 from typing import Any
@@ -160,23 +159,24 @@
     for position in iter_patch_position(
         image_size=image_size, patch_size=patch_size_, start_pos=start_pos, overlap=overlap, padded=padded
     ):
         yield tuple(slice(s, s + p) for s, p in zip(position, patch_size_))
 
 
 def dense_patch_slices(
-    image_size: Sequence[int], patch_size: Sequence[int], scan_interval: Sequence[int]
+    image_size: Sequence[int], patch_size: Sequence[int], scan_interval: Sequence[int], return_slice: bool = True
 ) -> list[tuple[slice, ...]]:
     """
     Enumerate all slices defining ND patches of size `patch_size` from an `image_size` input image.
 
     Args:
         image_size: dimensions of image to iterate over
         patch_size: size of patches to generate slices
         scan_interval: dense patch sampling interval
+        return_slice: whether to return a list of slices (or tuples of indices), defaults to True
 
     Returns:
         a list of slice objects defining each patch
 
     """
     num_spatial_dims = len(image_size)
     patch_size = get_valid_patch_size(image_size, patch_size)
@@ -196,15 +196,17 @@
         dim_starts = []
         for idx in range(scan_num[dim]):
             start_idx = idx * scan_interval[dim]
             start_idx -= max(start_idx + patch_size[dim] - image_size[dim], 0)
             dim_starts.append(start_idx)
         starts.append(dim_starts)
     out = np.asarray([x.flatten() for x in np.meshgrid(*starts, indexing="ij")]).T
-    return [tuple(slice(s, s + patch_size[d]) for d, s in enumerate(x)) for x in out]
+    if return_slice:
+        return [tuple(slice(s, s + patch_size[d]) for d, s in enumerate(x)) for x in out]
+    return [tuple((s, s + patch_size[d]) for d, s in enumerate(x)) for x in out]  # type: ignore
 
 
 def iter_patch_position(
     image_size: Sequence[int],
     patch_size: Sequence[int] | int | np.ndarray,
     start_pos: Sequence[int] = (),
     overlap: Sequence[float] | float = 0.0,
@@ -782,15 +784,14 @@
         if not qform_mismatch:
             return img_nii
         if not sform_mismatch:
             img_nii.set_qform(img_nii.get_sform())
             return img_nii
 
     norm = affine_to_spacing(img_nii.affine, r=d)
-    warnings.warn(f"Modifying image pixdim from {pixdim} to {norm}")
 
     img_nii.header.set_zooms(norm)
     return img_nii
 
 
 def zoom_affine(affine: np.ndarray, scale: np.ndarray | Sequence[float], diagonal: bool = True):
     """
@@ -1054,28 +1055,30 @@
 
 
 def compute_importance_map(
     patch_size: tuple[int, ...],
     mode: BlendMode | str = BlendMode.CONSTANT,
     sigma_scale: Sequence[float] | float = 0.125,
     device: torch.device | int | str = "cpu",
+    dtype: torch.dtype | str | None = torch.float32,
 ) -> torch.Tensor:
     """Get importance map for different weight modes.
 
     Args:
         patch_size: Size of the required importance map. This should be either H, W [,D].
         mode: {``"constant"``, ``"gaussian"``}
             How to blend output of overlapping windows. Defaults to ``"constant"``.
 
             - ``"constant``": gives equal weight to all predictions.
             - ``"gaussian``": gives less weight to predictions on edges of windows.
 
         sigma_scale: Sigma_scale to calculate sigma for each dimension
             (sigma = sigma_scale * dim_size). Used for gaussian mode only.
         device: Device to put importance map on.
+        dtype: Data type of the output importance map.
 
     Raises:
         ValueError: When ``mode`` is not one of ["constant", "gaussian"].
 
     Returns:
         Tensor of size patch_size.
 
@@ -1094,14 +1097,17 @@
             )
             x = torch.exp(x**2 / (-2 * sigmas[i] ** 2))  # 1D gaussian
             importance_map = importance_map.unsqueeze(-1) * x[(None,) * i] if i > 0 else x
     else:
         raise ValueError(
             f"Unsupported mode: {mode}, available options are [{BlendMode.CONSTANT}, {BlendMode.CONSTANT}]."
         )
+    # handle non-positive weights
+    min_non_zero = max(torch.min(importance_map).item(), 1e-3)
+    importance_map = torch.clamp_(importance_map.to(torch.float), min=min_non_zero).to(dtype)
     return importance_map
 
 
 def is_supported_format(filename: Sequence[PathLike] | PathLike, suffixes: Sequence[str]) -> bool:
     """
     Verify whether the specified file or files format match supported suffixes.
     If supported suffixes is None, skip the verification and return True.
```

## monai/data/wsi_reader.py

```diff
@@ -7,14 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import warnings
 from abc import abstractmethod
 from collections.abc import Sequence
 from os.path import abspath
 from typing import Any
 
 import numpy as np
 import torch
@@ -23,37 +24,50 @@
 from monai.data.image_reader import ImageReader, _stack_images
 from monai.data.utils import is_supported_format
 from monai.utils import (
     WSIPatchKeys,
     dtype_numpy_to_torch,
     dtype_torch_to_numpy,
     ensure_tuple,
+    ensure_tuple_rep,
     optional_import,
     require_pkg,
 )
+from monai.utils.misc import ConvertUnits
 
 OpenSlide, _ = optional_import("openslide", name="OpenSlide")
 TiffFile, _ = optional_import("tifffile", name="TiffFile")
 
 __all__ = ["BaseWSIReader", "WSIReader", "CuCIMWSIReader", "OpenSlideWSIReader", "TiffFileWSIReader"]
 
 
 class BaseWSIReader(ImageReader):
     """
     An abstract class that defines APIs to load patches from whole slide image files.
 
     Args:
-        level: the whole slide image level at which the image is extracted.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel.
         dtype: the data type of output image.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, e.g., "RGB" or "RGBA".
         kwargs: additional args for the reader
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     Typical usage of a concrete implementation of this class is:
 
     .. code-block:: python
 
         image_reader = MyWSIReader()
         wsi = image_reader.read(filepath, **kwargs)
         img_data, meta_data = image_reader.get_data(wsi)
@@ -73,28 +87,40 @@
     """
 
     supported_suffixes: list[str] = []
     backend = ""
 
     def __init__(
         self,
-        level: int,
-        channel_dim: int,
-        dtype: DtypeLike | torch.dtype,
-        device: torch.device | str | None,
-        mode: str,
+        level: int | None = None,
+        mpp: float | tuple[float, float] | None = None,
+        mpp_rtol: float = 0.05,
+        mpp_atol: float = 0.0,
+        power: int | None = None,
+        power_rtol: float = 0.05,
+        power_atol: float = 0.0,
+        channel_dim: int = 0,
+        dtype: DtypeLike | torch.dtype = np.uint8,
+        device: torch.device | str | None = None,
+        mode: str = "RGB",
         **kwargs,
     ):
         super().__init__()
         self.level = level
         self.channel_dim = channel_dim
         self.set_dtype(dtype)
         self.set_device(device)
         self.mode = mode
         self.kwargs = kwargs
+        self.mpp: tuple[float, float] | None = ensure_tuple_rep(mpp, 2) if mpp is not None else None  # type: ignore
+        self.power = power
+        self.mpp_rtol = mpp_rtol
+        self.mpp_atol = mpp_atol
+        self.power_rtol = power_rtol
+        self.power_atol = power_atol
         self.metadata: dict[Any, Any] = {}
 
     def set_dtype(self, dtype):
         self.dtype: torch.dtype | np.dtype
         if isinstance(dtype, torch.dtype):
             self.dtype = dtype
         else:
@@ -103,62 +129,143 @@
     def set_device(self, device):
         if device is None or isinstance(device, (torch.device, str)):
             self.device = device
         else:
             raise ValueError(f"`device` must be `torch.device`, `str` or `None` but {type(device)} is given.")
 
     @abstractmethod
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
+    def _find_closest_level(
+        self, name: str, value: tuple, value_at_levels: Sequence[tuple], atol: float, rtol: float
+    ) -> int:
+        """Find the level corresponding to the value of the quantity in the list of values at each level.
+        Args:
+            name: the name of the requested quantity
+            value: the value of requested quantity
+            value_at_levels: list of value of the quantity at each level
+            atol: the tolerance for the value
+            rtol: relative tolerance for the value
+        """
+        if value in value_at_levels:
+            return value_at_levels.index(value)
+
+        closest_value = min(value_at_levels, key=lambda a_value: sum([abs(x - y) for x, y in zip(a_value, value)]))  # type: ignore
+        for i in range(len(value)):
+            if abs(closest_value[i] - value[i]) > atol + rtol * abs(value[i]):
+                raise ValueError(
+                    f"The requested {name} < {value} > does not exist in this whole slide image "
+                    f"(with {name}_rtol={rtol} and {name}_atol={atol}). "
+                    f"Here is the list of available {name}: {value_at_levels}. "
+                    f"The closest matching available {name} is {closest_value}."
+                    f"Please consider changing the tolerances or use another {name}."
+                )
+        return value_at_levels.index(closest_value)
+
+    def get_valid_level(
+        self, wsi, level: int | None, mpp: float | tuple[float, float] | None, power: int | None
+    ) -> int:
+        """
+        Returns the level associated to the resolution parameters in the whole slide image.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number.
+            mpp: the micron-per-pixel resolution.
+            power: the objective power.
+
+        """
+
+        # Try instance parameters if no resolution is provided
+        if mpp is None and power is None and level is None:
+            mpp = self.mpp
+            power = self.power
+            level = self.level
+
+        # Ensure that at most one resolution parameter is provided.
+        resolution = [val[0] for val in [("level", level), ("mpp", mpp), ("power", power)] if val[1] is not None]
+        if len(resolution) > 1:
+            raise ValueError(f"Only one of `level`, `mpp`, or `power` should be provided. {resolution} are provided.")
+
+        n_levels = self.get_level_count(wsi)
+
+        if mpp is not None:
+            mpp_ = ensure_tuple_rep(mpp, 2)
+            available_mpps = [self.get_mpp(wsi, level) for level in range(n_levels)]
+            level = self._find_closest_level("mpp", mpp_, available_mpps, self.mpp_atol, self.mpp_rtol)
+        elif power is not None:
+            power_ = ensure_tuple(power)
+            available_powers = [(self.get_power(wsi, level),) for level in range(n_levels)]
+            level = self._find_closest_level("power", power_, available_powers, self.power_atol, self.power_rtol)
+        else:
+            if level is None:
+                # Set the default value if no resolution parameter is provided.
+                level = 0
+            if level >= n_levels:
+                raise ValueError(f"The maximum level of this image is {n_levels-1} while level={level} is requested)!")
+
+        return level
+
     @abstractmethod
     def get_level_count(self, wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
     def get_file_path(self, wsi) -> str:
         """Return the file path for the WSI object"""
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
+
+        """
+        raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
+
+    @abstractmethod
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
     def _get_patch(
         self, wsi, location: tuple[int, int], size: tuple[int, int], level: int, dtype: DtypeLike, mode: str
@@ -167,34 +274,34 @@
         Extracts and returns a patch image form the whole slide image.
 
         Args:
             wsi: a whole slide image object loaded from a file or a lis of such objects
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     def _get_metadata(
         self, wsi, patch: NdarrayOrTensor, location: tuple[int, int], size: tuple[int, int], level: int
     ) -> dict:
         """
         Returns metadata of the extracted patch from the whole slide image.
 
         Args:
-            wsi: the whole slide image object, from which the patch is loaded
-            patch: extracted patch from whole slide image
+            wsi: the whole slide image object, from which the patch is loaded.
+            patch: extracted patch from whole slide image.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
+            level: the level number.
 
         """
         if self.channel_dim >= len(patch.shape) or self.channel_dim < -len(patch.shape):
             raise ValueError(
                 f"The desired channel_dim ({self.channel_dim}) is out of bound for image shape: {patch.shape}"
             )
         channel_dim: int = self.channel_dim + (len(patch.shape) if self.channel_dim < 0 else 0)
@@ -212,45 +319,52 @@
 
     def get_data(
         self,
         wsi,
         location: tuple[int, int] = (0, 0),
         size: tuple[int, int] | None = None,
         level: int | None = None,
+        mpp: float | tuple[float, float] | None = None,
+        power: int | None = None,
         mode: str | None = None,
     ) -> tuple[np.ndarray, dict]:
         """
-        Verifies inputs, extracts patches from WSI image and generates metadata, and return them.
+        Verifies inputs, extracts patches from WSI image and generates metadata.
 
         Args:
-            wsi: a whole slide image object loaded from a file or a list of such objects
+            wsi: a whole slide image object loaded from a file or a list of such objects.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If not provided or None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            mode: the output image color mode, "RGB" or "RGBA". If not provided the default of "RGB" is used.
+            level: the whole slide image level at which the patches are extracted.
+            mpp: the resolution in micron per pixel at which the patches are extracted.
+            power: the objective power at which the patches are extracted.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         Returns:
             a tuples, where the first element is an image patch [CxHxW] or stack of patches,
-                and second element is a dictionary of metadata
+                and second element is a dictionary of metadata.
+
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If none of them are provided, it uses the defaults that are set during class instantiation.
+            If none of them are set here or during class instantiation, `level=0` will be used.
         """
         if mode is None:
             mode = self.mode
         patch_list: list = []
         metadata_list: list = []
+
         # CuImage object is iterable, so ensure_tuple won't work on single object
-        if not isinstance(wsi, list):
-            wsi = [wsi]
+        if not isinstance(wsi, (list, tuple)):
+            wsi = (wsi,)
         for each_wsi in ensure_tuple(wsi):
-            # Verify magnification level
-            if level is None:
-                level = self.level
-            max_level = self.get_level_count(each_wsi) - 1
-            if level > max_level:
-                raise ValueError(f"The maximum level of this image is {max_level} while level={level} is requested)!")
+            # get the valid level based on resolution info
+            level = self.get_valid_level(each_wsi, level, mpp, power)
 
             # Verify location
             if location is None:
                 location = (0, 0)
             wsi_size = self.get_size(each_wsi, 0)
             if location[0] > wsi_size[0] or location[1] > wsi_size[1]:
                 raise ValueError(f"Location is outside of the image: location={location}, image size={wsi_size}")
@@ -332,264 +446,339 @@
 
 class WSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using different backend libraries
 
     Args:
         backend: the name of backend whole slide image reader library, the default is cuCIM.
-        level: the level at which patches are extracted.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
-        mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
+        mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         num_workers: number of workers for multi-thread image loading (cucim backend only).
         kwargs: additional arguments to be passed to the backend library
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_backends = ["cucim", "openslide", "tifffile"]
 
     def __init__(
         self,
         backend="cucim",
-        level: int = 0,
+        level: int | None = None,
+        mpp: float | tuple[float, float] | None = None,
+        mpp_rtol: float = 0.05,
+        mpp_atol: float = 0.0,
+        power: int | None = None,
+        power_rtol: float = 0.05,
+        power_atol: float = 0.0,
         channel_dim: int = 0,
         dtype: DtypeLike | torch.dtype = np.uint8,
         device: torch.device | str | None = None,
         mode: str = "RGB",
         **kwargs,
     ):
         self.backend = backend.lower()
         self.reader: CuCIMWSIReader | OpenSlideWSIReader | TiffFileWSIReader
         if self.backend == "cucim":
             self.reader = CuCIMWSIReader(
-                level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs
+                level=level,
+                mpp=mpp,
+                mpp_rtol=mpp_rtol,
+                mpp_atol=mpp_atol,
+                power=power,
+                power_rtol=power_rtol,
+                power_atol=power_atol,
+                channel_dim=channel_dim,
+                dtype=dtype,
+                device=device,
+                mode=mode,
+                **kwargs,
             )
         elif self.backend == "openslide":
             self.reader = OpenSlideWSIReader(
-                level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs
+                level=level,
+                mpp=mpp,
+                mpp_rtol=mpp_rtol,
+                mpp_atol=mpp_atol,
+                power=power,
+                power_rtol=power_rtol,
+                power_atol=power_atol,
+                channel_dim=channel_dim,
+                dtype=dtype,
+                device=device,
+                mode=mode,
+                **kwargs,
             )
         elif self.backend == "tifffile":
             self.reader = TiffFileWSIReader(
-                level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs
+                level=level,
+                mpp=mpp,
+                mpp_rtol=mpp_rtol,
+                mpp_atol=mpp_atol,
+                power=power,
+                power_rtol=power_rtol,
+                power_atol=power_atol,
+                channel_dim=channel_dim,
+                dtype=dtype,
+                device=device,
+                mode=mode,
+                **kwargs,
             )
         else:
             raise ValueError(
                 f"The supported backends are cucim, openslide, and tifffile but '{self.backend}' was given."
             )
         self.supported_suffixes = self.reader.supported_suffixes
         self.level = self.reader.level
+        self.mpp_rtol = self.reader.mpp_rtol
+        self.mpp_atol = self.reader.mpp_atol
+        self.power = self.reader.power
+        self.power_rtol = self.reader.power_rtol
+        self.power_atol = self.reader.power_atol
         self.channel_dim = self.reader.channel_dim
         self.dtype = self.reader.dtype
         self.device = self.reader.device
         self.mode = self.reader.mode
         self.kwargs = self.reader.kwargs
         self.metadata = self.reader.metadata
+        self.mpp = self.reader.mpp
 
     def get_level_count(self, wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return self.reader.get_level_count(wsi)
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return self.reader.get_size(wsi, level)
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return self.reader.get_downsample_ratio(wsi, level)
 
     def get_file_path(self, wsi) -> str:
         """Return the file path for the WSI object"""
         return self.reader.get_file_path(wsi)
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return self.reader.get_mpp(wsi, level)
 
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the micro-per-pixel resolution of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
+
+        """
+        return self.reader.get_power(wsi, level)
+
     def _get_patch(
         self, wsi, location: tuple[int, int], size: tuple[int, int], level: int, dtype: DtypeLike, mode: str
     ) -> np.ndarray:
         """
         Extracts and returns a patch image form the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file or a lis of such objects
+            wsi: a whole slide image object loaded from a file or a lis of such objects.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
+            level: the level number.
             dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         return self.reader._get_patch(wsi=wsi, location=location, size=size, level=level, dtype=dtype, mode=mode)
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args for the reader module (overrides `self.kwargs` for existing keys).
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         return self.reader.read(data=data, **kwargs)
 
 
 @require_pkg(pkg_name="cucim")
 class CuCIMWSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using cuCIM library.
 
     Args:
-        level: the whole slide image level at which the image is extracted. (default=0)
-            This is overridden if the level argument is provided in `get_data`.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
-        num_workers: number of workers for multi-thread image loading
+        num_workers: number of workers for multi-thread image loading.
         kwargs: additional args for `cucim.CuImage` module:
             https://github.com/rapidsai/cucim/blob/main/cpp/include/cucim/cuimage.h
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_suffixes = ["tif", "tiff", "svs"]
     backend = "cucim"
 
-    def __init__(
-        self,
-        level: int = 0,
-        channel_dim: int = 0,
-        dtype: DtypeLike | torch.dtype = np.uint8,
-        device: torch.device | str | None = None,
-        mode: str = "RGB",
-        num_workers: int = 0,
-        **kwargs,
-    ):
-        super().__init__(level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs)
+    def __init__(self, num_workers: int = 0, **kwargs):
+        super().__init__(**kwargs)
         self.num_workers = num_workers
 
     @staticmethod
     def get_level_count(wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return wsi.resolutions["level_count"]  # type: ignore
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return (wsi.resolutions["level_dimensions"][level][1], wsi.resolutions["level_dimensions"][level][0])
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
-        return wsi.resolutions["level_downsamples"][level]  # type: ignore
+        return float(wsi.resolutions["level_downsamples"][level])
 
     @staticmethod
     def get_file_path(wsi) -> str:
         """Return the file path for the WSI object"""
         return str(abspath(wsi.path))
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
+        downsample_ratio = self.get_downsample_ratio(wsi, level)
+
+        if "aperio" in wsi.metadata:
+            mpp_ = wsi.metadata["aperio"].get("MPP")
+            if mpp_:
+                return (downsample_ratio * float(mpp_),) * 2
+        if "cucim" in wsi.metadata:
+            mpp_ = wsi.metadata["cucim"].get("spacing")
+            if mpp_ and isinstance(mpp_, Sequence) and len(mpp_) >= 2:
+                if mpp_[0] and mpp_[1]:
+                    return (downsample_ratio * mpp_[1], downsample_ratio * mpp_[0])
+
+        raise ValueError("`mpp` cannot be obtained for this file. Please use `level` instead.")
+
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
 
-        factor = float(wsi.resolutions["level_downsamples"][level])
-        return (wsi.metadata["cucim"]["spacing"][1] * factor, wsi.metadata["cucim"]["spacing"][0] * factor)
+        """
+        if "aperio" in wsi.metadata:
+            objective_power = wsi.metadata["aperio"].get("AppMag")
+            if objective_power:
+                downsample_ratio = self.get_downsample_ratio(wsi, level)
+                return float(objective_power) / downsample_ratio
+
+        raise ValueError(
+            "Currently, cuCIM backend can obtain the objective power only for Aperio images. "
+            "Please use `level` (or `mpp`) instead, or try OpenSlide backend."
+        )
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args that overrides `self.kwargs` for existing keys.
                 For more details look at https://github.com/rapidsai/cucim/blob/main/cpp/include/cucim/cuimage.h
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         cuimage_cls, _ = optional_import("cucim", name="CuImage")
         wsi_list: list = []
 
         filenames: Sequence[PathLike] = ensure_tuple(data)
         kwargs_ = self.kwargs.copy()
@@ -603,21 +792,21 @@
     def _get_patch(
         self, wsi, location: tuple[int, int], size: tuple[int, int], level: int, dtype: DtypeLike, mode: str
     ) -> np.ndarray:
         """
         Extracts and returns a patch image form the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file or a lis of such objects
+            wsi: a whole slide image object loaded from a file or a lis of such objects.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         # Extract a patch or the entire image
         # (reverse the order of location and size to become WxH for cuCIM)
         patch: np.ndarray = wsi.read_region(
             location=location[::-1], size=size[::-1], level=level, num_workers=self.num_workers
         )
@@ -642,122 +831,145 @@
 
 @require_pkg(pkg_name="openslide")
 class OpenSlideWSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using OpenSlide library.
 
     Args:
-        level: the whole slide image level at which the image is extracted. (default=0)
-            This is overridden if the level argument is provided in `get_data`.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         kwargs: additional args for `openslide.OpenSlide` module.
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_suffixes = ["tif", "tiff", "svs"]
     backend = "openslide"
 
-    def __init__(
-        self,
-        level: int = 0,
-        channel_dim: int = 0,
-        dtype: DtypeLike | torch.dtype = np.uint8,
-        device: torch.device | str | None = None,
-        mode: str = "RGB",
-        **kwargs,
-    ):
-        super().__init__(level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
     @staticmethod
     def get_level_count(wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return wsi.level_count  # type: ignore
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return (wsi.level_dimensions[level][1], wsi.level_dimensions[level][0])
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return wsi.level_downsamples[level]  # type: ignore
 
     @staticmethod
     def get_file_path(wsi) -> str:
         """Return the file path for the WSI object"""
         return str(abspath(wsi._filename))
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
-        unit = wsi.properties["tiff.ResolutionUnit"]
-        if unit == "centimeter":
-            factor = 10000.0
-        elif unit == "millimeter":
-            factor = 1000.0
-        elif unit == "micrometer":
-            factor = 1.0
-        elif unit == "inch":
-            factor = 25400.0
-        else:
-            raise ValueError(f"The resolution unit is not a valid tiff resolution: {unit}")
+        downsample_ratio = self.get_downsample_ratio(wsi, level)
+        if (
+            "openslide.mpp-x" in wsi.properties
+            and "openslide.mpp-y" in wsi.properties
+            and wsi.properties["openslide.mpp-y"]
+            and wsi.properties["openslide.mpp-x"]
+        ):
+            return (
+                downsample_ratio * float(wsi.properties["openslide.mpp-y"]),
+                downsample_ratio * float(wsi.properties["openslide.mpp-x"]),
+            )
+
+        if (
+            "tiff.XResolution" in wsi.properties
+            and "tiff.YResolution" in wsi.properties
+            and wsi.properties["tiff.YResolution"]
+            and wsi.properties["tiff.XResolution"]
+        ):
+            unit = wsi.properties.get("tiff.ResolutionUnit")
+            if unit is None:
+                warnings.warn("The resolution unit is missing, `micrometer` will be used as default.")
+                unit = "micrometer"
+
+            convert_to_micron = ConvertUnits(unit, "micrometer")
+            return (
+                convert_to_micron(downsample_ratio / float(wsi.properties["tiff.YResolution"])),
+                convert_to_micron(downsample_ratio / float(wsi.properties["tiff.XResolution"])),
+            )
 
-        factor *= wsi.level_downsamples[level]
-        return (factor / float(wsi.properties["tiff.YResolution"]), factor / float(wsi.properties["tiff.XResolution"]))
+        raise ValueError("`mpp` cannot be obtained for this file. Please use `level` instead.")
+
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
+
+        """
+        objective_power = wsi.properties.get("openslide.objective-power")
+        if objective_power:
+            downsample_ratio = self.get_downsample_ratio(wsi, level)
+            return float(objective_power) / downsample_ratio
+
+        raise ValueError("Objective `power` cannot be obtained for this file. Please use `level` (or `mpp`) instead.")
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args that overrides `self.kwargs` for existing keys.
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         wsi_list: list = []
 
         filenames: Sequence[PathLike] = ensure_tuple(data)
         kwargs_ = self.kwargs.copy()
         kwargs_.update(kwargs)
@@ -774,17 +986,17 @@
         Extracts and returns a patch image form the whole slide image.
 
         Args:
             wsi: a whole slide image object loaded from a file or a lis of such objects
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         # Extract a patch or the entire image
         # (reverse the order of location and size to become WxH for OpenSlide)
         pil_patch = wsi.read_region(location=location[::-1], size=size[::-1], level=level)
 
         # convert to RGB/RGBA
@@ -801,125 +1013,131 @@
 
 @require_pkg(pkg_name="tifffile")
 class TiffFileWSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using TiffFile library.
 
     Args:
-        level: the whole slide image level at which the image is extracted. (default=0)
-            This is overridden if the level argument is provided in `get_data`.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         kwargs: additional args for `tifffile.TiffFile` module.
 
+        Notes:
+            - Objective power cannot be obtained via TiffFile backend.
+            - Only one of resolution parameters, `level` or `mpp`, should be provided.
+                If such parameters are provided in `get_data` method, those will override the values provided here.
+                If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_suffixes = ["tif", "tiff", "svs"]
     backend = "tifffile"
 
-    def __init__(
-        self,
-        level: int = 0,
-        channel_dim: int = 0,
-        dtype: DtypeLike | torch.dtype = np.uint8,
-        device: torch.device | str | None = None,
-        mode: str = "RGB",
-        **kwargs,
-    ):
-        super().__init__(level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
     @staticmethod
     def get_level_count(wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return len(wsi.pages)
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return (wsi.pages[level].imagelength, wsi.pages[level].imagewidth)
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return float(wsi.pages[0].imagelength) / float(wsi.pages[level].imagelength)
 
     @staticmethod
     def get_file_path(wsi) -> str:
         """Return the file path for the WSI object"""
         return str(abspath(wsi.filehandle.path))
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
+        if (
+            "XResolution" in wsi.pages[level].tags
+            and "YResolution" in wsi.pages[level].tags
+            and wsi.pages[level].tags["XResolution"].value
+            and wsi.pages[level].tags["YResolution"].value
+        ):
+            unit = wsi.pages[level].tags.get("ResolutionUnit")
+            if unit is not None:
+                unit = str(unit.value)[8:]
+            else:
+                warnings.warn("The resolution unit is missing. `micrometer` will be used as default.")
+                unit = "micrometer"
 
-        unit = wsi.pages[level].tags["ResolutionUnit"].value
-        if unit == unit.CENTIMETER:
-            factor = 10000.0
-        elif unit == unit.MILLIMETER:
-            factor = 1000.0
-        elif unit == unit.MICROMETER:
-            factor = 1.0
-        elif unit == unit.INCH:
-            factor = 25400.0
-        else:
-            raise ValueError(f"The resolution unit is not a valid tiff resolution or missing: {unit.name}")
+            convert_to_micron = ConvertUnits(unit, "micrometer")
+            # Here x and y resolutions are rational numbers so each of them is represented by a tuple.
+            yres = wsi.pages[level].tags["YResolution"].value
+            xres = wsi.pages[level].tags["XResolution"].value
+            return convert_to_micron(yres[1] / yres[0]), convert_to_micron(xres[1] / xres[0])
 
-        # Here x and y resolutions are rational numbers so each of them is represented by a tuple.
-        yres = wsi.pages[level].tags["YResolution"].value
-        xres = wsi.pages[level].tags["XResolution"].value
-        return (factor * yres[1] / yres[0], factor * xres[1] / xres[0])
+        raise ValueError("`mpp`  cannot be obtained for this file. Please use `level` instead.")
+
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
+
+        """
+        raise ValueError(
+            "Currently, TiffFile does not provide a general API to obtain objective power."
+            "Please use `level` (or `mpp`) instead, or try other backends."
+        )
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args that overrides `self.kwargs` for existing keys.
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         wsi_list: list = []
 
         filenames: Sequence[PathLike] = ensure_tuple(data)
         kwargs_ = self.kwargs.copy()
         kwargs_.update(kwargs)
@@ -936,17 +1154,17 @@
         Extracts and returns a patch image form the whole slide image.
 
         Args:
             wsi: a whole slide image object loaded from a file or a lis of such objects
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         # Load the entire image
         wsi_image: np.ndarray = wsi.asarray(level=level).astype(dtype)
         if len(wsi_image.shape) < 3:
             wsi_image = wsi_image[..., None]
```

## monai/inferers/inferer.py

```diff
@@ -335,15 +335,15 @@
     Args:
         roi_size: the window size to execute SlidingWindow evaluation.
             If it has non-positive components, the corresponding `inputs` size will be used.
             if the components of the `roi_size` are non-positive values, the transform will use the
             corresponding components of img size. For example, `roi_size=(32, -1)` will be adapted
             to `(32, 64)` if the second spatial dimension size of img is `64`.
         sw_batch_size: the batch size to run window slices.
-        overlap: Amount of overlap between scans.
+        overlap: Amount of overlap between scans along each spatial dimension, defaults to ``0.25``.
         mode: {``"constant"``, ``"gaussian"``}
             How to blend output of overlapping windows. Defaults to ``"constant"``.
 
             - ``"constant``": gives equal weight to all predictions.
             - ``"gaussian``": gives less weight to predictions on edges of windows.
 
         sigma_scale: the standard deviation coefficient of the Gaussian window when `mode` is ``"gaussian"``.
@@ -362,48 +362,59 @@
             set to device=torch.device('cpu') the gpu memory consumption is less and independent of the
             `inputs` and `roi_size`. Output is on the `device`.
         progress: whether to print a tqdm progress bar.
         cache_roi_weight_map: whether to precompute the ROI weight map.
         cpu_thresh: when provided, dynamically switch to stitching on cpu (to save gpu memory)
             when input image volume is larger than this threshold (in pixels/voxels).
             Otherwise use ``"device"``. Thus, the output may end-up on either cpu or gpu.
+        buffer_steps: the number of sliding window iterations along the ``buffer_dim``
+            to be buffered on ``sw_device`` before writing to ``device``.
+            (Typically, ``sw_device`` is ``cuda`` and ``device`` is ``cpu``.)
+            default is None, no buffering. For the buffer dim, when spatial size is divisible by buffer_steps*roi_size,
+            (i.e. no overlapping among the buffers) non_blocking copy may be automatically enabled for efficiency.
+        buffer_dim: the spatial dimension along which the buffers are created.
+            0 indicates the first spatial dimension. Default is -1, the last spatial dimension.
 
     Note:
         ``sw_batch_size`` denotes the max number of windows per network inference iteration,
         not the batch size of inputs.
 
     """
 
     def __init__(
         self,
         roi_size: Sequence[int] | int,
         sw_batch_size: int = 1,
-        overlap: float = 0.25,
+        overlap: Sequence[float] | float = 0.25,
         mode: BlendMode | str = BlendMode.CONSTANT,
         sigma_scale: Sequence[float] | float = 0.125,
         padding_mode: PytorchPadMode | str = PytorchPadMode.CONSTANT,
         cval: float = 0.0,
         sw_device: torch.device | str | None = None,
         device: torch.device | str | None = None,
         progress: bool = False,
         cache_roi_weight_map: bool = False,
         cpu_thresh: int | None = None,
+        buffer_steps: int | None = None,
+        buffer_dim: int = -1,
     ) -> None:
         super().__init__()
         self.roi_size = roi_size
         self.sw_batch_size = sw_batch_size
         self.overlap = overlap
         self.mode: BlendMode = BlendMode(mode)
         self.sigma_scale = sigma_scale
         self.padding_mode = padding_mode
         self.cval = cval
         self.sw_device = sw_device
         self.device = device
         self.progress = progress
         self.cpu_thresh = cpu_thresh
+        self.buffer_steps = buffer_steps
+        self.buffer_dim = buffer_dim
 
         # compute_importance_map takes long time when computing on cpu. We thus
         # compute it once if it's static and then save it for future usage
         self.roi_weight_map = None
         try:
             if cache_roi_weight_map and isinstance(roi_size, Sequence) and min(roi_size) > 0:  # non-dynamic roi size
                 if device is None:
@@ -411,15 +422,16 @@
                 self.roi_weight_map = compute_importance_map(
                     ensure_tuple(self.roi_size), mode=mode, sigma_scale=sigma_scale, device=device
                 )
             if cache_roi_weight_map and self.roi_weight_map is None:
                 warnings.warn("cache_roi_weight_map=True, but cache is not created. (dynamic roi_size?)")
         except BaseException as e:
             raise RuntimeError(
-                "Seems to be OOM. Please try smaller roi_size, or use mode='constant' instead of mode='gaussian'. "
+                f"roi size {self.roi_size}, mode={mode}, sigma_scale={sigma_scale}, device={device}\n"
+                "Seems to be OOM. Please try smaller patch size or mode='constant' instead of mode='gaussian'."
             ) from e
 
     def __call__(
         self,
         inputs: torch.Tensor,
         network: Callable[..., torch.Tensor | Sequence[torch.Tensor] | dict[Any, torch.Tensor]],
         *args: Any,
@@ -451,14 +463,16 @@
             self.padding_mode,
             self.cval,
             self.sw_device,
             device,
             self.progress,
             self.roi_weight_map,
             None,
+            self.buffer_steps,
+            self.buffer_dim,
             *args,
             **kwargs,
         )
 
 
 class SaliencyInferer(Inferer):
     """
```

## monai/inferers/utils.py

```diff
@@ -7,55 +7,60 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-import warnings
+import itertools
 from collections.abc import Callable, Mapping, Sequence
-from typing import Any
+from typing import Any, Iterable
 
+import numpy as np
 import torch
 import torch.nn.functional as F
 
 from monai.data.meta_tensor import MetaTensor
 from monai.data.utils import compute_importance_map, dense_patch_slices, get_valid_patch_size
-from monai.transforms import Resize
 from monai.utils import (
     BlendMode,
     PytorchPadMode,
     convert_data_type,
     convert_to_dst_type,
     ensure_tuple,
+    ensure_tuple_rep,
     fall_back_tuple,
     look_up_option,
     optional_import,
+    pytorch_after,
 )
 
 tqdm, _ = optional_import("tqdm", name="tqdm")
+_nearest_mode = "nearest-exact" if pytorch_after(1, 11) else "nearest"
 
 __all__ = ["sliding_window_inference"]
 
 
 def sliding_window_inference(
-    inputs: torch.Tensor,
+    inputs: torch.Tensor | MetaTensor,
     roi_size: Sequence[int] | int,
     sw_batch_size: int,
     predictor: Callable[..., torch.Tensor | Sequence[torch.Tensor] | dict[Any, torch.Tensor]],
-    overlap: float = 0.25,
+    overlap: Sequence[float] | float = 0.25,
     mode: BlendMode | str = BlendMode.CONSTANT,
     sigma_scale: Sequence[float] | float = 0.125,
     padding_mode: PytorchPadMode | str = PytorchPadMode.CONSTANT,
     cval: float = 0.0,
     sw_device: torch.device | str | None = None,
     device: torch.device | str | None = None,
     progress: bool = False,
     roi_weight_map: torch.Tensor | None = None,
     process_fn: Callable | None = None,
+    buffer_steps: int | None = None,
+    buffer_dim: int = -1,
     *args: Any,
     **kwargs: Any,
 ) -> torch.Tensor | tuple[torch.Tensor, ...] | dict[Any, torch.Tensor]:
     """
     Sliding window inference on `inputs` with `predictor`.
 
     The outputs of `predictor` could be a tensor, a tuple, or a dictionary of tensors.
@@ -83,15 +88,15 @@
             where H'W'[D'] represents the output patch's spatial size, M is the number of output channels,
             N is `sw_batch_size`, e.g., the input shape is (7, 1, 128,128,128),
             the output could be a tuple of two tensors, with shapes: ((7, 5, 128, 64, 256), (7, 4, 64, 32, 128)).
             In this case, the parameter `overlap` and `roi_size` need to be carefully chosen
             to ensure the scaled output ROI sizes are still integers.
             If the `predictor`'s input and output spatial sizes are different,
             we recommend choosing the parameters so that ``overlap*roi_size*zoom_scale`` is an integer for each dimension.
-        overlap: Amount of overlap between scans.
+        overlap: Amount of overlap between scans along each spatial dimension, defaults to ``0.25``.
         mode: {``"constant"``, ``"gaussian"``}
             How to blend output of overlapping windows. Defaults to ``"constant"``.
 
             - ``"constant``": gives equal weight to all predictions.
             - ``"gaussian``": gives less weight to predictions on edges of windows.
 
         sigma_scale: the standard deviation coefficient of the Gaussian window when `mode` is ``"gaussian"``.
@@ -109,219 +114,286 @@
             By default the device (and accordingly the memory) of the `inputs` is used. If for example
             set to device=torch.device('cpu') the gpu memory consumption is less and independent of the
             `inputs` and `roi_size`. Output is on the `device`.
         progress: whether to print a `tqdm` progress bar.
         roi_weight_map: pre-computed (non-negative) weight map for each ROI.
             If not given, and ``mode`` is not `constant`, this map will be computed on the fly.
         process_fn: process inference output and adjust the importance map per window
+        buffer_steps: the number of sliding window iterations along the ``buffer_dim``
+            to be buffered on ``sw_device`` before writing to ``device``.
+            (Typically, ``sw_device`` is ``cuda`` and ``device`` is ``cpu``.)
+            default is None, no buffering. For the buffer dim, when spatial size is divisible by buffer_steps*roi_size,
+            (i.e. no overlapping among the buffers) non_blocking copy may be automatically enabled for efficiency.
+        buffer_dim: the spatial dimension along which the buffers are created.
+            0 indicates the first spatial dimension. Default is -1, the last spatial dimension.
         args: optional args to be passed to ``predictor``.
         kwargs: optional keyword args to be passed to ``predictor``.
 
     Note:
         - input must be channel-first and have a batch dim, supports N-D sliding window.
 
     """
-    compute_dtype = inputs.dtype
+    buffered = buffer_steps is not None and buffer_steps > 0
     num_spatial_dims = len(inputs.shape) - 2
-    if overlap < 0 or overlap >= 1:
-        raise ValueError("overlap must be >= 0 and < 1.")
+    if buffered:
+        if buffer_dim < -num_spatial_dims or buffer_dim > num_spatial_dims:
+            raise ValueError(f"buffer_dim must be in [{-num_spatial_dims}, {num_spatial_dims}], got {buffer_dim}.")
+        if buffer_dim < 0:
+            buffer_dim += num_spatial_dims
+    overlap = ensure_tuple_rep(overlap, num_spatial_dims)
+    for o in overlap:
+        if o < 0 or o >= 1:
+            raise ValueError(f"overlap must be >= 0 and < 1, got {overlap}.")
+    compute_dtype = inputs.dtype
 
     # determine image spatial size and batch size
     # Note: all input images must have the same image size and batch size
     batch_size, _, *image_size_ = inputs.shape
+    device = device or inputs.device
+    sw_device = sw_device or inputs.device
 
-    if device is None:
-        device = inputs.device
-    if sw_device is None:
-        sw_device = inputs.device
-
+    temp_meta = None
+    if isinstance(inputs, MetaTensor):
+        temp_meta = MetaTensor([]).copy_meta_from(inputs, copy_attr=False)
+    inputs = convert_data_type(inputs, torch.Tensor, wrap_sequence=True)[0]
     roi_size = fall_back_tuple(roi_size, image_size_)
+
     # in case that image size is smaller than roi size
     image_size = tuple(max(image_size_[i], roi_size[i]) for i in range(num_spatial_dims))
     pad_size = []
     for k in range(len(inputs.shape) - 1, 1, -1):
         diff = max(roi_size[k - 2] - inputs.shape[k], 0)
         half = diff // 2
         pad_size.extend([half, diff - half])
-
-    if max(pad_size) > 0:
+    if any(pad_size):
         inputs = F.pad(inputs, pad=pad_size, mode=look_up_option(padding_mode, PytorchPadMode), value=cval)
 
+    # Store all slices
     scan_interval = _get_scan_interval(image_size, roi_size, num_spatial_dims, overlap)
+    slices = dense_patch_slices(image_size, roi_size, scan_interval, return_slice=not buffered)
 
-    # Store all slices in list
-    slices = dense_patch_slices(image_size, roi_size, scan_interval)
     num_win = len(slices)  # number of windows per image
     total_slices = num_win * batch_size  # total number of windows
+    windows_range: Iterable
+    if not buffered:
+        non_blocking = False
+        windows_range = range(0, total_slices, sw_batch_size)
+    else:
+        slices, n_per_batch, b_slices, windows_range = _create_buffered_slices(
+            slices, batch_size, sw_batch_size, buffer_dim, buffer_steps
+        )
+        non_blocking, _ss = torch.cuda.is_available(), -1
+        for x in b_slices[:n_per_batch]:
+            if x[1] < _ss:  # detect overlapping slices
+                non_blocking = False
+                break
+            _ss = x[2]
 
     # Create window-level importance map
     valid_patch_size = get_valid_patch_size(image_size, roi_size)
     if valid_patch_size == roi_size and (roi_weight_map is not None):
         importance_map_ = roi_weight_map
     else:
         try:
+            valid_p_size = ensure_tuple(valid_patch_size)
             importance_map_ = compute_importance_map(
-                valid_patch_size, mode=mode, sigma_scale=sigma_scale, device=device
+                valid_p_size, mode=mode, sigma_scale=sigma_scale, device=sw_device, dtype=compute_dtype
             )
-        except BaseException as e:
+            if len(importance_map_.shape) == num_spatial_dims and not process_fn:
+                importance_map_ = importance_map_[None, None]  # adds batch, channel dimensions
+        except Exception as e:
             raise RuntimeError(
+                f"patch size {valid_p_size}, mode={mode}, sigma_scale={sigma_scale}, device={device}\n"
                 "Seems to be OOM. Please try smaller patch size or mode='constant' instead of mode='gaussian'."
             ) from e
-    importance_map_ = convert_data_type(importance_map_, torch.Tensor, device, compute_dtype)[0]
-
-    # handle non-positive weights
-    min_non_zero = max(torch.min(importance_map_).item(), 1e-3)
-    importance_map_ = torch.clamp_(importance_map_.to(torch.float32), min=min_non_zero).to(compute_dtype)
-
-    # Perform predictions
-    dict_key, output_image_list, count_map_list = None, [], []
-    _initialized_ss = -1
-    is_tensor_output = True  # whether the predictor's output is a tensor (instead of dict/tuple)
+    importance_map_ = convert_data_type(importance_map_, torch.Tensor, device=sw_device, dtype=compute_dtype)[0]
 
+    # stores output and count map
+    output_image_list, count_map_list, sw_device_buffer, b_s, b_i = [], [], [], 0, 0  # type: ignore
     # for each patch
-    for slice_g in tqdm(range(0, total_slices, sw_batch_size)) if progress else range(0, total_slices, sw_batch_size):
-        slice_range = range(slice_g, min(slice_g + sw_batch_size, total_slices))
+    for slice_g in tqdm(windows_range) if progress else windows_range:
+        slice_range = range(slice_g, min(slice_g + sw_batch_size, b_slices[b_s][0] if buffered else total_slices))
         unravel_slice = [
-            [slice(int(idx / num_win), int(idx / num_win) + 1), slice(None)] + list(slices[idx % num_win])
+            [slice(idx // num_win, idx // num_win + 1), slice(None)] + list(slices[idx % num_win])
             for idx in slice_range
         ]
-        window_data = torch.cat(
-            [convert_data_type(inputs[win_slice], torch.Tensor)[0] for win_slice in unravel_slice]
-        ).to(sw_device)
-        seg_prob_out = predictor(window_data, *args, **kwargs)  # batched patch segmentation
-
-        # convert seg_prob_out to tuple seg_prob_tuple, this does not allocate new memory.
-        seg_prob_tuple: tuple[torch.Tensor, ...]
-        if isinstance(seg_prob_out, torch.Tensor):
-            seg_prob_tuple = (seg_prob_out,)
-        elif isinstance(seg_prob_out, Mapping):
-            if dict_key is None:
-                dict_key = sorted(seg_prob_out.keys())  # track predictor's output keys
-            seg_prob_tuple = tuple(seg_prob_out[k] for k in dict_key)
-            is_tensor_output = False
+        if sw_batch_size > 1:
+            win_data = torch.cat([inputs[win_slice] for win_slice in unravel_slice]).to(sw_device)
         else:
-            seg_prob_tuple = ensure_tuple(seg_prob_out)
-            is_tensor_output = False
+            win_data = inputs[unravel_slice[0]].to(sw_device)
+        seg_prob_out = predictor(win_data, *args, **kwargs)  # batched patch
 
+        # convert seg_prob_out to tuple seg_tuple, this does not allocate new memory.
+        dict_keys, seg_tuple = _flatten_struct(seg_prob_out)
         if process_fn:
-            seg_prob_tuple, importance_map = process_fn(seg_prob_tuple, window_data, importance_map_)
+            seg_tuple, w_t = process_fn(seg_tuple, win_data, importance_map_)
+        else:
+            w_t = importance_map_
+        if len(w_t.shape) == num_spatial_dims:
+            w_t = w_t[None, None]
+        w_t = w_t.to(dtype=compute_dtype, device=sw_device)
+        if buffered:
+            c_start, c_end = b_slices[b_s][1:]
+            if not sw_device_buffer:
+                k = seg_tuple[0].shape[1]  # len(seg_tuple) > 1 is currently ignored
+                sp_size = list(image_size)
+                sp_size[buffer_dim] = c_end - c_start
+                sw_device_buffer = [torch.zeros(size=[1, k, *sp_size], dtype=compute_dtype, device=sw_device)]
+            for p, s in zip(seg_tuple[0], unravel_slice):
+                offset = s[buffer_dim + 2].start - c_start
+                s[buffer_dim + 2] = slice(offset, offset + roi_size[buffer_dim])
+                s[0] = slice(0, 1)
+                sw_device_buffer[0][s] += p * w_t
+            b_i += len(unravel_slice)
+            if b_i < b_slices[b_s][0]:
+                continue
         else:
-            importance_map = importance_map_
+            sw_device_buffer = list(seg_tuple)
 
-        # for each output in multi-output list
-        for ss, seg_prob in enumerate(seg_prob_tuple):
-            seg_prob = seg_prob.to(device)  # BxCxMxNxP or BxCxMxN
-
-            # compute zoom scale: out_roi_size/in_roi_size
-            zoom_scale = []
-            for axis, (img_s_i, out_w_i, in_w_i) in enumerate(
-                zip(image_size, seg_prob.shape[2:], window_data.shape[2:])
-            ):
-                _scale = out_w_i / float(in_w_i)
-                if not (img_s_i * _scale).is_integer():
-                    warnings.warn(
-                        f"For spatial axis: {axis}, output[{ss}] will have non-integer shape. Spatial "
-                        f"zoom_scale between output[{ss}] and input is {_scale}. Please pad inputs."
-                    )
-                zoom_scale.append(_scale)
-
-            if _initialized_ss < ss:  # init. the ss-th buffer at the first iteration
-                # construct multi-resolution outputs
-                output_classes = seg_prob.shape[1]
-                output_shape = [batch_size, output_classes] + [
-                    int(image_size_d * zoom_scale_d) for image_size_d, zoom_scale_d in zip(image_size, zoom_scale)
-                ]
+        for ss in range(len(sw_device_buffer)):
+            b_shape = sw_device_buffer[ss].shape
+            seg_chns, seg_shape = b_shape[1], b_shape[2:]
+            z_scale = None
+            if not buffered and seg_shape != roi_size:
+                z_scale = [out_w_i / float(in_w_i) for out_w_i, in_w_i in zip(seg_shape, roi_size)]
+                w_t = F.interpolate(w_t, seg_shape, mode=_nearest_mode)
+            if len(output_image_list) <= ss:
+                output_shape = [batch_size, seg_chns]
+                output_shape += [int(_i * _z) for _i, _z in zip(image_size, z_scale)] if z_scale else list(image_size)
                 # allocate memory to store the full output and the count for overlapping parts
-                output_image_list.append(torch.zeros(output_shape, dtype=compute_dtype, device=device))
+                new_tensor: Callable = torch.empty if non_blocking else torch.zeros  # type: ignore
+                output_image_list.append(new_tensor(output_shape, dtype=compute_dtype, device=device))
                 count_map_list.append(torch.zeros([1, 1] + output_shape[2:], dtype=compute_dtype, device=device))
-                _initialized_ss += 1
-
-            # resizing the importance_map
-            resizer = Resize(spatial_size=seg_prob.shape[2:], mode="nearest", anti_aliasing=False)
+                w_t_ = w_t.to(device)
+                for __s in slices:
+                    if z_scale is not None:
+                        __s = tuple(slice(int(_si.start * z_s), int(_si.stop * z_s)) for _si, z_s in zip(__s, z_scale))
+                    count_map_list[-1][(slice(None), slice(None), *__s)] += w_t_
+            if buffered:
+                o_slice = [slice(None)] * len(inputs.shape)
+                o_slice[buffer_dim + 2] = slice(c_start, c_end)
+                img_b = b_s // n_per_batch  # image batch index
+                o_slice[0] = slice(img_b, img_b + 1)
+                if non_blocking:
+                    output_image_list[0][o_slice].copy_(sw_device_buffer[0], non_blocking=non_blocking)
+                else:
+                    output_image_list[0][o_slice] += sw_device_buffer[0].to(device=device)
+            else:
+                sw_device_buffer[ss] *= w_t
+                sw_device_buffer[ss] = sw_device_buffer[ss].to(device)
+                _compute_coords(sw_batch_size, unravel_slice, z_scale, output_image_list[ss], sw_device_buffer[ss])
+        sw_device_buffer = []
+        if buffered:
+            b_s += 1
 
-            # store the result in the proper location of the full output. Apply weights from importance map.
-            for idx, original_idx in zip(slice_range, unravel_slice):
-                # zoom roi
-                original_idx_zoom = list(original_idx)  # 4D for 2D image, 5D for 3D image
-                for axis in range(2, len(original_idx_zoom)):
-                    zoomed_start = original_idx[axis].start * zoom_scale[axis - 2]
-                    zoomed_end = original_idx[axis].stop * zoom_scale[axis - 2]
-                    if not zoomed_start.is_integer() or (not zoomed_end.is_integer()):
-                        warnings.warn(
-                            f"For axis-{axis-2} of output[{ss}], the output roi range is not int. "
-                            f"Input roi range is ({original_idx[axis].start}, {original_idx[axis].stop}). "
-                            f"Spatial zoom_scale between output[{ss}] and input is {zoom_scale[axis - 2]}. "
-                            f"Corresponding output roi range is ({zoomed_start}, {zoomed_end}).\n"
-                            f"Please change overlap ({overlap}) or roi_size ({roi_size[axis-2]}) for axis-{axis-2}. "
-                            "Tips: if overlap*roi_size*zoom_scale is an integer, it usually works."
-                        )
-                    original_idx_zoom[axis] = slice(int(zoomed_start), int(zoomed_end), None)
-                importance_map_zoom = (
-                    resizer(importance_map.unsqueeze(0))[0].to(compute_dtype)
-                    if seg_prob.shape[2:] != importance_map.shape
-                    else importance_map.to(compute_dtype)
-                )
-                # store results and weights
-                output_image_list[ss][original_idx_zoom] += importance_map_zoom * seg_prob[idx - slice_g]
-                count_map_list[ss][original_idx_zoom] += (
-                    importance_map_zoom.unsqueeze(0).unsqueeze(0).expand(count_map_list[ss][original_idx_zoom].shape)
-                )
+    if non_blocking:
+        torch.cuda.current_stream().synchronize()
 
     # account for any overlapping sections
     for ss in range(len(output_image_list)):
-        output_image_list[ss] = output_image_list[ss]
-        _map = count_map_list.pop(0)
-        for _i in range(output_image_list[ss].shape[1]):
-            output_image_list[ss][:, _i : _i + 1, ...] /= _map
-        output_image_list[ss] = output_image_list[ss].to(compute_dtype)
+        output_image_list[ss] /= count_map_list.pop(0)
 
     # remove padding if image_size smaller than roi_size
-    for ss, output_i in enumerate(output_image_list):
-        zoom_scale = [
-            seg_prob_map_shape_d / roi_size_d for seg_prob_map_shape_d, roi_size_d in zip(output_i.shape[2:], roi_size)
-        ]
-
-        final_slicing: list[slice] = []
-        for sp in range(num_spatial_dims):
-            slice_dim = slice(pad_size[sp * 2], image_size_[num_spatial_dims - sp - 1] + pad_size[sp * 2])
-            slice_dim = slice(
-                int(round(slice_dim.start * zoom_scale[num_spatial_dims - sp - 1])),
-                int(round(slice_dim.stop * zoom_scale[num_spatial_dims - sp - 1])),
-            )
-            final_slicing.insert(0, slice_dim)
-        while len(final_slicing) < len(output_i.shape):
-            final_slicing.insert(0, slice(None))
-        output_image_list[ss] = output_i[final_slicing]
+    if any(pad_size):
+        for ss, output_i in enumerate(output_image_list):
+            zoom_scale = [_shape_d / _roi_size_d for _shape_d, _roi_size_d in zip(output_i.shape[2:], roi_size)]
+            final_slicing: list[slice] = []
+            for sp in range(num_spatial_dims):
+                si = num_spatial_dims - sp - 1
+                slice_dim = slice(
+                    int(round(pad_size[sp * 2] * zoom_scale[si])),
+                    int(round((pad_size[sp * 2] + image_size_[si]) * zoom_scale[si])),
+                )
+                final_slicing.insert(0, slice_dim)
+            output_image_list[ss] = output_i[(slice(None), slice(None), *final_slicing)]
 
-    if dict_key is not None:  # if output of predictor is a dict
-        final_output = dict(zip(dict_key, output_image_list))
+    final_output = _pack_struct(output_image_list, dict_keys)
+    if temp_meta is not None:
+        final_output = convert_to_dst_type(final_output, temp_meta, device=device)[0]
     else:
-        final_output = tuple(output_image_list)  # type: ignore
-    final_output = final_output[0] if is_tensor_output else final_output
+        final_output = convert_to_dst_type(final_output, inputs, device=device)[0]
 
-    if isinstance(inputs, MetaTensor):
-        final_output = convert_to_dst_type(final_output, inputs, device=device)[0]  # type: ignore
-    return final_output
+    return final_output  # type: ignore
+
+
+def _create_buffered_slices(slices, batch_size, sw_batch_size, buffer_dim, buffer_steps):
+    """rearrange slices for buffering"""
+    slices_np = np.asarray(slices)
+    slices_np = slices_np[np.argsort(slices_np[:, buffer_dim, 0], kind="mergesort")]
+    slices = [tuple(slice(c[0], c[1]) for c in i) for i in slices_np]
+    slices_np = slices_np[:, buffer_dim]
+
+    _, _, _b_lens = np.unique(slices_np[:, 0], return_counts=True, return_index=True)
+    b_ends = np.cumsum(_b_lens).tolist()  # possible buffer flush boundaries
+    x = [0, *b_ends][:: min(len(b_ends), int(buffer_steps))]
+    if x[-1] < b_ends[-1]:
+        x.append(b_ends[-1])
+    n_per_batch = len(x) - 1
+    windows_range = [
+        range(b * x[-1] + x[i], b * x[-1] + x[i + 1], sw_batch_size)
+        for b in range(batch_size)
+        for i in range(n_per_batch)
+    ]
+    b_slices = []
+    for _s, _r in enumerate(windows_range):
+        s_s = slices_np[windows_range[_s - 1].stop % len(slices) if _s > 0 else 0, 0]
+        s_e = slices_np[(_r.stop - 1) % len(slices), 1]
+        b_slices.append((_r.stop, s_s, s_e))  # buffer index, slice start, slice end
+    windows_range = itertools.chain(*windows_range)  # type: ignore
+    return slices, n_per_batch, b_slices, windows_range
+
+
+def _compute_coords(sw, coords, z_scale, out, patch):
+    """sliding window batch spatial scaling indexing for multi-resolution outputs."""
+    for original_idx, p in zip(coords, patch):
+        idx_zm = list(original_idx)  # 4D for 2D image, 5D for 3D image
+        if z_scale:
+            for axis in range(2, len(idx_zm)):
+                idx_zm[axis] = slice(
+                    int(original_idx[axis].start * z_scale[axis - 2]), int(original_idx[axis].stop * z_scale[axis - 2])
+                )
+        out[idx_zm] += p
 
 
 def _get_scan_interval(
-    image_size: Sequence[int], roi_size: Sequence[int], num_spatial_dims: int, overlap: float
+    image_size: Sequence[int], roi_size: Sequence[int], num_spatial_dims: int, overlap: Sequence[float]
 ) -> tuple[int, ...]:
     """
     Compute scan interval according to the image size, roi size and overlap.
     Scan interval will be `int((1 - overlap) * roi_size)`, if interval is 0,
     use 1 instead to make sure sliding window works.
 
     """
     if len(image_size) != num_spatial_dims:
-        raise ValueError("image coord different from spatial dims.")
+        raise ValueError(f"len(image_size) {len(image_size)} different from spatial dims {num_spatial_dims}.")
     if len(roi_size) != num_spatial_dims:
-        raise ValueError("roi coord different from spatial dims.")
+        raise ValueError(f"len(roi_size) {len(roi_size)} different from spatial dims {num_spatial_dims}.")
 
     scan_interval = []
-    for i in range(num_spatial_dims):
+    for i, o in zip(range(num_spatial_dims), overlap):
         if roi_size[i] == image_size[i]:
             scan_interval.append(int(roi_size[i]))
         else:
-            interval = int(roi_size[i] * (1 - overlap))
+            interval = int(roi_size[i] * (1 - o))
             scan_interval.append(interval if interval > 0 else 1)
     return tuple(scan_interval)
+
+
+def _flatten_struct(seg_out):
+    dict_keys = None
+    seg_probs: tuple[torch.Tensor, ...]
+    if isinstance(seg_out, torch.Tensor):
+        seg_probs = (seg_out,)
+    elif isinstance(seg_out, Mapping):
+        dict_keys = sorted(seg_out.keys())  # track predictor's output keys
+        seg_probs = tuple(seg_out[k] for k in dict_keys)
+    else:
+        seg_probs = ensure_tuple(seg_out)
+    return dict_keys, seg_probs
+
+
+def _pack_struct(seg_out, dict_keys=None):
+    if dict_keys is not None:
+        return dict(zip(dict_keys, seg_out))
+    if isinstance(seg_out, (list, tuple)) and len(seg_out) == 1:
+        return seg_out[0]
+    return ensure_tuple(seg_out)
```

## monai/metrics/hausdorff_distance.py

```diff
@@ -8,19 +8,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
+from typing import Any
 
 import numpy as np
 import torch
 
-from monai.metrics.utils import do_metric_reduction, get_mask_edges, get_surface_distance, ignore_background
+from monai.metrics.utils import (
+    do_metric_reduction,
+    get_mask_edges,
+    get_surface_distance,
+    ignore_background,
+    prepare_spacing,
+)
 from monai.utils import MetricReduction, convert_data_type
 
 from .metric import CumulativeIterationMetric
 
 __all__ = ["HausdorffDistanceMetric", "compute_hausdorff_distance", "compute_percent_hausdorff_distance"]
 
 
@@ -66,37 +74,49 @@
         self.include_background = include_background
         self.distance_metric = distance_metric
         self.percentile = percentile
         self.directed = directed
         self.reduction = reduction
         self.get_not_nans = get_not_nans
 
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor, **kwargs: Any) -> torch.Tensor:  # type: ignore[override]
         """
         Args:
             y_pred: input data to compute, typical segmentation model output.
                 It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
                 should be binarized.
             y: ground truth to compute the distance. It must be one-hot format and first dim is batch.
                 The values should be binarized.
+            kwargs: additional parameters, e.g. ``spacing`` should be passed to correctly compute the metric.
+                ``spacing``: spacing of pixel (or voxel). This parameter is relevant only
+                if ``distance_metric`` is set to ``"euclidean"``.
+                If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+                the length of the sequence must be equal to the image dimensions.
+                This spacing will be used for all images in the batch.
+                If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+                If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+                else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+                for all images in batch. Defaults to ``None``.
 
         Raises:
             ValueError: when `y_pred` has less than three dimensions.
         """
         dims = y_pred.ndimension()
         if dims < 3:
             raise ValueError("y_pred should have at least three dimensions.")
+
         # compute (BxC) for each channel for each batch
         return compute_hausdorff_distance(
             y_pred=y_pred,
             y=y,
             include_background=self.include_background,
             distance_metric=self.distance_metric,
             percentile=self.percentile,
             directed=self.directed,
+            spacing=kwargs.get("spacing"),
         )
 
     def aggregate(
         self, reduction: MetricReduction | str | None = None
     ) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         """
         Execute reduction logic for the output of `compute_hausdorff_distance`.
@@ -119,14 +139,15 @@
 def compute_hausdorff_distance(
     y_pred: np.ndarray | torch.Tensor,
     y: np.ndarray | torch.Tensor,
     include_background: bool = False,
     distance_metric: str = "euclidean",
     percentile: float | None = None,
     directed: bool = False,
+    spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None = None,
 ) -> torch.Tensor:
     """
     Compute the Hausdorff distance.
 
     Args:
         y_pred: input data to compute, typical segmentation model output.
             It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
@@ -137,50 +158,69 @@
             the predicted output. Defaults to ``False``.
         distance_metric: : [``"euclidean"``, ``"chessboard"``, ``"taxicab"``]
             the metric used to compute surface distance. Defaults to ``"euclidean"``.
         percentile: an optional float number between 0 and 100. If specified, the corresponding
             percentile of the Hausdorff Distance rather than the maximum result will be achieved.
             Defaults to ``None``.
         directed: whether to calculate directed Hausdorff distance. Defaults to ``False``.
+        spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
+            If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+            the length of the sequence must be equal to the image dimensions. This spacing will be used for all images in the batch.
+            If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+            If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+            else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+            for all images in batch. Defaults to ``None``.
     """
 
     if not include_background:
         y_pred, y = ignore_background(y_pred=y_pred, y=y)
     y_pred = convert_data_type(y_pred, output_type=torch.Tensor, dtype=torch.float)[0]
     y = convert_data_type(y, output_type=torch.Tensor, dtype=torch.float)[0]
 
     if y.shape != y_pred.shape:
         raise ValueError(f"y_pred and y should have same shapes, got {y_pred.shape} and {y.shape}.")
 
     batch_size, n_class = y_pred.shape[:2]
     hd = np.empty((batch_size, n_class))
+
+    img_dim = y_pred.ndim - 2
+    spacing_list = prepare_spacing(spacing=spacing, batch_size=batch_size, img_dim=img_dim)
+
     for b, c in np.ndindex(batch_size, n_class):
         (edges_pred, edges_gt) = get_mask_edges(y_pred[b, c], y[b, c])
         if not np.any(edges_gt):
             warnings.warn(f"the ground truth of class {c} is all 0, this may result in nan/inf distance.")
         if not np.any(edges_pred):
             warnings.warn(f"the prediction of class {c} is all 0, this may result in nan/inf distance.")
 
-        distance_1 = compute_percent_hausdorff_distance(edges_pred, edges_gt, distance_metric, percentile)
+        distance_1 = compute_percent_hausdorff_distance(
+            edges_pred, edges_gt, distance_metric, percentile, spacing_list[b]
+        )
         if directed:
             hd[b, c] = distance_1
         else:
-            distance_2 = compute_percent_hausdorff_distance(edges_gt, edges_pred, distance_metric, percentile)
+            distance_2 = compute_percent_hausdorff_distance(
+                edges_gt, edges_pred, distance_metric, percentile, spacing_list[b]
+            )
             hd[b, c] = max(distance_1, distance_2)
     return convert_data_type(hd, output_type=torch.Tensor, device=y_pred.device, dtype=torch.float)[0]
 
 
 def compute_percent_hausdorff_distance(
-    edges_pred: np.ndarray, edges_gt: np.ndarray, distance_metric: str = "euclidean", percentile: float | None = None
+    edges_pred: np.ndarray,
+    edges_gt: np.ndarray,
+    distance_metric: str = "euclidean",
+    percentile: float | None = None,
+    spacing: int | float | np.ndarray | Sequence[int | float] | None = None,
 ) -> float:
     """
     This function is used to compute the directed Hausdorff distance.
     """
 
-    surface_distance = get_surface_distance(edges_pred, edges_gt, distance_metric=distance_metric)
+    surface_distance = get_surface_distance(edges_pred, edges_gt, distance_metric=distance_metric, spacing=spacing)
 
     # for both pred and gt do not have foreground
     if surface_distance.shape == (0,):
         return np.nan
 
     if not percentile:
         return surface_distance.max()  # type: ignore[no-any-return]
```

## monai/metrics/loss_metric.py

```diff
@@ -7,14 +7,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from typing import Any
+
 import torch
 from torch.nn.modules.loss import _Loss
 
 from monai.metrics.utils import do_metric_reduction
 from monai.utils import MetricReduction
 
 from ..config import TensorOrList
@@ -88,15 +90,15 @@
         """
         data = self.get_buffer()
         if data is None:
             return (torch.tensor(0.0), torch.tensor(0.0)) if self.get_not_nans else torch.tensor(0.0)
         f, not_nans = do_metric_reduction(data, reduction or self.reduction)
         return (f, not_nans) if self.get_not_nans else f
 
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None) -> TensorOrList:
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None, **kwargs: Any) -> TensorOrList:
         """
         Input `y_pred` is compared with ground truth `y`.
         Both `y_pred` and `y` are expected to be a batch-first Tensor (BC[HWD]).
 
         Returns:
              a tensor with shape (BC[HWD]), or a list of tensors, each tensor with shape (C[HWD]).
         """
```

## monai/metrics/metric.py

```diff
@@ -45,43 +45,44 @@
 
     `__call__` is designed to handle `y_pred` and `y` (optional) in torch tensors or a list/tuple of tensors.
 
     Subclasses typically implement the `_compute_tensor` function for the actual tensor computation logic.
     """
 
     def __call__(
-        self, y_pred: TensorOrList, y: TensorOrList | None = None
+        self, y_pred: TensorOrList, y: TensorOrList | None = None, **kwargs: Any
     ) -> torch.Tensor | Sequence[torch.Tensor | Sequence[torch.Tensor]]:
         """
         Execute basic computation for model prediction `y_pred` and ground truth `y` (optional).
         It supports inputs of a list of "channel-first" Tensor and a "batch-first" Tensor.
 
         Args:
             y_pred: the raw model prediction data at one iteration, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
             y: the ground truth to compute, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
+            kwargs: additional parameters for specific metric computation logic (e.g. ``spacing`` for SurfaceDistanceMetric, etc.).
 
         Returns:
             The computed metric values at the iteration level.
             The output shape could be a `batch-first` tensor or a list of `batch-first` tensors.
             When it's a list of tensors, each item in the list can represent a specific type of metric.
 
         """
         # handling a list of channel-first data
         if isinstance(y_pred, (list, tuple)) or isinstance(y, (list, tuple)):
-            return self._compute_list(y_pred, y)
+            return self._compute_list(y_pred, y, **kwargs)
         # handling a single batch-first data
         if isinstance(y_pred, torch.Tensor):
             y_ = y.detach() if isinstance(y, torch.Tensor) else None
-            return self._compute_tensor(y_pred.detach(), y_)
+            return self._compute_tensor(y_pred.detach(), y_, **kwargs)
         raise ValueError("y_pred or y must be a list/tuple of `channel-first` Tensors or a `batch-first` Tensor.")
 
     def _compute_list(
-        self, y_pred: TensorOrList, y: TensorOrList | None = None
+        self, y_pred: TensorOrList, y: TensorOrList | None = None, **kwargs: Any
     ) -> torch.Tensor | list[torch.Tensor | Sequence[torch.Tensor]]:
         """
         Execute the metric computation for `y_pred` and `y` in a list of "channel-first" tensors.
 
         The return value is a "batch-first" tensor, or a list of "batch-first" tensors.
         When it's a list of tensors, each item in the list can represent a specific type of metric values.
 
@@ -89,28 +90,31 @@
         where each item is a tuple of three values `tp`, `fp`, `fn` for true positives, false positives,
         and false negatives respectively. This function will return a list of three items,
         (`tp_batched`, `fp_batched`, `fn_batched`), where each item is a `batch_size`-length tensor.
 
         Note: subclass may enhance the operation to have multi-thread support.
         """
         if y is not None:
-            ret = [self._compute_tensor(p.detach().unsqueeze(0), y_.detach().unsqueeze(0)) for p, y_ in zip(y_pred, y)]
+            ret = [
+                self._compute_tensor(p.detach().unsqueeze(0), y_.detach().unsqueeze(0), **kwargs)
+                for p, y_ in zip(y_pred, y)
+            ]
         else:
-            ret = [self._compute_tensor(p_.detach().unsqueeze(0), None) for p_ in y_pred]
+            ret = [self._compute_tensor(p_.detach().unsqueeze(0), None, **kwargs) for p_ in y_pred]
 
         # concat the list of results (e.g. a batch of evaluation scores)
         if isinstance(ret[0], torch.Tensor):
             return torch.cat(ret, dim=0)  # type: ignore[arg-type]
         # the result is a list of sequence of tensors (e.g. a batch of multi-class results)
         if isinstance(ret[0], (list, tuple)) and all(isinstance(i, torch.Tensor) for i in ret[0]):
             return [torch.cat(batch_i, dim=0) for batch_i in zip(*ret)]
         return ret
 
     @abstractmethod
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None) -> TensorOrList:
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None, **kwargs: Any) -> TensorOrList:
         """
         Computation logic for `y_pred` and `y` of an iteration, the data should be "batch-first" Tensors.
         A subclass should implement its own computation logic.
         The return value is usually a "batch_first" tensor, or a list of "batch_first" tensors.
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
@@ -314,32 +318,33 @@
 
     And to load `predictions` and `labels` from files, then compute metrics with multi-processing, please refer to:
     https://github.com/Project-MONAI/tutorials/blob/master/modules/compute_metric.py.
 
     """
 
     def __call__(
-        self, y_pred: TensorOrList, y: TensorOrList | None = None
+        self, y_pred: TensorOrList, y: TensorOrList | None = None, **kwargs: Any
     ) -> torch.Tensor | Sequence[torch.Tensor | Sequence[torch.Tensor]]:
         """
         Execute basic computation for model prediction and ground truth.
         It can support  both `list of channel-first Tensor` and `batch-first Tensor`.
         Users call this API to execute computation on every batch of data, then accumulate the results,
         or accumulate the original `y_pred` and `y`, then execute on the accumulated data.
 
         Args:
             y_pred: the model prediction data to compute, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
             y: the ground truth to compute, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
+            kwargs: additional parameters for specific metric computation logic (e.g. ``spacing`` for SurfaceDistanceMetric, etc.).
 
         Returns:
             The computed metric values at the iteration level. The output shape should be
             a `batch-first` tensor (BC[HWD]) or a list of `batch-first` tensors.
         """
-        ret = super().__call__(y_pred=y_pred, y=y)
+        ret = super().__call__(y_pred=y_pred, y=y, **kwargs)
         if isinstance(ret, (tuple, list)):
             self.extend(*ret)
         else:
             self.extend(ret)
 
         return ret
```

## monai/metrics/surface_dice.py

```diff
@@ -8,19 +8,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
+from typing import Any
 
 import numpy as np
 import torch
 
-from monai.metrics.utils import do_metric_reduction, get_mask_edges, get_surface_distance, ignore_background
+from monai.metrics.utils import (
+    do_metric_reduction,
+    get_mask_edges,
+    get_surface_distance,
+    ignore_background,
+    prepare_spacing,
+)
 from monai.utils import MetricReduction, convert_data_type
 
 from .metric import CumulativeIterationMetric
 
 
 class SurfaceDiceMetric(CumulativeIterationMetric):
     """
@@ -63,32 +71,43 @@
         super().__init__()
         self.class_thresholds = class_thresholds
         self.include_background = include_background
         self.distance_metric = distance_metric
         self.reduction = reduction
         self.get_not_nans = get_not_nans
 
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor, **kwargs: Any) -> torch.Tensor:  # type: ignore[override]
         r"""
         Args:
             y_pred: Predicted segmentation, typically segmentation model output.
                 It must be a one-hot encoded, batch-first tensor [B,C,H,W].
             y: Reference segmentation.
                 It must be a one-hot encoded, batch-first tensor [B,C,H,W].
+            kwargs: additional parameters, e.g. ``spacing`` should be passed to correctly compute the metric.
+                ``spacing``: spacing of pixel (or voxel). This parameter is relevant only
+                if ``distance_metric`` is set to ``"euclidean"``.
+                If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+                the length of the sequence must be equal to the image dimensions.
+                This spacing will be used for all images in the batch.
+                If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+                If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+                else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+                for all images in batch. Defaults to ``None``.
 
         Returns:
             Pytorch Tensor of shape [B,C], containing the NSD values :math:`\operatorname {NSD}_{b,c}` for each batch
             index :math:`b` and class :math:`c`.
         """
         return compute_surface_dice(
             y_pred=y_pred,
             y=y,
             class_thresholds=self.class_thresholds,
             include_background=self.include_background,
             distance_metric=self.distance_metric,
+            spacing=kwargs.get("spacing"),
         )
 
     def aggregate(
         self, reduction: MetricReduction | str | None = None
     ) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         r"""
         Aggregates the output of `_compute_tensor`.
@@ -113,14 +132,15 @@
 
 def compute_surface_dice(
     y_pred: torch.Tensor,
     y: torch.Tensor,
     class_thresholds: list[float],
     include_background: bool = False,
     distance_metric: str = "euclidean",
+    spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None = None,
 ) -> torch.Tensor:
     r"""
     This function computes the (Normalized) Surface Dice (NSD) between the two tensors `y_pred` (referred to as
     :math:`\hat{Y}`) and `y` (referred to as :math:`Y`). This metric determines which fraction of a segmentation
     boundary is correctly predicted. A boundary element is considered correctly predicted if the closest distance to the
     reference boundary is smaller than or equal to the specified threshold related to the acceptable amount of deviation in
     pixels. The NSD is bounded between 0 and 1.
@@ -163,14 +183,21 @@
             The thresholds relate to the acceptable amount of deviation in the segmentation boundary in pixels.
             Each threshold needs to be a finite, non-negative number.
         include_background: Whether to skip the surface dice computation on the first channel of
             the predicted output. Defaults to ``False``.
         distance_metric: The metric used to compute surface distances.
             One of [``"euclidean"``, ``"chessboard"``, ``"taxicab"``].
             Defaults to ``"euclidean"``.
+        spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
+            If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+            the length of the sequence must be equal to the image dimensions. This spacing will be used for all images in the batch.
+            If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+            If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+            else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+            for all images in batch. Defaults to ``None``.
 
     Raises:
         ValueError: If `y_pred` and/or `y` are not PyTorch tensors.
         ValueError: If `y_pred` and/or `y` do not have four dimensions.
         ValueError: If `y_pred` and/or `y` have different shapes.
         ValueError: If `y_pred` and/or `y` are not one-hot encoded
         ValueError: If the number of channels of `y_pred` and/or `y` is different from the number of class thresholds.
@@ -215,23 +242,30 @@
         raise ValueError("All class thresholds need to be finite.")
 
     if any(np.array(class_thresholds) < 0):
         raise ValueError("All class thresholds need to be >= 0.")
 
     nsd = np.empty((batch_size, n_class))
 
+    img_dim = y_pred.ndim - 2
+    spacing_list = prepare_spacing(spacing=spacing, batch_size=batch_size, img_dim=img_dim)
+
     for b, c in np.ndindex(batch_size, n_class):
         (edges_pred, edges_gt) = get_mask_edges(y_pred[b, c], y[b, c], crop=False)
         if not np.any(edges_gt):
             warnings.warn(f"the ground truth of class {c} is all 0, this may result in nan/inf distance.")
         if not np.any(edges_pred):
             warnings.warn(f"the prediction of class {c} is all 0, this may result in nan/inf distance.")
 
-        distances_pred_gt = get_surface_distance(edges_pred, edges_gt, distance_metric=distance_metric)
-        distances_gt_pred = get_surface_distance(edges_gt, edges_pred, distance_metric=distance_metric)
+        distances_pred_gt = get_surface_distance(
+            edges_pred, edges_gt, distance_metric=distance_metric, spacing=spacing_list[b]
+        )
+        distances_gt_pred = get_surface_distance(
+            edges_gt, edges_pred, distance_metric=distance_metric, spacing=spacing_list[b]
+        )
 
         boundary_complete = len(distances_pred_gt) + len(distances_gt_pred)
         boundary_correct = np.sum(distances_pred_gt <= class_thresholds[c]) + np.sum(
             distances_gt_pred <= class_thresholds[c]
         )
 
         if boundary_complete == 0:
```

## monai/metrics/surface_distance.py

```diff
@@ -8,19 +8,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
+from typing import Any
 
 import numpy as np
 import torch
 
-from monai.metrics.utils import do_metric_reduction, get_mask_edges, get_surface_distance, ignore_background
+from monai.metrics.utils import (
+    do_metric_reduction,
+    get_mask_edges,
+    get_surface_distance,
+    ignore_background,
+    prepare_spacing,
+)
 from monai.utils import MetricReduction, convert_data_type
 
 from .metric import CumulativeIterationMetric
 
 
 class SurfaceDistanceMetric(CumulativeIterationMetric):
     """
@@ -59,35 +67,47 @@
         super().__init__()
         self.include_background = include_background
         self.distance_metric = distance_metric
         self.symmetric = symmetric
         self.reduction = reduction
         self.get_not_nans = get_not_nans
 
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor, **kwargs: Any) -> torch.Tensor:  # type: ignore[override]
         """
         Args:
             y_pred: input data to compute, typical segmentation model output.
                 It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
                 should be binarized.
             y: ground truth to compute the distance. It must be one-hot format and first dim is batch.
                 The values should be binarized.
+            kwargs: additional parameters, e.g. ``spacing`` should be passed to correctly compute the metric.
+                ``spacing``: spacing of pixel (or voxel). This parameter is relevant only
+                if ``distance_metric`` is set to ``"euclidean"``.
+                If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+                the length of the sequence must be equal to the image dimensions.
+                This spacing will be used for all images in the batch.
+                If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+                If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+                else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+                for all images in batch. Defaults to ``None``.
 
         Raises:
             ValueError: when `y_pred` has less than three dimensions.
         """
         if y_pred.dim() < 3:
             raise ValueError("y_pred should have at least three dimensions.")
+
         # compute (BxC) for each channel for each batch
         return compute_average_surface_distance(
             y_pred=y_pred,
             y=y,
             include_background=self.include_background,
             symmetric=self.symmetric,
             distance_metric=self.distance_metric,
+            spacing=kwargs.get("spacing"),
         )
 
     def aggregate(
         self, reduction: MetricReduction | str | None = None
     ) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         """
         Execute reduction logic for the output of `compute_average_surface_distance`.
@@ -109,14 +129,15 @@
 
 def compute_average_surface_distance(
     y_pred: np.ndarray | torch.Tensor,
     y: np.ndarray | torch.Tensor,
     include_background: bool = False,
     symmetric: bool = False,
     distance_metric: str = "euclidean",
+    spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None = None,
 ) -> torch.Tensor:
     """
     This function is used to compute the Average Surface Distance from `y_pred` to `y`
     under the default setting.
     In addition, if sets ``symmetric = True``, the average symmetric surface distance between
     these two inputs will be returned.
     The implementation refers to `DeepMind's implementation <https://github.com/deepmind/surface-distance>`_.
@@ -129,34 +150,48 @@
             The values should be binarized.
         include_background: whether to skip distance computation on the first channel of
             the predicted output. Defaults to ``False``.
         symmetric: whether to calculate the symmetric average surface distance between
             `seg_pred` and `seg_gt`. Defaults to ``False``.
         distance_metric: : [``"euclidean"``, ``"chessboard"``, ``"taxicab"``]
             the metric used to compute surface distance. Defaults to ``"euclidean"``.
+        spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
+            If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+            the length of the sequence must be equal to the image dimensions. This spacing will be used for all images in the batch.
+            If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+            If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+            else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+            for all images in batch. Defaults to ``None``.
     """
 
     if not include_background:
         y_pred, y = ignore_background(y_pred=y_pred, y=y)
 
     y_pred = convert_data_type(y_pred, output_type=torch.Tensor, dtype=torch.float)[0]
     y = convert_data_type(y, output_type=torch.Tensor, dtype=torch.float)[0]
 
     if y.shape != y_pred.shape:
         raise ValueError(f"y_pred and y should have same shapes, got {y_pred.shape} and {y.shape}.")
 
     batch_size, n_class = y_pred.shape[:2]
     asd = np.empty((batch_size, n_class))
 
+    img_dim = y_pred.ndim - 2
+    spacing_list = prepare_spacing(spacing=spacing, batch_size=batch_size, img_dim=img_dim)
+
     for b, c in np.ndindex(batch_size, n_class):
         (edges_pred, edges_gt) = get_mask_edges(y_pred[b, c], y[b, c])
         if not np.any(edges_gt):
             warnings.warn(f"the ground truth of class {c} is all 0, this may result in nan/inf distance.")
         if not np.any(edges_pred):
             warnings.warn(f"the prediction of class {c} is all 0, this may result in nan/inf distance.")
-        surface_distance = get_surface_distance(edges_pred, edges_gt, distance_metric=distance_metric)
+        surface_distance = get_surface_distance(
+            edges_pred, edges_gt, distance_metric=distance_metric, spacing=spacing_list[b]
+        )
         if symmetric:
-            surface_distance_2 = get_surface_distance(edges_gt, edges_pred, distance_metric=distance_metric)
+            surface_distance_2 = get_surface_distance(
+                edges_gt, edges_pred, distance_metric=distance_metric, spacing=spacing_list[b]
+            )
             surface_distance = np.concatenate([surface_distance, surface_distance_2])
         asd[b, c] = np.nan if surface_distance.shape == (0,) else surface_distance.mean()
 
     return convert_data_type(asd, output_type=torch.Tensor, device=y_pred.device, dtype=torch.float)[0]
```

## monai/metrics/utils.py

```diff
@@ -8,14 +8,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
 from typing import Any
 
 import numpy as np
 import torch
 
 from monai.config import NdarrayOrTensor, NdarrayTensor
 from monai.transforms.croppad.array import SpatialCrop
@@ -168,41 +169,53 @@
     # Do binary erosion and use XOR to get edges
     edges_pred = binary_erosion(seg_pred) ^ seg_pred
     edges_gt = binary_erosion(seg_gt) ^ seg_gt
 
     return edges_pred, edges_gt
 
 
-def get_surface_distance(seg_pred: np.ndarray, seg_gt: np.ndarray, distance_metric: str = "euclidean") -> np.ndarray:
+def get_surface_distance(
+    seg_pred: np.ndarray,
+    seg_gt: np.ndarray,
+    distance_metric: str = "euclidean",
+    spacing: int | float | np.ndarray | Sequence[int | float] | None = None,
+) -> np.ndarray:
     """
     This function is used to compute the surface distances from `seg_pred` to `seg_gt`.
 
     Args:
         seg_pred: the edge of the predictions.
         seg_gt: the edge of the ground truth.
         distance_metric: : [``"euclidean"``, ``"chessboard"``, ``"taxicab"``]
             the metric used to compute surface distance. Defaults to ``"euclidean"``.
 
             - ``"euclidean"``, uses Exact Euclidean distance transform.
             - ``"chessboard"``, uses `chessboard` metric in chamfer type of transform.
             - ``"taxicab"``, uses `taxicab` metric in chamfer type of transform.
+        spacing: spacing of pixel (or voxel) along each axis. If a sequence, must be of
+            length equal to the image dimensions; if a single number, this is used for all axes.
+            If ``None``, spacing of unity is used. Defaults to ``None``.
+        spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
+            Several input options are allowed: (1) If a single number, isotropic spacing with that value is used.
+            (2) If a sequence of numbers, the length of the sequence must be equal to the image dimensions.
+            (3) If ``None``, spacing of unity is used. Defaults to ``None``.
 
     Note:
         If seg_pred or seg_gt is all 0, may result in nan/inf distance.
 
     """
 
     if not np.any(seg_gt):
         dis = np.inf * np.ones_like(seg_gt)
     else:
         if not np.any(seg_pred):
             dis = np.inf * np.ones_like(seg_gt)
             return np.asarray(dis[seg_gt])
         if distance_metric == "euclidean":
-            dis = distance_transform_edt(~seg_gt)
+            dis = distance_transform_edt(~seg_gt, sampling=spacing)
         elif distance_metric in {"chessboard", "taxicab"}:
             dis = distance_transform_cdt(~seg_gt, metric=distance_metric)
         else:
             raise ValueError(f"distance_metric {distance_metric} is not implemented.")
 
     return np.asarray(dis[seg_pred])
 
@@ -257,7 +270,67 @@
         pair_list = sorted(pair_data, key=lambda x: x[1], reverse=True)  # type: ignore
         pred_id, _ = zip(*pair_list)
 
     new_pred = torch.zeros_like(pred, dtype=torch.int)
     for idx, instance_id in enumerate(pred_id):
         new_pred[pred == instance_id] = idx + 1
     return new_pred
+
+
+def prepare_spacing(
+    spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None,
+    batch_size: int,
+    img_dim: int,
+) -> Sequence[None | int | float | np.ndarray | Sequence[int | float]]:
+    """
+    This function is used to prepare the `spacing` parameter to include batch dimension for the computation of
+    surface distance, hausdorff distance or surface dice.
+
+    An example with batch_size = 4 and img_dim = 3:
+    input spacing = None -> output spacing = [None, None, None, None]
+    input spacing = 0.8 -> output spacing = [0.8, 0.8, 0.8, 0.8]
+    input spacing = [0.8, 0.5, 0.9] -> output spacing = [[0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9]]
+    input spacing = [0.8, 0.7, 1.2, 0.8] -> output spacing = [0.8, 0.7, 1.2, 0.8] (same as input)
+
+    An example with batch_size = 3 and img_dim = 3:
+    input spacing = [0.8, 0.5, 0.9] -> output spacing = [[0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9]]
+
+    Args:
+        spacing: can be a float, a sequence of length `img_dim`, or a sequence with length `batch_size`
+        that includes floats or sequences of length `img_dim`.
+
+    Raises:
+        AssertionError: when `spacing` is a sequence of sequence, where the outer sequence length does not
+        equal `batch_size` or inner sequence length does not equal `img_dim`.
+
+    Returns:
+        spacing: a sequence with length `batch_size` that includes integers, floats or sequences of length `img_dim`.
+    """
+    if spacing is None or isinstance(spacing, (int, float)):
+        return list([spacing] * batch_size)
+    elif isinstance(spacing, (Sequence, np.ndarray)):
+        assert all(
+            [isinstance(s, type(spacing[0])) for s in list(spacing)]
+        ), "if `spacing` is a sequence, its elements should be of same type."
+
+        if isinstance(spacing[0], (Sequence, np.ndarray)):
+            assert (
+                len(spacing) == batch_size
+            ), "if `spacing` is a sequence of sequences, the outer sequence should have same length as batch size."
+            assert all(
+                [len(s) == img_dim for s in list(spacing)]
+            ), "each element of `spacing` list should either have same length as image dim."
+            assert all(
+                [isinstance(i, (int, float)) for s in list(spacing) for i in list(s)]
+            ), "if `spacing` is a sequence of sequences or 2D np.ndarray, the elements should be integers or floats."
+            return list(spacing)
+        elif isinstance(spacing[0], (int, float)):
+            assert (
+                len(spacing) == img_dim
+            ), "if `spacing` is a sequence of numbers, it should have same length as image dim."
+            return [spacing for _ in range(batch_size)]  # type: ignore
+        else:
+            raise AssertionError(f"`spacing` is a sequence of elements with unsupported type: {type(spacing[0])}")
+    else:
+        raise AssertionError(
+            "`spacing` should either be an integer, float, a sequence of numbers or a sequence of sequences."
+        )
```

## monai/networks/__init__.py

```diff
@@ -8,14 +8,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from .utils import (
+    convert_to_onnx,
     convert_to_torchscript,
     convert_to_trt,
     copy_model_state,
     eval_mode,
     get_state_dict,
     icnr_init,
     look_up_named_module,
```

## monai/networks/utils.py

```diff
@@ -10,14 +10,15 @@
 # limitations under the License.
 """
 Utilities and types for defining networks, these depend on PyTorch.
 """
 
 from __future__ import annotations
 
+import io
 import re
 import warnings
 from collections import OrderedDict
 from collections.abc import Callable, Mapping, Sequence
 from contextlib import contextmanager
 from copy import deepcopy
 from typing import Any
@@ -28,27 +29,32 @@
 
 from monai.apps.utils import get_logger, optional_import
 from monai.config import PathLike
 from monai.utils.misc import ensure_tuple, save_obj, set_determinism
 from monai.utils.module import look_up_option, pytorch_after
 from monai.utils.type_conversion import convert_to_dst_type, convert_to_tensor
 
+onnx, _ = optional_import("onnx")
+onnxreference, _ = optional_import("onnx.reference")
+onnxruntime, _ = optional_import("onnxruntime")
+
 __all__ = [
     "one_hot",
     "predict_segmentation",
     "normalize_transform",
     "to_norm_affine",
     "normal_init",
     "icnr_init",
     "pixelshuffle",
     "eval_mode",
     "train_mode",
     "get_state_dict",
     "copy_model_state",
     "save_state",
+    "convert_to_onnx",
     "convert_to_torchscript",
     "convert_to_trt",
     "meshgrid_ij",
     "meshgrid_xy",
     "replace_modules",
     "replace_modules_temp",
     "look_up_named_module",
@@ -548,14 +554,133 @@
             ckpt[k] = get_state_dict(v)
     else:
         ckpt = get_state_dict(src)
 
     save_obj(obj=ckpt, path=path, **kwargs)
 
 
+def convert_to_onnx(
+    model: nn.Module,
+    inputs: Sequence[Any],
+    input_names: Sequence[str] | None = None,
+    output_names: Sequence[str] | None = None,
+    opset_version: int | None = None,
+    dynamic_axes: Mapping[str, Mapping[int, str]] | Mapping[str, Sequence[int]] | None = None,
+    filename: Any | None = None,
+    verify: bool = False,
+    device: torch.device | None = None,
+    use_ort: bool = False,
+    ort_provider: Sequence[str] | None = None,
+    rtol: float = 1e-4,
+    atol: float = 0.0,
+    use_trace: bool = True,
+    **kwargs,
+):
+    """
+    Utility to convert a model into ONNX model and optionally verify with ONNX or onnxruntime.
+    See also: https://pytorch.org/docs/stable/onnx.html for how to convert a PyTorch model to ONNX.
+
+    Args:
+        model: source PyTorch model to save.
+        inputs: input sample data used by pytorch.onnx.export. It is also used in ONNX model verification.
+        input_names: optional input names of the ONNX model.
+        output_names: optional output names of the ONNX model.
+        opset_version: version of the (ai.onnx) opset to target. Must be >= 7 and not exceed
+        the latest opset version supported by PyTorch, for more details:
+            https://github.com/onnx/onnx/blob/main/docs/Operators.md and
+            https://github.com/pytorch/pytorch/blob/master/torch/onnx/_constants.py
+        dynamic_axes: specifies axes of tensors as dynamic (i.e. known only at run-time). If set to None,
+            the exported model will have the shapes of all input and output tensors set to match given
+            ones, for more details: https://pytorch.org/docs/stable/onnx.html#torch.onnx.export.
+        filename: optional filename to save the ONNX model, if None, don't save the ONNX model.
+        verify: whether to verify the ONNX model with ONNX or onnxruntime.
+        device: target PyTorch device to verify the model, if None, use CUDA if available.
+        use_ort: whether to use onnxruntime to verify the model.
+        ort_provider": onnxruntime provider to use, default is ["CPUExecutionProvider"].
+        rtol: the relative tolerance when comparing the outputs of PyTorch model and TorchScript model.
+        atol: the absolute tolerance when comparing the outputs of PyTorch model and TorchScript model.
+        use_trace: whether to use `torch.jit.trace` to export the torchscript model.
+        kwargs: other arguments except `obj` for `torch.jit.script()` to convert model, for more details:
+            https://pytorch.org/docs/master/generated/torch.jit.script.html.
+
+    """
+    model.eval()
+    with torch.no_grad():
+        torch_versioned_kwargs = {}
+        if use_trace:
+            # let torch.onnx.export to trace the model.
+            mode_to_export = model
+        else:
+            if not pytorch_after(1, 10):
+                if "example_outputs" not in kwargs:
+                    # https://github.com/pytorch/pytorch/blob/release/1.9/torch/onnx/__init__.py#L182
+                    raise TypeError(
+                        "example_outputs is required in scripting mode before PyTorch 1.10."
+                        "Please provide example outputs or use trace mode to export onnx model."
+                    )
+                torch_versioned_kwargs["example_outputs"] = kwargs["example_outputs"]
+                del kwargs["example_outputs"]
+            mode_to_export = torch.jit.script(model, **kwargs)
+
+        if filename is None:
+            f = io.BytesIO()
+            torch.onnx.export(
+                mode_to_export,
+                tuple(inputs),
+                f=f,
+                input_names=input_names,
+                output_names=output_names,
+                dynamic_axes=dynamic_axes,
+                opset_version=opset_version,
+                **torch_versioned_kwargs,
+            )
+            onnx_model = onnx.load_model_from_string(f.getvalue())
+        else:
+            torch.onnx.export(
+                mode_to_export,
+                tuple(inputs),
+                f=filename,
+                input_names=input_names,
+                output_names=output_names,
+                dynamic_axes=dynamic_axes,
+                opset_version=opset_version,
+                **torch_versioned_kwargs,
+            )
+            onnx_model = onnx.load(filename)
+
+    if verify:
+        if device is None:
+            device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+        inputs = [i.to(device) if isinstance(i, torch.Tensor) else i for i in inputs]
+        model = model.to(device)
+
+        with torch.no_grad():
+            set_determinism(seed=0)
+            torch_out = ensure_tuple(model(*inputs), True)
+
+        set_determinism(seed=0)
+        model_input_names = [i.name for i in onnx_model.graph.input]
+        input_dict = dict(zip(model_input_names, [i.cpu().numpy() for i in inputs]))
+        if use_ort:
+            ort_sess = onnxruntime.InferenceSession(
+                onnx_model.SerializeToString(), providers=ort_provider if ort_provider else ["CPUExecutionProvider"]
+            )
+            onnx_out = ort_sess.run(None, input_dict)
+        else:
+            sess = onnxreference.ReferenceEvaluator(onnx_model)
+            onnx_out = sess.run(None, input_dict)
+        set_determinism(seed=None)
+        # compare onnx/ort and PyTorch results
+        for r1, r2 in zip(torch_out, onnx_out):
+            torch.testing.assert_allclose(r1.cpu(), r2, rtol=rtol, atol=atol)
+
+    return onnx_model
+
+
 def convert_to_torchscript(
     model: nn.Module,
     filename_or_obj: Any | None = None,
     extra_files: dict | None = None,
     verify: bool = False,
     inputs: Sequence[Any] | None = None,
     device: torch.device | None = None,
@@ -577,26 +702,25 @@
         verify: whether to verify the input and output of TorchScript model.
             if `filename_or_obj` is not None, load the saved TorchScript model and verify.
         inputs: input test data to verify model, should be a sequence of data, every item maps to a argument
             of `model()` function.
         device: target device to verify the model, if None, use CUDA if available.
         rtol: the relative tolerance when comparing the outputs of PyTorch model and TorchScript model.
         atol: the absolute tolerance when comparing the outputs of PyTorch model and TorchScript model.
-        use_trace: whether to use `torch.jit.trace` to export the torchscript model.
-
-        kwargs: other arguments except `obj` for `torch.jit.script()` to convert model, for more details:
-            https://pytorch.org/docs/master/generated/torch.jit.script.html.
+        use_trace: whether to use `torch.jit.trace` to export the TorchScript model.
+        kwargs: other arguments except `obj` for `torch.jit.script()` or `torch.jit.trace()` (if use_trace is True)
+            to convert model, for more details: https://pytorch.org/docs/master/generated/torch.jit.script.html.
 
     """
     model.eval()
     with torch.no_grad():
         if use_trace:
             if inputs is None:
                 raise ValueError("Missing input data for tracing convert.")
-            script_module = torch.jit.trace(model, example_inputs=inputs)
+            script_module = torch.jit.trace(model, example_inputs=inputs, **kwargs)
         else:
             script_module = torch.jit.script(model, **kwargs)
         if filename_or_obj is not None:
             torch.jit.save(m=script_module, f=filename_or_obj, _extra_files=extra_files)
 
     if verify:
         if device is None:
@@ -620,46 +744,143 @@
             if isinstance(r1, torch.Tensor) or isinstance(r2, torch.Tensor):
                 assert_fn = torch.testing.assert_close if pytorch_after(1, 11) else torch.testing.assert_allclose
                 assert_fn(r1, r2, rtol=rtol, atol=atol)  # type: ignore
 
     return script_module
 
 
+def _onnx_trt_compile(
+    onnx_model,
+    min_shape: Sequence[int],
+    opt_shape: Sequence[int],
+    max_shape: Sequence[int],
+    device: int,
+    precision: str,
+    input_names: Sequence[str] | None,
+    output_names: Sequence[str] | None,
+):
+    """
+    This function takes an ONNX model as input, exports it to a TensorRT engine, wraps the TensorRT engine
+    to a TensorRT engine-based TorchScript model and return the TorchScript model.
+
+    Args:
+        onnx_model: the source ONNX model to compile.
+        min_shape: the minimum input shape of the converted TensorRT model.
+        opt_shape: the optimization input shape of the model, on which the TensorRT optimizes.
+        max_shape: the maximum input shape of the converted TensorRT model.
+        device: the target GPU index to convert and verify the model.
+        precision: the weight precision of the converted TensorRT engine-based TorchScript model.
+            Should be 'fp32' or 'fp16'.
+        input_names: optional input names of the ONNX model. Should be a sequence like
+            `['input_0', 'input_1', ..., 'input_N']` where N equals to the number of the
+            model inputs.
+        output_names: optional output names of the ONNX model. Should be a sequence like
+            `['output_0', 'output_1', ..., 'output_N']` where N equals to the number of
+            the model outputs.
+
+    """
+    trt, _ = optional_import("tensorrt", "8.5.3")
+    torch_tensorrt, _ = optional_import("torch_tensorrt", "1.4.0")
+
+    input_shapes = (min_shape, opt_shape, max_shape)
+    # default to an empty list to fit the `torch_tensorrt.ts.embed_engine_in_new_module` function.
+    input_names = [] if not input_names else input_names
+    output_names = [] if not output_names else output_names
+
+    # set up the TensorRT builder
+    torch_tensorrt.set_device(device)
+    logger = trt.Logger(trt.Logger.WARNING)
+    builder = trt.Builder(logger)
+    network = builder.create_network(1 << int(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH))
+    profile = builder.create_optimization_profile()
+    if input_names:
+        profile.set_shape(input_names[0], *input_shapes)
+
+    # parse the ONNX model
+    parser = trt.OnnxParser(network, logger)
+    success = parser.parse(onnx_model.SerializeToString())
+    if not success:
+        parser_error_message = ""
+        for idx in range(parser.num_errors):
+            parser_error_message += parser.get_error(idx).desc() + "\n"
+        raise Exception(f"TensorRT cannot parse the ONNX model, due to:\n{parser_error_message}")
+
+    # set up the conversion configuration
+    config = builder.create_builder_config()
+    config.set_memory_pool_limit(trt.MemoryPoolType.WORKSPACE, 1 << 31)
+    config.add_optimization_profile(profile)
+    if precision == "fp16":
+        config.set_flag(trt.BuilderFlag.FP16)
+    serialized_engine = builder.build_serialized_network(network, config)
+    f = io.BytesIO()
+    f.write(serialized_engine)
+
+    # wrap the serialized TensorRT engine back to a TorchScript module.
+    trt_model = torch_tensorrt.ts.embed_engine_in_new_module(
+        f.getvalue(), torch.device(f"cuda:{device}"), input_names, output_names
+    )
+    return trt_model
+
+
 def convert_to_trt(
     model: nn.Module,
     precision: str,
     input_shape: Sequence[int],
     dynamic_batchsize: Sequence[int] | None = None,
     use_trace: bool = False,
     filename_or_obj: Any | None = None,
     verify: bool = False,
     device: int | None = None,
+    use_onnx: bool | None = False,
+    onnx_input_names: Sequence[str] | None = ("input_0",),
+    onnx_output_names: Sequence[str] | None = ("output_0",),
     rtol: float = 1e-2,
     atol: float = 0.0,
+    **kwargs,
 ):
     """
-    Utility to convert a model into a TensorRT engine based torchscript model with optional input / output data verification.
+    Utility to export a model into a TensorRT engine-based TorchScript model with optional input / output data verification.
+
+    There are two ways to export a model:
+    1, Torch-TensorRT way: PyTorch module ---> TorchScript module ---> TensorRT engine-based TorchScript.
+    2, ONNX-TensorRT way: PyTorch module ---> TorchScript module ---> ONNX model ---> TensorRT engine --->
+    TensorRT engine-based TorchScript.
+
+    When exporting through the first way, some models suffer from the slowdown problem, since Torch-TensorRT
+    may only convert a little part of the PyTorch model to the TensorRT engine. However when exporting through
+    the second way, some Python data structures like `dict` are not supported. And some TorchScript models are
+    not supported by the ONNX if exported through `torch.jit.script`.
 
     Args:
         model: a source PyTorch model to convert.
-        precision: the weight precision of the converted TensorRT engine based torchscript models. Should be 'fp32' or 'fp16'.
+        precision: the weight precision of the converted TensorRT engine based TorchScript models. Should be 'fp32' or 'fp16'.
         input_shape: the input shape that is used to convert the model. Should be a list like [N, C, H, W] or
             [N, C, H, W, D].
-        dynamic_batchsize: a sequence with three elements to define the batch size range of the input for the model to be converted.
-            Should be a sequence like [MIN_BATCH, OPT_BATCH, MAX_BATCH]. After converted, the batchsize of model input should
-            between `MIN_BATCH` and `MAX_BATCH` and the `OPT_BATCH` is the best peformance batchsize that the TensorRT trys to fit.
-            We suggest the `OPT_BATCH` to be the most frequently used input batchsize in your application, default to None.
-        use_trace: whether using `torch.jit.trace` to convert the pytorch model to torchscript model and then convert to
-            a TensorRT engine based torchscript model, default to False.
+        dynamic_batchsize: a sequence with three elements to define the batch size range of the input for the model to be
+            converted. Should be a sequence like [MIN_BATCH, OPT_BATCH, MAX_BATCH]. After converted, the batchsize of model
+            input should between `MIN_BATCH` and `MAX_BATCH` and the `OPT_BATCH` is the best performance batchsize that the
+            TensorRT tries to fit. The `OPT_BATCH` should be the most frequently used input batchsize in the application,
+            default to None.
+        use_trace: whether using `torch.jit.trace` to convert the PyTorch model to a TorchScript model and then convert to
+            a TensorRT engine based TorchScript model or an ONNX model (if `use_onnx` is True), default to False.
         filename_or_obj: if not None, specify a file-like object (has to implement write and flush) or a string containing a
-            file path name to load the TensorRT engine based torchscript model for verifying.
-        verify: whether to verify the input and output of the TensorRT engine based torchscript model.
+            file path name to load the TensorRT engine based TorchScript model for verifying.
+        verify: whether to verify the input and output of the TensorRT engine based TorchScript model.
         device: the target GPU index to convert and verify the model. If None, use #0 GPU.
+        use_onnx: whether to use the ONNX-TensorRT way to export the TensorRT engine-based TorchScript model.
+        onnx_input_names: optional input names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `('input_0', 'input_1', ..., 'input_N')` where N equals to the number of the model inputs. If not
+            given, will use `('input_0',)`, which supposes the model only has one input.
+        onnx_output_names: optional output names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `('output_0', 'output_1', ..., 'output_N')` where N equals to the number of the model outputs. If
+            not given, will use `('output_0',)`, which supposes the model only has one output.
         rtol: the relative tolerance when comparing the outputs between the PyTorch model and TensorRT model.
         atol: the absolute tolerance when comparing the outputs between the PyTorch model and TensorRT model.
+        kwargs: other arguments except `module`, `inputs`, `enabled_precisions` and `device` for `torch_tensorrt.compile()`
+            to compile model, for more details: https://pytorch.org/TensorRT/py_api/torch_tensorrt.html#torch-tensorrt-py.
     """
 
     torch_tensorrt, _ = optional_import("torch_tensorrt", version="1.4.0")
 
     if not torch.cuda.is_available():
         raise Exception("Cannot find any GPU devices.")
 
@@ -673,42 +894,70 @@
         warnings.warn(f"The dynamic batch range sequence should have 3 elements, but got {dynamic_batchsize} elements.")
 
     device = device if device else 0
     target_device = torch.device(f"cuda:{device}") if device else torch.device("cuda:0")
     convert_precision = torch.float32 if precision == "fp32" else torch.half
     inputs = [torch.rand(ensure_tuple(input_shape)).to(target_device)]
 
-    # convert the torch model, torchscript model and input to target device
-    model = model.eval().to(target_device)
-    ir_model = convert_to_torchscript(model, device=target_device, inputs=inputs, use_trace=use_trace)
-    ir_model.eval().to(target_device)
-
     def scale_batch_size(input_shape: Sequence[int], scale_num: int):
         scale_shape = [*input_shape]
         scale_shape[0] *= scale_num
         return scale_shape
 
-    # Use the dynamic batchsize range to generate compiler input and compile the model
+    # Use the dynamic batchsize range to generate the min, opt and max model input shape
     if dynamic_batchsize:
         min_input_shape = scale_batch_size(input_shape, dynamic_batchsize[0])
         opt_input_shape = scale_batch_size(input_shape, dynamic_batchsize[1])
         max_input_shape = scale_batch_size(input_shape, dynamic_batchsize[2])
     else:
         min_input_shape = opt_input_shape = max_input_shape = input_shape
 
-    with torch.no_grad():
-        with torch.cuda.device(device=device):
-            input_placeholder = [
-                torch_tensorrt.Input(min_shape=min_input_shape, opt_shape=opt_input_shape, max_shape=max_input_shape)
-            ]
-            trt_model = torch_tensorrt.compile(
-                ir_model, inputs=input_placeholder, enabled_precisions=convert_precision, device=target_device
-            )
+    # convert the torch model to a TorchScript model on target device
+    model = model.eval().to(target_device)
+    ir_model = convert_to_torchscript(model, device=target_device, inputs=inputs, use_trace=use_trace)
+    ir_model.eval()
+
+    if use_onnx:
+        # set the batch dim as dynamic
+        dynamic_axes = {k: {0: "batchsize"} for k in onnx_input_names} if onnx_input_names else {}
+        dynamic_axes.update({k: {0: "batchsize"} for k in onnx_output_names} if onnx_output_names else {})
+        ir_model = convert_to_onnx(
+            model, inputs, onnx_input_names, onnx_output_names, use_trace=use_trace, dynamic_axes=dynamic_axes
+        )
+
+        # convert the model through the ONNX-TensorRT way
+        trt_model = _onnx_trt_compile(
+            ir_model,
+            min_shape=min_input_shape,
+            opt_shape=opt_input_shape,
+            max_shape=max_input_shape,
+            device=device,
+            precision=precision,
+            input_names=onnx_input_names,
+            output_names=onnx_output_names,
+        )
+    else:
+        # convert the model through the Torch-TensorRT way
+        ir_model.to(target_device)
+        with torch.no_grad():
+            with torch.cuda.device(device=device):
+                input_placeholder = [
+                    torch_tensorrt.Input(
+                        min_shape=min_input_shape, opt_shape=opt_input_shape, max_shape=max_input_shape
+                    )
+                ]
+                trt_model = torch_tensorrt.compile(
+                    ir_model,
+                    inputs=input_placeholder,
+                    enabled_precisions=convert_precision,
+                    device=target_device,
+                    **kwargs,
+                )
 
-    # verify the outputs between the trt model and torch model
+    # verify the outputs between the TensorRT model and PyTorch model
     if verify:
         if inputs is None:
             raise ValueError("Missing input data for verification.")
 
         trt_model = torch.jit.load(filename_or_obj) if filename_or_obj is not None else trt_model
 
         with torch.no_grad():
```

## monai/networks/blocks/selfattention.py

```diff
@@ -21,21 +21,29 @@
 
 class SABlock(nn.Module):
     """
     A self-attention block, based on: "Dosovitskiy et al.,
     An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale <https://arxiv.org/abs/2010.11929>"
     """
 
-    def __init__(self, hidden_size: int, num_heads: int, dropout_rate: float = 0.0, qkv_bias: bool = False) -> None:
+    def __init__(
+        self,
+        hidden_size: int,
+        num_heads: int,
+        dropout_rate: float = 0.0,
+        qkv_bias: bool = False,
+        save_attn: bool = False,
+    ) -> None:
         """
         Args:
-            hidden_size: dimension of hidden layer.
-            num_heads: number of attention heads.
-            dropout_rate: faction of the input units to drop.
-            qkv_bias: bias term for the qkv linear layer.
+            hidden_size (int): dimension of hidden layer.
+            num_heads (int): number of attention heads.
+            dropout_rate (float, optional): faction of the input units to drop. Defaults to 0.0.
+            qkv_bias (bool, optional): bias term for the qkv linear layer. Defaults to False.
+            save_attn (bool, optional): to make accessible the attention matrix. Defaults to False.
 
         """
 
         super().__init__()
 
         if not (0 <= dropout_rate <= 1):
             raise ValueError("dropout_rate should be between 0 and 1.")
@@ -48,18 +56,25 @@
         self.qkv = nn.Linear(hidden_size, hidden_size * 3, bias=qkv_bias)
         self.input_rearrange = Rearrange("b h (qkv l d) -> qkv b l h d", qkv=3, l=num_heads)
         self.out_rearrange = Rearrange("b h l d -> b l (h d)")
         self.drop_output = nn.Dropout(dropout_rate)
         self.drop_weights = nn.Dropout(dropout_rate)
         self.head_dim = hidden_size // num_heads
         self.scale = self.head_dim**-0.5
+        self.save_attn = save_attn
+        self.att_mat = torch.Tensor()
 
     def forward(self, x):
         output = self.input_rearrange(self.qkv(x))
         q, k, v = output[0], output[1], output[2]
         att_mat = (torch.einsum("blxd,blyd->blxy", q, k) * self.scale).softmax(dim=-1)
+        if self.save_attn:
+            # no gradients and new tensor;
+            # https://pytorch.org/docs/stable/generated/torch.Tensor.detach.html
+            self.att_mat = att_mat.detach()
+
         att_mat = self.drop_weights(att_mat)
         x = torch.einsum("bhxy,bhyd->bhxd", att_mat, v)
         x = self.out_rearrange(x)
         x = self.out_proj(x)
         x = self.drop_output(x)
         return x
```

## monai/networks/blocks/transformerblock.py

```diff
@@ -20,36 +20,43 @@
 class TransformerBlock(nn.Module):
     """
     A transformer block, based on: "Dosovitskiy et al.,
     An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale <https://arxiv.org/abs/2010.11929>"
     """
 
     def __init__(
-        self, hidden_size: int, mlp_dim: int, num_heads: int, dropout_rate: float = 0.0, qkv_bias: bool = False
+        self,
+        hidden_size: int,
+        mlp_dim: int,
+        num_heads: int,
+        dropout_rate: float = 0.0,
+        qkv_bias: bool = False,
+        save_attn: bool = False,
     ) -> None:
         """
         Args:
-            hidden_size: dimension of hidden layer.
-            mlp_dim: dimension of feedforward layer.
-            num_heads: number of attention heads.
-            dropout_rate: faction of the input units to drop.
-            qkv_bias: apply bias term for the qkv linear layer
+            hidden_size (int): dimension of hidden layer.
+            mlp_dim (int): dimension of feedforward layer.
+            num_heads (int): number of attention heads.
+            dropout_rate (float, optional): faction of the input units to drop. Defaults to 0.0.
+            qkv_bias (bool, optional): apply bias term for the qkv linear layer. Defaults to False.
+            save_attn (bool, optional): to make accessible the attention matrix. Defaults to False.
 
         """
 
         super().__init__()
 
         if not (0 <= dropout_rate <= 1):
             raise ValueError("dropout_rate should be between 0 and 1.")
 
         if hidden_size % num_heads != 0:
             raise ValueError("hidden_size should be divisible by num_heads.")
 
         self.mlp = MLPBlock(hidden_size, mlp_dim, dropout_rate)
         self.norm1 = nn.LayerNorm(hidden_size)
-        self.attn = SABlock(hidden_size, num_heads, dropout_rate, qkv_bias)
+        self.attn = SABlock(hidden_size, num_heads, dropout_rate, qkv_bias, save_attn)
         self.norm2 = nn.LayerNorm(hidden_size)
 
     def forward(self, x):
         x = x + self.attn(self.norm1(x))
         x = x + self.mlp(self.norm2(x))
         return x
```

## monai/networks/layers/factories.py

```diff
@@ -61,15 +61,14 @@
 
 from __future__ import annotations
 
 import warnings
 from collections.abc import Callable
 from typing import Any
 
-import torch
 import torch.nn as nn
 
 from monai.utils import look_up_option, optional_import
 
 InstanceNorm3dNVFuser, has_nvfuser = optional_import("apex.normalization", name="InstanceNorm3dNVFuser")
 
 __all__ = ["LayerFactory", "Dropout", "Norm", "Act", "Conv", "Pool", "Pad", "split_args"]
@@ -258,30 +257,21 @@
     This layer is based on a customized autograd function, which is not supported in TorchScript currently.
     Please switch to use `nn.InstanceNorm3d` if TorchScript is necessary.
 
     Please check the following link for more details about how to install `apex`:
     https://github.com/NVIDIA/apex#installation
 
     """
-    types = (nn.InstanceNorm1d, nn.InstanceNorm2d)
+
     if dim != 3:
+        types = (nn.InstanceNorm1d, nn.InstanceNorm2d)
         warnings.warn(f"`InstanceNorm3dNVFuser` only supports 3d cases, use {types[dim - 1]} instead.")
         return types[dim - 1]
-    # test InstanceNorm3dNVFuser installation with a basic example
-    has_nvfuser_flag = has_nvfuser
-    if not torch.cuda.is_available():
-        return nn.InstanceNorm3d
-    try:
-        layer = InstanceNorm3dNVFuser(num_features=1, affine=True).to("cuda:0")
-        inp = torch.randn([1, 1, 1, 1, 1]).to("cuda:0")
-        out = layer(inp)
-        del inp, out, layer
-    except Exception:
-        has_nvfuser_flag = False
-    if not has_nvfuser_flag:
+
+    if not has_nvfuser:
         warnings.warn(
             "`apex.normalization.InstanceNorm3dNVFuser` is not installed properly, use nn.InstanceNorm3d instead."
         )
         return nn.InstanceNorm3d
     return InstanceNorm3dNVFuser
```

## monai/networks/nets/hovernet.py

```diff
@@ -439,14 +439,16 @@
             and determining if suitable for the intended use. please check the following link for more details:
             https://github.com/vqdang/hover_net#data-format
             2. standard resnet50 weights of torchvision. Please check the following link for more details:
             https://pytorch.org/vision/main/_modules/torchvision/models/resnet.html#ResNet50_Weights
         adapt_standard_resnet: if the pretrained weights of the encoder follow the original format (preact-resnet50), this
             value should be `False`. If using the pretrained weights that follow torchvision's standard resnet50 format,
             this value should be `True`.
+        pretrained_state_dict_key: this arg is used when `pretrained_url` is provided and `adapt_standard_resnet` is True.
+            It is used to extract the expected state dict.
         freeze_encoder: whether to freeze the encoder of the network.
     """
 
     Mode = HoVerNetMode
     Branch = HoVerNetBranch
 
     def __init__(
@@ -457,14 +459,15 @@
         out_classes: int = 0,
         act: str | tuple = ("relu", {"inplace": True}),
         norm: str | tuple = "batch",
         decoder_padding: bool = False,
         dropout_prob: float = 0.0,
         pretrained_url: str | None = None,
         adapt_standard_resnet: bool = False,
+        pretrained_state_dict_key: str | None = None,
         freeze_encoder: bool = False,
     ) -> None:
         super().__init__()
 
         if isinstance(mode, str):
             mode = mode.upper()
         self.mode = look_up_option(mode, HoVerNetMode)
@@ -562,15 +565,15 @@
                 nn.init.kaiming_normal_(torch.as_tensor(m.weight))
             elif isinstance(m, nn.BatchNorm2d):
                 nn.init.constant_(torch.as_tensor(m.weight), 1)
                 nn.init.constant_(torch.as_tensor(m.bias), 0)
 
         if pretrained_url is not None:
             if adapt_standard_resnet:
-                weights = _remap_standard_resnet_model(pretrained_url)
+                weights = _remap_standard_resnet_model(pretrained_url, state_dict_key=pretrained_state_dict_key)
             else:
                 weights = _remap_preact_resnet_model(pretrained_url)
             _load_pretrained_encoder(self, weights)
 
     def forward(self, x: torch.Tensor) -> dict[str, torch.Tensor]:
         if self.mode == HoVerNetMode.ORIGINAL.value:
             if x.shape[-1] != 270 or x.shape[-2] != 270:
@@ -605,25 +608,33 @@
     model_dict = model.state_dict()
     state_dict = {
         k: v for k, v in state_dict.items() if (k in model_dict) and (model_dict[k].shape == state_dict[k].shape)
     }
 
     model_dict.update(state_dict)
     model.load_state_dict(model_dict)
+    if len(state_dict.keys()) == 0:
+        warnings.warn(
+            "no key will be updated. Please check if 'pretrained_url' or `pretrained_state_dict_key` is correct."
+        )
+    else:
+        print(f"{len(state_dict)} out of {len(model_dict)} keys are updated with pretrained weights.")
 
 
 def _remap_preact_resnet_model(model_url: str):
     pattern_conv0 = re.compile(r"^(conv0\.\/)(.+)$")
     pattern_block = re.compile(r"^(d\d+)\.(.+)$")
     pattern_layer = re.compile(r"^(.+\.d\d+)\.units\.(\d+)(.+)$")
     pattern_bna = re.compile(r"^(.+\.d\d+)\.blk_bna\.(.+)")
     # download the pretrained weights into torch hub's default dir
     weights_dir = os.path.join(torch.hub.get_dir(), "preact-resnet50.pth")
     download_url(model_url, fuzzy=True, filepath=weights_dir, progress=False)
-    state_dict = torch.load(weights_dir, map_location=None)["desc"]
+    state_dict = torch.load(weights_dir, map_location=None if torch.cuda.is_available() else torch.device("cpu"))[
+        "desc"
+    ]
     for key in list(state_dict.keys()):
         new_key = None
         if pattern_conv0.match(key):
             new_key = re.sub(pattern_conv0, r"conv0.conv\2", key)
         elif pattern_block.match(key):
             new_key = re.sub(pattern_block, r"res_blocks.\1.\2", key)
             if pattern_layer.match(new_key):
@@ -635,28 +646,30 @@
             del state_dict[key]
         if "upsample2x" in key:
             del state_dict[key]
 
     return state_dict
 
 
-def _remap_standard_resnet_model(model_url: str):
+def _remap_standard_resnet_model(model_url: str, state_dict_key: str | None = None):
     pattern_conv0 = re.compile(r"^conv1\.(.+)$")
     pattern_bn1 = re.compile(r"^bn1\.(.+)$")
     pattern_block = re.compile(r"^layer(\d+)\.(\d+)\.(.+)$")
     # bn3 to next denselayer's preact/bn
     pattern_block_bn3 = re.compile(r"^(res_blocks.d\d+\.layers\.denselayer_)(\d+)\.layers\.bn3\.(.+)$")
     # bn1, bn2 to conv1/bn, conv2/bn
     pattern_block_bn = re.compile(r"^(res_blocks.d\d+\.layers\.denselayer_\d+\.layers)\.bn(\d+)\.(.+)$")
     pattern_downsample0 = re.compile(r"^(res_blocks.d\d+).+\.downsample\.0\.(.+)")
     pattern_downsample1 = re.compile(r"^(res_blocks.d\d+).+\.downsample\.1\.(.+)")
     # download the pretrained weights into torch hub's default dir
     weights_dir = os.path.join(torch.hub.get_dir(), "resnet50.pth")
     download_url(model_url, fuzzy=True, filepath=weights_dir, progress=False)
-    state_dict = torch.load(weights_dir, map_location=None)
+    state_dict = torch.load(weights_dir, map_location=None if torch.cuda.is_available() else torch.device("cpu"))
+    if state_dict_key is not None:
+        state_dict = state_dict[state_dict_key]
 
     for key in list(state_dict.keys()):
         new_key = None
         if pattern_conv0.match(key):
             new_key = re.sub(pattern_conv0, r"conv0.conv.\1", key)
         elif pattern_bn1.match(key):
             new_key = re.sub(pattern_bn1, r"conv0.bn.\1", key)
```

## monai/networks/nets/vit.py

```diff
@@ -42,32 +42,35 @@
         pos_embed: str = "conv",
         classification: bool = False,
         num_classes: int = 2,
         dropout_rate: float = 0.0,
         spatial_dims: int = 3,
         post_activation="Tanh",
         qkv_bias: bool = False,
+        save_attn: bool = False,
     ) -> None:
         """
         Args:
-            in_channels: dimension of input channels.
-            img_size: dimension of input image.
-            patch_size: dimension of patch size.
-            hidden_size: dimension of hidden layer.
-            mlp_dim: dimension of feedforward layer.
-            num_layers: number of transformer blocks.
-            num_heads: number of attention heads.
-            pos_embed: position embedding layer type.
-            classification: bool argument to determine if classification is used.
-            num_classes: number of classes if classification is used.
-            dropout_rate: faction of the input units to drop.
-            spatial_dims: number of spatial dimensions.
-            post_activation: add a final acivation function to the classification head when `classification` is True.
-                Default to "Tanh" for `nn.Tanh()`. Set to other values to remove this function.
-            qkv_bias: apply bias to the qkv linear layer in self attention block
+            in_channels (int): dimension of input channels.
+            img_size (Union[Sequence[int], int]): dimension of input image.
+            patch_size (Union[Sequence[int], int]): dimension of patch size.
+            hidden_size (int, optional): dimension of hidden layer. Defaults to 768.
+            mlp_dim (int, optional): dimension of feedforward layer. Defaults to 3072.
+            num_layers (int, optional): number of transformer blocks. Defaults to 12.
+            num_heads (int, optional): number of attention heads. Defaults to 12.
+            pos_embed (str, optional): position embedding layer type. Defaults to "conv".
+            classification (bool, optional): bool argument to determine if classification is used. Defaults to False.
+            num_classes (int, optional): number of classes if classification is used. Defaults to 2.
+            dropout_rate (float, optional): faction of the input units to drop. Defaults to 0.0.
+            spatial_dims (int, optional): number of spatial dimensions. Defaults to 3.
+            post_activation (str, optional): add a final acivation function to the classification head
+                when `classification` is True. Default to "Tanh" for `nn.Tanh()`.
+                Set to other values to remove this function.
+            qkv_bias (bool, optional): apply bias to the qkv linear layer in self attention block. Defaults to False.
+            save_attn (bool, optional): to make accessible the attention in self attention block. Defaults to False.
 
         Examples::
 
             # for single channel input with image size of (96,96,96), conv position embedding and segmentation backbone
             >>> net = ViT(in_channels=1, img_size=(96,96,96), pos_embed='conv')
 
             # for 3-channel with image size of (128,128,128), 24 layers and classification backbone
@@ -94,15 +97,18 @@
             hidden_size=hidden_size,
             num_heads=num_heads,
             pos_embed=pos_embed,
             dropout_rate=dropout_rate,
             spatial_dims=spatial_dims,
         )
         self.blocks = nn.ModuleList(
-            [TransformerBlock(hidden_size, mlp_dim, num_heads, dropout_rate, qkv_bias) for i in range(num_layers)]
+            [
+                TransformerBlock(hidden_size, mlp_dim, num_heads, dropout_rate, qkv_bias, save_attn)
+                for i in range(num_layers)
+            ]
         )
         self.norm = nn.LayerNorm(hidden_size)
         if self.classification:
             self.cls_token = nn.Parameter(torch.zeros(1, 1, hidden_size))
             if post_activation == "Tanh":
                 self.classification_head = nn.Sequential(nn.Linear(hidden_size, num_classes), nn.Tanh())
             else:
```

## monai/transforms/compose.py

```diff
@@ -457,15 +457,15 @@
             unpack_items=self.unpack_items,
             lazy_evaluation=self.lazy_evaluation,  # type: ignore
             overrides=self.overrides,
             override_keys=self.override_keys,
             threading=threading,
             log_stats=self.log_stats,
             verbose=self.verbose,
-        )  # type: ignore
+        )
 
     def inverse(self, data):
         invertible_transforms = [t for t in self.flatten().transforms if isinstance(t, InvertibleTransform)]
         if not invertible_transforms:
             warnings.warn("inverse has been called but no invertible transforms have been supplied")
 
         # loop backwards over transforms
```

## monai/transforms/utils.py

```diff
@@ -314,15 +314,15 @@
     # Prepare fg/bg indices
     if label.shape[0] > 1:
         label = label[1:]  # for One-Hot format data, remove the background channel
     label_flat = ravel(any_np_pt(label, 0))  # in case label has multiple dimensions
     fg_indices = nonzero(label_flat)
     if image is not None:
         img_flat = ravel(any_np_pt(image > image_threshold, 0))
-        img_flat, *_ = convert_to_dst_type(img_flat, label, dtype=img_flat.dtype)
+        img_flat, *_ = convert_to_dst_type(img_flat, label, dtype=bool)
         bg_indices = nonzero(img_flat & ~label_flat)
     else:
         bg_indices = nonzero(~label_flat)
 
     # no need to save the indices in GPU, otherwise, still need to move to CPU at runtime when crop by indices
     fg_indices, *_ = convert_data_type(fg_indices, device=torch.device("cpu"))
     bg_indices, *_ = convert_data_type(bg_indices, device=torch.device("cpu"))
@@ -330,14 +330,15 @@
 
 
 def map_classes_to_indices(
     label: NdarrayOrTensor,
     num_classes: int | None = None,
     image: NdarrayOrTensor | None = None,
     image_threshold: float = 0.0,
+    max_samples_per_class: int | None = None,
 ) -> list[NdarrayOrTensor]:
     """
     Filter out indices of every class of the input label data, return the indices after fattening.
     It can handle both One-Hot format label and Argmax format label, must provide `num_classes` for
     Argmax label.
 
     For example:
@@ -348,36 +349,46 @@
     Args:
         label: use the label data to get the indices of every class.
         num_classes: number of classes for argmax label, not necessary for One-Hot label.
         image: if image is not None, only return the indices of every class that are within the valid
             region of the image (``image > image_threshold``).
         image_threshold: if enabled `image`, use ``image > image_threshold`` to
             determine the valid image content area and select class indices only in this area.
+        max_samples_per_class: maximum length of indices in each class to reduce memory consumption.
+            Default is None, no subsampling.
 
     """
     img_flat: NdarrayOrTensor | None = None
     if image is not None:
         img_flat = ravel((image > image_threshold).any(0))
 
-    indices: list[NdarrayOrTensor] = []
     # assuming the first dimension is channel
     channels = len(label)
 
     num_classes_: int = channels
     if channels == 1:
         if num_classes is None:
-            raise ValueError("if not One-Hot format label, must provide the num_classes.")
+            raise ValueError("channels==1 indicates not using One-Hot format label, must provide ``num_classes``.")
         num_classes_ = num_classes
 
+    indices: list[NdarrayOrTensor] = []
     for c in range(num_classes_):
-        label_flat = ravel(any_np_pt(label[c : c + 1] if channels > 1 else label == c, 0))
-        label_flat = img_flat & label_flat if img_flat is not None else label_flat
+        if channels > 1:
+            label_flat = ravel(convert_data_type(label[c], dtype=bool)[0])
+        else:
+            label_flat = ravel(label == c)
+        if img_flat is not None:
+            label_flat = img_flat & label_flat
         # no need to save the indices in GPU, otherwise, still need to move to CPU at runtime when crop by indices
         cls_indices: NdarrayOrTensor = convert_data_type(nonzero(label_flat), device=torch.device("cpu"))[0]
-        indices.append(cls_indices)
+        if max_samples_per_class and len(cls_indices) > max_samples_per_class and len(cls_indices) > 1:
+            sample_id = np.round(np.linspace(0, len(cls_indices) - 1, max_samples_per_class)).astype(int)
+            indices.append(cls_indices[sample_id])
+        else:
+            indices.append(cls_indices)
 
     return indices
 
 
 def weighted_patch_samples(
     spatial_size: int | Sequence[int],
     w: NdarrayOrTensor,
```

## monai/transforms/croppad/array.py

```diff
@@ -1149,14 +1149,16 @@
             `image_threshold`, and randomly select crop centers based on them, expect to be 1 dim array
             of spatial indices after flattening. a typical usage is to call `ClassesToIndices` transform first
             and cache the results for better performance.
         allow_smaller: if `False`, an exception will be raised if the image is smaller than
             the requested ROI in any dimension. If `True`, any smaller dimensions will remain
             unchanged.
         warn: if `True` prints a warning if a class is not present in the label.
+        max_samples_per_class: maximum length of indices to sample in each class to reduce memory consumption.
+            Default is None, no subsampling.
 
     """
 
     backend = SpatialCrop.backend
 
     def __init__(
         self,
@@ -1166,26 +1168,28 @@
         num_classes: int | None = None,
         num_samples: int = 1,
         image: torch.Tensor | None = None,
         image_threshold: float = 0.0,
         indices: list[NdarrayOrTensor] | None = None,
         allow_smaller: bool = False,
         warn: bool = True,
+        max_samples_per_class: int | None = None,
     ) -> None:
         self.spatial_size = spatial_size
         self.ratios = ratios
         self.label = label
         self.num_classes = num_classes
         self.num_samples = num_samples
         self.image = image
         self.image_threshold = image_threshold
         self.centers: tuple[tuple] | None = None
         self.indices = indices
         self.allow_smaller = allow_smaller
         self.warn = warn
+        self.max_samples_per_class = max_samples_per_class
 
     def randomize(
         self,
         label: torch.Tensor | None = None,
         indices: list[NdarrayOrTensor] | None = None,
         image: torch.Tensor | None = None,
     ) -> None:
@@ -1193,15 +1197,17 @@
         if indices_ is None:
             if isinstance(label, MetaTensor) and label.pending_operations:
                 warnings.warn("label has pending operations, the fg/bg indices may be incorrect.")
             if isinstance(image, MetaTensor) and image.pending_operations:
                 warnings.warn("image has pending operations, the fg/bg indices may be incorrect.")
             if label is None:
                 raise ValueError("label must not be None.")
-            indices_ = map_classes_to_indices(label, self.num_classes, image, self.image_threshold)
+            indices_ = map_classes_to_indices(
+                label, self.num_classes, image, self.image_threshold, self.max_samples_per_class
+            )
         _shape = None
         if label is not None:
             _shape = label.peek_pending_shape() if isinstance(label, MetaTensor) else label.shape[1:]
         elif image is not None:
             _shape = image.peek_pending_shape() if isinstance(image, MetaTensor) else image.shape[1:]
         if _shape is None:
             raise ValueError("label or image must be provided to infer the output spatial shape.")
```

## monai/transforms/croppad/dictionary.py

```diff
@@ -958,15 +958,16 @@
             of spatial indices after flattening. a typical usage is to call `ClassesToIndices` transform first
             and cache the results for better performance.
         allow_smaller: if `False`, an exception will be raised if the image is smaller than
             the requested ROI in any dimension. If `True`, any smaller dimensions will remain
             unchanged.
         allow_missing_keys: don't raise exception if key is missing.
         warn: if `True` prints a warning if a class is not present in the label.
-
+        max_samples_per_class: maximum length of indices in each class to reduce memory consumption.
+            Default is None, no subsampling.
 
     """
 
     backend = RandCropByLabelClasses.backend
 
     def __init__(
         self,
@@ -978,27 +979,29 @@
         num_samples: int = 1,
         image_key: str | None = None,
         image_threshold: float = 0.0,
         indices_key: str | None = None,
         allow_smaller: bool = False,
         allow_missing_keys: bool = False,
         warn: bool = True,
+        max_samples_per_class: int | None = None,
     ) -> None:
         MapTransform.__init__(self, keys, allow_missing_keys)
         self.label_key = label_key
         self.image_key = image_key
         self.indices_key = indices_key
         self.cropper = RandCropByLabelClasses(
             spatial_size=spatial_size,
             ratios=ratios,
             num_classes=num_classes,
             num_samples=num_samples,
             image_threshold=image_threshold,
             allow_smaller=allow_smaller,
             warn=warn,
+            max_samples_per_class=max_samples_per_class,
         )
 
     def set_random_state(
         self, seed: int | None = None, state: np.random.RandomState | None = None
     ) -> RandCropByLabelClassesd:
         super().set_random_state(seed, state)
         self.cropper.set_random_state(seed, state)
```

## monai/transforms/lazy/utils.py

```diff
@@ -154,15 +154,15 @@
         matrix: affine transformation matrix.
         kwargs: currently supports (see also: ``monai.utils.enums.LazyAttr``)
 
             - "lazy_shape" for output spatial shape
             - "lazy_padding_mode"
             - "lazy_interpolation_mode" (this option might be ignored when ``mode="auto"``.)
             - "lazy_align_corners"
-            - "lazy_dtype"
+            - "lazy_dtype" (dtype for resampling computation; this might be ignored when ``mode="auto"``.)
             - "atol" for tolerance for matrix floating point comparison.
             - "lazy_resample_mode" for resampling backend, default to `"auto"`. Setting to other values will use the
               `monai.transforms.SpatialResample` for resampling.
 
     See Also:
         :py:class:`monai.transforms.SpatialResample`
     """
@@ -214,14 +214,15 @@
             allclose(matrix_np, np.eye(len(matrix_np)), atol=atol)
             and len(in_shape) == len(out_spatial_size)
             and allclose(convert_to_numpy(in_shape, wrap_sequence=True), out_spatial_size)
         ):
             img.affine = call_kwargs["dst_affine"]
             return img
         img = monai.transforms.crop_or_pad_nd(img, matrix_np, out_spatial_size, mode=call_kwargs["padding_mode"])
+        img = img.to(torch.float32)  # consistent with monai.transforms.spatial.functional.spatial_resample
         img.affine = call_kwargs["dst_affine"]
         return img
 
     resampler = monai.transforms.SpatialResample(**init_kwargs)
     resampler.lazy_evaluation = False  # resampler is a lazytransform
     with resampler.trace_transform(False):  # don't track this transform in `img`
         return resampler(img=img, **call_kwargs)
```

## monai/transforms/spatial/array.py

```diff
@@ -226,14 +226,15 @@
         kw_args["dst_affine"] = kw_args.pop("src_affine")
         kw_args["spatial_size"] = transform[TraceKeys.ORIG_SIZE]
         if kw_args.get("align_corners") == TraceKeys.NONE:
             kw_args["align_corners"] = False
         with self.trace_transform(False):
             # we can't use `self.__call__` in case a child class calls this inverse.
             out: torch.Tensor = SpatialResample.__call__(self, data, **kw_args)
+        kw_args["src_affine"] = kw_args.get("dst_affine")
         return out
 
 
 class ResampleToMatch(SpatialResample):
     """Resample an image to match given metadata. The affine matrix will be aligned,
     and the size of the output image will match."""
 
@@ -3056,15 +3057,15 @@
 
         Returns:
             tuple[NdarrayOrTensor, numpy.ndarray]:  tuple of filtered patches and locations.
         """
         n_dims = len(image_np.shape)
         idx = argwhere(image_np.sum(tuple(range(1, n_dims))) < self.threshold).reshape(-1)
         idx_np = convert_data_type(idx, np.ndarray)[0]
-        return image_np[idx], locations[idx_np]  # type: ignore
+        return image_np[idx], locations[idx_np]
 
     def filter_count(self, image_np: NdarrayOrTensor, locations: np.ndarray) -> tuple[NdarrayOrTensor, np.ndarray]:
         """
         Sort the patches based on the sum of their intensity, and just keep `self.num_patches` of them.
 
         Args:
             image_np: a numpy.ndarray or torch.Tensor representing a stack of patches.
@@ -3079,15 +3080,15 @@
                 idx = argsort(image_np.sum(tuple(range(1, n_dims))))
             elif self.sort_fn == GridPatchSort.MAX:
                 idx = argsort(-image_np.sum(tuple(range(1, n_dims))))
             else:
                 raise ValueError(f'`sort_fn` should be either "min", "max" or None! {self.sort_fn} provided!')
             idx = idx[: self.num_patches]
             idx_np = convert_data_type(idx, np.ndarray)[0]
-            image_np = image_np[idx]  # type: ignore
+            image_np = image_np[idx]
             locations = locations[idx_np]
         return image_np, locations
 
     def __call__(self, array: NdarrayOrTensor) -> MetaTensor:
         """
         Extract the patches (sweeping the entire image in a row-major sliding-window manner with possible overlaps).
```

## monai/transforms/utility/array.py

```diff
@@ -1017,33 +1017,40 @@
         return fg_indices, bg_indices
 
 
 class ClassesToIndices(Transform, MultiSampleTrait):
     backend = [TransformBackends.NUMPY, TransformBackends.TORCH]
 
     def __init__(
-        self, num_classes: int | None = None, image_threshold: float = 0.0, output_shape: Sequence[int] | None = None
+        self,
+        num_classes: int | None = None,
+        image_threshold: float = 0.0,
+        output_shape: Sequence[int] | None = None,
+        max_samples_per_class: int | None = None,
     ) -> None:
         """
         Compute indices of every class of the input label data, return a list of indices.
         If no output_shape specified, output data will be 1 dim indices after flattening.
         This transform can help pre-compute indices of the class regions for other transforms.
         A typical usage is to randomly select indices of classes to crop.
         The main logic is based on :py:class:`monai.transforms.utils.map_classes_to_indices`.
 
         Args:
             num_classes: number of classes for argmax label, not necessary for One-Hot label.
             image_threshold: if enabled `image` at runtime, use ``image > image_threshold`` to
                 determine the valid image content area and select only the indices of classes in this area.
             output_shape: expected shape of output indices. if not None, unravel indices to specified shape.
+            max_samples_per_class: maximum length of indices to sample in each class to reduce memory consumption.
+                Default is None, no subsampling.
 
         """
         self.num_classes = num_classes
         self.image_threshold = image_threshold
         self.output_shape = output_shape
+        self.max_samples_per_class = max_samples_per_class
 
     def __call__(
         self, label: NdarrayOrTensor, image: NdarrayOrTensor | None = None, output_shape: Sequence[int] | None = None
     ) -> list[NdarrayOrTensor]:
         """
         Args:
             label: input data to compute the indices of every class.
@@ -1052,15 +1059,17 @@
             output_shape: expected shape of output indices. if None, use `self.output_shape` instead.
 
         """
 
         if output_shape is None:
             output_shape = self.output_shape
         indices: list[NdarrayOrTensor]
-        indices = map_classes_to_indices(label, self.num_classes, image, self.image_threshold)
+        indices = map_classes_to_indices(
+            label, self.num_classes, image, self.image_threshold, self.max_samples_per_class
+        )
         if output_shape is not None:
             indices = [unravel_indices(cls_indices, output_shape) for cls_indices in indices]
 
         return indices
 
 
 class ConvertToMultiChannelBasedOnBratsClasses(Transform):
```

## monai/transforms/utility/dictionary.py

```diff
@@ -1302,34 +1302,37 @@
             for example, if computed on `label` and `postfix = "_cls_indices"`, the key will be `label_cls_indices`.
         num_classes: number of classes for argmax label, not necessary for One-Hot label.
         image_key: if image_key is not None, use ``image > image_threshold`` to define valid region, and only select
             the indices within the valid region.
         image_threshold: if enabled image_key, use ``image > image_threshold`` to determine the valid image content
             area and select only the indices of classes in this area.
         output_shape: expected shape of output indices. if not None, unravel indices to specified shape.
+        max_samples_per_class: maximum length of indices to sample in each class to reduce memory consumption.
+            Default is None, no subsampling.
         allow_missing_keys: don't raise exception if key is missing.
 
     """
 
     backend = ClassesToIndices.backend
 
     def __init__(
         self,
         keys: KeysCollection,
         indices_postfix: str = "_cls_indices",
         num_classes: int | None = None,
         image_key: str | None = None,
         image_threshold: float = 0.0,
         output_shape: Sequence[int] | None = None,
+        max_samples_per_class: int | None = None,
         allow_missing_keys: bool = False,
     ) -> None:
         super().__init__(keys, allow_missing_keys)
         self.indices_postfix = indices_postfix
         self.image_key = image_key
-        self.converter = ClassesToIndices(num_classes, image_threshold, output_shape)
+        self.converter = ClassesToIndices(num_classes, image_threshold, output_shape, max_samples_per_class)
 
     def __call__(self, data: Mapping[Hashable, Any]):
         d = dict(data)
         image = d[self.image_key] if self.image_key else None
         for key in self.key_iterator(d):
             d[str(key) + self.indices_postfix] = self.converter(d[key], image)
```

## monai/utils/enums.py

```diff
@@ -10,14 +10,16 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import random
 from enum import Enum
 
+from monai.utils import deprecated
+
 __all__ = [
     "StrEnum",
     "NumpyPadMode",
     "GridSampleMode",
     "SplineMode",
     "InterpolateMode",
     "UpsampleMode",
@@ -52,14 +54,15 @@
     "LabelStatsKeys",
     "AlgoEnsembleKeys",
     "HoVerNetMode",
     "HoVerNetBranch",
     "LazyAttr",
     "BundleProperty",
     "BundlePropertyConfig",
+    "AlgoKeys",
 ]
 
 
 class StrEnum(str, Enum):
     """
     Enum subclass that converts its value to a string.
 
@@ -588,14 +591,15 @@
     PIXEL_PCT = "foreground_percentage"
     IMAGE_INTST = "image_intensity"
     LABEL = "label"
     LABEL_SHAPE = "shape"
     LABEL_NCOMP = "ncomponents"
 
 
+@deprecated(since="1.2", msg_suffix="please use `AlgoKeys` instead.")
 class AlgoEnsembleKeys(StrEnum):
     """
     Default keys for Mixed Ensemble
     """
 
     ID = "identifier"
     ALGO = "infer_algo"
@@ -660,7 +664,22 @@
     `ID` is the config item ID of the property.
     `REF_ID` is the ID of config item which is supposed to refer to this property.
     this field is only useful to check the optional property ID.
     """
 
     ID = "id"
     REF_ID = "refer_id"
+
+
+class AlgoKeys(StrEnum):
+    """
+    Default keys for templated Auto3DSeg Algo.
+    `ID` is the identifier of the algorithm. The string has the format of <name>_<idx>_<other>.
+    `ALGO` is the Auto3DSeg Algo instance.
+    `IS_TRAINED` is the status that shows if the Algo has been trained.
+    `SCORE` is the score the Algo has achieved after training.
+    """
+
+    ID = "identifier"
+    ALGO = "algo_instance"
+    IS_TRAINED = "is_trained"
+    SCORE = "best_metric"
```

## monai/utils/misc.py

```diff
@@ -19,14 +19,15 @@
 import shutil
 import tempfile
 import types
 import warnings
 from ast import literal_eval
 from collections.abc import Callable, Iterable, Sequence
 from distutils.util import strtobool
+from math import log10
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, TypeVar, cast, overload
 
 import numpy as np
 import torch
 
 from monai.config.type_definitions import NdarrayOrTensor, NdarrayTensor, PathLike
@@ -64,14 +65,17 @@
     "has_option",
     "sample_slices",
     "check_parent_dir",
     "save_obj",
     "label_union",
     "path_to_uri",
     "pprint_edges",
+    "check_key_duplicates",
+    "CheckKeyDuplicatesYamlLoader",
+    "ConvertUnits",
 ]
 
 _seed = None
 _flag_deterministic = torch.backends.cudnn.deterministic
 _flag_cudnn_benchmark = torch.backends.cudnn.benchmark
 NP_MAX = np.iinfo(np.uint32).max
 MAX_SEED = NP_MAX + 1  # 2**32, the actual seed should be in [0, MAX_SEED - 1] for uint32
@@ -719,7 +723,80 @@
             if key in mapping:
                 if os.environ.get("MONAI_FAIL_ON_DUPLICATE_CONFIG", "0") == "1":
                     raise ValueError(f"Duplicate key: `{key}`")
                 else:
                     warnings.warn(f"Duplicate key: `{key}`")
             mapping.add(key)
         return super().construct_mapping(node, deep)
+
+
+class ConvertUnits:
+    """
+    Convert the values from input unit to the target unit
+
+    Args:
+        input_unit: the unit of the input quantity
+        target_unit: the unit of the target quantity
+
+    """
+
+    imperial_unit_of_length = {"inch": 0.0254, "foot": 0.3048, "yard": 0.9144, "mile": 1609.344}
+
+    unit_prefix = {
+        "peta": 15,
+        "tera": 12,
+        "giga": 9,
+        "mega": 6,
+        "kilo": 3,
+        "hecto": 2,
+        "deca": 1,
+        "deci": -1,
+        "centi": -2,
+        "milli": -3,
+        "micro": -6,
+        "nano": -9,
+        "pico": -12,
+        "femto": -15,
+    }
+    base_units = ["meter", "byte", "bit"]
+
+    def __init__(self, input_unit: str, target_unit: str) -> None:
+        self.input_unit, input_base = self._get_valid_unit_and_base(input_unit)
+        self.target_unit, target_base = self._get_valid_unit_and_base(target_unit)
+        if input_base == target_base:
+            self.unit_base = input_base
+        else:
+            raise ValueError(
+                "Both input and target units should be from the same quantity. "
+                f"Input quantity is {input_base} while target quantity is {target_base}"
+            )
+        self._calculate_conversion_factor()
+
+    def _get_valid_unit_and_base(self, unit):
+        unit = str(unit).lower()
+        if unit in self.imperial_unit_of_length:
+            return unit, "meter"
+        for base_unit in self.base_units:
+            if unit.endswith(base_unit):
+                return unit, base_unit
+        raise ValueError(f"Currently, it only supports length conversion but `{unit}` is given.")
+
+    def _get_unit_power(self, unit):
+        """Calculate the power of the unit factor with respect to the base unit"""
+        if unit in self.imperial_unit_of_length:
+            return log10(self.imperial_unit_of_length[unit])
+
+        prefix = unit[: len(self.unit_base)]
+        if prefix == "":
+            return 1.0
+        return self.unit_prefix[prefix]
+
+    def _calculate_conversion_factor(self):
+        """Calculate unit conversion factor with respect to the input unit"""
+        if self.input_unit == self.target_unit:
+            return 1.0
+        input_power = self._get_unit_power(self.input_unit)
+        target_power = self._get_unit_power(self.target_unit)
+        self.conversion_factor = 10 ** (input_power - target_power)
+
+    def __call__(self, value: int | float) -> Any:
+        return float(value) * self.conversion_factor
```

## monai/utils/module.py

```diff
@@ -8,14 +8,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import enum
+import functools
 import os
 import pdb
 import re
 import sys
 import warnings
 from collections.abc import Callable, Collection, Hashable, Mapping
 from functools import partial, wraps
@@ -504,14 +505,15 @@
     """
     dep, has_dep = optional_import(dep_name)
     if has_dep and hasattr(dep, "__version__"):
         return dep.__version__
     return default
 
 
+@functools.lru_cache(None)
 def get_torch_version_tuple():
     """
     Returns:
         tuple of ints represents the pytorch major/minor version.
     """
     return tuple(int(x) for x in torch.__version__.split(".")[:2])
 
@@ -558,14 +560,15 @@
             if isinstance(l, int) and isinstance(r, int):
                 return l < r
             return f"{l}" < f"{r}"
 
     return True
 
 
+@functools.lru_cache(None)
 def pytorch_after(major: int, minor: int, patch: int = 0, current_ver_string: str | None = None) -> bool:
     """
     Compute whether the current pytorch version is after or equal to the specified version.
     The current system pytorch version is determined by `torch.__version__` or
     via system environment variable `PYTORCH_VER`.
 
     Args:
```

## monai/utils/type_conversion.py

```diff
@@ -41,15 +41,15 @@
 
 # conversion map for types unsupported by torch.as_tensor
 UNSUPPORTED_TYPES = {np.dtype("uint16"): np.int32, np.dtype("uint32"): np.int64, np.dtype("uint64"): np.int64}
 
 
 def get_numpy_dtype_from_string(dtype: str) -> np.dtype:
     """Get a numpy dtype (e.g., `np.float32`) from its string (e.g., `"float32"`)."""
-    return np.empty([], dtype=dtype).dtype
+    return np.empty([], dtype=str(dtype).split(".")[-1]).dtype
 
 
 def get_torch_dtype_from_string(dtype: str) -> torch.dtype:
     """Get a torch dtype (e.g., `torch.float32`) from its string (e.g., `"float32"`)."""
     return dtype_numpy_to_torch(get_numpy_dtype_from_string(dtype))
```

## Comparing `monai-1.2.0rc3.dist-info/LICENSE` & `monai-1.2.0rc4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `monai-1.2.0rc3.dist-info/METADATA` & `monai-1.2.0rc4.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai
-Version: 1.2.0rc3
+Version: 1.2.0rc4
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
@@ -59,14 +59,16 @@
 Requires-Dist: fire ; extra == 'all'
 Requires-Dist: jsonschema ; extra == 'all'
 Requires-Dist: pynrrd ; extra == 'all'
 Requires-Dist: pydicom ; extra == 'all'
 Requires-Dist: h5py ; extra == 'all'
 Requires-Dist: nni ; extra == 'all'
 Requires-Dist: optuna ; extra == 'all'
+Requires-Dist: onnx (>=1.13.0) ; extra == 'all'
+Requires-Dist: onnxruntime ; (python_version <= "3.10") and extra == 'all'
 Provides-Extra: cucim
 Requires-Dist: cucim (>=22.8.1) ; extra == 'cucim'
 Provides-Extra: einops
 Requires-Dist: einops ; extra == 'einops'
 Provides-Extra: fire
 Requires-Dist: fire ; extra == 'fire'
 Provides-Extra: gdown
@@ -87,16 +89,23 @@
 Requires-Dist: matplotlib ; extra == 'matplotlib'
 Provides-Extra: mlflow
 Requires-Dist: mlflow ; extra == 'mlflow'
 Provides-Extra: nibabel
 Requires-Dist: nibabel ; extra == 'nibabel'
 Provides-Extra: ninja
 Requires-Dist: ninja ; extra == 'ninja'
+Provides-Extra: nni
+Requires-Dist: nni ; extra == 'nni'
+Provides-Extra: onnx
+Requires-Dist: onnx (>=1.13.0) ; extra == 'onnx'
+Requires-Dist: onnxruntime ; (python_version <= "3.10") and extra == 'onnx'
 Provides-Extra: openslide
 Requires-Dist: openslide-python (==1.1.2) ; extra == 'openslide'
+Provides-Extra: optuna
+Requires-Dist: optuna ; extra == 'optuna'
 Provides-Extra: pandas
 Requires-Dist: pandas ; extra == 'pandas'
 Provides-Extra: pillow
 Requires-Dist: pillow (!=8.3.0) ; extra == 'pillow'
 Provides-Extra: psutil
 Requires-Dist: psutil ; extra == 'psutil'
 Provides-Extra: pydicom
```

## Comparing `monai-1.2.0rc3.dist-info/RECORD` & `monai-1.2.0rc4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 monai/__init__.py,sha256=N68MC4_ibRXAO-vquIMx4tT--Er8hAHlKkmIrVBLsbY,2276
-monai/_version.py,sha256=v6FyooUy75h9LCy6fig5Wp6_e9DXu_xFquJViN89lNo,500
+monai/_version.py,sha256=LKob9njkBRLKzrCDQ-koS9kyRykOiNZWbifkG05gSkQ,500
 monai/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 monai/_extensions/__init__.py,sha256=NEBPreRhQ8H9gVvgrLr_y52_TmqB96u_u4VQmeNT93I,642
 monai/_extensions/loader.py,sha256=7SiKw36q-nOzH8CRbBurFrz7GM40GCu7rc93Tm8XpnI,3643
 monai/_extensions/gmm/gmm.cpp,sha256=GLC_KOEFUlEB8fUs6vjeuZBxIqzuatZBDc-ZoAtQ6Xg,2931
 monai/_extensions/gmm/gmm.h,sha256=c9n8RLa4r9jTbqpY4cCHFm3ldVER_FN8pG2hQx3Lb3c,1760
 monai/_extensions/gmm/gmm_cpu.cpp,sha256=cyKn-7DjtVCPb9bnGb0bWUfagb3KUFX9rD6mI5BEXrs,1118
 monai/_extensions/gmm/gmm_cuda.cu,sha256=2CvNdiuc6JiEsdK31iiHJQytubn81fxIQim-At_-1HA,16213
 monai/_extensions/gmm/gmm_cuda_linalg.cuh,sha256=Glqg2oAcUFUXg-DVfpROkiv-DdXvvVdM1nyiFm8qlHY,3520
 monai/apps/__init__.py,sha256=VDIc3HB_uFbqKL1TS-OeRvryEMDfzm22KJRzwpkXsGo,908
 monai/apps/datasets.py,sha256=OOfRSKDAL4IEh4bsRZDQddl_d_7tbVUy7QXZsUSFWig,34560
 monai/apps/utils.py,sha256=lyUDb-HUvEb8xPAi0cwQcKEGaSrgKi8H9sikYNRyTL4,13505
 monai/apps/auto3dseg/__init__.py,sha256=nacmbm8szCtL6Jf_ZaL8JQtiBlM6B3_TiI3HHZfJLt0,952
 monai/apps/auto3dseg/__main__.py,sha256=xtGFmv2ok6wK3SDCUm3yOF8XUHwNz3nKP1Zw9fxRsv0,1349
-monai/apps/auto3dseg/auto_runner.py,sha256=8cS1sYiv6bTVmeQHSlyZPX4vs8gRvnTBzIkzOy-65_c,35021
-monai/apps/auto3dseg/bundle_gen.py,sha256=fohDpyTwoqh0He071djRPq7aNRvYgrB9_UBbfxZjy_4,22395
-monai/apps/auto3dseg/data_analyzer.py,sha256=asZfLvvdVPd-JeXcG2inqnTTVyU_2EVrzhHfvZINUbY,13587
-monai/apps/auto3dseg/ensemble_builder.py,sha256=66YshcHdqX8GtKUp8ty3aroRUkoQHOZnTYm9hllkhnE,11371
-monai/apps/auto3dseg/hpo_gen.py,sha256=giTr8TkgFC6AqPJtWfkyAA-2qLRbbi4mQw-5WvhHb5Y,17378
+monai/apps/auto3dseg/auto_runner.py,sha256=HRYHlmnti6ssXLjJJeH90hjx3lhzTMNAyg6nG0l2KjA,36092
+monai/apps/auto3dseg/bundle_gen.py,sha256=VNPgHeXEJlmTXCQkGKwNtBvzJW5ZOAKfPijx4Go5PQY,23164
+monai/apps/auto3dseg/data_analyzer.py,sha256=cVoPCOa2M2uIY8PVzCiHYgwt2ERSvpKFIDpA_UvvLH0,17319
+monai/apps/auto3dseg/ensemble_builder.py,sha256=vEHC0mcvWZeuXaIH7hFj9p22M6MWBNoxtWcZGUgSfUI,11249
+monai/apps/auto3dseg/hpo_gen.py,sha256=XnWjoSgkrZOS8W_AaSaXpShJjSxx5l0xaYDkJVlqewk,17523
 monai/apps/auto3dseg/transforms.py,sha256=eHueZBNFMgGa9Nz96JE7KxTH05mpMfWxaD1QHxQ-B98,3733
-monai/apps/auto3dseg/utils.py,sha256=8CSlARjXoBkowlT7ZaKzIKeC1F9_lOd54hNdTJInO_w,2481
+monai/apps/auto3dseg/utils.py,sha256=KdU5E8jNghdONNwb2aZ7eYjA5zGkoNq_1s-drq3csm8,2765
 monai/apps/deepedit/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/deepedit/interaction.py,sha256=h9zTmhHAmwndR315RknqXtLWYqyYGvdcmjP6EpRrzHg,4501
 monai/apps/deepedit/transforms.py,sha256=sgFUuMqMlxmvWmsx-lHajoUHVDMp9fLo7UiwG60IYU8,37435
 monai/apps/deepgrow/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/deepgrow/dataset.py,sha256=W0wv1QujA4sZgrAcBS64dl3OBbDBM2cF4RK0fDCQnRU,10054
 monai/apps/deepgrow/interaction.py,sha256=l-wCmetMi4g-gcgMjA68firOX4RKvFm8WgefwiUFtTs,3739
 monai/apps/deepgrow/transforms.py,sha256=C38Q5ZdR98JWFyR5lNnhIaibL9zf14c111KDLaYvwB8,42011
@@ -51,36 +51,30 @@
 monai/apps/mmars/model_desc.py,sha256=k7WSMRuyQN8xPax8aUmGKiTNZmcVatdqPYCgxDih-x4,9996
 monai/apps/nnunet/__init__.py,sha256=gyqmg1fxPf3RF6LL25gnpMTfNS14uxweuJ93e4UzjB8,745
 monai/apps/nnunet/__main__.py,sha256=h5GTEHSZliEZ38_4WOtqujPa-C3M6if-0huNHmreaNI,2975
 monai/apps/nnunet/nnunetv2_runner.py,sha256=iqKvjUHH22jq0TmkHawRvMigEKBIDIirhpT3lbYDXQY,38587
 monai/apps/nnunet/utils.py,sha256=u1jVSAJeOmpCmXczqnGuU4jnSevsawwLbuFUUKB8XrI,6791
 monai/apps/nuclick/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/nuclick/transforms.py,sha256=vCw2IpuMLLZ3C2NtBj59Kxjy1cHm4K3VCm7KMP71aug,24948
-monai/apps/pathology/__init__.py,sha256=QLVT5fpZz7uyjOE6s6ZnF6xYWvwAUvuDQWAJmjpPN6U,1156
+monai/apps/pathology/__init__.py,sha256=SRBbxgPzZdtC22TpY1m0-Z3SSBfMig6xYVSdgOClgXg,1030
 monai/apps/pathology/utils.py,sha256=GtVzcr8mc1MsojpUx3tI7IYs7yhIo_HtnY0msv5pkwM,2860
-monai/apps/pathology/data/__init__.py,sha256=PnH6qvFrTrw9DC6j9B2VapaRttiLlznA9gbygpfq7kI,702
-monai/apps/pathology/data/datasets.py,sha256=3QSMa_KVvZjgcpCrdRGRy-Ne813l8BIBd58JgJsisnk,15184
 monai/apps/pathology/engines/__init__.py,sha256=sqR2PUjmFf46jRRQA8ZZ9umbQzuLGDpBaRWQNVA2r7Q,650
 monai/apps/pathology/engines/utils.py,sha256=Zr_DuWZ3qcIiNM7QjFSzgojeRPJV_UP5yGWIxrU5gI0,2397
-monai/apps/pathology/handlers/__init__.py,sha256=pwOarLrm98KMBGrkE5og0FEDst1uirzJZddc_DFtTsw,657
-monai/apps/pathology/handlers/prob_map_producer.py,sha256=w5o4WHMj1wLLAUDuKSHQL75Tv0dP53nSEMarMNKuY_4,4851
+monai/apps/pathology/handlers/__init__.py,sha256=YRvZ5C6I56qvu1DTGROJV5Sq0ZF3t6f34vV3Vdeg9Hk,609
 monai/apps/pathology/handlers/utils.py,sha256=qqf-4qHoZPsoVtQ_m4oMjRJ2TV880W3wgN0juzGfpLE,2315
 monai/apps/pathology/inferers/__init__.py,sha256=dpBmAMzyXnEUUnbuU-4DRUYXAtTQ-We_VCkMy0RIaS0,660
-monai/apps/pathology/inferers/inferer.py,sha256=s8I_G-t1BDXok2HGA8aJYX3domfInuYW5wePd_qAgCo,9088
+monai/apps/pathology/inferers/inferer.py,sha256=fSC-biNx6tpOrM5795qScyVOAbiUw6I2klD8zVdRMTA,9148
 monai/apps/pathology/losses/__init__.py,sha256=yPGavYe8N6_bKvRN1-1awGmgnHZKpjQww3QML6UMRPQ,650
 monai/apps/pathology/losses/hovernet_loss.py,sha256=Sw9wBAilBOKB8oKaPU4yKxVOl8y4lv-XzgJ6iFN0AyU,7293
 monai/apps/pathology/metrics/__init__.py,sha256=c7xRUzhQesEWRIUFF6vM-Qs9v0Lv8QzCNNd-hJOCL-I,646
-monai/apps/pathology/metrics/lesion_froc.py,sha256=izLB-I1Ej-ewQc3DXDmZ_V_XuGQIfIvM_KzR7TakvUQ,7227
-monai/apps/pathology/transforms/__init__.py,sha256=IRSRmbOTJavTdTHVNL1mtYF26wbYUZuPVsVZvuh5Chg,2412
+monai/apps/pathology/metrics/lesion_froc.py,sha256=yA5bsJAAn6eIQ5Q1m0rOVAsjl9YpAXisgkJ6TxfpPhU,7225
+monai/apps/pathology/transforms/__init__.py,sha256=c3YkornqjX-fHRnwkpn_PxmnMje6pif1qxPdFNyQUWU,2243
 monai/apps/pathology/transforms/post/__init__.py,sha256=WUZbaM2bg13mpbnNhol0D0A328XgUspTWtPvli1Uqpk,1995
-monai/apps/pathology/transforms/post/array.py,sha256=n2QyFVYlADxnHcJUXkr88oKczDUeDh5g98gNOPNlKkc,36850
-monai/apps/pathology/transforms/post/dictionary.py,sha256=t8B62m5O-Ku3rsiXCmJjM3oqBzxL8rICAtXj9_5gQFQ,25716
-monai/apps/pathology/transforms/spatial/__init__.py,sha256=YqRIlh5xL1d8kay411eviELymfrzWsiv11SwhX1gIuk,763
-monai/apps/pathology/transforms/spatial/array.py,sha256=VpO38N76DY1pxUXqIGi5qHT-PWBSXXIS_LPNseiMqeY,10919
-monai/apps/pathology/transforms/spatial/dictionary.py,sha256=JTL2BmL3xvYmFvuUoQbs__g-OZOgrUzdvcIWzlbfv0E,5442
+monai/apps/pathology/transforms/post/array.py,sha256=_FxrRpFOnpspUdXTi5_4zHZOx9mT_4-suh96FPjEajo,37322
+monai/apps/pathology/transforms/post/dictionary.py,sha256=5qQ00PM5XJpzfJDvshi9dfGKsnxtsUO4e9FGwekv7KI,25992
 monai/apps/pathology/transforms/stain/__init__.py,sha256=i9HfrXiQHG5XHfqMtz2g7yBX7p1uN0xcGAPCYyXSmV8,836
 monai/apps/pathology/transforms/stain/array.py,sha256=Dr1fCmkQzc8n40XbLAHpq1EG5wkMqTjWgYN2FGJfMGk,8366
 monai/apps/pathology/transforms/stain/dictionary.py,sha256=sTF7DJVXQe1SBQrhC84Xl2kmINqoTX6Tb8YSv2VH9Vs,4761
 monai/apps/reconstruction/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/apps/reconstruction/complex_utils.py,sha256=vIVCweWwPHL5bYK3a7aDMS64CI7L9AUh9l2gG3cisM4,8393
 monai/apps/reconstruction/fastmri_reader.py,sha256=CbAWHN9-b8TFgIpsu1UmS0zHZg3lvqIyraZFODoTMdM,3644
 monai/apps/reconstruction/mri_utils.py,sha256=WEentr9IfCdTRcRELYkIgRx2oCaIoc1JEVE1FJfQlqQ,2000
@@ -100,52 +94,52 @@
 monai/apps/tcia/utils.py,sha256=O-CGB_gF3MTh2BcdJw-KZ2luHvhB6HvEBqOwsRAa1HY,6152
 monai/auto3dseg/__init__.py,sha256=DbZC7wqx4zBNcguLQGu8bGmAiKnk9LvjtQDtwdwG19I,1164
 monai/auto3dseg/algo_gen.py,sha256=X8OrOGAEqbhJ06zbDWDCuZRs1HXjejt5CpW5qsWGkDk,4209
 monai/auto3dseg/analyzer.py,sha256=5CImSIYLFvGJ0QsUUFAvjiWkWmwZk0OeckHbe6Rgeng,41223
 monai/auto3dseg/operations.py,sha256=1sNDWnz5Zs2-scpb1wotxar7yGYQ-VPI-_b2KnZqW9g,5110
 monai/auto3dseg/seg_summarizer.py,sha256=39zXmyRe9aNhXS9ZliDJsUEDqzU1OPtUG5tL1peJsx0,8725
 monai/auto3dseg/utils.py,sha256=QOapCrMbguQz_t5BsU_YAY4DWwjKA38i4sc-TWgzKJA,12193
-monai/bundle/__init__.py,sha256=AVXOioyrDe4l3NJi4kGWvVp8v_HG5u7QsVf7L8EpCNU,1306
-monai/bundle/__main__.py,sha256=aEUfiji0MNL_pv3NA-aiAufKhS2_q63E2W6knEtgPLQ,858
+monai/bundle/__init__.py,sha256=EFeyJGNju0ijBfKkobpdymGvbuAX_ZJWQd8sa6OWOSw,1341
+monai/bundle/__main__.py,sha256=EiWkpt3yIcT8uBKg99kQBWTYoFgSpHjR7GAvIKA9EME,926
 monai/bundle/config_item.py,sha256=sBQ_Kg93EFET_pZcdzdMatnrB2FD2bMvmg_LpupdwMA,16035
 monai/bundle/config_parser.py,sha256=tX8ZKDW43uWzCQ8EBUROu-U9wJItzF7_XzotLK-wt60,22410
 monai/bundle/properties.py,sha256=CUTh7CVwZu4D59SRf2b1p-03OD2G9VVi5JUutazmC8A,8628
 monai/bundle/reference_resolver.py,sha256=3KpSa-1n1hptY6N1C-3yt5pybTXB7QUVj8fNWWGvN2U,14353
-monai/bundle/scripts.py,sha256=FWE1-ssQpLw_gaA-JBw5w3Ot0kzwIaSKsV7_wpokMj8,53473
+monai/bundle/scripts.py,sha256=K8c5RLc-QgrAZX80mk4JRL3kP13DYTCvNgl7OLIjc3M,63733
 monai/bundle/utils.py,sha256=Vou6ko4OjT1v8xOT99bZuFaAB-NPpTj-oZ4KjBJsYsY,8911
-monai/bundle/workflows.py,sha256=nG5H7yskNcwUxg1a9WHzGFD0n4uYfM5olyLIrpAUjz8,16484
+monai/bundle/workflows.py,sha256=57BZ_GB-a3Qy7O_KtP-n-n_LS4Rku9FTi_Y2zubv7wE,16520
 monai/config/__init__.py,sha256=CN28CfTdsp301gv8YXfVvkbztCfbAqrLKrJi_C8oP9s,1048
 monai/config/deviceconfig.py,sha256=TifpuOAhccn1A3UCtInAnfciyGLHSNIen5ZRmUB8eKI,9913
 monai/config/type_definitions.py,sha256=0fAuI-_uX2Ac_33bgDVXKmBSl-fJNFcsOqBqYV16fhk,3485
 monai/data/__init__.py,sha256=9FhsQ7GHbTNAX25vLY1oR63b3q7jpJpVMfLigs5h0bs,5087
 monai/data/box_utils.py,sha256=YbG6lOoYwUGmwcNmoKzq2xnNTbYA4LMkHmfsqteopCg,50102
 monai/data/csv_saver.py,sha256=fcZF4kBNQnDFwQjV9TS4zjq_zqsv_u3QldxRprMC7zI,4952
 monai/data/dataloader.py,sha256=-n_LUfm3tlSHxh1at1xOmQkMrWQaKm3KBNo4A27PECE,3835
 monai/data/dataset.py,sha256=iNchlXTej2dCzsnpRBmVNjhB_MIWCcBk-fjfFdQAKHI,68927
 monai/data/dataset_summary.py,sha256=P16hTM71E85H-Cku8FS1ypJzopD76Itla3QQGk_Z0dM,10216
 monai/data/decathlon_datalist.py,sha256=Lmaj-4rufQ1Jibtzj8tO8htU2PhfZFo7SbZ68SmXRfU,10318
 monai/data/fft_utils.py,sha256=in9Zu8hC4oSVzuA-Zl236X6EkvgFka0RXdOxgvdGkv0,4448
 monai/data/folder_layout.py,sha256=IsHW1-Bkupn_T8r6MgFTIJQh5HwCg0xQwOKmgBtl0gE,6344
 monai/data/grid_dataset.py,sha256=xHG9ibEpiQtXCEpJ-07dy2-79KvzBRpJhdC3Tag6ZP8,12484
 monai/data/image_dataset.py,sha256=OhNJ3awauWtqsDhefIGDw3UYGF3RoleeNUPdJOKg3kI,7008
-monai/data/image_reader.py,sha256=UPI3CrrI15M65nGW_rom0Yt8xQdz5fZaS_IwB2rLQLA,71785
+monai/data/image_reader.py,sha256=9OF-ldu0RRJz4HSfgYm-5jl30ezzuJMnke3Wyx2ARXI,60619
 monai/data/image_writer.py,sha256=22ob-wAahyiJHkuQfT_JrsVMxIMCrW9TSJHCO2GMmBI,39872
 monai/data/iterable_dataset.py,sha256=fxSNYi8idu3uB4ECn8g3NbgCcRQk7pFbGuOxqhtyQjo,13309
 monai/data/itk_torch_bridge.py,sha256=_SlMLySrYvy0SEwVEU4Z8jteqWRJIHy5nySDHhCMDNo,14097
 monai/data/meta_obj.py,sha256=OxfcCSBFuN0fUpyIa9ey9HuqrqimARNnEZPuqRRXjLo,8800
-monai/data/meta_tensor.py,sha256=cN3sGoZwlCMp4i9cjLD3TCm8ckNOJ1iKFf5CJqtNtSM,27125
+monai/data/meta_tensor.py,sha256=_TnJfKyeOP6qO2d_9aMdRTk0tRlmjtUwTXUYVKPVTcM,27321
 monai/data/samplers.py,sha256=8N72tdua63XByOrQ1SigMGimnwK9Y2KGOrsQEjIjhHI,5268
 monai/data/synthetic.py,sha256=H0MaQq2nnYxXEMlvOW1-XoWJWY_VKsgZ75tWLO1aCXg,7375
 monai/data/test_time_augmentation.py,sha256=H1yUph4SkJ-bmKRXS-SRZfNKtWkihR7o4PTUWKuHxOw,9780
 monai/data/thread_buffer.py,sha256=FtJlRwLHQzU9sf3XJk4G7b_-uKXaRQHAOMauc-zWN2Q,8840
 monai/data/torchscript_utils.py,sha256=auz2GtrklxY6PMzvd-i9Kk73uIv0qydpOtzdSfZxrhE,5500
-monai/data/utils.py,sha256=v8E0LzWqx49UtwiZoFEteq6bh4TI6cVkhhrduGr8rMQ,64334
+monai/data/utils.py,sha256=qNGP8YUAJl6N9xB8WCxPQE1JgWqQstv_qHoO35dwpX0,64795
 monai/data/video_dataset.py,sha256=5Q7bHXg32rOVQjiyLUrVuqAkpTa33uydCrZwNJw7iFM,9059
 monai/data/wsi_datasets.py,sha256=mQVqd58NmFVKxRVCHjJ0ga863H5hsgmH1j-VXkiQGeA,18631
-monai/data/wsi_reader.py,sha256=_ddiG3KnhTkbYLpeqEagAjXPJ_5qXW2BBiPUuINQ584,38749
+monai/data/wsi_reader.py,sha256=3l_OzDM2tsCEuLbUWsHKJb3Bj9nEAwGV84hFX8QmtIY,49442
 monai/engines/__init__.py,sha256=07lWK9BRezM98bHM8Z1VBXcPs7JPnulDYtg8uXQzOio,1133
 monai/engines/evaluator.py,sha256=clfURplaABOZhhxYjYRz1ZHIQHEAGnGqljW0Ub9HbO8,24568
 monai/engines/multi_gpu_supervised_trainer.py,sha256=9UiqHpWvKxkj24-4EAzbHrRdMlSgohH-rFBus1M_Cnw,7278
 monai/engines/trainer.py,sha256=Nxt-lz0puqcWHEyVnhqR1qXwzR8PxlVSiPwH8phZAG8,21347
 monai/engines/utils.py,sha256=gmDzkD4SIL9DeFBgWdjbf2e6yTQp_e3lA9aAJRwZmDQ,11631
 monai/engines/workflow.py,sha256=EAWMehQz28o-fX8MKSVBjhI1YAM7-Gt-w1HfzcMl4gI,15250
 monai/fl/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
@@ -185,18 +179,18 @@
 monai/handlers/smartcache_handler.py,sha256=OA6v4EC2geH419eBKSAGSb-XNxO_qSPmJ2fkh7TOv-s,3051
 monai/handlers/stats_handler.py,sha256=35tkttd-LFKfE6bO9wPVOr5oHwiP2yEWXcZSSURtN9E,14251
 monai/handlers/surface_distance.py,sha256=jfuRpuzG7Ia-Ye0Izce1n4UPBghe1xtwBPwXx3fmODw,3313
 monai/handlers/tensorboard_handlers.py,sha256=FGd3KT7AoulwWOGbiJqDAyjMpZzuIyZZoNsatRdDoNE,23325
 monai/handlers/utils.py,sha256=PumzyMPAisJ_A-4RkgkNq31YfulhuI1UcOF9-Xj2_Dw,9855
 monai/handlers/validation_handler.py,sha256=xpRB3IB7pckzgTgdzTGb_gG6tIezeIvtmhJHPNYrpvY,3269
 monai/inferers/__init__.py,sha256=B3e24tgM92C6J49FAOcawvpuyl_svG8OqfHMUjNFLl0,857
-monai/inferers/inferer.py,sha256=tnSwO7eAkuuBdk_ef0nll1yyTtA4eHOzJhymLAhfkAY,26855
+monai/inferers/inferer.py,sha256=mdP1QnMrGRIigHi8ZDfnvmsXlIYyJt0Q8Uxi2cSJooA,27881
 monai/inferers/merger.py,sha256=onJ9OiCV9YOdsljd5YFZ3Dx6nSWv_gfCf7s5TSb6tHs,6393
 monai/inferers/splitter.py,sha256=dfU1AQWVvcbqt2hvZJqk_hFh6EtFrtgBoV7aId1ns7k,9397
-monai/inferers/utils.py,sha256=KDAs3tk7VgAHnc6EG0aUFp5SRN74Mkgjx-_VuS-IxnQ,16770
+monai/inferers/utils.py,sha256=O2nhe9bvN2scUmHoOX0o6yZrzEkUAtkjBJyUzhfSpCY,20036
 monai/losses/__init__.py,sha256=9-QH3s0s1XACosZPhJz5LrDskiwjjcMMt9Rhr-LE4PU,1409
 monai/losses/contrastive.py,sha256=okmuiRPpwAhInBmk7wUFm0BogaxiP0EgqdV0lxIhbHY,3430
 monai/losses/deform.py,sha256=GJpIQMGFf97SMd-5PswsMFrvRokaO_NabgQn73KDfcw,4979
 monai/losses/dice.py,sha256=11wqc7MN5BfOh0STfO6YMGto9BxjmzOgnXBSPadH6Ds,46326
 monai/losses/ds_loss.py,sha256=do2z8NyW5_KUgIgiZieql_XTHd1-eK1_uVUozKQoFqs,3733
 monai/losses/focal_loss.py,sha256=GfblgQtA4qMcGhLnQdUJJrv8zQczB4GH4k6L2ZxKnRY,9490
 monai/losses/giou_loss.py,sha256=Mogq6fR0tO__Xj0Ul388QMEx03XrSS-Ue96i9ahY-uo,2795
@@ -209,28 +203,28 @@
 monai/metrics/__init__.py,sha256=NcFg8BER-LIJkfhK3sHkgorRHwST6RXQbbvOIimsYT8,1977
 monai/metrics/active_learning_metrics.py,sha256=uKID2O4mnY-9P2ZzyT4sqJd2NfgzjSpNKpAwulWCozU,8211
 monai/metrics/confusion_matrix.py,sha256=8CMnqIaNK9_cf-5Z_6E_g-blh1FnvnCmuGahJSlptgM,15101
 monai/metrics/cumulative_average.py,sha256=UINnp__332Kb4gDdIu6WAror11kQ0GxCeLydlsFx6tc,5578
 monai/metrics/f_beta_score.py,sha256=ucr0ktzfM9jZanV3aqKZnlc23tf1z5r399ZEhxgu6Pc,4026
 monai/metrics/froc.py,sha256=tGM3hIU17yNdj1YG1yW22UUpTc8nH7ZZXChvZY_T_40,6157
 monai/metrics/generalized_dice.py,sha256=0nk3-IT9s3SQshVf1QStGEmH0iBxtofzXx_bf1EWhVw,8262
-monai/metrics/hausdorff_distance.py,sha256=v4ihFZMSMoPaDJ6CU-bN2DAidUOPg31YGH5vFaLwB38,9120
-monai/metrics/loss_metric.py,sha256=mY3M3WaZwj4qcbjANJoqxv3UBYkjTIbezFe_wG8YXM4,4868
+monai/metrics/hausdorff_distance.py,sha256=PDnr94AMWIBp1U0lql95BqL6wHvk3j_moqH2UTjeeBs,11470
+monai/metrics/loss_metric.py,sha256=m9jXobVHKLeDY_8yrA9m7FwfapSAb-kYIdUJOsbvBvY,4907
 monai/metrics/meandice.py,sha256=UsEJVAFbEZC7QM2j3tTleQSUTX5XWDwUPu6E0ipKZ68,10937
 monai/metrics/meaniou.py,sha256=MJd-4v-DArd_uDMWgUJhuV2CBXuU7hB2W3-IM_VxeSg,7209
-monai/metrics/metric.py,sha256=jflbJgw2NmLST9Y7fetk8xG6V0vuse59y8NAtOjMVjs,14720
+monai/metrics/metric.py,sha256=N-lnphEmh13Y2he1gnVWhwMRgMpO4r_X3uDzxiaRnmY,15140
 monai/metrics/panoptic_quality.py,sha256=2CfSB1B0mwVOfTCuRNuYAn7XI8G4NPFRPc7NTbv5JNc,13679
 monai/metrics/regression.py,sha256=mAWkqnFZGtb2pgmAXhb4T0MNrrU50Qup6UJjGF3XwjI,18235
 monai/metrics/rocauc.py,sha256=CJOAzDamB8TcFP1bEg-I1m5V1-Pq5RMaLFdM6MtNa_E,8038
-monai/metrics/surface_dice.py,sha256=YHzs1UlV3xgon1YVS1xZnorjoedQj6pLutLl5PFViYg,12166
-monai/metrics/surface_distance.py,sha256=9AQ5u0qEEj3bC-hoC_9nHWdcBsmzQRAl6i5L02whzhQ,7928
-monai/metrics/utils.py,sha256=c6O6zshEYHLRB7tE0PVC7a18amsK7IQ07ysqWhglUn4,11172
+monai/metrics/surface_dice.py,sha256=3ged6augFI0tUieS4z0kNIWnIvil4HPlHlMybJttzhA,14415
+monai/metrics/surface_distance.py,sha256=KDbdKdQz1r8gOm0INLxAQrnaZn_71p5Tz3906rlv6k8,10186
+monai/metrics/utils.py,sha256=Vt4RxljPbrPYfpLDAAdnjtyraRLo4JgWTh0BaHKYNew,15100
 monai/metrics/wrapper.py,sha256=eV2iUvtOViEDqt_o9rw7a3-3tL7XAoKAr1yolViDDWk,11772
-monai/networks/__init__.py,sha256=XvFvlD9B_-PP3CJJSi4i6zlWhOA7C4QAnjoCq2mFO1Q,999
-monai/networks/utils.py,sha256=TPbLlQDeSu52NN48ihS8XGh6aCYzKpSjVPR9T08wWdI,34353
+monai/networks/__init__.py,sha256=X-z-kmVt9kwoNPgfYITGycnvG_9HC3_RSRKD2YC35Ag,1020
+monai/networks/utils.py,sha256=smhCOr6f8MssKq7UkHnCt1HzIU9SQnzS0xCrzpbUv18,46286
 monai/networks/blocks/__init__.py,sha256=umyJFI-rDAMuseC0gD1vwCE3EowQpWjVfuCLKGFoL1g,2134
 monai/networks/blocks/acti_norm.py,sha256=bVGXbTZ_ssRvmED5R7LOQ7jj4V6WbVFl8JMO-4iZ2Dk,4275
 monai/networks/blocks/activation.py,sha256=S5k3zcP2PsHBkeIxgWgNg8ppW80tTResVP2j9ZsvTFw,5839
 monai/networks/blocks/aspp.py,sha256=GGGE7NfWj77RkaWHbcLuUP4Aff-WeiDrtgtFuSoekQk,4380
 monai/networks/blocks/backbone_fpn_utils.py,sha256=0WDppafm-y8_HeyaFLJI7Hq7wcwcs6nrptGgLbUgXOI,7490
 monai/networks/blocks/convolutions.py,sha256=gRmbYfy3IR4taiXuxeH5KGOFjP55FoVWfP4e1L6ai0s,11686
 monai/networks/blocks/crf.py,sha256=gHyRgBWD9DmmbCJnXwsMa6WN7N9fDLuT_SwH8MnHhXE,5009
@@ -243,24 +237,24 @@
 monai/networks/blocks/feature_pyramid_network.py,sha256=ahk2jHYiWY7ddTwIjxijs0WtI_3V3qXY3KqlD4Zso9Y,10586
 monai/networks/blocks/fft_utils_t.py,sha256=8bOvhLgP5nDLz8QwzD4XnRaxE9-tGba2-b_QDK8IWSs,8263
 monai/networks/blocks/localnet_block.py,sha256=1tUJZh5A0Wlhy0J7kW4Sko7FVTvUjPwHJLqZNeu-O2I,11454
 monai/networks/blocks/mlp.py,sha256=udgUVvHJdyZK2DG3We4zJyNy6eB2zUJfPyI1rUMu1YI,2813
 monai/networks/blocks/patchembedding.py,sha256=gBiMZyXrmmJTR1ystbuV4fSkH-CO0R1oEGJ-jhxipxM,7987
 monai/networks/blocks/regunet_block.py,sha256=1FLIwVBtk66II6xQ7Q4LMY8DP0rMmeftN7HuaEgnf3A,8825
 monai/networks/blocks/segresnet_block.py,sha256=iwzhEJlACvmv3C9LRDkMuDs9DJtYtYAGOyDj9HhlvDg,3245
-monai/networks/blocks/selfattention.py,sha256=IqoSFSxUamVpih-sQ74d7oQwVyrN8CWvwL5-OZddjD4,2567
+monai/networks/blocks/selfattention.py,sha256=FUUxq5LFBHxHQz3WKK8oZK7KVPtyhL2H9PrtYLTIeuw,3099
 monai/networks/blocks/squeeze_and_excitation.py,sha256=y2kXgoSFxywu-KCGYbI_d-NCCAEbuKAIY5gSqO_T7TI,12752
-monai/networks/blocks/transformerblock.py,sha256=hci2qoZERQ0V2hvnEqib_j6uhsuOwh7twxZjsEgk3po,2047
+monai/networks/blocks/transformerblock.py,sha256=GHVjtyTjNskTRrhQzRGvI7uhvUajP_eCmQ97o3qRU3I,2322
 monai/networks/blocks/unetr_block.py,sha256=d_rqE76OFfd3QRcHuor5Zei2pOrupoleBWu3eYUup0c,9049
 monai/networks/blocks/upsample.py,sha256=If8gyKSt6oLVBabNPdPdIa-vhLPd041NdzGEE5xiC-E,13312
 monai/networks/blocks/warp.py,sha256=ATXWLFOVOx06jbCOYKvuuC1e8hXLoDhRwRVO2rYt79Q,6656
 monai/networks/layers/__init__.py,sha256=W5G4vpUDG8m3U5NTxxKhvM8NSHLDaeg1aFfnSolEu2s,1562
 monai/networks/layers/convutils.py,sha256=zwbYK4WJO1Tj2KASnOfxwYnb3p4pizXxdZRm6I1P3j4,8288
 monai/networks/layers/drop_path.py,sha256=SZtRNa1bDwk1rXWbUe70YDaw6H_NKeplm_Wk5Ye1L4Y,1802
-monai/networks/layers/factories.py,sha256=dTAGSXUwRd2IcSKVRi3pdmkBU85jUwvsh--S2tpdZAo,13058
+monai/networks/layers/factories.py,sha256=k06YAo6v9cZ5HO61HM7XxK_XedbgA8-d5IrUmWT3s5w,12620
 monai/networks/layers/filtering.py,sha256=7ru9Yt3yOM-ko-UqzYp-2tMpb8VHt5d767F-KkzrqYY,17992
 monai/networks/layers/gmm.py,sha256=yndDwTq_q8M_jsgIKvPfAEBAfzftARFy9emrde_rOtU,3324
 monai/networks/layers/simplelayers.py,sha256=ufiioPsyzkCb7uIJCNBvba366z4ZTVK3NSZdI-QRnMA,28470
 monai/networks/layers/spatial_transforms.py,sha256=J0pMm04zvHG605OzSNbT5dtdOWiJDbOsBB_ds8n6PyA,25576
 monai/networks/layers/utils.py,sha256=_387-Au76QG5wwGs7ESg0ocGTcBzw4DJz19H7vrPKjM,4296
 monai/networks/layers/weight_init.py,sha256=ehwI5F7jm_lmDkK4qVL7ocIzCEPx5UPgLaURcsfMNwk,2253
 monai/networks/nets/__init__.py,sha256=Lj_s7D5U_IT5wA-FeTEMeWZHn85YZNL7sYLAmWpOZVE,3141
@@ -274,97 +268,97 @@
 monai/networks/nets/dints.py,sha256=42ehcT_zyoVTiOzMHDglTJ42hcslaw5PQZBvjKKPl9o,44771
 monai/networks/nets/dynunet.py,sha256=S2DX_tby7e5iCHL7q6X6f-vT6HwP6tbb2lRq9gHVJ24,18210
 monai/networks/nets/efficientnet.py,sha256=nmXG3D2UDUcj0Ce5TllVihtO8ZCgT1gDa03iI-x8gUQ,40643
 monai/networks/nets/flexible_unet.py,sha256=1FwOvDijaD-2V8nAaW2ibr5DYpl8Ule8LtPADH3TNb0,14147
 monai/networks/nets/fullyconnectednet.py,sha256=j5uo68qnYSxgH_sEMRh7s3QGNKFaJAIxmx8OixEv2Ig,7212
 monai/networks/nets/generator.py,sha256=q20EAl9N7Q56t78JiZaUEkPhYWyD02oqO0yekJCd9x0,6581
 monai/networks/nets/highresnet.py,sha256=CQTRix9HDRz_ey4jsnuHv-DWrqmH4rksTHXy_EVX5dM,8882
-monai/networks/nets/hovernet.py,sha256=tsYVeNv8JT3RDcn3IQj42hJHBfrmJk6kk_GXYdrjS80,27864
+monai/networks/nets/hovernet.py,sha256=SR46NPeUa7THwo5ic9hHPIlyl9GVbpx4aNqLUeyCogQ,28678
 monai/networks/nets/milmodel.py,sha256=tbyrLBibi5IVeMxe_erka8k9xw3KDtQOId5DwfSZU2o,9812
 monai/networks/nets/netadapter.py,sha256=JtcME9pcg8ud4jHKZKM9fE-8leP2PQXgUIfKBdB0wcA,6102
 monai/networks/nets/regressor.py,sha256=RDbBCppgOOBid-ISRNE9nDpRcKLMSdD_xFgOVKtGneU,6488
 monai/networks/nets/regunet.py,sha256=RZhLX6o0lqv3IEL2TOadTbypfpAj6yaibMzNb2gSwJQ,17189
 monai/networks/nets/resnet.py,sha256=M7MVLoeiXxN4KXUq42HBCJshYqK37U34zHcQPMHDMm0,16785
 monai/networks/nets/segresnet.py,sha256=xNkSIvdk7kAyc3eVn-U_gGj8MoGVc5nklFKc_fkgOUs,13994
 monai/networks/nets/segresnet_ds.py,sha256=RRHTxsWrxI17282KtoFSEPJeBIcQIOdHeSHQpvUGFY8,15667
 monai/networks/nets/senet.py,sha256=gulqPMYmSABbMbN39NElGzSU1TKGviJas7EPTBaZ60A,19289
 monai/networks/nets/swin_unetr.py,sha256=kV5cSRWxtjTF25mOCSenxRsI0jyvIn1CBxttUCIdWSo,42000
 monai/networks/nets/torchvision_fc.py,sha256=cPQJ8xWl3zXB6YAyCR7BIR2W737GclYw8fqVr6f8LvQ,6248
 monai/networks/nets/transchex.py,sha256=TpdKj3nH-PWu_2S6JYPiAcjVld7TGPVyt52rKsbm9gY,16626
 monai/networks/nets/unet.py,sha256=CvQMZcHrfQnwfkWlJNRld82rBDNSuCOArYvabMO8YIM,13722
 monai/networks/nets/unetr.py,sha256=6sWCpH8FzITiiqThDgelARZrQVs64cZERcTb690NbJs,7943
 monai/networks/nets/varautoencoder.py,sha256=I8EgeVJWGn0KspyMjAbBFRE3oD67rUqLFH3-p9cbA2c,6285
-monai/networks/nets/vit.py,sha256=u23aFydgJWocr2yWnjl_0erI-AmXs-H9xsUx1XExX8k,5017
+monai/networks/nets/vit.py,sha256=PpE7SCdpqO5VhVaUNb_GrIhdUQXbJloJ_afGuPFMSic,5655
 monai/networks/nets/vitautoenc.py,sha256=AmnUQsUrm72z1cbadMYRD-V21ZuK3LxL2oKc10jP2nE,4817
 monai/networks/nets/vnet.py,sha256=6acwIN_NLyW1ANcT8C4Dr7RLCnBPJ2jxJlNbJvxHVdI,10011
 monai/optimizers/__init__.py,sha256=XUL7o9vSL7bZImpxVZqcc1c8MwUMrOZL4nJ-mjAA7yM,796
 monai/optimizers/lr_finder.py,sha256=5OKluV_a71VPNX_7BzFH7vCqcSYPXbuR3XlLwHCaASs,21948
 monai/optimizers/lr_scheduler.py,sha256=UJYzkhqxsYkyaisnCu0ba_kcAM6IL-lLskdDtHWOBnc,3652
 monai/optimizers/novograd.py,sha256=KOl3qiwsDg06rbZ48uLZI05kHxXUtwTfHp1P9Yn8Ot0,5661
 monai/optimizers/utils.py,sha256=vDgyMemHQAwAueZlnMIu4HuNJ5BSSEw_Csru2YnudJs,4131
 monai/transforms/__init__.py,sha256=TD6NsLbPLymA6zew4P4sPrrSwBnTtKfH9kzo6Vcfh-A,15216
 monai/transforms/adaptors.py,sha256=IxmzJncOfEO2NPzuxP3Z41DZDqa1VLJ19Gz89ks_DyA,8946
-monai/transforms/compose.py,sha256=G8tLyeuzm_PMN5b6E3GIRCd5JnGey1AWZHqAkoUZf0Y,40548
+monai/transforms/compose.py,sha256=hDNFTg6vhnYbILozdlHjy0KNmOqUE5PJWRd_mfa_AQs,40532
 monai/transforms/inverse.py,sha256=hXuDcwbJGjoWa5VeL-4vBHN2OkZ98cEZPlNIhi3kptU,17160
 monai/transforms/inverse_batch_transform.py,sha256=T1Kl7FQdE9omIm5SCCY9xnxGwaUxyfkgbJEtjB8LEuE,7054
 monai/transforms/nvtx.py,sha256=1EKEXZIhTUFKoIrJmd_fevwrHwo731dVFUFJQFiOk3w,3386
 monai/transforms/traits.py,sha256=HPAfD0ujRS0FYKH6bhwtKikW8Pebwrn9SoC4u7JChLg,2885
 monai/transforms/transform.py,sha256=c8B8bGgg55gpmXf3SBNUlvKyOim0s1rGTgv7RZsiZh4,18234
-monai/transforms/utils.py,sha256=9q3WilSMbBfIdAwmXBIubumxEs8KKIZ30dk7PEvIEIE,70604
+monai/transforms/utils.py,sha256=NNKpgYvz7TBbUCLmH1HdXRhGvQyjYdSYuvnsHtrdzV0,71153
 monai/transforms/utils_create_transform_ims.py,sha256=v-MDiukqHkmCGpcRCSZDr14taMcoOuTDeZlL67Wr48E,31081
 monai/transforms/utils_pytorch_numpy_unification.py,sha256=BItSUa0J50ihOXNxxf21C9I-GenjWgoeaKx9EZ0f7Sk,18397
 monai/transforms/croppad/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
-monai/transforms/croppad/array.py,sha256=C1eGp2IKHSE3rLEauM4tCbEDrjnkdxA7i42ew-G1gtU,68405
+monai/transforms/croppad/array.py,sha256=XNgxZ-LUIId5t0rGf_ujo8stzxSfZz95fszyY3OcFk0,68728
 monai/transforms/croppad/batch.py,sha256=0JMO2XSwS9LuM1oiogoPl9HfEBpNbcw-OyrUEXFY5rM,6194
-monai/transforms/croppad/dictionary.py,sha256=sISSreih2ku8MOFBO1fGg_3CD4WJDP3ICdqXOAoz6HI,53819
+monai/transforms/croppad/dictionary.py,sha256=8IHu2L6rU_RBgIOq_gd4TbKjOThuuXPzkSeAx7Lu9HA,54071
 monai/transforms/croppad/functional.py,sha256=XWJx8URCgkSLBUH3InD48QFcJ_YvAhVC4QNdjrs1c2c,12673
 monai/transforms/intensity/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/intensity/array.py,sha256=GnuSE0yc-YHCNn8BRGzVrMQ50b5rn-GUXHWjFQZH_Qs,98613
 monai/transforms/intensity/dictionary.py,sha256=-W9HVPA2VQUrqplmcI43Qo8EJXgMXARgcRmlhDasM0k,76501
 monai/transforms/io/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/io/array.py,sha256=7DUqkN5P2qYrUOA2wngcltYWAGmWCN45lr3nZMvrxw4,25430
 monai/transforms/io/dictionary.py,sha256=QKQSRnmHLPLZFnmaSERTAUUI3c0J9K4RwSsWv_rts00,17821
 monai/transforms/lazy/__init__.py,sha256=SvkdIlyzIDgO8oaGIrTr1YcLTjh2mZ510ySc9tEbRpk,699
 monai/transforms/lazy/functional.py,sha256=oeHyM_HcL8EhwhCXamEWYUZUlHAXUGKjSsZl1x4URJQ,5552
-monai/transforms/lazy/utils.py,sha256=caNmBikrT899FcA8aFCDUyQpT6WTXykH6D6CTgrdlTY,9551
+monai/transforms/lazy/utils.py,sha256=iNy9RH17_EOAd8F7G2v8oa6FP6L4Jz4aKN_LVUtiNIw,9739
 monai/transforms/meta_utility/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/meta_utility/dictionary.py,sha256=YqbYeZOi4cFEmEPmrw2VIpOIwre6wxYB2UGZSrf-MoM,4896
 monai/transforms/post/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/post/array.py,sha256=Yb_qbOGoaQZFp7CpOA-4iZXvAxz3RtmDlhoPFNh3jWg,40858
 monai/transforms/post/dictionary.py,sha256=OaB9YzrJe0FztM9PETSXNNIihDiad1hnbNqnon7Mp2U,39905
 monai/transforms/signal/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/signal/array.py,sha256=gmTqVYcpsK74UaVbbIjpNFLS1emC_HrQR_AQL0H_GSE,16378
 monai/transforms/smooth_field/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
 monai/transforms/smooth_field/array.py,sha256=T_TfWUDpDi8rQMFuNI6VZNsWPPUUtXM6dkTwz0C34Ow,17833
 monai/transforms/smooth_field/dictionary.py,sha256=iU4V2VjSy2H1K03KgumMUr3cyZVWEJS0W-tgc6SZtP4,11194
 monai/transforms/spatial/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
-monai/transforms/spatial/array.py,sha256=IaCFtnPFT55NPn4zcuJFkeDLfWt3IXkpwaQXOWm1Ox8,168592
+monai/transforms/spatial/array.py,sha256=Kb31oLKWr0Ccn2tKpirQta9_fM2EaMdfKggGkpLoPbI,168618
 monai/transforms/spatial/dictionary.py,sha256=4glbxbo4Cb0SbujSr9Fsk-OOLWR6yxiTQ_6LNcxll-s,107151
 monai/transforms/spatial/functional.py,sha256=Yr5Y93djwatUdoubmj_3I4_NnKF8QoF_X3FnYlTtCoU,31494
 monai/transforms/utility/__init__.py,sha256=s9djSd6kvViPnFvMR11Dgd30Lv4oY6FaPJr4ZZJZLq0,573
-monai/transforms/utility/array.py,sha256=Q7ywQuZCojEzyTnLOdixr4yJ5St6ErSBiHqOkWEo7XI,69977
-monai/transforms/utility/dictionary.py,sha256=X7V94ATq0gWaFVYqZ031mrOTYy4I7wRYFOiSaD5hY-M,75587
+monai/transforms/utility/array.py,sha256=XOmxF_8sMcE7bavWUTjkst_zjx6af6DuUVU7jWueNKU,70325
+monai/transforms/utility/dictionary.py,sha256=MGcIVsjIj8Pm_h_H8txfLQ70IgPFGEUsdL8PYwsig5M,75816
 monai/utils/__init__.py,sha256=CHO02RotqHQrQQWeSwC9boO8PW93ZI3A36O9lkzJBtI,3366
 monai/utils/aliases.py,sha256=21E1KGE6ZMWVYbRMXWVtut2fC9qs7U6QFarxOQa4s6A,4099
 monai/utils/decorators.py,sha256=YRK5iEMdbc2INrWnBNDSMTaHge_0ezRf2b9yJGL-opg,3129
 monai/utils/deprecate_utils.py,sha256=gKeEV4MsI51qeQ5gci2me_C-0e-tDwa3VZzd3XPQqLk,14759
 monai/utils/dist.py,sha256=DHLwTqVqFkxP0NbOQ3kkWd-1IQuvf5_rKKABSUQ-Bs0,8526
-monai/utils/enums.py,sha256=KgtwTI0-pJJsh_ajmB4cM9xNKPlIx1e-q229RFiGVbs,16215
+monai/utils/enums.py,sha256=ePkeJe5oPVsPJ5QycXyqsLed0DinlX-83bn0rJPH_Mw,16807
 monai/utils/jupyter_utils.py,sha256=F-QSbGDtHnR8FYnh6PsU2hC0nU6GOpGa4GneOeGiP9Y,15637
-monai/utils/misc.py,sha256=8g_0oVP8E8joQHUa6pdPtHsjPneI85yWIqYbOFl3_hc,24927
-monai/utils/module.py,sha256=1UTPMZKDVHnP_UbtYd90UnYjtANw276aVQnvVdsbIlo,23560
+monai/utils/misc.py,sha256=t6JGy38QlppWA6cuVsTdJzW1IL4-HGvuJNaNM4a9x5A,27512
+monai/utils/module.py,sha256=G_DwRNvTGxOeFmvNJIAzfDD_Ft7-4dRfkC-5ifW3kEM,23631
 monai/utils/nvtx.py,sha256=i9JBxR1uhW1ZCgLPLlTx8b907QlXkFzJyTBLMlFjhtU,6876
 monai/utils/profiling.py,sha256=HwP5q-OGebATkqPs4IMY6D7jfq2dSVf2AI6Jz_WbBkU,15936
 monai/utils/state_cacher.py,sha256=ERBE-mnnf47MwKSq-pNbfu1D2C4ZqKH-mORyLaBa3EE,5955
-monai/utils/type_conversion.py,sha256=tssPNqdU3izO0SCdwhNMfvt0umiv0fpXeEO3bVgwta4,21127
+monai/utils/type_conversion.py,sha256=ELgFzH78a2ovAVK4882CFJG1vE0_FLv77tB0lfjxM5w,21147
 monai/visualize/__init__.py,sha256=p7dv9-hRa9vAhlpHyk86yap9HgeDeJRO3pXmFhDx8Mc,1038
 monai/visualize/class_activation_maps.py,sha256=9BXlP-laeqz9rndM08DXZz97NzJcEsFPdC67k0B4CF8,16156
 monai/visualize/gradient_based.py,sha256=UInBLirXMr44xjxJRInlYW8onO3Zv58rDTWrZMDQzMM,6277
 monai/visualize/img2tensorboard.py,sha256=_p5olAefUs6t-y17z0TK32fKxNnUNXVkb0Op1SkfLMM,9200
 monai/visualize/occlusion_sensitivity.py,sha256=g3Au0X6LXoGKY9gPeuNWvNuFtynmPiUWgs_veCEIb_Q,18816
 monai/visualize/utils.py,sha256=xJbG68R-W17aqm0cpmMrypbZaiVfUaG9GWMFtKV7VUo,9966
 monai/visualize/visualizer.py,sha256=qckyaMZCbezYUwE20k5yc-Pb7UozVavMDbrmyQwfYHY,1377
-monai-1.2.0rc3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-monai-1.2.0rc3.dist-info/METADATA,sha256=y5ZOWbH8MKsOsyws4aqV4UKgBHC1ODDfR55elFYdEEI,9782
-monai-1.2.0rc3.dist-info/WHEEL,sha256=0h21Y7oqvIL-9QbJF1g3jP2rD5J3zEtwU-dXgjYrodE,112
-monai-1.2.0rc3.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
-monai-1.2.0rc3.dist-info/RECORD,,
+monai-1.2.0rc4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+monai-1.2.0rc4.dist-info/METADATA,sha256=fAE0BgtqM3KQTlwTmidpvplbQ6rylinwAJ9O_EalKLA,10172
+monai-1.2.0rc4.dist-info/WHEEL,sha256=4eiHlt0TVen4nP2Hk3uswqTjaQx4-AtDU2XnmdNg0Pw,112
+monai-1.2.0rc4.dist-info/top_level.txt,sha256=UaNwRzLGORdus41Ip446s3bBfViLkdkDsXDo34J2P44,6
+monai-1.2.0rc4.dist-info/RECORD,,
```

