# Comparing `tmp/hordelib-0.5.12.tar.gz` & `tmp/hordelib-0.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hordelib-0.5.12.tar", last modified: Tue Apr 11 21:35:06 2023, max compression
+gzip compressed data, was "hordelib-0.5.18.tar", last modified: Tue Apr 11 23:00:56 2023, max compression
```

## Comparing `hordelib-0.5.12.tar` & `hordelib-0.5.18.tar`

### file list

```diff
@@ -1,636 +1,636 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.959448 hordelib-0.5.12/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 21:34:37.000000 hordelib-0.5.12/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 21:34:37.000000 hordelib-0.5.12/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.863441 hordelib-0.5.12/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.875442 hordelib-0.5.12/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 21:34:37.000000 hordelib-0.5.12/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-11 21:34:37.000000 hordelib-0.5.12/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-11 21:34:37.000000 hordelib-0.5.12/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-11 21:34:37.000000 hordelib-0.5.12/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 21:34:37.000000 hordelib-0.5.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48103 2023-04-11 21:35:06.959448 hordelib-0.5.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-11 21:34:37.000000 hordelib-0.5.12/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-11 21:34:37.000000 hordelib-0.5.12/build_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.875442 hordelib-0.5.12/hordelib/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 21:35:06.000000 hordelib-0.5.12/hordelib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.879442 hordelib-0.5.12/hordelib/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.879442 hordelib-0.5.12/hordelib/clip/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/clip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/clip/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/clip/coca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/clip/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    12030 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/clip/interrogate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/clip/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    14194 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/comfy_horde.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/config_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/horde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/install_comfy.patch
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/install_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.879442 hordelib-0.5.12/hordelib/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/aitemplate.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/blip.json
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/clip.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/codeformer.json
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/db.json
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/db_dep.json
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/db_embeds.json
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/diffusers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/esrgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/gfpgan.json
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/safety_checker.json
--rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_database/stable_diffusion.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.883442 hordelib-0.5.12/hordelib/model_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25054 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/blip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/codeformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/compvis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/esrgan.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/gfpgan.py
--rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/hyper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7081 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/model_manager/torch_hijack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.883442 hordelib-0.5.12/hordelib/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.883442 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.883442 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/binary/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/canny/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/color/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/hed/
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/install.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.887443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
--rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.891443 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.867441 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.895444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.895444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.899444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.899444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.867441 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.899444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.899444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.899444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.903444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.903444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.907444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.907444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.907444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.907444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.907444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.907444 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.915445 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.915445 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.919445 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.919445 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.923446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.923446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.923446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.871442 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.927446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.931446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.931446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.931446 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.935447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
--rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.935447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.939447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.939447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.939447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.939447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.939447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.939447 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.939447 hordelib-0.5.12/hordelib/nodes/facerestore/
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.943447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.943447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/align_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.943447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/retinaface/
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.943447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.943447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.943447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.943447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.947447 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/face_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/node_clip_similarities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/node_controlnet_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/node_image_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/node_image_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/node_model_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/nodes/node_upscale_model_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.947447 hordelib-0.5.12/hordelib/pipeline_designs/
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipeline_designs/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipeline_designs/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipeline_designs/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipeline_designs/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.947447 hordelib-0.5.12/hordelib/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipelines/pipeline_controlnet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipelines/pipeline_controlnet_annotator.json
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipelines/pipeline_image_facefix.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipelines/pipeline_image_upscale.json
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipelines/pipeline_stable_diffusion.json
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/pipelines/pipeline_stable_diffusion_paint.json
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/run_comfyui.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/shared_model_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.947447 hordelib-0.5.12/hordelib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     5913 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 21:34:37.000000 hordelib-0.5.12/hordelib/utils/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.879442 hordelib-0.5.12/hordelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48103 2023-04-11 21:35:06.000000 hordelib-0.5.12/hordelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38487 2023-04-11 21:35:06.000000 hordelib-0.5.12/hordelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:35:06.000000 hordelib-0.5.12/hordelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 21:35:06.000000 hordelib-0.5.12/hordelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 21:35:06.000000 hordelib-0.5.12/hordelib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.951448 hordelib-0.5.12/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_annotator.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_db0.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_facefix.png
--rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_inpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_inpaint_alpha.png
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_inpaint_mask.png
--rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_inpaint_original.png
--rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-11 21:34:37.000000 hordelib-0.5.12/images/test_outpaint.png
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-11 21:34:57.000000 hordelib-0.5.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 21:34:37.000000 hordelib-0.5.12/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 21:34:57.000000 hordelib-0.5.12/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 21:35:06.959448 hordelib-0.5.12/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.959448 hordelib-0.5.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/make_index.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:35:06.959448 hordelib-0.5.12/tests/model_managers/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/model_managers/test_comvis.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/model_managers/test_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/model_managers/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_facefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_img2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_img2img_inpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_img2img_outpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_inpainting.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_txt2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_txt2img_hires.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/run_upscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_comfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_comfy_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_horde_controlnet_annotator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_horde_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_horde_inference_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_horde_inference_img2img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_horde_inference_painting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_horde_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_safety_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_shared_model_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 21:34:37.000000 hordelib-0.5.12/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-11 21:34:37.000000 hordelib-0.5.12/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.755997 hordelib-0.5.18/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 23:00:33.000000 hordelib-0.5.18/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-11 23:00:33.000000 hordelib-0.5.18/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.671998 hordelib-0.5.18/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.679998 hordelib-0.5.18/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 23:00:33.000000 hordelib-0.5.18/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-11 23:00:33.000000 hordelib-0.5.18/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-11 23:00:33.000000 hordelib-0.5.18/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-11 23:00:33.000000 hordelib-0.5.18/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-11 23:00:33.000000 hordelib-0.5.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48103 2023-04-11 23:00:56.755997 hordelib-0.5.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-04-11 23:00:33.000000 hordelib-0.5.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 23:00:33.000000 hordelib-0.5.18/build_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.679998 hordelib-0.5.18/hordelib/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-11 23:00:56.000000 hordelib-0.5.18/hordelib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.679998 hordelib-0.5.18/hordelib/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.683998 hordelib-0.5.18/hordelib/clip/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/clip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/clip/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/clip/coca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/clip/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/clip/interrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/clip/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/comfy_horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/config_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/horde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/install_comfy.patch
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/install_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.683998 hordelib-0.5.18/hordelib/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/aitemplate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/blip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/clip.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/codeformer.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)   218801 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/db_dep.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/db_embeds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/diffusers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/esrgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/gfpgan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/safety_checker.json
+-rw-r--r--   0 runner    (1001) docker     (123)   243306 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_database/stable_diffusion.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.683998 hordelib-0.5.18/hordelib/model_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/codeformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/compvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/esrgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/gfpgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/model_manager/torch_hijack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/canny/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/canny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/color/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/hed/
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/install.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22985 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.687998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14625 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.691998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.695998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.671998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.695998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.695998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.699998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.699998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_160k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_40k.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/schedules/schedule_80k.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.671998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.699998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.699998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.699998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.699998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.703998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15999 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/swish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.703998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22125 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.703998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.703998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41996 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.707998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.707998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25196 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.707998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.711998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15624 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.715998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.715998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20867 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25157 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15805 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.715998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22532 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/iter_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.719998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.719998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.719998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26305 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.719998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.723997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.723997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19217 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.675998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.727997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.727997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.727997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.727997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.727997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/base_pixel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.727997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.731998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.735998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31035 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.735998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.735998 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24415 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18353 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18518 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18169 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.739997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.739997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.739997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.739997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.739997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.739997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/align_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/retinaface/
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/extract_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.743997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/bisenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/parsenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.747997 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23302 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/face_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/node_clip_similarities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/node_controlnet_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/node_image_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/node_image_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/node_model_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/nodes/node_upscale_model_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.747997 hordelib-0.5.18/hordelib/pipeline_designs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipeline_designs/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipeline_designs/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipeline_designs/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipeline_designs/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipeline_designs/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.747997 hordelib-0.5.18/hordelib/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipelines/pipeline_controlnet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipelines/pipeline_controlnet_annotator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipelines/pipeline_image_facefix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipelines/pipeline_image_upscale.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipelines/pipeline_stable_diffusion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/pipelines/pipeline_stable_diffusion_paint.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/run_comfyui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/shared_model_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.747997 hordelib-0.5.18/hordelib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 23:00:33.000000 hordelib-0.5.18/hordelib/utils/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.679998 hordelib-0.5.18/hordelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48103 2023-04-11 23:00:56.000000 hordelib-0.5.18/hordelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38487 2023-04-11 23:00:56.000000 hordelib-0.5.18/hordelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 23:00:56.000000 hordelib-0.5.18/hordelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 23:00:56.000000 hordelib-0.5.18/hordelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 23:00:56.000000 hordelib-0.5.18/hordelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.751997 hordelib-0.5.18/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71522 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_annotator.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36815 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_db0.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   538159 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_facefix.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1474994 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_inpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)   411844 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_inpaint_alpha.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_inpaint_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)   407128 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_inpaint_original.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1467500 2023-04-11 23:00:33.000000 hordelib-0.5.18/images/test_outpaint.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-11 23:00:48.000000 hordelib-0.5.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 23:00:33.000000 hordelib-0.5.18/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 23:00:48.000000 hordelib-0.5.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 23:00:56.755997 hordelib-0.5.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.755997 hordelib-0.5.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/make_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 23:00:56.755997 hordelib-0.5.18/tests/model_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/model_managers/test_comvis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/model_managers/test_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/model_managers/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_facefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_img2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_img2img_inpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_img2img_outpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_inpainting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_txt2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_txt2img_hires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/run_upscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_comfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_comfy_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_horde_controlnet_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_horde_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_horde_inference_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_horde_inference_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_horde_inference_painting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_horde_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_safety_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_shared_model_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 23:00:33.000000 hordelib-0.5.18/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-11 23:00:33.000000 hordelib-0.5.18/tox.ini
```

### Comparing `hordelib-0.5.12/.github/workflows/maintests.yml` & `hordelib-0.5.18/.github/workflows/maintests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/.github/workflows/prtests.yml` & `hordelib-0.5.18/.github/workflows/prtests.yml`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/.github/workflows/release.yml` & `hordelib-0.5.18/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -44,24 +44,27 @@
     # Install build deps
     - name: "🛠 Install pypa/build"
       if: ${{ steps.release.outputs.version != '' }}
       run: >-
         python -m pip install build --user
 
     - name: "✏️ Generate release changelog"
+      id: changelog
       if: ${{ steps.release.outputs.version != '' }}
       uses: heinrichreimer/github-changelog-generator-action@v2.3
       with:
         unreleased: false
         token: ${{ secrets.GITHUB_TOKEN }}
 
     # Patches our requirements.txt and pyproject.toml
     # Build a changelog
     - name: "🔧 Prepare our build for release"
       if: ${{ steps.release.outputs.version != '' }}
+      env:
+        CHANGELOG: ${{ steps.changelog.outputs.changelog }}
       run: >-
         python build_helper.py
 
     # Build a pypi distribution using the env var version number
     - name: "🔧 Build a binary wheel and a source tarball"
       if: ${{ steps.release.outputs.version != '' }}
       run: >-
```

