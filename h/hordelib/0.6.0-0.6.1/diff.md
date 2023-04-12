# Comparing `tmp/hordelib-0.6.0.tar.gz` & `tmp/hordelib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.6.0.tar", last modified: Wed Apr 12 12:41:24 2023, max compression
+gzip compressed data, was "hordelib-0.6.1.tar", last modified: Wed Apr 12 16:29:59 2023, max compression
```

## Comparing `hordelib-0.6.0.tar` & `hordelib-0.6.1.tar`

### file list

```diff
@@ -1,640 +1,639 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.225544 hordelib-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 12:40:58.000000 hordelib-0.6.0/.changelog
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-12 12:40:58.000000 hordelib-0.6.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 12:40:58.000000 hordelib-0.6.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.093541 hordelib-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.109542 hordelib-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 12:40:58.000000 hordelib-0.6.0/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-12 12:40:58.000000 hordelib-0.6.0/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-12 12:40:58.000000 hordelib-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-12 12:40:58.000000 hordelib-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    16762 2023-04-12 12:41:11.000000 hordelib-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-12 12:40:58.000000 hordelib-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48216 2023-04-12 12:41:24.225544 hordelib-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-12 12:40:58.000000 hordelib-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-12 12:40:58.000000 hordelib-0.6.0/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.109542 hordelib-0.6.0/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 12:41:23.000000 hordelib-0.6.0/hordelib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.113541 hordelib-0.6.0/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.113541 hordelib-0.6.0/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/clip/interrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15010 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.117542 hordelib-0.6.0/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/blip.json
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/codeformer.json
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/db.json
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/safety_checker.json
--rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_database/stable_diffusion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.117542 hordelib-0.6.0/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/model_manager/torch_hijack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.117542 hordelib-0.6.0/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.121542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.125542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.125542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.125542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.125542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.097541 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.129542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.133542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.137542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.137542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.097541 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.137542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.141542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.141542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.141542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.145542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.145542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.149542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.149542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.149542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.153542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.153542 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.161543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.165543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.165543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.169543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.169543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.173543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.173543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.177543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.177543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.177543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.105541 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.177543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.177543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.177543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.177543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.181543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.181543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.181543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.185543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.185543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.185543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.193543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.193543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.193543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.197543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.197543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.197543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.201543 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.201543 hordelib-0.6.0/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.201543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.201543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.201543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.201543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.205543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.205543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.205543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.205543 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.209544 hordelib-0.6.0/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.209544 hordelib-0.6.0/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/run_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/shared_model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.209544 hordelib-0.6.0/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/utils/ioredirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 12:40:58.000000 hordelib-0.6.0/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.109542 hordelib-0.6.0/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48216 2023-04-12 12:41:23.000000 hordelib-0.6.0/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38574 2023-04-12 12:41:24.000000 hordelib-0.6.0/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:41:23.000000 hordelib-0.6.0/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 12:41:23.000000 hordelib-0.6.0/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 12:41:23.000000 hordelib-0.6.0/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.217544 hordelib-0.6.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-12 12:40:58.000000 hordelib-0.6.0/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-12 12:41:14.000000 hordelib-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 12:40:58.000000 hordelib-0.6.0/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 12:41:14.000000 hordelib-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:41:24.225544 hordelib-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.225544 hordelib-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/make_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:41:24.225544 hordelib-0.6.0/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_img2img_inpaint_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/run_upscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_comfy_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 12:40:58.000000 hordelib-0.6.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 12:40:58.000000 hordelib-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:59.004231 hordelib-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 16:29:43.000000 hordelib-0.6.1/.changelog
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-12 16:29:43.000000 hordelib-0.6.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.920230 hordelib-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.932230 hordelib-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 16:29:43.000000 hordelib-0.6.1/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-12 16:29:43.000000 hordelib-0.6.1/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-12 16:29:43.000000 hordelib-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-12 16:29:43.000000 hordelib-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18366 2023-04-12 16:29:49.000000 hordelib-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-12 16:29:43.000000 hordelib-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48935 2023-04-12 16:29:59.004231 hordelib-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-04-12 16:29:43.000000 hordelib-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-12 16:29:43.000000 hordelib-0.6.1/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.932230 hordelib-0.6.1/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 16:29:58.000000 hordelib-0.6.1/hordelib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.932230 hordelib-0.6.1/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.936230 hordelib-0.6.1/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/clip/interrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.936230 hordelib-0.6.1/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/blip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/codeformer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/safety_checker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_database/stable_diffusion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.936230 hordelib-0.6.1/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24866 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/model_manager/torch_hijack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.940230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.944230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.948230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.948230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.948230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.924230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.948230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.948230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.952230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.952230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.924230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.952230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.952230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.952230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.952230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.956230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.956230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.956230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.960230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.960230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.960230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.960230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.964230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.968230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.968230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.972231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.972231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.972231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.928230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.976230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.980230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.980230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.980230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.980230 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.984231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.984231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.988231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.992231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.992231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.992231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.992231 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.992231 hordelib-0.6.1/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.996231 hordelib-0.6.1/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/run_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/shared_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.996231 hordelib-0.6.1/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/utils/ioredirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-12 16:29:43.000000 hordelib-0.6.1/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:58.932230 hordelib-0.6.1/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48935 2023-04-12 16:29:58.000000 hordelib-0.6.1/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38566 2023-04-12 16:29:58.000000 hordelib-0.6.1/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 16:29:58.000000 hordelib-0.6.1/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 16:29:58.000000 hordelib-0.6.1/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-12 16:29:58.000000 hordelib-0.6.1/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:59.000231 hordelib-0.6.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-12 16:29:43.000000 hordelib-0.6.1/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-12 16:29:43.000000 hordelib-0.6.1/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-12 16:29:43.000000 hordelib-0.6.1/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-12 16:29:43.000000 hordelib-0.6.1/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-12 16:29:44.000000 hordelib-0.6.1/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-12 16:29:44.000000 hordelib-0.6.1/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-12 16:29:44.000000 hordelib-0.6.1/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-12 16:29:44.000000 hordelib-0.6.1/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-04-12 16:29:51.000000 hordelib-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 16:29:44.000000 hordelib-0.6.1/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 16:29:51.000000 hordelib-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 16:29:59.004231 hordelib-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:59.004231 hordelib-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/make_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 16:29:59.004231 hordelib-0.6.1/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/model_managers/test_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_img2img_inpaint_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/run_upscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_comfy_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 16:29:44.000000 hordelib-0.6.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-12 16:29:44.000000 hordelib-0.6.1/tox.ini
```

### Comparing `hordelib-0.6.0/.changelog` & `hordelib-0.6.1/.changelog`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/.github/workflows/maintests.yml` & `hordelib-0.6.1/.github/workflows/maintests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/.github/workflows/prtests.yml` & `hordelib-0.6.1/.github/workflows/prtests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/.github/workflows/release.yml` & `hordelib-0.6.1/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       if: ${{ steps.release.outputs.version != '' }}
       uses: actions/setup-node@v3
 
     - name: "✏️ Generate release changelog"
       if: ${{ steps.release.outputs.version != '' }}
       run: |
         npm -g install auto-changelog
-        auto-changelog --template=.changelog --ignore-commit-pattern="update changelog" --ignore-commit-pattern="version bump"
+        auto-changelog --template=.changelog --ignore-commit-pattern="update changelog" --ignore-commit-pattern="version bump" --ignore-commit-pattern="Merge pull"
 
     # Try to add the changelog back to the releases branch
     - uses: EndBug/add-and-commit@v9
       with:
         add: 'CHANGELOG.md'
         message: 'ci: update changelog'
         committer_name: GitHub Actions
```

### Comparing `hordelib-0.6.0/.gitignore` & `hordelib-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/CHANGELOG.md` & `hordelib-0.6.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,198 +1,207 @@
 ## hordelib Changelog
 
