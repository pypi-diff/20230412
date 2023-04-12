# Comparing `tmp/truss-0.4.1.tar.gz` & `tmp/truss-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.1.tar", max compression
+gzip compressed data, was "truss-0.4.2.tar", max compression
```

## Comparing `truss-0.4.1.tar` & `truss-0.4.2.tar`

### file list

```diff
@@ -1,174 +1,156 @@
--rw-r--r--   0        0        0     5483 2023-03-16 23:42:08.954956 truss-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-03-16 23:42:08.954956 truss-0.4.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-03-16 23:42:08.954956 truss-0.4.1/LICENSE
--rw-r--r--   0        0        0     5958 2023-03-16 23:42:08.954956 truss-0.4.1/README.md
--rw-r--r--   0        0        0     3316 2023-03-16 23:42:08.954956 truss-0.4.1/ROADMAP.md
--rw-r--r--   0        0        0      461 2023-03-16 23:42:08.954956 truss-0.4.1/context_builder.Dockerfile
--rw-r--r--   0        0        0     2205 2023-03-16 23:42:09.058956 truss-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      330 2023-03-16 23:42:09.058956 truss-0.4.1/truss/__init__.py
--rw-r--r--   0        0        0    13286 2023-03-16 23:42:09.058956 truss-0.4.1/truss/build.py
--rw-r--r--   0        0        0    10452 2023-03-16 23:42:09.058956 truss-0.4.1/truss/cli.py
--rw-r--r--   0        0        0     2700 2023-03-16 23:42:09.058956 truss-0.4.1/truss/constants.py
--rw-r--r--   0        0        0     1233 2023-03-16 23:42:09.058956 truss-0.4.1/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     5791 2023-03-16 23:42:09.058956 truss-0.4.1/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4507 2023-03-16 23:42:09.058956 truss-0.4.1/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1976 2023-03-16 23:42:09.058956 truss-0.4.1/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     1686 2023-03-16 23:42:09.058956 truss-0.4.1/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-03-16 23:42:09.058956 truss-0.4.1/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-03-16 23:42:09.066956 truss-0.4.1/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-03-16 23:42:09.066956 truss-0.4.1/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-03-16 23:42:09.066956 truss-0.4.1/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-03-16 23:42:09.066956 truss-0.4.1/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-03-16 23:42:09.066956 truss-0.4.1/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-03-16 23:42:09.066956 truss-0.4.1/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-03-16 23:42:09.066956 truss-0.4.1/truss/errors.py
--rw-r--r--   0        0        0      824 2023-03-16 23:42:09.066956 truss-0.4.1/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-03-16 23:42:09.066956 truss-0.4.1/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2709 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6565 2023-03-16 23:42:09.066956 truss-0.4.1/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-03-16 23:42:09.066956 truss-0.4.1/truss/notebook.py
--rw-r--r--   0        0        0     8643 2023-03-16 23:42:09.066956 truss-0.4.1/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-03-16 23:42:09.066956 truss-0.4.1/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2388 2023-03-16 23:42:09.066956 truss-0.4.1/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-03-16 23:42:09.066956 truss-0.4.1/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-03-16 23:42:09.066956 truss-0.4.1/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-03-16 23:42:09.066956 truss-0.4.1/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-03-16 23:42:09.066956 truss-0.4.1/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/__init__.py
--rw-r--r--   0        0        0     1375 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1849 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       82 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      979 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0     2616 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/docs/README.md
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     2272 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0     1173 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1696 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0     1196 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      875 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1708 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0      237 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1352 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     3318 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      733 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     4943 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      162 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0      855 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1666 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1898 2023-03-16 23:42:09.066956 truss-0.4.1/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0      216 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0      669 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0     1006 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/__init__.py
--rw-r--r--   0        0        0       85 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/common/__init__.py
--rw-r--r--   0        0        0      237 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/common/errors.py
--rw-r--r--   0        0        0      338 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/common/lib_support.py
--rw-r--r--   0        0        0     1339 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/common/logging.py
--rw-r--r--   0        0        0     3270 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/common/util.py
--rw-r--r--   0        0        0      669 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/config.yaml
--rw-r--r--   0        0        0      709 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/inference_server.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/model/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/model/dummy
--rw-r--r--   0        0        0     1006 2023-03-16 23:42:09.066956 truss-0.4.1/truss/test_data/truss_container_fs/app/model/model.py
--rw-r--r--   0        0        0     4943 2023-03-16 23:42:09.070956 truss-0.4.1/truss/test_data/truss_container_fs/app/model_wrapper.py
--rw-r--r--   0        0        0      162 2023-03-16 23:42:09.070956 truss-0.4.1/truss/test_data/truss_container_fs/app/requirements.txt
--rw-r--r--   0        0        0      138 2023-03-16 23:42:09.070956 truss-0.4.1/truss/test_data/truss_container_fs/app/shared/README.md
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.070956 truss-0.4.1/truss/test_data/truss_container_fs/app/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-03-16 23:42:09.070956 truss-0.4.1/truss/test_data/truss_container_fs/app/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/__init__.py
--rw-r--r--   0        0        0    18668 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/conftest.py
--rw-r--r--   0        0        0      783 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0      487 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0     8816 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/patch/test_patch.py
--rw-r--r--   0        0        0      394 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6937 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     1910 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_build.py
--rw-r--r--   0        0        0     1959 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_docker.py
--rw-r--r--   0        0        0     2605 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    30999 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      433 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-03-16 23:42:09.070956 truss-0.4.1/truss/tests/test_validation.py
--rw-r--r--   0        0        0     9289 2023-03-16 23:42:09.070956 truss-0.4.1/truss/truss_config.py
--rw-r--r--   0        0        0     2841 2023-03-16 23:42:09.070956 truss-0.4.1/truss/truss_gatherer.py
--rw-r--r--   0        0        0    39722 2023-03-16 23:42:09.070956 truss-0.4.1/truss/truss_handle.py
--rw-r--r--   0        0        0     5195 2023-03-16 23:42:09.070956 truss-0.4.1/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-03-16 23:42:09.070956 truss-0.4.1/truss/types.py
--rw-r--r--   0        0        0     2350 2023-03-16 23:42:09.070956 truss-0.4.1/truss/utils.py
--rw-r--r--   0        0        0     2317 2023-03-16 23:42:09.070956 truss-0.4.1/truss/validation.py
--rw-r--r--   0        0        0     7297 1970-01-01 00:00:00.000000 truss-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-04-12 20:02:08.670506 truss-0.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-04-12 20:02:08.670506 truss-0.4.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-04-12 20:02:08.670506 truss-0.4.2/LICENSE
+-rw-r--r--   0        0        0     5958 2023-04-12 20:02:08.670506 truss-0.4.2/README.md
+-rw-r--r--   0        0        0     3316 2023-04-12 20:02:08.670506 truss-0.4.2/ROADMAP.md
+-rw-r--r--   0        0        0      465 2023-04-12 20:02:08.670506 truss-0.4.2/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2205 2023-04-12 20:02:08.766507 truss-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-04-12 20:02:08.766507 truss-0.4.2/truss/__init__.py
+-rw-r--r--   0        0        0    13286 2023-04-12 20:02:08.766507 truss-0.4.2/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-04-12 20:02:08.766507 truss-0.4.2/truss/cli.py
+-rw-r--r--   0        0        0     2700 2023-04-12 20:02:08.766507 truss-0.4.2/truss/constants.py
+-rw-r--r--   0        0        0     1233 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     5791 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4507 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1976 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     1686 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-04-12 20:02:08.766507 truss-0.4.2/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-04-12 20:02:08.766507 truss-0.4.2/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-04-12 20:02:08.766507 truss-0.4.2/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-04-12 20:02:08.766507 truss-0.4.2/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-04-12 20:02:08.766507 truss-0.4.2/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-04-12 20:02:08.766507 truss-0.4.2/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-04-12 20:02:08.766507 truss-0.4.2/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2709 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6565 2023-04-12 20:02:08.766507 truss-0.4.2/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-04-12 20:02:08.766507 truss-0.4.2/truss/notebook.py
+-rw-r--r--   0        0        0     9521 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2388 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-04-12 20:02:08.766507 truss-0.4.2/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-04-12 20:02:08.766507 truss-0.4.2/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-04-12 20:02:08.766507 truss-0.4.2/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1375 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-04-12 20:02:08.766507 truss-0.4.2/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1849 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       82 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      979 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0     2616 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/docs/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     2272 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0     1173 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0     1196 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1708 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1352 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     3318 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     5511 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      416 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      733 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     4943 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      162 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0      855 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1666 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1898 2023-04-12 20:02:08.770507 truss-0.4.2/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0      216 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0      669 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0     1006 2023-04-12 20:02:08.770507 truss-0.4.2/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/__init__.py
+-rw-r--r--   0        0        0    19167 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/conftest.py
+-rw-r--r--   0        0        0      783 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0      487 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0     9348 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_patch.py
+-rw-r--r--   0        0        0      394 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-04-12 20:02:08.770507 truss-0.4.2/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6937 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     1910 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_build.py
+-rw-r--r--   0        0        0     2359 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     2605 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    31557 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      433 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-04-12 20:02:08.774507 truss-0.4.2/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     9289 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_config.py
+-rw-r--r--   0        0        0     2841 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    39722 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_handle.py
+-rw-r--r--   0        0        0     5195 2023-04-12 20:02:08.774507 truss-0.4.2/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-04-12 20:02:08.774507 truss-0.4.2/truss/types.py
+-rw-r--r--   0        0        0     2350 2023-04-12 20:02:08.774507 truss-0.4.2/truss/utils.py
+-rw-r--r--   0        0        0     2317 2023-04-12 20:02:08.774507 truss-0.4.2/truss/validation.py
+-rw-r--r--   0        0        0     7297 1970-01-01 00:00:00.000000 truss-0.4.2/PKG-INFO
```

### Comparing `truss-0.4.1/CODE_OF_CONDUCT.md` & `truss-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/CONTRIBUTING.md` & `truss-0.4.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/LICENSE` & `truss-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/README.md` & `truss-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/ROADMAP.md` & `truss-0.4.2/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/pyproject.toml` & `truss-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.1"
+version = "0.4.2"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.1/truss/build.py` & `truss-0.4.2/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/cli.py` & `truss-0.4.2/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/constants.py` & `truss-0.4.2/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/image_builder/image_builder.py` & `truss-0.4.2/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.2/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.2/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/image_builder/util.py` & `truss-0.4.2/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.2/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/local_loader/train_local.py` & `truss-0.4.2/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.2/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/contexts/local_loader/utils.py` & `truss-0.4.2/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/docker.py` & `truss-0.4.2/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/environment_inference/requirements_inference.py` & `truss-0.4.2/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/errors.py` & `truss-0.4.2/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/local/local_config.py` & `truss-0.4.2/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/local/local_config_handler.py` & `truss-0.4.2/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_framework.py` & `truss-0.4.2/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/__init__.py` & `truss-0.4.2/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.2/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/keras.py` & `truss-0.4.2/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/lightgbm.py` & `truss-0.4.2/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/mlflow.py` & `truss-0.4.2/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/pytorch.py` & `truss-0.4.2/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/sklearn.py` & `truss-0.4.2/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_frameworks/xgboost.py` & `truss-0.4.2/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/model_inference.py` & `truss-0.4.2/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/patch/calc_patch.py` & `truss-0.4.2/truss/patch/calc_patch.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,40 @@
     PatchType,
     PythonRequirementPatch,
     SystemPackagePatch,
 )
 from truss.truss_config import TrussConfig
 from truss.truss_spec import TrussSpec
 