### Comparing `hordelib-0.5.12/.gitignore` & `hordelib-0.5.18/.gitignore`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/LICENSE` & `hordelib-0.5.18/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/PKG-INFO` & `hordelib-0.5.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.5.12
+Version: 0.5.18
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-0.5.12/README.md` & `hordelib-0.5.18/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/build_helper.py` & `hordelib-0.5.18/build_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # build_helper.py
 # This is just a build helper script to build the pypi package.
+import os
 import subprocess
 
 
 def run(command):
     result = subprocess.run(command, shell=True, text=True)
     if result.returncode:
         raise Exception(result.stderr)
@@ -39,15 +40,32 @@
             newfile.append(f"#{line}")
         else:
             newfile.append(line)
     with open("pyproject.toml", "w") as outfile:
         outfile.writelines(newfile)
 
 
+def dump_changelog():
+    if os.path.exists("CHANGELOG.md"):
+        print(os.listdir())
+    else:
+        print("NO CHANGELOG.md")
+    try:
+        with open("CHANGELOG.md") as infile:
+            contents = infile.read()
+        print(contents)
+    except IOError:
+        pass
+
+    # with open("CHANGELOG.md", "wt") as outfile:
+    #     outfile.write(os.getenv("CHANGELOG", "coming soon"))
+
+
 patch_requirements()
 patch_toml()
+dump_changelog()
 
 # try:
 #     run(["python", "-m", "build"])
 # finally:
 #     patch_requirements(unpatch=True)
 #     patch_toml(unpatch=True)
```

### Comparing `hordelib-0.5.12/hordelib/cache/cache.py` & `hordelib-0.5.18/hordelib/cache/cache.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/clip/bulk.py` & `hordelib-0.5.18/hordelib/clip/bulk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/clip/coca.py` & `hordelib-0.5.18/hordelib/clip/coca.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/clip/image.py` & `hordelib-0.5.18/hordelib/clip/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/clip/interrogate.py` & `hordelib-0.5.18/hordelib/clip/interrogate.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         top = [
             {
                 "text": text_array[top_labels[0][i].numpy()],
                 "confidence": (top_probs[0][i].numpy() * 100),
             }
             for i in range(top_count)
         ]
-        return top
+        return top  # noqa: RET504
 
     def __call__(
         self,
         image: Image.Image = None,
         filename: str = None,
         directory: str = None,
         text_array: Union[List[str], Dict[str, List[str]], None] = None,
@@ -253,27 +253,27 @@
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
                 )
                 logger.debug(f"{k}: {results[k]}")
             return results
-        elif rank and not similarity:
+        if rank and not similarity:
             results = {}
             for k in text_array:
                 results[k] = self.rank(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
                     top_count,
                 )
                 logger.debug(f"{k}: {results[k]}")
             return results