+## [v0.6.1](https://github.com/jug-dev/hordelib/compare/v0.6.0...v0.6.1)
+
+12 April 2023
+
+- feat: make logging setup and control optional [`#106`](https://github.com/jug-dev/hordelib/pull/106) (Jug)
+- style: Automatic formatting/lint with length 119 [`845764a`](https://github.com/jug-dev/hordelib/commit/845764ad5765f2b4e7c442a25f421af493fc7c88)  (tazlin)
+- docs: cleanup readme for viewing in an editor [`76a7f7f`](https://github.com/jug-dev/hordelib/commit/76a7f7f7198da1f988d1972e2b9082944b97af3a)  (Jug)
+- ci: update changelog [`ef7b248`](https://github.com/jug-dev/hordelib/commit/ef7b248703b10d9a43646b9a223e61f6fbba85db)  (jug-dev)
+
 ## [v0.6.0](https://github.com/jug-dev/hordelib/compare/v0.5.24...v0.6.0)
 
 12 April 2023
 
 - fix: suppress terminal spam [`#104`](https://github.com/jug-dev/hordelib/pull/104) (Jug)
 - feat: add support for separate source_mask [`#103`](https://github.com/jug-dev/hordelib/pull/103) (Jug)
-- Merge pull request #105 from jug-dev/main [`b2c6825`](https://github.com/jug-dev/hordelib/commit/b2c68254996ba0a51d0c1c2e7be3ef03b3e4c1cf)  (Jug)
 - ci: update changelog [`390be6d`](https://github.com/jug-dev/hordelib/commit/390be6d06b6f1ca044cdfdc3478d2165963f3825)  (jug-dev)
+- ci: ignore old version bump commits [`ecd1107`](https://github.com/jug-dev/hordelib/commit/ecd11079e38029bd3026fe8b91becf8e0971ea8e)  (Jug)
 
 ## [v0.5.24](https://github.com/jug-dev/hordelib/compare/v0.5.23...v0.5.24)
 
 12 April 2023
 
-- ci: include changelog link on pypi page [`#101`](https://github.com/jug-dev/hordelib/pull/101) (Jug)
 - ci: update changelog [`f40bea4`](https://github.com/jug-dev/hordelib/commit/f40bea47e3d9827f267b101bdce9260cb2a354e9)  (jug-dev)
+- ci: include changelog link on pypi page [`a617c23`](https://github.com/jug-dev/hordelib/commit/a617c2381a46b9e3b421074dfb5162c3a600c131)  (Jug)
 
 ## [v0.5.23](https://github.com/jug-dev/hordelib/compare/v0.5.22...v0.5.23)
 
 12 April 2023
 
-- ci: customise the changelog format [`#100`](https://github.com/jug-dev/hordelib/pull/100) (Jug)
 - ci: update changelog [`3f2d6c7`](https://github.com/jug-dev/hordelib/commit/3f2d6c7cab87547971b2f93860f543c227f37512)  (jug-dev)
+- ci: customise the changelog format [`c85285a`](https://github.com/jug-dev/hordelib/commit/c85285ab213862d32dde591cbf714e2d2c3dd3ba)  (Jug)
 
 ## [v0.5.22](https://github.com/jug-dev/hordelib/compare/v0.5.21...v0.5.22)
 
 12 April 2023
 
-- ci: auto update changelog in releases branch [`#99`](https://github.com/jug-dev/hordelib/pull/99) (Jug)
+- ci: auto update changelog in releases branch [`6e775bd`](https://github.com/jug-dev/hordelib/commit/6e775bd52137b013c4e793553d1c4cddee8b6d66)  (Jug)
 
 ## [v0.5.21](https://github.com/jug-dev/hordelib/compare/v0.5.20...v0.5.21)
 
 12 April 2023
 
-- ci: try to generate changelog for the right version [`#98`](https://github.com/jug-dev/hordelib/pull/98) (Jug)
+- ci: try to generate changelog for the right version [`2b86531`](https://github.com/jug-dev/hordelib/commit/2b865314cb8f6f387e181a87771739cf983f1fa6)  (Jug)
 
 ## [v0.5.20](https://github.com/jug-dev/hordelib/compare/v0.5.19...v0.5.20)
 
 12 April 2023
 
-- ci: ci again [`#97`](https://github.com/jug-dev/hordelib/pull/97) (Jug)
-- ci: more tweaks [`#96`](https://github.com/jug-dev/hordelib/pull/96) (Jug)
-- ci: try a better changelog generator [`#95`](https://github.com/jug-dev/hordelib/pull/95) (Jug)
+- ci: try a better changelog generator [`a03b5fc`](https://github.com/jug-dev/hordelib/commit/a03b5fcd052269451004e4c9f45ef5775f5331d8)  (Jug)
+- ci: more tweaks [`81ac9b5`](https://github.com/jug-dev/hordelib/commit/81ac9b587fdeacf1159c9a01f7ef9c06a24bcc52)  (Jug)
+- ci: ci again [`a185c41`](https://github.com/jug-dev/hordelib/commit/a185c410e3cadcd56bd5b2d63712abd2859884e5)  (Jug)
 
 ## [v0.5.19](https://github.com/jug-dev/hordelib/compare/v0.5.18...v0.5.19)
 
 12 April 2023
 
-- ci: changelog wasn't include in setuptools [`#94`](https://github.com/jug-dev/hordelib/pull/94) (Jug)
+- ci: changelog wasn't include in setuptools [`652e53c`](https://github.com/jug-dev/hordelib/commit/652e53cf4db43e6e5502edc05b299da3e8f63644)  (Jug)
 
 ## [v0.5.18](https://github.com/jug-dev/hordelib/compare/v0.5.17...v0.5.18)
 
 11 April 2023
 
-- ci: release ci tweaks [`#93`](https://github.com/jug-dev/hordelib/pull/93) (Jug)
+- ci: release ci tweaks [`1adf7ce`](https://github.com/jug-dev/hordelib/commit/1adf7ce5d1c607ea04011803324e20b26e348a3c)  (Jug)
 
 ## [v0.5.17](https://github.com/jug-dev/hordelib/compare/v0.5.16...v0.5.17)
 
 11 April 2023
 
-- release: patch release [`#92`](https://github.com/jug-dev/hordelib/pull/92) (Jug)
-- style: Incremental formatting lint catchup [`#88`](https://github.com/jug-dev/hordelib/pull/88) (tazlin)
 - style: Incremental style/lint catchup [`1cb70d2`](https://github.com/jug-dev/hordelib/commit/1cb70d2eb3c219bff304c4ed0ac34f7456946281)  (tazlin)
 - ci: Enables a couple ruff rules for CI [`17bd0f8`](https://github.com/jug-dev/hordelib/commit/17bd0f8b1cfd73f3e1429ad4c9b007623517de35)  (tazlin)
 - ci: another day another way to do changelogs [`6e7ed60`](https://github.com/jug-dev/hordelib/commit/6e7ed604fee66388570b9e953f25599d49a3bc9a)  (Jug)
 
 ## [v0.5.16](https://github.com/jug-dev/hordelib/compare/v0.5.15...v0.5.16)
 
 11 April 2023
 
-- ci: more ci tweaks [`#91`](https://github.com/jug-dev/hordelib/pull/91) (Jug)
+- ci: more ci tweaks [`7bbc0c3`](https://github.com/jug-dev/hordelib/commit/7bbc0c3491c12e00ee54fa5f96e73fcf801ae6f7)  (Jug)
 
 ## [v0.5.15](https://github.com/jug-dev/hordelib/compare/v0.5.14...v0.5.15)
 
 11 April 2023
 
-- ci: this is never going to work is it [`#90`](https://github.com/jug-dev/hordelib/pull/90) (Jug)
+- ci: this is never going to work is it [`797a317`](https://github.com/jug-dev/hordelib/commit/797a3172666e4eab9fe88bc22307e7ee84063441)  (Jug)
 
 ## [v0.5.14](https://github.com/jug-dev/hordelib/compare/v0.5.13...v0.5.14)
 
 11 April 2023
 
-- ci: another day another ci hack [`#89`](https://github.com/jug-dev/hordelib/pull/89) (Jug)
+- ci: another day another ci hack [`bf007ac`](https://github.com/jug-dev/hordelib/commit/bf007ace0740eeebf17dd95013d5d68cf332a209)  (Jug)
 
 ## [v0.5.13](https://github.com/jug-dev/hordelib/compare/v0.5.12...v0.5.13)
 
 11 April 2023
 
-- ci: optimistically try to output a changelog [`#87`](https://github.com/jug-dev/hordelib/pull/87) (Jug)
+- ci: optimistically try to output a changelog [`cfc71a2`](https://github.com/jug-dev/hordelib/commit/cfc71a28468b391e70bd85a8b3b57550f51ec328)  (Jug)
 
 ## [v0.5.12](https://github.com/jug-dev/hordelib/compare/v0.5.11...v0.5.12)
 
 11 April 2023
 
-- ci: Try harder to generate a changelog [`#86`](https://github.com/jug-dev/hordelib/pull/86) (Jug)
+- ci: Try harder to generate a changelog [`4eff72d`](https://github.com/jug-dev/hordelib/commit/4eff72df9c5ea8c811a4fb09099aa2bc10319fc5)  (Jug)
 
 ## [v0.5.11](https://github.com/jug-dev/hordelib/compare/v0.5.10...v0.5.11)
 
 11 April 2023
 
-- release: minor build changes [`#85`](https://github.com/jug-dev/hordelib/pull/85) (Jug)
 - ci: add some notes to the release ci [`faf9788`](https://github.com/jug-dev/hordelib/commit/faf9788de1e284a1d0b4b54b5c36b1a5fc789ff9)  (Jug)
 - ci: generate a changelog once again [`8749370`](https://github.com/jug-dev/hordelib/commit/8749370ca78a0e5413293f5ca1a9a60859fd5e97)  (Jug)
 
 ## [v0.5.10](https://github.com/jug-dev/hordelib/compare/v0.5.9...v0.5.10)
 
 11 April 2023
 
-- ci: tweak release scripts [`#84`](https://github.com/jug-dev/hordelib/pull/84) (Jug)
 - docs: remove changelog [`62dae03`](https://github.com/jug-dev/hordelib/commit/62dae03cd056ee19a7a433a1c360e026266329a7)  (Jug)
+- ci: tweak release scripts [`bf9a6a7`](https://github.com/jug-dev/hordelib/commit/bf9a6a76a7014e263a3554fefe5c8195c782f6f0)  (Jug)
 
 ## [v0.5.9](https://github.com/jug-dev/hordelib/compare/v0.5.8...v0.5.9)
 
 11 April 2023
 
-- ci: more tweaks to the ci process [`#83`](https://github.com/jug-dev/hordelib/pull/83) (Jug)
+- ci: more tweaks to the ci process [`522d269`](https://github.com/jug-dev/hordelib/commit/522d2699385c32b89cbcdf45d89bb6801daaadfb)  (Jug)
 
 ## [v0.5.8](https://github.com/jug-dev/hordelib/compare/v0.5.7...v0.5.8)
 
 11 April 2023
 
 ## [v0.5.7](https://github.com/jug-dev/hordelib/compare/v0.5.6...v0.5.7)
 
 11 April 2023
 
-- release: fixes to img2img and hires fix [`#82`](https://github.com/jug-dev/hordelib/pull/82) (Jug)
 - fix: img2img + highres_fix  [`#80`](https://github.com/jug-dev/hordelib/pull/80) (Divided by Zer0)
+- build: version bump [`bc135ea`](https://github.com/jug-dev/hordelib/commit/bc135ea09ef95a8c86d066ad985a05aa04c8dfff)  (github-actions)
 - ci: try to publish to pypi on release [`deb6eb5`](https://github.com/jug-dev/hordelib/commit/deb6eb5f7661be5ebbb91e121c382338a89ecb76)  (Jug)
 - ci: tweaks to the release ci [`c234ea7`](https://github.com/jug-dev/hordelib/commit/c234ea7157b4c70e62adbc2b71d7220a86e1ec98)  (Jug)
 
 ## [v0.5.6](https://github.com/jug-dev/hordelib/compare/v0.5.5...v0.5.6)
 
 11 April 2023
 
-- release: testing speed increase [`#79`](https://github.com/jug-dev/hordelib/pull/79) (Jug)
 - tests: class scope on inference tests for speedup [`#78`](https://github.com/jug-dev/hordelib/pull/78) (Divided by Zer0)
 - docs: recreate LICENSE [`158a70f`](https://github.com/jug-dev/hordelib/commit/158a70f32ab27dbea6eae9d37c2eddad90016263)  (Jug)
 - docs: remove license to recreate it [`8ee4dde`](https://github.com/jug-dev/hordelib/commit/8ee4ddeb40b1824d029a7eca138cd76e61b484f0)  (Jug)
 - build: placeholder changelog [`bbf880e`](https://github.com/jug-dev/hordelib/commit/bbf880e011ea34325beb0bbb46a0ad1545e25af0)  (Jug)
 
 ## [v0.5.5](https://github.com/jug-dev/hordelib/compare/v0.5.4...v0.5.5)
 
 11 April 2023
 
 ## [v0.5.4](https://github.com/jug-dev/hordelib/compare/v0.5.3...v0.5.4)
 
 11 April 2023
 
-- release: fixes and refactorings [`#77`](https://github.com/jug-dev/hordelib/pull/77) (Jug)
 - build: add release mode flag [`#76`](https://github.com/jug-dev/hordelib/pull/76) (Jug)
 - refactor!: Second big Model Manager rework step [`#75`](https://github.com/jug-dev/hordelib/pull/75) (tazlin)
 - fix: adjust mlsd annotator defaults [`#74`](https://github.com/jug-dev/hordelib/pull/74) (Jug)
 - chore: resolve merge conflicts [`007bc44`](https://github.com/jug-dev/hordelib/commit/007bc441ff448eda879994212fc0e5ad896b4e84)  (Jug)
 - docs: remove the changelog from main [`6a650f2`](https://github.com/jug-dev/hordelib/commit/6a650f215482c316f77de2e8fb98609c4d60fbc7)  (Jug)
 - fix: normal map and mlsd annotators [`203873d`](https://github.com/jug-dev/hordelib/commit/203873dc6e904f73f48c56d1b9f68509e3213c15)  (Jug)
 
 ## [v0.5.3](https://github.com/jug-dev/hordelib/compare/v0.5.2...v0.5.3)
 
 11 April 2023
 
 - build: patch release [`#73`](https://github.com/jug-dev/hordelib/pull/73) (Jug)
 - build: try to fix test running and build [`9df056d`](https://github.com/jug-dev/hordelib/commit/9df056d98d4502398bb13437f51522cb6a0feebf)  (Jug)
+- build: version bump [`82a4b82`](https://github.com/jug-dev/hordelib/commit/82a4b82b22d97495e2ddde23c716c8aa57cb0b46)  (github-actions)
 
 ## [v0.5.2](https://github.com/jug-dev/hordelib/compare/v0.5.1...v0.5.2)
 
 11 April 2023
 
 - build: upgrade to torch 2, xformers 18 and latest comfyui [`#68`](https://github.com/jug-dev/hordelib/pull/68) (Jug)
+- build: version bump [`6af3e1e`](https://github.com/jug-dev/hordelib/commit/6af3e1e236d559497e28eed19f0a0ace5bb66bc5)  (github-actions)
 
 ## [v0.5.1](https://github.com/jug-dev/hordelib/compare/v0.5.0...v0.5.1)
 
 11 April 2023
 
 - feat: Added is_model_loaded() to HyperMM [`#67`](https://github.com/jug-dev/hordelib/pull/67) (Divided by Zer0)
+- build: version bump [`41b4ad2`](https://github.com/jug-dev/hordelib/commit/41b4ad246db6f992ccebe09542e0f9a1276f6f25)  (github-actions)
 
 ## [v0.5.0](https://github.com/jug-dev/hordelib/compare/v0.4.2...v0.5.0)
 
 11 April 2023
 
 - feat: add support for return_control_map [`#66`](https://github.com/jug-dev/hordelib/pull/66) (Jug)
+- build: version bump [`667bb06`](https://github.com/jug-dev/hordelib/commit/667bb06f15be835eae8f393e5da46039e72ff133)  (github-actions)
 - docs: update ci test badge [`e2b137e`](https://github.com/jug-dev/hordelib/commit/e2b137ed43d5b63c8a6f1d7899a31bbb78aa7045)  (Jug)
 
 ## [v0.4.2](https://github.com/jug-dev/hordelib/compare/v0.4.1...v0.4.2)
 
 11 April 2023
 
 - fix: resize img2img before inference [`#63`](https://github.com/jug-dev/hordelib/pull/63) (Divided by Zer0)
 - fix: add timezone to build results [`#61`](https://github.com/jug-dev/hordelib/pull/61) (Jug)
 - tests: gfpgan test and size assets [`#62`](https://github.com/jug-dev/hordelib/pull/62) (Divided by Zer0)
 - docs: update with pypi test notes [`dd41120`](https://github.com/jug-dev/hordelib/commit/dd4112023d39e280fb61a1342707af4765f3b4df)  (Jug)
+- build: version bump [`e9525bc`](https://github.com/jug-dev/hordelib/commit/e9525bc8cc0bdcf33e4b6cc5c386027bf679268f)  (github-actions)
 
 ## [v0.4.1](https://github.com/jug-dev/hordelib/compare/v0.4.0...v0.4.1)
 
 10 April 2023
 
 - feat: Make use of the ControlNet ModelManager [`#53`](https://github.com/jug-dev/hordelib/pull/53) (Divided by Zer0)
 - test: fix test with red border around it [`#58`](https://github.com/jug-dev/hordelib/pull/58) (Jug)
```

### Comparing `hordelib-0.6.0/LICENSE` & `hordelib-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/PKG-INFO` & `hordelib-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.6.0
+Version: 0.6.1
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,21 +675,22 @@
 Requires-Python: <3.11,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: CHANGELOG.md
 
 # hordelib
 
-[![PyPI version](https://badge.fury.io/py/hordelib.svg?branch=main&nocache=1)](https://badge.fury.io/py/hordelib)
-[![Downloads](https://pepy.tech/badge/hordelib)](https://pepy.tech/project/hordelib)
-![GitHub license](https://img.shields.io/github/license/jug-dev/hordelib)
-
-[![Build](https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
-[![Test Images](https://badgen.net/badge/main/latest-images/blue?icon=awesome)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
-[![Test Images](https://badgen.net/badge/develop/latest-images/blue?icon=awesome)](http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable)
+[![PyPI Version][pypi-image]][pypi-url]
+[![Downloads][downloads-image]][downloads-url]
+![GitHub license][license-url]
+
+[![Build][build-image]][build-url]
+[![Test Images][main-test-image]][main-test-url]
+[![Test Images][pr-test-image]][pr-test-url]
+[![Release Changelog][changelog-image]][changelog-url]
 
 `hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of this project can be found in the AI Horde Discord server: [https://discord.gg/3DxrhksKzn](https://discord.gg/3DxrhksKzn)
 
 NOTE: This project is in early development and is not yet in use by Stable Horde.
 
@@ -749,14 +750,23 @@
 pil_image.save("test.png")
 ```
 
 Note that `hordelib.initialise()` will erase all command line arguments from argv. So make sure you parse them before you call that.
 
 See `tests/run_*.py` for more standalone examples.
 
+### Logging
+
+If you don't want `hordelib` to setup and control the logging configuration initialise with:
+
+```python
+import hordelib
+hordelib.initialise(setup_logging=False)
+```
+
 ## Development
 
 Requirements:
 - `git` (install git)
 - `tox` (`pip install tox`)
 - Set the environmental variable `AIWORKER_CACHE_HOME` to point to a model directory.
 
@@ -885,7 +895,23 @@
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
 
 Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
+
+<!-- Badges: -->
+
+[pypi-image]: https://badge.fury.io/py/hordelib.svg?branch=main&nocache=1
+[pypi-url]: https://badge.fury.io/py/hordelib
+[downloads-image]: https://pepy.tech/badge/hordelib
+[downloads-url]: https://pepy.tech/project/hordelib
+[license-url]: https://img.shields.io/github/license/jug-dev/hordelib
+[build-image]: https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main
+[build-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
+[main-test-image]: https://badgen.net/badge/main/latest-images/blue?icon=awesome
+[main-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
+[pr-test-image]: https://badgen.net/badge/develop/latest-images/blue?icon=awesome
+[pr-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable
+[changelog-image]: https://img.shields.io/badge/Release-Changelog-yellow
+[changelog-url]: https://github.com/jug-dev/hordelib/blob/releases/CHANGELOG.md
```

### Comparing `hordelib-0.6.0/README.md` & `hordelib-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # hordelib
 
-[![PyPI version](https://badge.fury.io/py/hordelib.svg?branch=main&nocache=1)](https://badge.fury.io/py/hordelib)
-[![Downloads](https://pepy.tech/badge/hordelib)](https://pepy.tech/project/hordelib)
-![GitHub license](https://img.shields.io/github/license/jug-dev/hordelib)
-
-[![Build](https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
-[![Test Images](https://badgen.net/badge/main/latest-images/blue?icon=awesome)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
-[![Test Images](https://badgen.net/badge/develop/latest-images/blue?icon=awesome)](http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable)
+[![PyPI Version][pypi-image]][pypi-url]
+[![Downloads][downloads-image]][downloads-url]
+![GitHub license][license-url]
+
+[![Build][build-image]][build-url]
+[![Test Images][main-test-image]][main-test-url]
+[![Test Images][pr-test-image]][pr-test-url]
+[![Release Changelog][changelog-image]][changelog-url]
 
 `hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of this project can be found in the AI Horde Discord server: [https://discord.gg/3DxrhksKzn](https://discord.gg/3DxrhksKzn)
 
 NOTE: This project is in early development and is not yet in use by Stable Horde.
 
@@ -70,14 +71,23 @@
 pil_image.save("test.png")
 ```
 
 Note that `hordelib.initialise()` will erase all command line arguments from argv. So make sure you parse them before you call that.
 
 See `tests/run_*.py` for more standalone examples.
 
+### Logging
+
+If you don't want `hordelib` to setup and control the logging configuration initialise with:
+
+```python
+import hordelib
+hordelib.initialise(setup_logging=False)
+```
+
 ## Development
 
 Requirements:
 - `git` (install git)
 - `tox` (`pip install tox`)
 - Set the environmental variable `AIWORKER_CACHE_HOME` to point to a model directory.
 
@@ -206,7 +216,23 @@
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
 
 Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
+
+<!-- Badges: -->
+
+[pypi-image]: https://badge.fury.io/py/hordelib.svg?branch=main&nocache=1
+[pypi-url]: https://badge.fury.io/py/hordelib
+[downloads-image]: https://pepy.tech/badge/hordelib
+[downloads-url]: https://pepy.tech/project/hordelib
+[license-url]: https://img.shields.io/github/license/jug-dev/hordelib
+[build-image]: https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main
+[build-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
+[main-test-image]: https://badgen.net/badge/main/latest-images/blue?icon=awesome
+[main-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
+[pr-test-image]: https://badgen.net/badge/develop/latest-images/blue?icon=awesome
+[pr-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable
+[changelog-image]: https://img.shields.io/badge/Release-Changelog-yellow
+[changelog-url]: https://github.com/jug-dev/hordelib/blob/releases/CHANGELOG.md
```

### Comparing `hordelib-0.6.0/build_helper.py` & `hordelib-0.6.1/build_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/cache/cache.py` & `hordelib-0.6.1/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/clip/bulk.py` & `hordelib-0.6.1/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/clip/coca.py` & `hordelib-0.6.1/hordelib/clip/coca.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,12 +22,8 @@
                 raise ValueError(f"Could not open image {input_image}: {e}")
 
         image = self.transform(input_image).unsqueeze(0).to(self.device)
         if self.half_precision:
             image = image.half()
         generated = self.model.generate(image)
 
-        return (
-            open_clip.decode(generated[0])
-            .split("<end_of_text>")[0]
-            .replace("<start_of_text>", "")
-        )
+        return open_clip.decode(generated[0]).split("<end_of_text>")[0].replace("<start_of_text>", "")
```

### Comparing `hordelib-0.6.0/hordelib/clip/image.py` & `hordelib-0.6.1/hordelib/clip/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,17 +39,15 @@
             ).hexdigest()
         preprocess_images = []
         to_remove = []
         with torch.no_grad():
             for pil_image in pil_images:
                 try:
                     preprocess_images.append(
-                        self.model["preprocess"](pil_image["pil_image"])
-                        .unsqueeze(0)
-                        .to(self.model["device"]),
+                        self.model["preprocess"](pil_image["pil_image"]).unsqueeze(0).to(self.model["device"]),
                     )
                 except RuntimeError as e:
                     logger.error(e)
                     logger.error(pil_image)
                     to_remove.append(pil_image)
                     continue
             for pil_image in to_remove:
@@ -92,19 +90,15 @@
         If image is not in cache, embed it and save it to cache
         Returns SHA256 hash of image
         """
         if image is None and filename is None:
             raise ValueError("Either image or filename must be set")
         if image is not None and filename is not None:
             raise ValueError("Only one of image or filename must be set")
-        pil_image = (
-            Image.open(f"{directory}/{filename}").convert("RGB")
-            if image is None
-            else image
-        )
+        pil_image = Image.open(f"{directory}/{filename}").convert("RGB") if image is None else image
         if image is None:
             file_hash = hashlib.sha256(
                 open(f"{directory}/{filename}", "rb").read(),
             ).hexdigest()
             image_hash = hashlib.sha256(pil_image.tobytes()).hexdigest()
         else:
             file_hash = None
@@ -114,16 +108,12 @@
             if cached:
                 logger.debug(f"Image {image_hash} already in cache")
                 return image_hash
         else:
             logger.debug(f"Skipping cache for image {image_hash}")
         logger.debug(f"Embedding image {image_hash}")
         with torch.no_grad():
-            preprocess_image = (
-                self.model["preprocess"](pil_image)
-                .unsqueeze(0)
-                .to(self.model["device"])
-            )
+            preprocess_image = self.model["preprocess"](pil_image).unsqueeze(0).to(self.model["device"])
         image_features = self.model["model"].encode_image(preprocess_image).float()
         self._save(image_features, image_hash)
         self.cache.add_sqlite_row(file=filename, hash=file_hash, pil_hash=image_hash)
         return image_hash
```

### Comparing `hordelib-0.6.0/hordelib/clip/interrogate.py` & `hordelib-0.6.1/hordelib/clip/interrogate.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,17 +182,15 @@
         top_count = min(top_count, len(text_array))
         if key not in self.embed_lists:
             self.load(key, text_array, individual=False, device=device)
         text_features = self.embed_lists[key].to(device)
 
         similarity = torch.zeros((1, len(text_array))).to(device)
         for i in range(image_features.shape[0]):
-            similarity += (
-                100.0 * image_features[i].unsqueeze(0) @ text_features.T
-            ).softmax(dim=-1)
+            similarity += (100.0 * image_features[i].unsqueeze(0) @ text_features.T).softmax(dim=-1)
         similarity /= image_features.shape[0]
 
         top_probs, top_labels = similarity.cpu().topk(top_count, dim=-1)
         top = [
             {
                 "text": text_array[top_labels[0][i].numpy()],
                 "confidence": (top_probs[0][i].numpy() * 100),
@@ -239,17 +237,15 @@
         if isinstance(text_array, list):
             text_array = {"default": text_array}
         elif isinstance(text_array, dict):
             pass
         image_embed = ImageEmbed(self.model_info, self.cache_image)
         image_hash = image_embed(image, filename, directory)
         image_embed_array = np.load(f"{self.cache_image.cache_dir}/{image_hash}.npy")
-        image_features = (
-            torch.from_numpy(image_embed_array).float().to(self.model_info["device"])
-        )
+        image_features = torch.from_numpy(image_embed_array).float().to(self.model_info["device"])
         if similarity and not rank:
             results = {}
             for k in text_array:
                 results[k] = self.similarity(
                     image_features,
                     text_array[k],
                     k,
```

### Comparing `hordelib-0.6.0/hordelib/clip/text.py` & `hordelib-0.6.1/hordelib/clip/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     @autocast_cuda
     def _batch(self, text_list: list):
         for text in text_list:
             if isinstance(text["prompt"], bytes):
                 text["prompt"] = text["prompt"].decode("utf-8")
             text["hash"] = hashlib.sha256(text["prompt"]).hexdigest()
         text_tokens = [
-            clip.tokenize(text["prompt"], truncate=True).to(self.model_info["device"])
-            for text in text_list
+            clip.tokenize(text["prompt"], truncate=True).to(self.model_info["device"]) for text in text_list
         ]
         text_tokens = torch.cat(text_tokens, dim=0)
         with torch.no_grad():
             text_features = self.model_info["model"].encode_text(text_tokens).float()
         for text_embed_array, text in zip(text_features, text_list):
             self.executor.submit(self._save, text_embed_array, text["hash"])
             self.cache.add_sqlite_row(text["filename"], text["hash"], text["hash"])
```

### Comparing `hordelib-0.6.0/hordelib/comfy_horde.py` & `hordelib-0.6.1/hordelib/comfy_horde.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,15 @@
     # XXX # TODO One day this signature should be generic, and not comfy specific
     # XXX # This can remain a comfy call, but the rest of the code should be able
     # XXX # to pretend it isn't
 
     # Redirect IO
     stdio = OutputCollector()
     with contextlib.redirect_stdout(stdio):
-        (
-            modelPatcher,
-            clipModel,
-            vae,
-            clipVisionModel,
-        ) = comfy.sd.load_checkpoint_guess_config(
+        (modelPatcher, clipModel, vae, clipVisionModel) = comfy.sd.load_checkpoint_guess_config(
             ckpt_path=ckpt_path,
             output_vae=output_vae,
             output_clip=output_clip,
             embedding_directory=embeddings_path,
         )
     stdio.replay()
 
@@ -64,17 +59,15 @@
 def horde_load_controlnet(  # XXX Needs docstring
     controlnet_path: str,
     target_model,
 ) -> comfy.sd.ControlNet | comfy.sd.T2IAdapter | None:
     # Redirect IO
     stdio = OutputCollector()
     with contextlib.redirect_stdout(stdio):
-        controlnet = comfy.sd.load_controlnet(
-            ckpt_path=controlnet_path, model=target_model
-        )
+        controlnet = comfy.sd.load_controlnet(ckpt_path=controlnet_path, model=target_model)
     stdio.replay()
     return controlnet
 
 
 class Comfy_Horde:
     """Handles horde-specific behavior against ComfyUI."""
 
@@ -116,31 +109,23 @@
     def _load_custom_nodes(self) -> None:
         execution.nodes.init_custom_nodes()
         execution.nodes.load_custom_nodes(self._this_dir("nodes"))
 
     def _fix_pipeline_types(self, data: dict) -> dict:
         # We have a list of nodes and each node has a class type, which we may want to change
         for nodename, node in data.items():
-            if ("class_type" in node) and (
-                node["class_type"] in Comfy_Horde.NODE_REPLACEMENTS
-            ):
+            if ("class_type" in node) and (node["class_type"] in Comfy_Horde.NODE_REPLACEMENTS):
                 logger.debug(
                     f"Changed type {data[nodename]['class_type']} to {Comfy_Horde.NODE_REPLACEMENTS[node['class_type']]}",
                 )
-                data[nodename]["class_type"] = Comfy_Horde.NODE_REPLACEMENTS[
-                    node["class_type"]
-                ]
+                data[nodename]["class_type"] = Comfy_Horde.NODE_REPLACEMENTS[node["class_type"]]
         # Now we've fixed up node types, check for any node input parameter rename needed
         for nodename, node in data.items():
-            if ("class_type" in node) and (
-                node["class_type"] in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS
-            ):
-                for oldname, newname in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS[
-                    node["class_type"]
-                ].items():
+            if ("class_type" in node) and (node["class_type"] in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS):
+                for oldname, newname in Comfy_Horde.NODE_PARAMETER_REPLACEMENTS[node["class_type"]].items():
                     if "inputs" in node and oldname in node["inputs"]:
                         node["inputs"][newname] = node["inputs"][oldname]
                         del node["inputs"][oldname]
                 logger.debug(f"Renamed node input {nodename}.{oldname} to {newname}")
 
         return data
```

### Comparing `hordelib-0.6.0/hordelib/config_path.py` & `hordelib-0.6.1/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/consts.py` & `hordelib-0.6.1/hordelib/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 from enum import Enum, auto
 
 from hordelib.config_path import get_hordelib_path
 
 COMFYUI_VERSION = "c767e9426ae81bed4f52c7be0625f0efc4cbe16b"
 """The exact version of ComfyUI version to load."""
 
-REMOTE_MODEL_DB = (
-    "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/"
-)
+REMOTE_MODEL_DB = "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/"
 """The default base endpoint where to find model databases. See MODEL_DB_NAMES for valid database names."""
 
 RELEASE_VERSION = os.path.exists(os.path.join(get_hordelib_path(), "_version.py"))
 """A flag for if this is a pypi release or a git dev mode"""
 
 
 class HordeSupportedBackends(Enum):
```

### Comparing `hordelib-0.6.0/hordelib/horde.py` & `hordelib-0.6.1/hordelib/horde.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,17 +134,15 @@
         # sampler in our upscale sampler.
         if payload.get("hires_fix"):
             params["upscale_sampler.seed"] = params["sampler.seed"]
             params["upscale_sampler.scheduler"] = params["sampler.scheduler"]
             params["upscale_sampler.cfg"] = params["sampler.cfg"]
             params["upscale_sampler.steps"] = params["sampler.steps"]
             params["upscale_sampler.sampler_name"] = params["sampler.sampler_name"]
-            params[
-                "upscale_sampler.denoise"
-            ] = 0.6  # XXX is this ok for latent upscale denoise?
+            params["upscale_sampler.denoise"] = 0.6  # XXX is this ok for latent upscale denoise?
             # Adjust image sizes
             width = params.get("empty_latent_image.width", 0)
             height = params.get("empty_latent_image.height", 0)
             if width > 512 and height > 512:
                 final_width = width
                 final_height = height
                 params["latent_upscale.width"] = final_width
@@ -174,32 +172,28 @@
                 del params["source_processing"]
 
         return params
 
     # Fix any nonsensical requests
     def _validate_BASIC_INFERENCE_PARAMS(self, payload):
         # Turn off hires fix if we're not generating a hires image
-        if "hires_fix" in payload and (
-            payload["width"] <= 512 or payload["height"] <= 512
-        ):
+        if "hires_fix" in payload and (payload["width"] <= 512 or payload["height"] <= 512):
             payload["hires_fix"] = False
 
         # Remove source_processing if it's not valid
         img_proc = payload.get("source_processing")
         if img_proc and img_proc not in HordeLib.SOURCE_IMAGE_PROCESSING_OPTIONS:
             del payload["source_processing"]
         # Remove source image if we don't need it
         if payload.get("source_image"):
             if not img_proc or img_proc not in HordeLib.SOURCE_IMAGE_PROCESSING_OPTIONS:
                 del payload["source_image"]
 
         # Turn off hires fix if we're painting as the dimensions are from the image
-        if "hires_fix" in payload and (
-            img_proc == "inpainting" or img_proc == "outpainting"
-        ):
+        if "hires_fix" in payload and (img_proc == "inpainting" or img_proc == "outpainting"):
             payload["hires_fix"] = False
 
     def _get_appropriate_pipeline(self, params):
         # Determine the correct pipeline based on the parameters we have
         pipeline = None
 
         # Hires fix
@@ -277,17 +271,15 @@
         except (UnidentifiedImageError, AttributeError):
             logger.warning(
                 "Source mask could not be parsed. Falling back to img2img without mask",
             )
             del payload["source_mask"]
 
         if payload.get("source_mask"):
-            payload["source_image"] = self._add_image_alpha_channel(
-                payload["source_image"], payload["source_mask"]
-            )
+            payload["source_image"] = self._add_image_alpha_channel(payload["source_image"], payload["source_mask"])
 
     def basic_inference(self, payload: dict[str, str | None]) -> Image.Image | None:
         generator = Comfy_Horde()
         # Validate our payload parameters
         self._validate_BASIC_INFERENCE_PARAMS(payload)
         self._resize_sources_to_request(payload)
         # Determine our parameters
```

### Comparing `hordelib-0.6.0/hordelib/initialisation.py` & `hordelib-0.6.1/hordelib/initialisation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # initialisation.py
 # Initialise hordelib.
 import sys
 
 from loguru import logger
 
-import hordelib.utils.logger
 from hordelib import install_comfy
 from hordelib.config_path import get_hordelib_path, set_system_path
 from hordelib.consts import (
     COMFYUI_VERSION,
     DEFAULT_MODEL_MANAGERS,
     MODEL_CATEGORY_NAMES,
     RELEASE_VERSION,
 )
+from hordelib.utils.logger import HordeLog
 
 
 def initialise(
     model_managers_to_load: dict[MODEL_CATEGORY_NAMES, bool] = DEFAULT_MODEL_MANAGERS,
+    setup_logging=True,
 ):
+    # Setup logging if requested
+    if setup_logging:
+        HordeLog.initialise()
+
     logger.level("DEBUG")  # XXX # FIXME
 
     # If developer mode, don't permit some things
     if not RELEASE_VERSION and " " in get_hordelib_path():
         # Our runtime patching can't handle this
         raise Exception(
-            "Do not run this project in developer mode from a path that "
-            "contains spaces in directory names.",
+            "Do not run this project in developer mode from a path that " "contains spaces in directory names.",
         )
 
     # Ensure we have ComfyUI
     logger.debug("Clearing command line args in sys.argv before ComfyUI load")
     sys_arg_bkp = sys.argv.copy()
     sys.argv = sys.argv[:1]
     installer = install_comfy.Installer()
```

### Comparing `hordelib-0.6.0/hordelib/install_comfy.patch` & `hordelib-0.6.1/hordelib/install_comfy.patch`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/install_comfy.py` & `hordelib-0.6.1/hordelib/install_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/aitemplate.json` & `hordelib-0.6.1/hordelib/model_database/aitemplate.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/blip.json` & `hordelib-0.6.1/hordelib/model_database/blip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/clip.json` & `hordelib-0.6.1/hordelib/model_database/clip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/controlnet.json` & `hordelib-0.6.1/hordelib/model_database/controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/db.json` & `hordelib-0.6.1/hordelib/model_database/db.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/db_dep.json` & `hordelib-0.6.1/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/db_embeds.json` & `hordelib-0.6.1/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/diffusers.json` & `hordelib-0.6.1/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/esrgan.json` & `hordelib-0.6.1/hordelib/model_database/esrgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/gfpgan.json` & `hordelib-0.6.1/hordelib/model_database/gfpgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/safety_checker.json` & `hordelib-0.6.1/hordelib/model_database/safety_checker.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_database/stable_diffusion.json` & `hordelib-0.6.1/hordelib/model_database/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/base.py` & `hordelib-0.6.1/hordelib/model_manager/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,17 +186,15 @@
         return self.available_models
 
     def get_available_models_by_types(self, model_types: list[str] | None = None):
         if not model_types:
             model_types = ["ckpt", "diffusers"]
         models_available = []
         for model in self.model_reference:
-            if self.model_reference[model][
-                "type"
-            ] in model_types and self.check_available(
+            if self.model_reference[model]["type"] in model_types and self.check_available(
                 self.get_model_files(model),
             ):
                 models_available.append(model)
         return models_available
 
     def count_available_models_by_types(self, model_types: list[str] | None = None):
         return len(self.get_available_models_by_types(model_types))
@@ -325,17 +323,15 @@
         if not os.path.isfile(file_name):
             raise FileNotFoundError(f"No file {file_name}")
 
         # Check if we have a cached sha256 hash for the source file
         # and use that unless our source file is newer than our hash
         sha256_file = f"{os.path.splitext(file_name)[0]}.sha256"
         source_timestamp = os.path.getmtime(file_name)
-        hash_timestamp = (
-            os.path.getmtime(sha256_file) if os.path.isfile(sha256_file) else 0
-        )
+        hash_timestamp = os.path.getmtime(sha256_file) if os.path.isfile(sha256_file) else 0
         if hash_timestamp > source_timestamp:
             # Use our cached hash
             with open(sha256_file) as handle:
                 sha256_hash = handle.read().split()[0]
             return sha256_hash
 
         # Calculate the hash of the source file
@@ -377,15 +373,15 @@
 
         # If sha256 is not available, fall back to md5
         if "md5sum" in file_details:
             logger.debug(f"Getting md5sum of {full_path}")
             md5_file_hash = self.get_file_md5sum_hash(full_path)
             logger.debug(f"md5sum: {md5_file_hash}")
             logger.debug(f"Expected: {file_details['md5sum']}")
-            return file_details["md5sum"] != md5_file_hash
+            return file_details["md5sum"] == md5_file_hash
 
         # If no hashes available, return True for now
         # THIS IS A SECURITY RISK, EVENTUALLY WE SHOULD RETURN FALSE
         # But currently not all models specify hashes
         # XXX this warning preexists me (@tazlin), probably should look into it
 
         return True
@@ -453,18 +449,15 @@
         Other:
         - write content to file
         - symlink file
         - delete file
         - unzip file
         """
         # XXX this function is wacky in its premise and needs to be reworked
-        if (
-            model_name in self.available_models
-            and model_name not in self.tainted_models
-        ):
+        if model_name in self.available_models and model_name not in self.tainted_models:
             logger.info(f"{model_name} is already available.")
             return True
         download = self.get_model_download(model_name)
         files = self.get_model_files(model_name)
         for i in range(len(download)):
             file_path = (
                 f"{download[i]['file_path']}/{download[i]['file_name']}"
@@ -539,18 +532,15 @@
                     os.path.join(self.modelFolderPath, download_path),
                 )
                 logger.info(f"delete {zip_path}")
                 os.remove(zip_path)
                 logger.info(f"delete {temp_path}")
                 shutil.rmtree(temp_path)
             else:
-                if (
-                    not self.check_file_available(file_path)
-                    or model_name in self.tainted_models
-                ):
+                if not self.check_file_available(file_path) or model_name in self.tainted_models:
                     logger.debug(f"Downloading {download_url} to {file_path}")
                     self.download_file(download_url, file_path)
         if not self.validate_model(model_name):
             return False
         return True
 
     def download_all_models(self) -> bool:
@@ -590,16 +580,15 @@
         if torch.cuda.is_available():
             number_of_cuda_devices = torch.cuda.device_count()
             cuda_arch = []
             for i in range(number_of_cuda_devices):
                 cuda_device = {
                     "id": i,
                     "name": torch.cuda.get_device_name(i),
-                    "sm": torch.cuda.get_device_capability(i)[0] * 10
-                    + torch.cuda.get_device_capability(i)[1],
+                    "sm": torch.cuda.get_device_capability(i)[0] * 10 + torch.cuda.get_device_capability(i)[1],
                 }
                 cuda_arch.append(cuda_device)
             cuda_arch = sorted(cuda_arch, key=lambda k: k["sm"], reverse=True)
             recommended_gpu = [x for x in cuda_arch if x["sm"] == cuda_arch[0]["sm"]]
             return cuda_arch, recommended_gpu
 
         return None, None
```

### Comparing `hordelib-0.6.0/hordelib/model_manager/blip.py` & `hordelib-0.6.1/hordelib/model_manager/blip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/clip.py` & `hordelib-0.6.1/hordelib/model_manager/clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/codeformer.py` & `hordelib-0.6.1/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/compvis.py` & `hordelib-0.6.1/hordelib/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/controlnet.py` & `hordelib-0.6.1/hordelib/model_manager/controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/diffusers.py` & `hordelib-0.6.1/hordelib/model_manager/diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/esrgan.py` & `hordelib-0.6.1/hordelib/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/gfpgan.py` & `hordelib-0.6.1/hordelib/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/hyper.py` & `hordelib-0.6.1/hordelib/model_manager/hyper.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,18 +325,15 @@
                 cpu_only=cpu_only,
             )
             if success:
                 self.loaded_models.update(
                     {model_name: self.clip.loaded_models[model_name]},
                 )
             return success
-        if (
-            self.codeformer is not None
-            and model_name in self.codeformer.model_reference
-        ):
+        if self.codeformer is not None and model_name in self.codeformer.model_reference:
             success = self.codeformer.load(
                 model_name=model_name,
             )
             if success:
                 self.loaded_models.update(
                     {model_name: self.codeformer.loaded_models[model_name]},
                 )
@@ -375,18 +372,15 @@
                 model_name=model_name,
             )
             if success:
                 self.loaded_models.update(
                     {model_name: self.gfpgan.loaded_models[model_name]},
                 )
             return success
-        if (
-            self.safety_checker is not None
-            and model_name in self.safety_checker.model_reference
-        ):
+        if self.safety_checker is not None and model_name in self.safety_checker.model_reference:
             success = self.safety_checker.load(
                 model_name=model_name,
             )
             if success:
                 self.loaded_models.update(
                     {model_name: self.safety_checker.loaded_models[model_name]},
                 )
```

### Comparing `hordelib-0.6.0/hordelib/model_manager/safety_checker.py` & `hordelib-0.6.1/hordelib/model_manager/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/model_manager/torch_hijack.py` & `hordelib-0.6.1/hordelib/model_manager/torch_hijack.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,19 +100,15 @@
                 **kwargs,
             )
 
         def transformers_utils_hub_get_file_from_cache(original, url, *args, **kwargs):
             # this file is always 404, prevent making request
             # XXX looks like some old hack
             bad_url = "https://huggingface.co/openai/clip-vit-large-patch14/resolve/main/added_tokens.json"
-            if (
-                url == bad_url
-                or url == "openai/clip-vit-large-patch14"
-                and args[0] == "added_tokens.json"
-            ):
+            if url == bad_url or url == "openai/clip-vit-large-patch14" and args[0] == "added_tokens.json":
                 return None
 
             try:  # XXX this is some weird, hard to follow behavior
                 res = original(url, *args, local_files_only=True, **kwargs)
                 if res is None:
                     res = original(url, *args, local_files_only=False, **kwargs)
                 return res
```

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/install.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-0.6.1/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/__init__.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-0.6.1/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.6.1/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-0.6.1/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,15 @@
     FUNCTION = "load_controlnet"
 
     CATEGORY = "loaders"
 
     def load_controlnet(self, model, control_net_name, model_manager):
         logger.debug(f"Loading controlnet {control_net_name} through our custom node")
 
-        if (
-            not model_manager
-            or not model_manager.manager
-            or not model_manager.manager.controlnet
-        ):
+        if not model_manager or not model_manager.manager or not model_manager.manager.controlnet:
             logger.error("controlnet model_manager appears to be missing!")
             raise RuntimeError  # XXX better guarantees need to be made
 
         merged_model = model_manager.manager.controlnet.merge_controlnet(
             control_net_name,
             model,
         )
```

### Comparing `hordelib-0.6.0/hordelib/nodes/node_image_loader.py` & `hordelib-0.6.1/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/node_image_output.py` & `hordelib-0.6.1/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/node_model_loader.py` & `hordelib-0.6.1/hordelib/nodes/node_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-0.6.1/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-0.6.1/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-0.6.1/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-0.6.1/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-0.6.1/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-0.6.1/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.6.1/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-0.6.1/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-0.6.1/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-0.6.1/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-0.6.1/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-0.6.1/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.6.1/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.6.1/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-0.6.1/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/run_comfyui.py` & `hordelib-0.6.1/hordelib/run_comfyui.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/safety_checker.py` & `hordelib-0.6.1/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/shared_model_manager.py` & `hordelib-0.6.1/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/utils/cast.py` & `hordelib-0.6.1/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/utils/ioredirect.py` & `hordelib-0.6.1/hordelib/utils/ioredirect.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/hordelib/utils/logger.py` & `hordelib-0.6.1/hordelib/utils/logger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,234 @@
 import sys
 from functools import partialmethod
 
 from loguru import logger
 
-STDOUT_LEVELS = ["GENERATION", "PROMPT"]
-INIT_LEVELS = ["INIT", "INIT_OK", "INIT_WARN", "INIT_ERR"]
-MESSAGE_LEVELS = ["MESSAGE"]
-STATS_LEVELS = ["STATS"]
-# By default we're at error level or higher
-verbosity = 20
-quiet = 0
-
-
-def set_logger_verbosity(count):
-    global verbosity
-    # The count comes reversed. So count = 0 means minimum verbosity
-    # While count 5 means maximum verbosity
-    # So the more count we have, the lowe we drop the versbosity maximum
-    verbosity = 20 - (count * 10)
-
-
-def quiesce_logger(count):
-    global quiet
-    # The bigger the count, the more silent we want our logger
-    quiet = count * 10
-
-
-def is_stdout_log(record):
-    if record["level"].name not in STDOUT_LEVELS:
-        return False
-    if record["level"].no < verbosity + quiet:
-        return False
-    return True
-
-
-def is_init_log(record):
-    if record["level"].name not in INIT_LEVELS:
-        return False
-    if record["level"].no < verbosity + quiet:
-        return False
-    return True
-
-
-def is_msg_log(record):
-    if record["level"].name not in MESSAGE_LEVELS:
-        return False
-    if record["level"].no < verbosity + quiet:
-        return False
-    return True
-
-
-def is_stderr_log(record):
-    if (
-        record["level"].name
-        in STDOUT_LEVELS + INIT_LEVELS + MESSAGE_LEVELS + STATS_LEVELS
-    ):
-        return False
-    if record["level"].no < verbosity + quiet:
-        return False
-    return True
-
-
-def is_stats_log(record):
-    if record["level"].name not in STATS_LEVELS:
-        return False
-    return True
-
-
-def is_not_stats_log(record):
-    if record["level"].name in STATS_LEVELS:
-        return False
-    return True
-
-
-def is_trace_log(record):
-    if record["level"].name not in ["TRACE", "ERROR"]:
-        return False
-    return True
-
-
-def test_logger():
-    logger.generation(
-        "This is a generation message\nIt is typically multiline\nThee Lines".encode(
-            "unicode_escape",
-        ).decode("utf-8"),
-    )
-    logger.prompt("This is a prompt message")
-    logger.debug("Debug Message")
-    logger.info("Info Message")
-    logger.warning("Info Warning")
-    logger.error("Error Message")
-    logger.critical("Critical Message")
-    logger.init("This is an init message", status="Starting")
-    logger.init_ok("This is an init message", status="OK")
-    logger.init_warn("This is an init message", status="Warning")
-    logger.init_err("This is an init message", status="Error")
-    logger.message("This is user message")
-    sys.exit()
-
-
-logfmt = (
-    "<level>{level: <10}</level> | <green>{time:YYYY-MM-DD HH:mm:ss.SSSSSS}</green> | "
-    "<green>{name}</green>:<green>{function}</green>:<green>{line}</green> - <level>{message}</level>"
-)
-genfmt = "<level>{level: <10}</level> @ <green>{time:YYYY-MM-DD HH:mm:ss.SSSSSS}</green> | <level>{message}</level>"
-initfmt = "<magenta>INIT      </magenta> | <level>{extra[status]: <11}</level> | <magenta>{message}</magenta>"
-msgfmt = "<level>{level: <10}</level> | <level>{message}</level>"
-
-try:
-    logger.level("GENERATION", no=24, color="<cyan>")
-    logger.level("PROMPT", no=23, color="<yellow>")
-    logger.level("INIT", no=31, color="<white>")
-    logger.level("INIT_OK", no=31, color="<green>")
-    logger.level("INIT_WARN", no=31, color="<yellow>")
-    logger.level("INIT_ERR", no=31, color="<red>")
-    # Messages contain important information without which this application might not be able to be used
-    # As such, they have the highest priority
-    logger.level("MESSAGE", no=61, color="<green>")
-    # Stats are info that might not display well in the terminal
-    logger.level("STATS", no=19, color="<blue>")
-except TypeError:
-    pass
-
-logger.__class__.generation = partialmethod(logger.__class__.log, "GENERATION")
-logger.__class__.prompt = partialmethod(logger.__class__.log, "PROMPT")
-logger.__class__.init = partialmethod(logger.__class__.log, "INIT")
-logger.__class__.init_ok = partialmethod(logger.__class__.log, "INIT_OK")
-logger.__class__.init_warn = partialmethod(logger.__class__.log, "INIT_WARN")
-logger.__class__.init_err = partialmethod(logger.__class__.log, "INIT_ERR")
-logger.__class__.message = partialmethod(logger.__class__.log, "MESSAGE")
-logger.__class__.stats = partialmethod(logger.__class__.log, "STATS")
-
-config = {
-    "handlers": [
-        {
-            "sink": sys.stderr,
-            "format": logfmt,
-            "colorize": True,
-            "filter": is_stderr_log,
-        },
-        {
-            "sink": sys.stdout,
-            "format": genfmt,
-            "level": "PROMPT",
-            "colorize": True,
-            "filter": is_stdout_log,
-        },
-        {
-            "sink": sys.stdout,
-            "format": initfmt,
-            "level": "INIT",
-            "colorize": True,
-            "filter": is_init_log,
-        },
-        {
-            "sink": sys.stdout,
-            "format": msgfmt,
-            "level": "MESSAGE",
-            "colorize": True,
-            "filter": is_msg_log,
-        },
-        {
-            "sink": "logs/bridge.log",
-            "format": logfmt,
-            "level": "DEBUG",
-            "colorize": False,
-            "filter": is_not_stats_log,
-            "retention": "2 days",
-            "rotation": "3 hours",
-        },
-        {
-            "sink": "logs/stats.log",
-            "format": logfmt,
-            "level": "STATS",
-            "colorize": False,
-            "filter": is_stats_log,
-            "retention": "7 days",
-            "rotation": "1 days",
-        },
-        {
-            "sink": "logs/trace.log",
-            "format": logfmt,
-            "level": "TRACE",
-            "colorize": False,
-            "filter": is_trace_log,
-            "retention": "3 days",
-            "rotation": "1 days",
-            "backtrace": True,
-            "diagnose": True,
-        },
-    ],
-}
-logger.configure(**config)
+
+class HordeLog:
+    STDOUT_LEVELS = ["GENERATION", "PROMPT"]
+    INIT_LEVELS = ["INIT", "INIT_OK", "INIT_WARN", "INIT_ERR"]
+    MESSAGE_LEVELS = ["MESSAGE"]
+    STATS_LEVELS = ["STATS"]
+
+    # By default we're at error level or higher
+    verbosity = 20
+    quiet = 0
+
+    # Our sink IDs
+    sinks = []
+
+    @classmethod
+    def set_logger_verbosity(cls, count):
+        # The count comes reversed. So count = 0 means minimum verbosity
+        # While count 5 means maximum verbosity
+        # So the more count we have, the lowe we drop the versbosity maximum
+        cls.verbosity = 20 - (count * 10)
+
+    @classmethod
+    def quiesce_logger(cls, count):
+        # The bigger the count, the more silent we want our logger
+        cls.quiet = count * 10
+
+    @classmethod
+    def is_stdout_log(cls, record):
+        if record["level"].name not in HordeLog.STDOUT_LEVELS:
+            return False
+        if record["level"].no < cls.verbosity + cls.quiet:
+            return False
+        return True
+
+    @classmethod
+    def is_init_log(cls, record):
+        if record["level"].name not in HordeLog.INIT_LEVELS:
+            return False
+        if record["level"].no < cls.verbosity + cls.quiet:
+            return False
+        return True
+
+    @classmethod
+    def is_msg_log(cls, record):
+        if record["level"].name not in HordeLog.MESSAGE_LEVELS:
+            return False
+        if record["level"].no < cls.verbosity + cls.quiet:
+            return False
+        return True
+
+    @classmethod
+    def is_stderr_log(cls, record):
+        if (
+            record["level"].name
+            in HordeLog.STDOUT_LEVELS + HordeLog.INIT_LEVELS + HordeLog.MESSAGE_LEVELS + HordeLog.STATS_LEVELS
+        ):
+            return False
+        if record["level"].no < cls.verbosity + cls.quiet:
+            return False
+        return True
+
+    @classmethod
+    def is_stats_log(cls, record):
+        if record["level"].name not in HordeLog.STATS_LEVELS:
+            return False
+        return True
+
+    @classmethod
+    def is_not_stats_log(cls, record):
+        if record["level"].name in HordeLog.STATS_LEVELS:
+            return False
+        return True
+
+    @classmethod
+    def is_trace_log(cls, record):
+        if record["level"].name not in ["TRACE", "ERROR"]:
+            return False
+        return True
+
+    @classmethod
+    def test_logger(cls):
+        logger.generation(
+            "This is a generation message\nIt is typically multiline\nThee Lines".encode(
+                "unicode_escape",
+            ).decode("utf-8"),
+        )
+        logger.prompt("This is a prompt message")
+        logger.debug("Debug Message")
+        logger.info("Info Message")
+        logger.warning("Info Warning")
+        logger.error("Error Message")
+        logger.critical("Critical Message")
+        logger.init("This is an init message", status="Starting")
+        logger.init_ok("This is an init message", status="OK")
+        logger.init_warn("This is an init message", status="Warning")
+        logger.init_err("This is an init message", status="Error")
+        logger.message("This is user message")
+        sys.exit()
+
+    @classmethod
+    def initialise(cls, setup_logging=True):
+        if setup_logging:
+            cls.setup()
+            cls.set_sinks()
+        else:
+            cls.setup_compatibility()
+
+    @classmethod
+    def setup_compatibility(cls):
+        logger.__class__.generation = partialmethod(logger.__class__.log, "INFO")
+        logger.__class__.prompt = partialmethod(logger.__class__.log, "INFO")
+        logger.__class__.init = partialmethod(logger.__class__.log, "INIT")
+        logger.__class__.init_ok = partialmethod(logger.__class__.log, "INFO")
+        logger.__class__.init_warn = partialmethod(logger.__class__.log, "INFO")
+        logger.__class__.init_err = partialmethod(logger.__class__.log, "ERROR")
+        logger.__class__.message = partialmethod(logger.__class__.log, "INFO")
+        logger.__class__.stats = partialmethod(logger.__class__.log, "DEBUG")
+
+    @classmethod
+    def setup(cls):
+        cls.logfmt = (
+            "<level>{level: <10}</level> | <green>{time:YYYY-MM-DD HH:mm:ss.SSSSSS}</green> | "
+            "<green>{name}</green>:<green>{function}</green>:<green>{line}</green> - <level>{message}</level>"
+        )
+        cls.genfmt = (
+            "<level>{level: <10}</level> @ <green>{time:YYYY-MM-DD HH:mm:ss.SSSSSS}</green> | <level>{message}</level>"
+        )
+        cls.initfmt = (
+            "<magenta>INIT      </magenta> | <level>{extra[status]: <11}</level> | <magenta>{message}</magenta>"
+        )
+        cls.msgfmt = "<level>{level: <10}</level> | <level>{message}</level>"
+
+        try:
+            logger.level("GENERATION", no=24, color="<cyan>")
+            logger.level("PROMPT", no=23, color="<yellow>")
+            logger.level("INIT", no=31, color="<white>")
+            logger.level("INIT_OK", no=31, color="<green>")
+            logger.level("INIT_WARN", no=31, color="<yellow>")
+            logger.level("INIT_ERR", no=31, color="<red>")
+            # Messages contain important information without which this application might not be able to be used
+            # As such, they have the highest priority
+            logger.level("MESSAGE", no=61, color="<green>")
+            # Stats are info that might not display well in the terminal
+            logger.level("STATS", no=19, color="<blue>")
+        except TypeError:
+            pass
+
+        logger.__class__.generation = partialmethod(logger.__class__.log, "GENERATION")
+        logger.__class__.prompt = partialmethod(logger.__class__.log, "PROMPT")
+        logger.__class__.init = partialmethod(logger.__class__.log, "INIT")
+        logger.__class__.init_ok = partialmethod(logger.__class__.log, "INIT_OK")
+        logger.__class__.init_warn = partialmethod(logger.__class__.log, "INIT_WARN")
+        logger.__class__.init_err = partialmethod(logger.__class__.log, "INIT_ERR")
+        logger.__class__.message = partialmethod(logger.__class__.log, "MESSAGE")
+        logger.__class__.stats = partialmethod(logger.__class__.log, "STATS")
+
+    @classmethod
+    def set_sinks(cls):
+        # Remove any existing sinks that we added
+        for sink in cls.sinks:
+            try:
+                logger.remove(sink)
+            except ValueError:
+                # Someone else beat us to it
+                pass
+        cls.sinks = []
+
+        config = {
+            "handlers": [
+                {
+                    "sink": sys.stderr,
+                    "format": cls.logfmt,
+                    "colorize": True,
+                    "filter": cls.is_stderr_log,
+                },
+                {
+                    "sink": sys.stdout,
+                    "format": cls.genfmt,
+                    "level": "PROMPT",
+                    "colorize": True,
+                    "filter": cls.is_stdout_log,
+                },
+                {
+                    "sink": sys.stdout,
+                    "format": cls.initfmt,
+                    "level": "INIT",
+                    "colorize": True,
+                    "filter": cls.is_init_log,
+                },
+                {
+                    "sink": sys.stdout,
+                    "format": cls.msgfmt,
+                    "level": "MESSAGE",
+                    "colorize": True,
+                    "filter": cls.is_msg_log,
+                },
+                {
+                    "sink": "logs/bridge.log",
+                    "format": cls.logfmt,
+                    "level": "DEBUG",
+                    "colorize": False,
+                    "filter": cls.is_not_stats_log,
+                    "retention": "2 days",
+                    "rotation": "3 hours",
+                },
+                {
+                    "sink": "logs/stats.log",
+                    "format": cls.logfmt,
+                    "level": "STATS",
+                    "colorize": False,
+                    "filter": cls.is_stats_log,
+                    "retention": "7 days",
+                    "rotation": "1 days",
+                },
+                {
+                    "sink": "logs/trace.log",
+                    "format": cls.logfmt,
+                    "level": "TRACE",
+                    "colorize": False,
+                    "filter": cls.is_trace_log,
+                    "retention": "3 days",
+                    "rotation": "1 days",
+                    "backtrace": True,
+                    "diagnose": True,
+                },
+            ],
+        }
+
+        cls.sinks = logger.configure(**config)
```

### Comparing `hordelib-0.6.0/hordelib.egg-info/PKG-INFO` & `hordelib-0.6.1/hordelib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.6.0
+Version: 0.6.1
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,21 +675,22 @@
 Requires-Python: <3.11,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: CHANGELOG.md
 
 # hordelib
 
-[![PyPI version](https://badge.fury.io/py/hordelib.svg?branch=main&nocache=1)](https://badge.fury.io/py/hordelib)
-[![Downloads](https://pepy.tech/badge/hordelib)](https://pepy.tech/project/hordelib)
-![GitHub license](https://img.shields.io/github/license/jug-dev/hordelib)
-
-[![Build](https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
-[![Test Images](https://badgen.net/badge/main/latest-images/blue?icon=awesome)](http://hordelib.s3-website-eu-west-1.amazonaws.com/)
-[![Test Images](https://badgen.net/badge/develop/latest-images/blue?icon=awesome)](http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable)
+[![PyPI Version][pypi-image]][pypi-url]
+[![Downloads][downloads-image]][downloads-url]
+![GitHub license][license-url]
+
+[![Build][build-image]][build-url]
+[![Test Images][main-test-image]][main-test-url]
+[![Test Images][pr-test-image]][pr-test-url]
+[![Release Changelog][changelog-image]][changelog-url]
 
 `hordelib` is a thin wrapper around [ComfyUI](https://github.com/comfyanonymous/ComfyUI) primarily to enable the [AI Horde](https://aihorde.net/) to run inference pipelines designed visually in the ComfyUI GUI.
 
 The developers of this project can be found in the AI Horde Discord server: [https://discord.gg/3DxrhksKzn](https://discord.gg/3DxrhksKzn)
 
 NOTE: This project is in early development and is not yet in use by Stable Horde.
 
@@ -749,14 +750,23 @@
 pil_image.save("test.png")
 ```
 
 Note that `hordelib.initialise()` will erase all command line arguments from argv. So make sure you parse them before you call that.
 
 See `tests/run_*.py` for more standalone examples.
 
+### Logging
+
+If you don't want `hordelib` to setup and control the logging configuration initialise with:
+
+```python
+import hordelib
+hordelib.initialise(setup_logging=False)
+```
+
 ## Development
 
 Requirements:
 - `git` (install git)
 - `tox` (`pip install tox`)
 - Set the environmental variable `AIWORKER_CACHE_HOME` to point to a model directory.
 
@@ -885,7 +895,23 @@
 
 To create a patch file:
 - Make the required changes to a clean install of ComfyUI and then run `git diff > yourfile.patch` then move the patch file to wherever you want to save it.
 
 Note that the patch file _really_ needs to be in UTF-8 format and some common terminals, e.g. Powershell, won't do this by default. In Powershell to create a patch file use: `git diff | Set-Content -Encoding utf8 -Path yourfile.patch`
 
 Patches can be applied with the `hordelib.install_comfyui.Installer` classes `apply_patch()` method.
+
+<!-- Badges: -->
+
+[pypi-image]: https://badge.fury.io/py/hordelib.svg?branch=main&nocache=1
+[pypi-url]: https://badge.fury.io/py/hordelib
+[downloads-image]: https://pepy.tech/badge/hordelib
+[downloads-url]: https://pepy.tech/project/hordelib
+[license-url]: https://img.shields.io/github/license/jug-dev/hordelib
+[build-image]: https://github.com/jug-dev/hordelib/actions/workflows/maintests.yml/badge.svg?branch=main
+[build-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
+[main-test-image]: https://badgen.net/badge/main/latest-images/blue?icon=awesome
+[main-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/
+[pr-test-image]: https://badgen.net/badge/develop/latest-images/blue?icon=awesome
+[pr-test-url]: http://hordelib.s3-website-eu-west-1.amazonaws.com/unstable
+[changelog-image]: https://img.shields.io/badge/Release-Changelog-yellow
+[changelog-url]: https://github.com/jug-dev/hordelib/blob/releases/CHANGELOG.md
```

### Comparing `hordelib-0.6.0/hordelib.egg-info/SOURCES.txt` & `hordelib-0.6.1/hordelib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 .changelog
-.flake8
 .git-blame-ignore-revs
 .gitignore
 CHANGELOG.md
 LICENSE
 README.md
 build_helper.py
 pyproject.toml
```

### Comparing `hordelib-0.6.0/images/test_annotator.jpg` & `hordelib-0.6.1/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/images/test_db0.jpg` & `hordelib-0.6.1/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/images/test_facefix.png` & `hordelib-0.6.1/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/images/test_inpaint.png` & `hordelib-0.6.1/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/images/test_inpaint_alpha.png` & `hordelib-0.6.1/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/images/test_inpaint_mask.png` & `hordelib-0.6.1/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/images/test_inpaint_original.png` & `hordelib-0.6.1/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/images/test_outpaint.png` & `hordelib-0.6.1/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/pyproject.toml` & `hordelib-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     "default:::hordelib.*"
 ]
 testpaths = [
     "tests"
 ]
 
 [tool.black]
+line-length = 119
 # Exclude ComfyUI and any packages we have installed in nodes/
 exclude = '''
 /(
     ComfyUI
   | \.tox
   | nodes[\\/].*
 )/
```

### Comparing `hordelib-0.6.0/requirements.txt` & `hordelib-0.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/make_index.py` & `hordelib-0.6.1/tests/make_index.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/model_managers/test_comvis.py` & `hordelib-0.6.1/tests/model_managers/test_comvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/model_managers/test_diffusers.py` & `hordelib-0.6.1/tests/model_managers/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/model_managers/test_safety_checker.py` & `hordelib-0.6.1/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_controlnet.py` & `hordelib-0.6.1/tests/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_controlnet_annotator.py` & `hordelib-0.6.1/tests/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_facefix.py` & `hordelib-0.6.1/tests/run_facefix.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_img2img.py` & `hordelib-0.6.1/tests/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_img2img_hires.py` & `hordelib-0.6.1/tests/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_img2img_inpaint.py` & `hordelib-0.6.1/tests/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_img2img_inpaint_mask.py` & `hordelib-0.6.1/tests/run_img2img_inpaint_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_img2img_outpaint.py` & `hordelib-0.6.1/tests/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_inpainting.py` & `hordelib-0.6.1/tests/run_inpainting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_txt2img.py` & `hordelib-0.6.1/tests/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_txt2img_hires.py` & `hordelib-0.6.1/tests/run_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/run_upscale.py` & `hordelib-0.6.1/tests/run_upscale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_clip.py` & `hordelib-0.6.1/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_comfy.py` & `hordelib-0.6.1/tests/test_comfy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_comfy_install.py` & `hordelib-0.6.1/tests/test_comfy_install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_horde_controlnet_annotator.py` & `hordelib-0.6.1/tests/test_horde_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_horde_inference.py` & `hordelib-0.6.1/tests/test_horde_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_horde_inference_controlnet.py` & `hordelib-0.6.1/tests/test_horde_inference_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_horde_inference_img2img.py` & `hordelib-0.6.1/tests/test_horde_inference_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_horde_inference_painting.py` & `hordelib-0.6.1/tests/test_horde_inference_painting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_horde_pp.py` & `hordelib-0.6.1/tests/test_horde_pp.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,15 @@
         yield
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_RealESRGAN_x4plus(self):
         SharedModelManager.manager.load("RealESRGAN_x4plus")
-        assert (
-            SharedModelManager.manager.esrgan.is_model_loaded("RealESRGAN_x4plus")
-            is True
-        )
+        assert SharedModelManager.manager.esrgan.is_model_loaded("RealESRGAN_x4plus") is True
         data = {
             "model": "RealESRGAN_x4plus",
             "source_image": self.image,
         }
         assert self.horde is not None
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
@@ -50,18 +47,15 @@
         assert width == self.width * 4
         assert height == self.height * 4
         pil_image.save("images/horde_image_upscale_RealESRGAN_x4plus.webp", quality=90)
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_RealESRGAN_x2plus(self):
         SharedModelManager.manager.load("RealESRGAN_x2plus")
-        assert (
-            SharedModelManager.manager.esrgan.is_model_loaded("RealESRGAN_x2plus")
-            is True
-        )
+        assert SharedModelManager.manager.esrgan.is_model_loaded("RealESRGAN_x2plus") is True
         data = {
             "model": "RealESRGAN_x2plus",
             "source_image": self.image,
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
@@ -106,34 +100,30 @@
             "images/horde_image_upscale_RealESRGAN_x4plus_anime_6B.webp",
             quality=90,
         )
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_4x_AnimeSharp(self):
         SharedModelManager.manager.load("4x_AnimeSharp")
-        assert (
-            SharedModelManager.manager.esrgan.is_model_loaded("4x_AnimeSharp") is True
-        )
+        assert SharedModelManager.manager.esrgan.is_model_loaded("4x_AnimeSharp") is True
         data = {
             "model": "4x_AnimeSharp",
             "source_image": self.image,
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 4
         assert height == self.height * 4
         pil_image.save("images/horde_image_upscale_4x_AnimeSharp.webp", quality=90)
 
     @pytest.mark.mm_model("codeformer")
     def test_image_facefix_codeformers(self):
         SharedModelManager.manager.load("CodeFormers")
-        assert (
-            SharedModelManager.manager.codeformer.is_model_loaded("CodeFormers") is True
-        )
+        assert SharedModelManager.manager.codeformer.is_model_loaded("CodeFormers") is True
         data = {
             "model": "CodeFormers",
             "source_image": Image.open("images/test_facefix.png"),
         }
         pil_image = self.horde.image_facefix(data)
         assert pil_image is not None
         width, height = pil_image.size
```

### Comparing `hordelib-0.6.0/tests/test_inference.py` & `hordelib-0.6.1/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tests/test_safety_checker.py` & `hordelib-0.6.1/tests/test_safety_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,13 @@
         yield
         del self.horde
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
     def test_safety_checker_with_preload(self):
         SharedModelManager.manager.load("safety_checker")
-        assert (
-            SharedModelManager.manager.safety_checker.is_model_loaded("safety_checker")
-            is True
-        )
+        assert SharedModelManager.manager.safety_checker.is_model_loaded("safety_checker") is True
         assert is_image_nsfw(self.image) is False
 
     def test_safety_checker_without_preload(self):
-        assert (
-            SharedModelManager.manager.safety_checker.is_model_loaded("safety_checker")
-            is False
-        )
+        assert SharedModelManager.manager.safety_checker.is_model_loaded("safety_checker") is False
         assert is_image_nsfw(self.image) is False
```

### Comparing `hordelib-0.6.0/tests/test_shared_model_manager.py` & `hordelib-0.6.1/tests/test_shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.6.0/tox.ini` & `hordelib-0.6.1/tox.ini`

 * *Files identical despite different names*