+PYCACHE_IGNORE_PATTERNS = [
+    "**/__pycache__/**/*",
+    "**/__pycache__/**",
+]
+
 
 def calc_truss_patch(
-    truss_dir: Path, previous_truss_signature: TrussSignature
+    truss_dir: Path,
+    previous_truss_signature: TrussSignature,
+    ignore_patterns: Optional[List[str]] = None,
 ) -> Optional[List[Patch]]:
     """
     Calculate patch for a truss from a previous state.
 
     Returns: None if patch cannot be calculated, otherwise a list of patches.
         Note that the none return value is pretty important, patch coverage
         is limited and this usually indicates that the identified change cannot
         be expressed with currently supported patches.
     """
+    if ignore_patterns is None:
+        ignore_patterns = PYCACHE_IGNORE_PATTERNS
+
     changed_paths = _calc_changed_paths(
-        truss_dir, previous_truss_signature.content_hashes_by_path
+        truss_dir,
+        previous_truss_signature.content_hashes_by_path,
+        ignore_patterns,
     )
     # TODO(pankaj) Calculate model code patches only for now, add config changes
     # later.
     truss_spec = TrussSpec(truss_dir)
     model_module_path = str(truss_spec.model_module_dir.relative_to(truss_dir))
     training_module_path = str(truss_spec.training_module_dir.relative_to(truss_dir))
 