-        else:
+        else:  # noqa: RET505
             similarity = {}
             for k in text_array:
                 similarity[k] = self.similarity(
                     image_features,
                     text_array[k],
                     k,
                     self.model_info["device"],
```

### Comparing `hordelib-0.5.12/hordelib/clip/text.py` & `hordelib-0.5.18/hordelib/clip/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,11 +67,11 @@
             text_features = self.model_info["model"].encode_text(text_tokens).float()
         text_features /= text_features.norm(dim=-1, keepdim=True)
         text_embed_array = text_features.cpu().detach().numpy()
         if filename:
             np.save(f"{self.cache.cache_dir}/{text_hash}", text_embed_array)
             self.cache.add_sqlite_row(filename, text_hash, text_hash)
             return None
-        else:
-            np.save(f"{self.cache.cache_dir}/{text_hash}", text_embed_array)
-            self.cache.add_sqlite_row(text, text_hash, text_hash)
-            return None
+
+        np.save(f"{self.cache.cache_dir}/{text_hash}", text_embed_array)
+        self.cache.add_sqlite_row(text, text_hash, text_hash)
+        return None
```

### Comparing `hordelib-0.5.12/hordelib/comfy_horde.py` & `hordelib-0.5.18/hordelib/comfy_horde.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,16 @@
     }
 
     # We may wish some ComfyUI standard nodes had different names for consistency. Here
     # we can dynamically rename some node input parameter names.
     NODE_PARAMETER_REPLACEMENTS = {
         "HordeCheckpointLoader": {
             # We name this "model_name" as then we can use the same generic code in our model loaders
-            "ckpt_name": "model_name"
-        }
+            "ckpt_name": "model_name",
+        },
     }
 
     def __init__(self) -> None:
         self.client_id = None  # used for receiving comfyUI async events
         self.pipelines = {}
 
         # Load our pipelines
@@ -231,28 +231,28 @@
                     break
 
                 current = current[k]
 
             if not skip:
                 if not current.get(keys[-1]):
                     logger.warning(
-                        f"Attempt to set parameter CREATED parameter '{key}'"
+                        f"Attempt to set parameter CREATED parameter '{key}'",
                     )
                 current[keys[-1]] = value
 
     # Connect the named input to the named node (output).
     # Used for dynamic switching of pipeline graphs
     @classmethod
     def reconnect_input(cls, dct, input, output):
         logger.debug(f"Request to reconnect input {input} to output {output}")
 
         # First check the output even exists
         if output not in dct.keys():
             logger.warning(
-                f"Can not reconnect input {input} to {output} as {output} does not exist"
+                f"Can not reconnect input {input} to {output} as {output} does not exist",
             )
             return None
 
         keys = input.split(".")
         if "inputs" not in keys:
             keys.insert(1, "inputs")
         current = dct
@@ -304,20 +304,24 @@
             if "controlnet_model_loader.model_manager" not in params:
                 logger.debug("Injecting controlnet model manager")
                 params["controlnet_model_loader.model_manager"] = SharedModelManager
             # Connect to the correct pre-processor node
             if params.get("return_control_map", False):
                 # Connect annotator to output image directly
                 self.reconnect_input(
-                    pipeline, "output_image.images", params["control_type"]
+                    pipeline,
+                    "output_image.images",
+                    params["control_type"],
                 )
             else:
                 # Connect annotator to controlnet apply node
                 self.reconnect_input(
-                    pipeline, "controlnet_apply.image", params["control_type"]
+                    pipeline,
+                    "controlnet_apply.image",
+                    params["control_type"],
                 )
 
         # Set the pipeline parameters
         self._set(pipeline, **params)
 
         # Run it!
         inference = execution.PromptExecutor(self)
```

### Comparing `hordelib-0.5.12/hordelib/config_path.py` & `hordelib-0.5.18/hordelib/config_path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/consts.py` & `hordelib-0.5.18/hordelib/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # consts.py
 import os
-from hordelib.config_path import get_hordelib_path
 from enum import Enum, auto
 
+from hordelib.config_path import get_hordelib_path
+
 COMFYUI_VERSION = "c767e9426ae81bed4f52c7be0625f0efc4cbe16b"
 """The exact version of ComfyUI version to load."""
 
 REMOTE_MODEL_DB = (
     "https://raw.githubusercontent.com/db0/AI-Horde-image-model-reference/main/"
 )
 """The default base endpoint where to find model databases. See MODEL_DB_NAMES for valid database names."""
```

### Comparing `hordelib-0.5.12/hordelib/horde.py` & `hordelib-0.5.18/hordelib/horde.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # horde.py
 # Main interface for the horde to this library.
 import contextlib
 
-from PIL import Image, UnidentifiedImageError
 from loguru import logger
+from PIL import Image, UnidentifiedImageError
 
 from hordelib.comfy_horde import Comfy_Horde
 from hordelib.shared_model_manager import SharedModelManager
 
 
 class HordeLib:
     # Horde to comfy sampler mapping
@@ -241,32 +241,32 @@
         try:
             # We must not resize during hires_fix as it causes the final image to come out blurry
             if source_image.size != (
                 payload["width"],
                 payload["height"],
             ) and not payload.get("hires_fix"):
                 payload["source_image"] = source_image.resize(
-                    (payload["width"], payload["height"])
+                    (payload["width"], payload["height"]),
                 )
         except (UnidentifiedImageError, AttributeError):
             logger.warning("Source image could not be parsed. Falling back to text2img")
             del payload["source_image"]
             del payload["source_processing"]
             return
         source_mask = payload.get("source_mask")
         if not source_mask:
             return
         try:
             if source_mask.size != (payload["width"], payload["height"]):
                 payload["source_mask"] = source_mask.resize(
-                    (payload["width"], payload["height"])
+                    (payload["width"], payload["height"]),
                 )
         except (UnidentifiedImageError, AttributeError):
             logger.warning(
-                "Source mask could not be parsed. Falling back to img2img without mask"
+                "Source mask could not be parsed. Falling back to img2img without mask",
             )
             del payload["source_mask"]
 
     def basic_inference(self, payload: dict[str, str | None]) -> Image.Image | None:
         generator = Comfy_Horde()
         # Validate our payload parameters
         self._validate_BASIC_INFERENCE_PARAMS(payload)
```

### Comparing `hordelib-0.5.12/hordelib/initialisation.py` & `hordelib-0.5.18/hordelib/initialisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Initialise hordelib.
 import sys
 
 from loguru import logger
 
 import hordelib.utils.logger
 from hordelib import install_comfy
-from hordelib.config_path import set_system_path, get_hordelib_path
+from hordelib.config_path import get_hordelib_path, set_system_path
 from hordelib.consts import (
     COMFYUI_VERSION,
     DEFAULT_MODEL_MANAGERS,
     MODEL_CATEGORY_NAMES,
     RELEASE_VERSION,
 )
 
@@ -21,15 +21,15 @@
     logger.level("DEBUG")  # XXX # FIXME
 
     # If developer mode, don't permit some things
     if not RELEASE_VERSION and " " in get_hordelib_path():
         # Our runtime patching can't handle this
         raise Exception(
             "Do not run this project in developer mode from a path that "
-            "contains spaces in directory names."
+            "contains spaces in directory names.",
         )
 
     # Ensure we have ComfyUI
     logger.debug("Clearing command line args in sys.argv before ComfyUI load")
     sys_arg_bkp = sys.argv.copy()
     sys.argv = sys.argv[:1]
     installer = install_comfy.Installer()
```

### Comparing `hordelib-0.5.12/hordelib/install_comfy.patch` & `hordelib-0.5.18/hordelib/install_comfy.patch`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/install_comfy.py` & `hordelib-0.5.18/hordelib/install_comfy.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,22 +30,21 @@
 
             return commit_hash
         except Exception:
             return ""
 
     @classmethod
     def _run_get_result(cls, command, directory=get_hordelib_path()):
-        result = subprocess.run(
+        return subprocess.run(
             command,
             shell=True,
             text=True,
             capture_output=True,
             cwd=directory,
         )
-        return result
 
     @classmethod
     def _run(cls, command, directory=get_hordelib_path()) -> tuple[bool, str] | None:
         try:
             result = cls._run_get_result(command, directory)
         except Exception as Ex:
             logger.error(Ex)
@@ -97,19 +96,21 @@
         cls._run("git pull", get_comfyui_path())
         cls._run(f"git checkout {comfy_version}", get_comfyui_path())
 
     @classmethod
     def apply_patch(cls, patchfile):
         # Check if the patch has already been applied
         result = cls._run_get_result(
-            f"git apply --check {patchfile}", get_comfyui_path()
+            f"git apply --check {patchfile}",
+            get_comfyui_path(),
         )
         could_apply = not result.returncode
         result = cls._run_get_result(
-            f"git apply --reverse --check {patchfile}", get_comfyui_path()
+            f"git apply --reverse --check {patchfile}",
+            get_comfyui_path(),
         )
         could_reverse = not result.returncode
         if could_apply:
             # Apply the patch
             logger.info(f"Applying patch {patchfile}")
             result = cls._run_get_result(f"git apply {patchfile}", get_comfyui_path())
             logger.debug(f"{result}")
```

### Comparing `hordelib-0.5.12/hordelib/model_database/aitemplate.json` & `hordelib-0.5.18/hordelib/model_database/aitemplate.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/blip.json` & `hordelib-0.5.18/hordelib/model_database/blip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/clip.json` & `hordelib-0.5.18/hordelib/model_database/clip.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/controlnet.json` & `hordelib-0.5.18/hordelib/model_database/controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/db.json` & `hordelib-0.5.18/hordelib/model_database/db.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/db_dep.json` & `hordelib-0.5.18/hordelib/model_database/db_dep.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/db_embeds.json` & `hordelib-0.5.18/hordelib/model_database/db_embeds.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/diffusers.json` & `hordelib-0.5.18/hordelib/model_database/diffusers.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/esrgan.json` & `hordelib-0.5.18/hordelib/model_database/esrgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/gfpgan.json` & `hordelib-0.5.18/hordelib/model_database/gfpgan.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/safety_checker.json` & `hordelib-0.5.18/hordelib/model_database/safety_checker.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_database/stable_diffusion.json` & `hordelib-0.5.18/hordelib/model_database/stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_manager/base.py` & `hordelib-0.5.18/hordelib/model_manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,17 @@
     def getFullModelPath(self, model_name: str):
         """Returns the fully qualified filename for the specified model."""
         ckpt_path = self.get_model_files(model_name)[0]["path"]  # XXX Rework?
         return f"{self.modelFolderPath}/{ckpt_path}"
 
     @abstractmethod
     def modelToRam(
-        self, model_name: str, **kwargs
+        self,
+        model_name: str,
+        **kwargs,
     ) -> dict[str, typing.Any]:  # XXX Flesh out signature
         """"""  # XXX # FIXME These functions need something resembling error detection/logging.
 
     def get_model(self, model_name: str):
         return self.model_reference.get(model_name)
 
     def get_model_files(self, model_name: str):
@@ -367,29 +369,23 @@
 
         # Default to sha256 hashes
         if "sha256sum" in file_details:
             logger.debug(f"Getting sha256sum of {full_path}")
             sha256_file_hash = self.get_file_sha256_hash(full_path)
             logger.debug(f"sha256sum: {sha256_file_hash}")
             logger.debug(f"Expected: {file_details['sha256sum']}")
-            if file_details["sha256sum"] != sha256_file_hash:
-                return False
-            else:
-                return True
+            return file_details["sha256sum"] == sha256_file_hash
 
         # If sha256 is not available, fall back to md5
         if "md5sum" in file_details:
             logger.debug(f"Getting md5sum of {full_path}")
             md5_file_hash = self.get_file_md5sum_hash(full_path)
             logger.debug(f"md5sum: {md5_file_hash}")
             logger.debug(f"Expected: {file_details['md5sum']}")
-            if file_details["md5sum"] != md5_file_hash:
-                return False
-            else:
-                return True
+            return file_details["md5sum"] != md5_file_hash
 
         # If no hashes available, return True for now
         # THIS IS A SECURITY RISK, EVENTUALLY WE SHOULD RETURN FALSE
         # But currently not all models specify hashes
         # XXX this warning preexists me (@tazlin), probably should look into it
 
         return True
@@ -491,54 +487,60 @@
                 input("")
                 continue
             # TODO: simplify
             if "file_content" in download[i]:
                 file_content = download[i]["file_content"]
                 logger.info(f"writing {file_content} to {file_path}")
                 os.makedirs(
-                    os.path.join(self.modelFolderPath, download_path), exist_ok=True
+                    os.path.join(self.modelFolderPath, download_path),
+                    exist_ok=True,
                 )
                 with open(
                     os.path.join(
-                        self.modelFolderPath, os.path.join(download_path, download_name)
+                        self.modelFolderPath,
+                        os.path.join(download_path, download_name),
                     ),
                     "w",
                 ) as f:
                     f.write(file_content)
             elif "symlink" in download[i]:
                 logger.info(f"symlink {file_path} to {download[i]['symlink']}")
                 symlink = download[i]["symlink"]
                 os.makedirs(
-                    os.path.join(self.modelFolderPath, download_path), exist_ok=True
+                    os.path.join(self.modelFolderPath, download_path),
+                    exist_ok=True,
                 )
                 os.symlink(
                     symlink,
                     os.path.join(
-                        self.modelFolderPath, os.path.join(download_path, download_name)
+                        self.modelFolderPath,
+                        os.path.join(download_path, download_name),
                     ),
                 )
             elif "git" in download[i]:
                 logger.info(f"git clone {download_url} to {file_path}")
                 os.makedirs(
-                    os.path.join(self.modelFolderPath, file_path), exist_ok=True
+                    os.path.join(self.modelFolderPath, file_path),
+                    exist_ok=True,
                 )
                 git.Git(os.path.join(self.modelFolderPath, file_path)).clone(
-                    download_url
+                    download_url,
                 )
             elif "unzip" in download[i]:
                 zip_path = f"{self.modelFolderPath}/{download_name}.zip"
                 temp_path = f"{self.modelFolderPath}/{str(uuid4())}/"
                 os.makedirs(temp_path, exist_ok=True)
                 self.download_file(download_url, zip_path)
                 logger.info(f"unzip {zip_path}")
                 with zipfile.ZipFile(zip_path, "r") as zip_ref:
                     zip_ref.extractall(temp_path)
                 logger.info(f"moving {temp_path} to {download_path}")
                 shutil.move(
-                    temp_path, os.path.join(self.modelFolderPath, download_path)
+                    temp_path,
+                    os.path.join(self.modelFolderPath, download_path),
                 )
                 logger.info(f"delete {zip_path}")
                 os.remove(zip_path)
                 logger.info(f"delete {temp_path}")
                 shutil.rmtree(temp_path)
             else:
                 if (
@@ -595,16 +597,16 @@
                     "sm": torch.cuda.get_device_capability(i)[0] * 10
                     + torch.cuda.get_device_capability(i)[1],
                 }
                 cuda_arch.append(cuda_device)
             cuda_arch = sorted(cuda_arch, key=lambda k: k["sm"], reverse=True)
             recommended_gpu = [x for x in cuda_arch if x["sm"] == cuda_arch[0]["sm"]]
             return cuda_arch, recommended_gpu
-        else:
-            return None, None
+
+        return None, None
 
     def get_filtered_models(self, **kwargs):
         """
         Get all models
         :param kwargs: filter based on metadata of the model reference db
         :return: list of models
         """
```

### Comparing `hordelib-0.5.12/hordelib/model_manager/blip.py` & `hordelib-0.5.18/hordelib/model_manager/blip.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,33 +68,33 @@
         model_name,
         half_precision=True,
         gpu_id=0,
         cpu_only=False,
         blip_image_eval_size=512,
     ):
         raise NotImplementedError("BLIP is not currently implemented!")