@@ -96,29 +108,29 @@
             patches.extend(config_patches)
         else:
             return None
     return patches
 
 
 def _calc_changed_paths(
-    root: Path, previous_root_path_content_hashes: Dict[str, str]
-) -> dict:
+    root: Path,
+    previous_root_path_content_hashes: Dict[str, str],
+    ignore_patterns: Optional[List[str]],
+) -> Dict[str, List[str]]:
     """
     TODO(pankaj) add support for directory creation in patch
     """
-    root_relative_paths = set(
-        (str(path.relative_to(root)) for path in root.glob("**/*"))
-    )
+    unignored_paths = _calc_unignored_paths(root, ignore_patterns)
     previous_root_relative_paths = set(previous_root_path_content_hashes.keys())
 
-    added_paths = root_relative_paths - previous_root_relative_paths
-    removed_paths = previous_root_relative_paths - root_relative_paths
+    added_paths = unignored_paths - previous_root_relative_paths
+    removed_paths = previous_root_relative_paths - unignored_paths
 
     updated_paths = set()
-    common_paths = root_relative_paths.intersection(previous_root_relative_paths)
+    common_paths = unignored_paths.intersection(previous_root_relative_paths)
     for path in common_paths:
         full_path: Path = root / path
         if full_path.is_file():
             content_hash = file_content_hash_str(full_path)
             previous_content_hash = previous_root_path_content_hashes[path]
             if content_hash != previous_content_hash:
                 updated_paths.add(path)
@@ -126,14 +138,31 @@
     return {
         "added": list(added_paths),
         "updated": list(updated_paths),
         "removed": list(removed_paths),
     }
 
 
+def _calc_unignored_paths(
+    root: Path, ignore_patterns: Optional[List[str]] = None
+) -> Set[str]:
+    root_relative_ignored_paths = set()
+    if ignore_patterns is not None:
+        for ignore_pattern in ignore_patterns:
+            ignored_paths_for_pattern = set(
+                (str(path.relative_to(root)) for path in root.glob(ignore_pattern))
+            )
+            root_relative_ignored_paths.update(ignored_paths_for_pattern)
+
+    root_relative_paths = set(
+        (str(path.relative_to(root)) for path in root.glob("**/*"))
+    )
+    return root_relative_paths - root_relative_ignored_paths
+
+
 def _calc_config_patches(
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> Optional[List[Patch]]:
     """Calculate patch based on changes to config.
 
     Returns None if patch cannot be calculated. Empty list means no relevant
     differences found.
```

### Comparing `truss-0.4.1/truss/patch/dir_signature.py` & `truss-0.4.2/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/patch/hash.py` & `truss-0.4.2/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/patch/types.py` & `truss-0.4.2/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/readme_generator.py` & `truss-0.4.2/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/README.md.jinja` & `truss-0.4.2/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/base.Dockerfile.jinja` & `truss-0.4.2/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/application.py` & `truss-0.4.2/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/endpoints.py` & `truss-0.4.2/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/helpers/errors.py` & `truss-0.4.2/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.2/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.2/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.2/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.2/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/helpers/types.py` & `truss-0.4.2/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/control/control/server.py` & `truss-0.4.2/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/custom/model/model.py` & `truss-0.4.2/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/docs/README.md` & `truss-0.4.2/truss/templates/docs/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.2/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/keras/model/model.py` & `truss-0.4.2/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/lightgbm/model/model.py` & `truss-0.4.2/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/mlflow/model/model.py` & `truss-0.4.2/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/pipeline/model/model.py` & `truss-0.4.2/truss/templates/pipeline/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/pytorch/model/model.py` & `truss-0.4.2/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/server/common/logging.py` & `truss-0.4.2/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/server/common/serialization.py` & `truss-0.4.2/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/server/common/truss_server.py` & `truss-0.4.2/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/server/inference_server.py` & `truss-0.4.2/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/server/model_wrapper.py` & `truss-0.4.2/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/server.Dockerfile.jinja` & `truss-0.4.2/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/shared/secrets_resolver.py` & `truss-0.4.2/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/sklearn/model/model.py` & `truss-0.4.2/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/training/job.py` & `truss-0.4.2/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/templates/xgboost/model/model.py` & `truss-0.4.2/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/auto-mpg.data` & `truss-0.4.2/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/happy.ipynb` & `truss-0.4.2/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.2/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.2/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/readme_int_example.md` & `truss-0.4.2/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/readme_no_example.md` & `truss-0.4.2/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/readme_str_example.md` & `truss-0.4.2/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/test_truss/config.yaml` & `truss-0.4.2/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/test_truss/model/model.py` & `truss-0.4.2/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/test_data/truss_container_fs/app/shared/secrets_resolver.py` & `truss-0.4.2/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 import os
-from collections.abc import Mapping
+from contextlib import contextmanager
 from pathlib import Path
-from typing import Dict
 
+from truss.templates.shared.secrets_resolver import SecretsResolver
 
-class SecretsResolver:
-    SECRETS_MOUNT_DIR = "/secrets"
-    SECRET_ENV_VAR_PREFIX = "TRUSS_SECRET_"
-
-    @staticmethod
-    def get_secrets(config: dict):
-        return Secrets(config.get("secrets", {}))
-
-    @staticmethod
-    def _resolve_secret(secret_name: str, default_value: str):
-        secret_value = default_value
-        secret_env_var_name = SecretsResolver.SECRET_ENV_VAR_PREFIX + secret_name
-        if secret_env_var_name in os.environ:
-            secret_value = os.environ[secret_env_var_name]
-        secret_path = SecretsResolver._secrets_mount_dir_path() / secret_name
-        if secret_path.exists() and secret_path.is_file():
-            with secret_path.open() as secret_file:
-                secret_value = secret_file.read()
-        return secret_value
-
-    @staticmethod
-    def _secrets_mount_dir_path():
-        return Path(SecretsResolver.SECRETS_MOUNT_DIR)
-
-
-class Secrets(Mapping):
-    def __init__(self, base_secrets: Dict[str, str]):
-        self._base_secrets = base_secrets
-
-    def __getitem__(self, key: str) -> str:
-        return SecretsResolver._resolve_secret(key, self._base_secrets[key])
-
-    def __iter__(self):
-        raise NotImplementedError(
-            "Secrets are meant for lookup and can't be iterated on"
-        )
+CONFIG = {"secrets": {"secret_key": "default_secret_value"}}
 
-    def __len__(self):
-        return len(self._base_secrets)
+
+def test_resolve_default_value():
+    secrets = SecretsResolver.get_secrets(CONFIG)
+    assert secrets["secret_key"] == "default_secret_value"
+
+
+def test_resolve_env_var():
+    secrets = SecretsResolver.get_secrets(CONFIG)
+    with _override_env_var("TRUSS_SECRET_secret_key", "secret_value_from_env"):
+        assert secrets["secret_key"] == "secret_value_from_env"
+
+
+def test_resolve_mounted_secrets(tmp_path):
+    secrets = SecretsResolver.get_secrets(CONFIG)
+    with (tmp_path / "secret_key").open("w") as f:
+        f.write("secret_value_from_mounted_secrets")
+    with _secrets_mount_dir(tmp_path), _override_env_var(
+        "TRUSS_SECRET_secret_key", "secret_value_from_env"
+    ):
+        assert secrets["secret_key"] == "secret_value_from_mounted_secrets"
+
+
+@contextmanager
+def _secrets_mount_dir(path: Path):
+    orig_secrets_mount_dir = SecretsResolver.SECRETS_MOUNT_DIR
+    SecretsResolver.SECRETS_MOUNT_DIR = str(path)
+    try:
+        yield
+    finally:
+        SecretsResolver.SECRETS_MOUNT_DIR = orig_secrets_mount_dir
+
+
+@contextmanager
+def _override_env_var(key: str, value: str):
+    orig_value = os.environ.get(key, None)
+    try:
+        os.environ[key] = value
+        yield
+    finally:
+        if orig_value is not None:
+            os.environ[key] = orig_value
+        else:
+            del os.environ[key]
```

### Comparing `truss-0.4.1/truss/tests/conftest.py` & `truss-0.4.2/truss/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import contextlib
 import importlib
 import os
-import shutil
 import subprocess
 import sys
 import time
 from pathlib import Path
 
 import lightgbm as lgb
 import numpy as np
@@ -656,19 +655,33 @@
     with handle.spec.model_class_filepath.open("w") as file:
         file.write(CUSTOM_MODEL_CODE_FOR_SECRETS_TESTING)
     yield dir_path
 
 
 @pytest.fixture
 def truss_container_fs(tmp_path):
+    ROOT = str(Path(__file__).parent.parent.parent.resolve())
+    subprocess.run(["truss", "run-image", "truss/test_data/test_truss"], cwd=ROOT)
     truss_fs = tmp_path / "truss_fs"
-    truss_fs_test_data_path = (
-        Path(__file__).parent.parent / "test_data" / "truss_container_fs"
+    truss_fs.mkdir()
+
+    ps_output = subprocess.check_output(
+        [
+            "docker",
+            "ps",
+            "--filter",
+            "label=truss_dir=truss/test_data/test_truss",
+            "--format",
+            "'{{.Names}},{{.Image}}'",
+        ]
     )
-    shutil.copytree(str(truss_fs_test_data_path), str(truss_fs))
+    container_name, image = ps_output.decode("utf-8").strip()[1:-1].split(",")
+    subprocess.run(["docker", "cp", f"{container_name}:/app", str(truss_fs / "app")])
+    subprocess.run(["docker", "kill", container_name])
+    subprocess.run(["docker", "rmi", image, "-f"])
     return truss_fs
 
 
 @pytest.fixture
 def patch_ping_test_server():
     port = "5001"
     proc = subprocess.Popen(
```

### Comparing `truss-0.4.1/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.2/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.2/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.2/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/local/test_local_config_handler.py` & `truss-0.4.2/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.2/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.2/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.2/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.2/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.2/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.2/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/patch/test_hash.py` & `truss-0.4.2/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/patch/test_patch.py` & `truss-0.4.2/truss/tests/patch/test_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,30 @@
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE, path="model.py", content=new_model_file_content
         ),
     )
 
 
+def test_calc_truss_ignore_pycache(custom_model_truss_dir: Path):
+    prev_sign = calc_truss_signature(custom_model_truss_dir)
+    top_pycache_path = custom_model_truss_dir / "__pycache__"
+    top_pycache_path.mkdir()
+    (top_pycache_path / "bla.pyc").touch()
+    model_pycache_path = custom_model_truss_dir / "model" / "__pycache__"
+    model_pycache_path.mkdir()
+    (model_pycache_path / "foo.pyo").touch()
+
+    patches = calc_truss_patch(
+        custom_model_truss_dir,
+        prev_sign,
+    )
+    assert len(patches) == 0
+
+
 def test_calc_config_patches_add_python_requirement(custom_model_truss_dir: Path):
     patches = _apply_config_change_and_calc_patches(
         custom_model_truss_dir,
         lambda config: config.requirements.append("requests==1.0.0"),
     )
     assert len(patches) == 1
     patch = patches[0]
```

### Comparing `truss-0.4.1/truss/tests/samples.py` & `truss-0.4.2/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.2/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/templates/control/control/test_server.py` & `truss-0.4.2/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.2/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_backward.py` & `truss-0.4.2/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_build.py` & `truss-0.4.2/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_config.py` & `truss-0.4.2/truss/tests/test_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,7 +64,20 @@
         ),
     ],
 )
 def test_parse_resources(input_dict, expect_resources, output_dict):
     parsed_result = Resources.from_dict(input_dict)
     assert parsed_result == expect_resources
     assert parsed_result.to_dict() == output_dict
+
+
+@pytest.mark.parametrize(
+    "input_str, expected_acc",
+    [
+        (None, AcceleratorSpec(None, 0)),
+        ("T4", AcceleratorSpec(Accelerator.T4, 1)),
+        ("A10G:4", AcceleratorSpec(Accelerator.A10G, 4)),
+        ("A100:8", AcceleratorSpec(Accelerator.A100, 8)),
+    ],
+)
+def test_acc_spec_from_str(input_str, expected_acc):
+    assert AcceleratorSpec.from_str(input_str) == expected_acc
```

### Comparing `truss-0.4.1/truss/tests/test_context_builder_image.py` & `truss-0.4.2/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_docker.py` & `truss-0.4.2/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_model_inference.py` & `truss-0.4.2/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_notebooks.py` & `truss-0.4.2/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.2/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_truss_gatherer.py` & `truss-0.4.2/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/tests/test_truss_handle.py` & `truss-0.4.2/truss/tests/test_truss_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -687,14 +687,23 @@
         th.add_system_package(pkg)
         return th.docker_predict([1], tag=tag, binary=binary)
 
     def predict_with_system_requirement_removed(pkg):
         th.remove_system_package(pkg)
         return th.docker_predict([1], tag=tag, binary=binary)
 
+    def predict_with_ignored_changes():
+        top_pycache_path = custom_model_control / "__pycache__"
+        top_pycache_path.mkdir()
+        (top_pycache_path / "bla.pyc").touch()
+        model_pycache_path = custom_model_control / "model" / "__pycache__"
+        model_pycache_path.mkdir()
+        (model_pycache_path / "foo.pyc").touch()
+        return th.docker_predict([1], tag=tag, binary=binary)
+
     def current_num_docker_images() -> int:
         return len(th.get_all_docker_images())
 
     with ensure_kill_all():
         result = th.docker_predict([1], tag=tag, binary=binary)
         assert result[0] == 1
         orig_num_truss_images = len(th.get_all_docker_images())
@@ -731,14 +740,18 @@
         assert current_num_docker_images() == orig_num_truss_images
         _verify_system_requirement_not_installed_on_container(container, system_pkg)
 
         result = predict_with_unpatchable_change()
         assert result[0] == 2
         assert current_num_docker_images() == orig_num_truss_images + 1
 
+        result = predict_with_ignored_changes()
+        assert result[0] == 2
+        assert current_num_docker_images() == orig_num_truss_images + 1
+
 
 @pytest.mark.integration
 def test_control_truss_huggingface(
     huggingface_truss_handle_small_model,
 ):
     th = TrussHandle(huggingface_truss_handle_small_model)
     th.live_reload()
```

### Comparing `truss-0.4.1/truss/tests/test_validation.py` & `truss-0.4.2/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/truss_config.py` & `truss-0.4.2/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/truss_gatherer.py` & `truss-0.4.2/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/truss_handle.py` & `truss-0.4.2/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/truss_spec.py` & `truss-0.4.2/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/types.py` & `truss-0.4.2/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/utils.py` & `truss-0.4.2/truss/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/truss/validation.py` & `truss-0.4.2/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.1/PKG-INFO` & `truss-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.1
+Version: 0.4.2
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.11
```