-        if not self.cuda_available:
-            cpu_only = True
-        vit = "base" if model_name == "BLIP" else "large"
-        model_path = self.get_model_files(model_name)[0]["path"]
-        model_path = f"{self.modelFolderPath}/{model_path}"
-        if cpu_only:
-            device = torch.device("cpu")
-            half_precision = False
-        else:
-            device = torch.device(f"cuda:{gpu_id}" if self.cuda_available else "cpu")
-        logger.info(f"Loading model {model_name} on {device}")
-        logger.info(f"Model path: {model_path}")
-        with importlib_resources.as_file(self.pkg / "med_config.json") as med_config:
-            logger.info(f"Med config path: {med_config}")
-            model = blip_decoder(
-                # XXX # FIXME
-                pretrained=model_path,
-                med_config=med_config,
-                image_size=blip_image_eval_size,
-                vit=vit,
-            )
-        model = model.eval()
-        model.to(device)
-        if half_precision:
-            model = model.half()
-        return {"model": model, "device": device, "half_precision": half_precision}
+        # if not self.cuda_available:
+        #     cpu_only = True
+        # vit = "base" if model_name == "BLIP" else "large"
+        # model_path = self.get_model_files(model_name)[0]["path"]
+        # model_path = f"{self.modelFolderPath}/{model_path}"
+        # if cpu_only:
+        #     device = torch.device("cpu")
+        #     half_precision = False
+        # else:
+        #     device = torch.device(f"cuda:{gpu_id}" if self.cuda_available else "cpu")
+        # logger.info(f"Loading model {model_name} on {device}")
+        # logger.info(f"Model path: {model_path}")
+        # with importlib_resources.as_file(self.pkg / "med_config.json") as med_config:
+        #     logger.info(f"Med config path: {med_config}")
+        #     model = blip_decoder(
+        #         # XXX # FIXME
+        #         pretrained=model_path,
+        #         med_config=med_config,
+        #         image_size=blip_image_eval_size,
+        #         vit=vit,
+        #     )
+        # model = model.eval()
+        # model.to(device)
+        # if half_precision:
+        #     model = model.half()
+        # return {"model": model, "device": device, "half_precision": half_precision}
```

### Comparing `hordelib-0.5.12/hordelib/model_manager/clip.py` & `hordelib-0.5.18/hordelib/model_manager/clip.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,24 @@
     def __init__(self, download_reference=False):
         super().__init__(
             models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.clip],
             download_reference=download_reference,
         )
 
     def load_data_lists(self):
-        data_lists = {}
+        # data_lists = {}
         # data_lists["artist"] = load_list(self.pkg / "artists.txt")
         # data_lists["flavors"] = load_list(self.pkg / "flavors.txt")
         # data_lists["medium"] = load_list(self.pkg / "mediums.txt")
         # data_lists["movement"] = load_list(self.pkg / "movements.txt")
         # data_lists["trending"] = load_list(self.pkg / "sites.txt")
         # data_lists["techniques"] = load_list(self.pkg / "techniques.txt")
         # data_lists["tags"] = load_list(self.pkg / "tags.txt")
-        return data_lists
+        # return data_list
+        return {}
 
     def load_coca(self, model_name, half_precision=True, gpu_id=0, cpu_only=False):
         model_path = self.get_model_files(model_name)[0]["path"]
         model_path = f"{self.modelFolderPath}/{model_path}"
         if cpu_only:
             device = torch.device("cpu")
             half_precision = False
@@ -145,15 +146,15 @@
                 half_precision,
                 gpu_id,
                 cpu_only,
             )
             self.loaded_models[model_name] = loaded_model_info
         else:
             logger.error(
-                f"Unknown model type: {self.model_reference[model_name]['type']}"
+                f"Unknown model type: {self.model_reference[model_name]['type']}",
             )
             return None
         if not loaded_model_info:
             logger.init_error(f"Failed to load {model_name}", status="Error")
             return None
 
         logger.info(f"Loading {model_name}", status="Success")  # logger.init_ok
```

### Comparing `hordelib-0.5.12/hordelib/model_manager/codeformer.py` & `hordelib-0.5.18/hordelib/model_manager/codeformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_manager/compvis.py` & `hordelib-0.5.18/hordelib/model_manager/compvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_manager/controlnet.py` & `hordelib-0.5.18/hordelib/model_manager/controlnet.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             models_db_name=MODEL_DB_NAMES[MODEL_CATEGORY_NAMES.controlnet],
             download_reference=download_reference,
         )
         self.control_nets = {}
 
     def modelToRam(self, model_name: str):
         raise NotImplementedError(
-            "Controlnet requires special handling. Use `ControlNetModelManager.merge_controlnet(...)` instead of `load()`."
+            "Controlnet requires special handling. Use `ControlNetModelManager.merge_controlnet(...)` instead of `load()`.",
         )  # XXX # TODO There might be way to avoid this.
 
     def merge_controlnet(
         self,
         control_type,
         model,
         model_baseline="stable diffusion 1",
@@ -40,31 +40,34 @@
             logger.info(
                 f"{controlnet_name} downloaded",
                 status="Downloading",
             )  # logger.init_ok
 
         logger.info(f"{control_type}", status="Merging")  # logger.init
         controlnet_path = os.path.join(
-            self.modelFolderPath, self.get_controlnet_filename(controlnet_name)
+            self.modelFolderPath,
+            self.get_controlnet_filename(controlnet_name),
         )
         controlnet = horde_load_controlnet(
             controlnet_path=controlnet_path,
             target_model=model,
         )
         return (controlnet,)
 
     def download_control_type(
-        self, control_type, sd_baselines=["stable diffusion 1", "stable diffusion 2"]
+        self,
+        control_type,
+        sd_baselines=["stable diffusion 1", "stable diffusion 2"],
     ):
         # We need to do a rename, as they're named differently in the model reference
         for bl in sd_baselines:
             controlnet_name = self.get_controlnet_name(control_type, bl)
             if controlnet_name not in self.model_reference:
                 logger.warning(
-                    f"Could not find {controlnet_name} reference to download"
+                    f"Could not find {controlnet_name} reference to download",
                 )
                 continue
             self.download_model(controlnet_name)
 
     def get_controlnet_name(self, control_type, sd_baseline):
         """We have control nets for both SD and SD2
         So to know which version we need, se use this method to map general control_type (e.g. 'canny')
@@ -73,15 +76,17 @@
         baseline_appends = {
             "stable diffusion 1": "",
             "stable diffusion 2": "_sd2",
         }
         return f"control_{control_type}{baseline_appends[sd_baseline]}"
 
     def check_control_type_available(
-        self, control_type, sd_baseline="stable diffusion 1"
+        self,
+        control_type,
+        sd_baseline="stable diffusion 1",
     ):
         # We need to do a rename, as they're named differently in the model reference
         controlnet_name = self.get_controlnet_name(control_type, sd_baseline)
         return self.check_model_available(controlnet_name)
 
     def get_controlnet_filename(self, controlnet_name) -> str | None:
         """Gets the `.safetensors` filename for the model
```

### Comparing `hordelib-0.5.12/hordelib/model_manager/diffusers.py` & `hordelib-0.5.18/hordelib/model_manager/diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_manager/esrgan.py` & `hordelib-0.5.18/hordelib/model_manager/esrgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_manager/gfpgan.py` & `hordelib-0.5.18/hordelib/model_manager/gfpgan.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/model_manager/hyper.py` & `hordelib-0.5.18/hordelib/model_manager/hyper.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,17 @@
             if getattr(self, argName) is not None:
                 continue
 
             modelmanager = MODEL_MANAGERS_TYPE_LOOKUP[argName]
 
             # at runtime modelmanager() will be CompVisModelManager(), ClipModelManager(), etc
             setattr(
-                self, argName, modelmanager(download_reference=False)
+                self,
+                argName,
+                modelmanager(download_reference=False),
             )  # XXX # FIXME # HACK
 
         self.refreshManagers()
 
     def refreshManagers(self) -> None:  # XXX rename + docstring rewrite
         """Called when one of the `BaseModelManager` changes, updating `available_models`."""
         model_types = [
```

### Comparing `hordelib-0.5.12/hordelib/model_manager/safety_checker.py` & `hordelib-0.5.18/hordelib/model_manager/safety_checker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typing
+
 import torch
 from diffusers.pipelines.stable_diffusion.safety_checker import (
     StableDiffusionSafetyChecker,
 )
 from loguru import logger
 
 from hordelib.consts import MODEL_CATEGORY_NAMES, MODEL_DB_NAMES
```

### Comparing `hordelib-0.5.12/hordelib/model_manager/torch_hijack.py` & `hordelib-0.5.18/hordelib/model_manager/torch_hijack.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import transformers
 
 
 def instantiate_from_config(config):
     if "target" not in config:
         if config == "__is_first_stage__":
             return None
-        elif config == "__is_unconditional__":
+        if config == "__is_unconditional__":
             return None
         raise KeyError("Expected key `target` to instantiate.")
     return get_obj_from_str(config["target"])(**config.get("params", {}))
 
 
 def get_obj_from_str(string, reload=False):
     module, cls = string.rsplit(".", 1)
```

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/README.md` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/README.md`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/color/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/hed/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/install.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/LICENSE`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/get_data.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/guidedfilter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/html.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/image_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/leres/pix2pix/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/api.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/midas/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mp_face_mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/mp_pose_hand/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/body.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/openpose/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/pidinet/model.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/ade20k.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/cityscapes_769x769.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_context_59.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/pascal_voc12.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ann_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/apcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ccnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/danet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/deeplabv3plus_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dmnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/dnl_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/emanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/encnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fcn_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/fpn_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/gcnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/lraspp_m-v3-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/nonlocal_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_hr18.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/ocrnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pointrend_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/psanet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_r50-d8.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/pspnet_unet_s5-d16.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_r50.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/configs/_base_/models/upernet_uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_g.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_h32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/exp/upernet_global_small/test_config_w32.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/arraymisc/quantization.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/alexnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/activation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/context_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv2d_adaptive_padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/conv_ws.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/depthwise_separable_conv_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/generalized_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hsigmoid.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/hswish.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/non_local.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/norm.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/padding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/plugin.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/scale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/transformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/upsample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/bricks/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/flops_counter.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/fuse_conv_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/cnn/vgg.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/engine/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/geometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/image/photometric.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/mmcls.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/model_zoo/open_mmlab.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/assign_score_withk.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/ball_query.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/border_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/box_iou_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/carafe.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/cc_attention.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/contour_expand.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/corner_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/correlation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deform_roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/deprecated_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/focal_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/furthest_point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/fused_bias_leakyrelu.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/gather_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/group_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/info.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/iou3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/knn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/masked_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/merge_cells.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/modulated_deform_conv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/multi_scale_deform_attn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/nms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/pixel_group.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/point_sample.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_in_boxes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/points_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/psa_mask.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roi_pool.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roiaware_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/roipoint_pool3d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/saconv.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/scatter_points.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/sync_bn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_interpolate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/three_nn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/tin_shift.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/ops/voxelize.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/_functions.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_container.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/distributed_deprecated.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/scatter_gather.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/parallel/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_module.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/base_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/dist_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/epoch_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/fp16_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/ema.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/evaluation.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/dvclive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/mlflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/neptune.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/pavi.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/text.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/logger/wandb.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/momentum_updater.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/profiler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sampler_seed.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/hooks/sync_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/iter_based_runner.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/log_buffer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/priority.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/runner/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/config.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/ext_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_jit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/path.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/registry.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/testing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/timer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/trace.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/version.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/io.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/video/processing.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/color.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/image.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv/visualization/optflow.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmcv_custom/checkpoint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/test.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/apis/train.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/class_names.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/eval_hooks.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/core/seg/sampler/ohem_pixel_sampler.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/ade.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/chase_db1.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/custom.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/dataset_wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/hrf.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pascal_context.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/compose.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/formating.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/loading.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/pipelines/transforms.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/stare.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/datasets/voc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/cgnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/fast_scnn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/hrnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnest.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/resnext.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/unet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/uniformer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/builder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ann_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/apc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cascade_decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/cc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/da_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/decode_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dm_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/dnl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ema_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/enc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/fpn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/gc_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/lraspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/nl_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/ocr_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/point_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psa_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/psp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_aspp_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/sep_fcn_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/decode_heads/uper_head.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/accuracy.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/dice_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/lovasz_loss.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/losses/utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/fpn.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/necks/multilevel_neck.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/base.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/cascade_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/segmentors/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/drop.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/inverted_residual.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/make_divisible.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/res_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/se_layer.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/self_attention_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/up_conv_block.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/models/utils/weight_init.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/encoding.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/ops/wrappers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/uniformer/mmseg/utils/logger.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/comfy_controlnet_preprocessors/util.py` & `hordelib-0.5.18/hordelib/nodes/comfy_controlnet_preprocessors/util.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/__init__.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/__init__.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/align_trans.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/align_trans.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/matlab_cp2tform.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_net.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/retinaface/retinaface_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/face_detector.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/common.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/experimental.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolo.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/general.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/detection/yolov5face/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/__init__.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/bisenet.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/bisenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/parsenet.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/parsenet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/parsing/resnet.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/parsing/resnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/face_restoration_helper.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/face_utils.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/face_utils.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/facerestore/facelib/utils/misc.py` & `hordelib-0.5.18/hordelib/nodes/facerestore/facelib/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/node_clip_similarities.py` & `hordelib-0.5.18/hordelib/nodes/node_clip_similarities.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/node_controlnet_model_loader.py` & `hordelib-0.5.18/hordelib/nodes/node_controlnet_model_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,13 +32,13 @@
             raise RuntimeError  # XXX better guarantees need to be made
 
         merged_model = model_manager.manager.controlnet.merge_controlnet(
             control_net_name,
             model,
         )
 
-        return merged_model
+        return merged_model  # noqa: RET504
 
 
 NODE_CLASS_MAPPINGS = {"HordeDiffControlNetLoader": HordeDiffControlNetLoader}
 
 logger.debug("Loaded HordeDiffControlNetLoader")
```

### Comparing `hordelib-0.5.12/hordelib/nodes/node_image_loader.py` & `hordelib-0.5.18/hordelib/nodes/node_image_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/node_image_output.py` & `hordelib-0.5.18/hordelib/nodes/node_image_output.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/node_model_loader.py` & `hordelib-0.5.18/hordelib/nodes/node_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/nodes/node_upscale_model_loader.py` & `hordelib-0.5.18/hordelib/nodes/node_upscale_model_loader.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipeline_designs/pipeline_controlnet.json` & `hordelib-0.5.18/hordelib/pipeline_designs/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipeline_designs/pipeline_controlnet_annotator.json` & `hordelib-0.5.18/hordelib/pipeline_designs/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipeline_designs/pipeline_image_facefix.json` & `hordelib-0.5.18/hordelib/pipeline_designs/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipeline_designs/pipeline_image_upscale.json` & `hordelib-0.5.18/hordelib/pipeline_designs/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipeline_designs/pipeline_stable_diffusion.json` & `hordelib-0.5.18/hordelib/pipeline_designs/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.5.18/hordelib/pipeline_designs/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json` & `hordelib-0.5.18/hordelib/pipeline_designs/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipelines/pipeline_controlnet.json` & `hordelib-0.5.18/hordelib/pipelines/pipeline_controlnet.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipelines/pipeline_controlnet_annotator.json` & `hordelib-0.5.18/hordelib/pipelines/pipeline_controlnet_annotator.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipelines/pipeline_image_facefix.json` & `hordelib-0.5.18/hordelib/pipelines/pipeline_image_facefix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipelines/pipeline_image_upscale.json` & `hordelib-0.5.18/hordelib/pipelines/pipeline_image_upscale.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipelines/pipeline_stable_diffusion.json` & `hordelib-0.5.18/hordelib/pipelines/pipeline_stable_diffusion.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json` & `hordelib-0.5.18/hordelib/pipelines/pipeline_stable_diffusion_hires_fix.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/pipelines/pipeline_stable_diffusion_paint.json` & `hordelib-0.5.18/hordelib/pipelines/pipeline_stable_diffusion_paint.json`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/run_comfyui.py` & `hordelib-0.5.18/hordelib/run_comfyui.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class ComfyWebAppLauncher:
     @classmethod
     def run_comfyui(cls):
         # Launch a browser
         webbrowser.open("http://127.0.0.1:8188/")
         logger.warning(
-            "Wait a moment and then refresh your browser. It takes a while to load the backend."
+            "Wait a moment and then refresh your browser. It takes a while to load the backend.",
         )
 
         # Tell comfyui where are custom nodes are
         os.environ["AIWORKER_CUSTOM_NODES"] = os.path.join(get_hordelib_path(), "nodes")
 
         # Now launch the comfyui process and replace our current process
         os.chdir(get_comfyui_path())
```

### Comparing `hordelib-0.5.12/hordelib/safety_checker.py` & `hordelib-0.5.18/hordelib/safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/shared_model_manager.py` & `hordelib-0.5.18/hordelib/shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/utils/cast.py` & `hordelib-0.5.18/hordelib/utils/cast.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/hordelib/utils/logger.py` & `hordelib-0.5.18/hordelib/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         return False
     return True
 
 
 def test_logger():
     logger.generation(
         "This is a generation message\nIt is typically multiline\nThee Lines".encode(
-            "unicode_escape"
+            "unicode_escape",
         ).decode("utf-8"),
     )
     logger.prompt("This is a prompt message")
     logger.debug("Debug Message")
     logger.info("Info Message")
     logger.warning("Info Warning")
     logger.error("Error Message")
```

### Comparing `hordelib-0.5.12/hordelib.egg-info/PKG-INFO` & `hordelib-0.5.18/hordelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hordelib
-Version: 0.5.12
+Version: 0.5.18
 Summary: A thin wrapper around ComfyUI to allow use by AI Horde.
 Author-email: Jug <jugdev@proton.me>, db0 <mail@dbzer0.com>, tazlin <tazlin.on.github@gmail.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `hordelib-0.5.12/hordelib.egg-info/SOURCES.txt` & `hordelib-0.5.18/hordelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_annotator.jpg` & `hordelib-0.5.18/images/test_annotator.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_db0.jpg` & `hordelib-0.5.18/images/test_db0.jpg`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_facefix.png` & `hordelib-0.5.18/images/test_facefix.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_inpaint.png` & `hordelib-0.5.18/images/test_inpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_inpaint_alpha.png` & `hordelib-0.5.18/images/test_inpaint_alpha.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_inpaint_mask.png` & `hordelib-0.5.18/images/test_inpaint_mask.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_inpaint_original.png` & `hordelib-0.5.18/images/test_inpaint_original.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/images/test_outpaint.png` & `hordelib-0.5.18/images/test_outpaint.png`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/pyproject.toml` & `hordelib-0.5.18/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 
 [tool.ruff] # XXX this isn't part of CI yet
 line-length=100 # XXX is this length settled on?
 exclude=["comfy_controlnet_preprocessors", "facerestore"]
 ignore=[
     "E501", # XXX line too long (comments are the big offender right now)
     "F401", # imported but unused
+    "E402", # Module level import not at top of file
+    "A002", # Argument `x` is shadowing a python builtin
+    "A001", # Variable `x` is shadowing a python builtin
+    "INP001", # ... is part of an implicit namespace package. Add an `__init__.py`.
 ]
 select = [
     "A",    # flake8-builtins
     "I",    # isort
     # "S",    # Bandit
     "F",    # pyflakes
     "E",    # pycodestyle errors
@@ -91,15 +95,15 @@
     "INP",  # flake8-no-pep420
     "PIE",  # flake8-pie
     # "T20",  # flake8-print
     # "UP",   # pyupgrade
     "RSE",  # flake8-raise
     "RET",  # flake8-return
     # "SLF",  # flake8-self
-    "SIM",  # flake8-simplify
-    "ARG",  # flake8-unused-arguments
+    # "SIM",  # flake8-simplify
+    # "ARG",  # flake8-unused-arguments
     # "TRY",  # tryceratops
     "RUF100"
 ]
 
 [tool.ruff.per-file-ignores]
 "comfy_horde.py" = ["I001", "F401"]
```

### Comparing `hordelib-0.5.12/requirements.txt` & `hordelib-0.5.18/requirements.txt`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/make_index.py` & `hordelib-0.5.18/tests/make_index.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # make_index.py
 # This isn't a test.
 # It's a 30 second hack to create an index.html that shows all our tests results.
-import os
-import glob
 import datetime
-
+import glob
+import os
 
 TEMPLATE = """
 <!DOCTYPE html>
 <html lang="en">
 <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
@@ -90,15 +89,16 @@
         in_refs.append(href(filename))
 
     # Poor man's template engine :)
     refs.sort()
     indexhtml = TEMPLATE.replace("[images]", "".join(refs))
     indexhtml = indexhtml.replace("[input_images]", "".join(in_refs))
     indexhtml = indexhtml.replace(
-        "[timestamp]", datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S")
+        "[timestamp]",
+        datetime.datetime.utcnow().strftime("%Y-%m-%d %H:%M:%S"),
     )
 
     # Output results
     with open("images/index.html", "wt") as outfile:
         outfile.write(indexhtml)
```

### Comparing `hordelib-0.5.12/tests/model_managers/test_comvis.py` & `hordelib-0.5.18/tests/model_managers/test_comvis.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/model_managers/test_diffusers.py` & `hordelib-0.5.18/tests/model_managers/test_diffusers.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/model_managers/test_safety_checker.py` & `hordelib-0.5.18/tests/model_managers/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_controlnet.py` & `hordelib-0.5.18/tests/run_controlnet.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_controlnet_annotator.py` & `hordelib-0.5.18/tests/run_controlnet_annotator.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_facefix.py` & `hordelib-0.5.18/tests/run_facefix.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_img2img.py` & `hordelib-0.5.18/tests/run_img2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_img2img_hires.py` & `hordelib-0.5.18/tests/run_img2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_img2img_inpaint.py` & `hordelib-0.5.18/tests/run_img2img_inpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_img2img_outpaint.py` & `hordelib-0.5.18/tests/run_img2img_outpaint.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_inpainting.py` & `hordelib-0.5.18/tests/run_inpainting.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_txt2img.py` & `hordelib-0.5.18/tests/run_txt2img.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_txt2img_hires.py` & `hordelib-0.5.18/tests/run_txt2img_hires.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/run_upscale.py` & `hordelib-0.5.18/tests/run_upscale.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/test_clip.py` & `hordelib-0.5.18/tests/test_clip.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/test_comfy.py` & `hordelib-0.5.18/tests/test_comfy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # test_setup.py
 import glob
+
 import pytest
 
 from hordelib.comfy_horde import Comfy_Horde
 
 
 class TestSetup:
     NUMBER_OF_PIPELINES = len(glob.glob("hordelib/pipelines/*.json"))
```

### Comparing `hordelib-0.5.12/tests/test_comfy_install.py` & `hordelib-0.5.18/tests/test_comfy_install.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/test_horde_controlnet_annotator.py` & `hordelib-0.5.18/tests/test_horde_controlnet_annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 
         for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
             if preproc == "scribble":
                 # Not valid for normal image input test
                 continue
             assert (
                 SharedModelManager.manager.controlnet.check_control_type_available(
-                    preproc, "stable diffusion 1"
+                    preproc,
+                    "stable diffusion 1",
                 )
                 is True
             )
             data["control_type"] = preproc
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
             pil_image.save(f"images/horde_annotator_{preproc}.webp", quality=90)
```

### Comparing `hordelib-0.5.12/tests/test_horde_inference.py` & `hordelib-0.5.18/tests/test_horde_inference.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/test_horde_inference_controlnet.py` & `hordelib-0.5.18/tests/test_horde_inference_controlnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 
         for preproc in HordeLib.CONTROLNET_IMAGE_PREPROCESSOR_MAP.keys():
             if preproc == "scribble":
                 # Not valid for normal image input test
                 continue
             assert (
                 SharedModelManager.manager.controlnet.check_control_type_available(
-                    preproc, "stable diffusion 1"
+                    preproc,
+                    "stable diffusion 1",
                 )
                 is True
             )
             data["control_type"] = preproc
             pil_image = self.horde.basic_inference(data)
             assert pil_image is not None
             pil_image.save(f"images/horde_controlnet_{preproc}.webp", quality=90)
```

### Comparing `hordelib-0.5.12/tests/test_horde_inference_img2img.py` & `hordelib-0.5.18/tests/test_horde_inference_img2img.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,9 +215,10 @@
             "n_iter": 1,
             "model": "Deliberate",
             "source_image": "THIS SHOULD FAILOVER TO TEXT2IMG",
             "source_processing": "img2img",
         }
         assert self.horde is not None
         pil_image = self.horde.basic_inference(data)
+        assert pil_image is not None
         assert "source_image" not in data
         assert "source_processing" not in data
```

### Comparing `hordelib-0.5.12/tests/test_horde_inference_painting.py` & `hordelib-0.5.18/tests/test_horde_inference_painting.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         SharedModelManager._instance = None
         SharedModelManager.manager = None
 
     def test_inpainting_alpha_mask(self):
         SharedModelManager.manager.load("stable_diffusion_inpainting")
         assert (
             SharedModelManager.manager.diffusers.is_model_loaded(
-                "stable_diffusion_inpainting"
+                "stable_diffusion_inpainting",
             )
             is True
         )
         data = {
             "sampler_name": "k_dpmpp_2m",
             "cfg_scale": 7.5,
             "denoising_strength": 0.6,
```

### Comparing `hordelib-0.5.12/tests/test_horde_pp.py` & `hordelib-0.5.18/tests/test_horde_pp.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,29 +85,30 @@
         pil_image.save("images/horde_image_upscale_NMKD_Siax.webp", quality=90)
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_RealESRGAN_x4plus_anime_6B(self):
         SharedModelManager.manager.load("RealESRGAN_x4plus_anime_6B")
         assert (
             SharedModelManager.manager.esrgan.is_model_loaded(
-                "RealESRGAN_x4plus_anime_6B"
+                "RealESRGAN_x4plus_anime_6B",
             )
             is True
         )
         data = {
             "model": "RealESRGAN_x4plus_anime_6B",
             "source_image": self.image,
         }
         pil_image = self.horde.image_upscale(data)
         assert pil_image is not None
         width, height = pil_image.size
         assert width == self.width * 4
         assert height == self.height * 4
         pil_image.save(
-            "images/horde_image_upscale_RealESRGAN_x4plus_anime_6B.webp", quality=90
+            "images/horde_image_upscale_RealESRGAN_x4plus_anime_6B.webp",
+            quality=90,
         )
 
     @pytest.mark.mm_model("esrgan")
     def test_image_upscale_4x_AnimeSharp(self):
         SharedModelManager.manager.load("4x_AnimeSharp")
         assert (
             SharedModelManager.manager.esrgan.is_model_loaded("4x_AnimeSharp") is True
```

### Comparing `hordelib-0.5.12/tests/test_inference.py` & `hordelib-0.5.18/tests/test_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,9 +135,10 @@
             "clip_skip.stop_at_clip_layer": -1,
         }
         images = self.comfy.run_image_pipeline("stable_diffusion_hires_fix", params)
         assert images is not None
 
         image = Image.open(images[0]["imagedata"])
         image.save(
-            "images/pipeline_stable_diffusion_hires_fix_clip_skip_2.webp", quality=90
+            "images/pipeline_stable_diffusion_hires_fix_clip_skip_2.webp",
+            quality=90,
         )
```

### Comparing `hordelib-0.5.12/tests/test_safety_checker.py` & `hordelib-0.5.18/tests/test_safety_checker.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tests/test_shared_model_manager.py` & `hordelib-0.5.18/tests/test_shared_model_manager.py`

 * *Files identical despite different names*

### Comparing `hordelib-0.5.12/tox.ini` & `hordelib-0.5.18/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tox]
 env_list =
     format
+    lint-weak-check
     tests
 
 [coverage:run]
 omit =
     ComfyUI/*
     */nodes/*
     */config.py
@@ -16,15 +17,14 @@
 
 [coverage:report]
 omit =
     ComfyUI/*
     */nodes/*
     */config.py
     */config-3.py
-lcov_report = term coverage.lcov
 ignore_errors = True
 skip_empty = True
 
 [testenv]
 description = base evironment with all dependancies
 passenv =
     HORDELIB_TESTING
@@ -46,21 +46,33 @@
 [testenv:lint]
 description = check linting rules
 deps =
     ruff==0.0.261
 skip_install = true
 commands = ruff .
 
-[testenv:sortimports]
-description = check linting rules
+[testenv:lint-weak-check]
+description = check only certain few linting rules
 deps =
     ruff==0.0.261
 skip_install = true
-commands = ruff --fix --exclude comfy_horde.py --select I001 .
+commands = ruff --select COM,I .
 
+[testenv:lint-weak-fix]
+description = fixes only certain few linting rules
+deps =
+    black==22.3.0
+    ruff==0.0.261
+skip_install = true
+commands = 
+    black .
+    ruff --fix --select COM,I .
+    black .
+    ruff --fix --select COM,I .
+    
 [testenv:comfyui]
 description = run comfyui
 skip_install = true
 commands =
     {envpython} -m hordelib.run_comfyui
 
 [testenv:tests]
```

