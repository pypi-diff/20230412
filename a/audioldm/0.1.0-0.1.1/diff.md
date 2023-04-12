# Comparing `tmp/audioldm-0.1.0.tar.gz` & `tmp/audioldm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm-0.1.0.tar", last modified: Mon Apr 10 13:47:09 2023, max compression
+gzip compressed data, was "audioldm-0.1.1.tar", last modified: Wed Apr 12 12:39:45 2023, max compression
```

## Comparing `audioldm-0.1.0.tar` & `audioldm-0.1.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.317385 audioldm-0.1.0/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    15035 2023-04-10 06:44:17.000000 audioldm-0.1.0/LICENSE
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)       86 2023-04-10 06:44:17.000000 audioldm-0.1.0/MANIFEST.in
--rw-r--r--   0 tiger     (1000) tiger     (1000)    10920 2023-04-10 13:47:09.314005 audioldm-0.1.0/PKG-INFO
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    10271 2023-04-10 08:05:27.000000 audioldm-0.1.0/README.md
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    13173 2023-04-10 07:11:35.000000 audioldm-0.1.0/app.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.636739 audioldm-0.1.0/audioldm/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      132 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4751 2023-04-10 07:14:59.000000 audioldm-0.1.0/audioldm/__main__.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.707851 audioldm-0.1.0/audioldm/audio/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)       78 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2642 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/audio_processing.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6374 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/stft.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2759 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/audio/tools.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.718051 audioldm-0.1.0/audioldm/clap/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6318 2023-04-10 07:02:06.000000 audioldm-0.1.0/audioldm/clap/encoders.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.925058 audioldm-0.1.0/audioldm/clap/open_clip/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      639 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     1220 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/bert.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)  1356917 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    11070 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/factory.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     7177 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/feature_fusion.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    48104 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/htsat.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2243 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/linear_probe.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    16143 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/loss.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    33147 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.100740 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-base.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      498 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-large.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/HTSAT-tiny.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-10.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-fmax-18k.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      496 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14-win-1536.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      497 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-14.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      495 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/PANN-6.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      388 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN101-quickgelu.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      364 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN101.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      389 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50-quickgelu.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      364 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      365 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50x16.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      365 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/RN50x4.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      294 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-B-16.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      318 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      294 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-B-32.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      296 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/model_configs/ViT-L-14.json
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     5085 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/openai.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    23398 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/pann_model.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6501 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/pretrained.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4337 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/timm_model.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     6400 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/tokenizer.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     1051 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/transform.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    12103 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/utils.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)       22 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/open_clip/version.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.206260 audioldm-0.1.0/audioldm/clap/training/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    84448 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/audioset_textmap.npy
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    34417 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/data.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     5165 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/distributed.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    22199 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/imagenet_zeroshot_data.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3208 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/infer_demo.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      943 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/logger.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    25459 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/lp_main.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    10607 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/lp_train.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    22551 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/main.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    17283 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/params.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      661 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/scheduler.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    36331 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/train.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3429 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/clap/training/zero_shot.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.229407 audioldm-0.1.0/audioldm/hifigan/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)      180 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/hifigan/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     5524 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/hifigan/models.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     2110 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/hifigan/utilities.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.272894 audioldm-0.1.0/audioldm/latent_diffusion/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    15343 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/attention.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    13593 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/ddim.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    16399 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/ddpm.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3066 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/ema.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    39155 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/openaimodel.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     9863 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/latent_diffusion/util.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    28164 2023-04-10 06:45:17.000000 audioldm-0.1.0/audioldm/ldm.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    10650 2023-04-10 06:58:19.000000 audioldm-0.1.0/audioldm/pipeline.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     9803 2023-04-10 13:43:23.000000 audioldm-0.1.0/audioldm/utils.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.297363 audioldm-0.1.0/audioldm/variational_autoencoder/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)        0 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/__init__.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3132 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/autoencoder.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     3097 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/distributions.py
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)    34390 2023-04-10 06:44:17.000000 audioldm-0.1.0/audioldm/variational_autoencoder/modules.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:08.663418 audioldm-0.1.0/audioldm.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)    10920 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3310 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)      189 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        9 2023-04-10 13:47:08.000000 audioldm-0.1.0/audioldm.egg-info/top_level.txt
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-04-10 13:47:09.310793 audioldm-0.1.0/bin/
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4751 2023-04-10 07:23:00.000000 audioldm-0.1.0/bin/audioldm
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)       31 2023-04-10 06:44:17.000000 audioldm-0.1.0/bin/audioldm.cmd
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-04-10 13:47:09.317005 audioldm-0.1.0/setup.cfg
--rwxrwxrwx   0 tiger     (1000) tiger     (1000)     4510 2023-04-10 08:01:38.000000 audioldm-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.395088 audioldm-0.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)    15035 2023-04-10 06:44:17.000000 audioldm-0.1.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       86 2023-04-10 06:44:17.000000 audioldm-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11323 2023-04-12 12:39:45.392334 audioldm-0.1.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    10674 2023-04-12 12:39:04.000000 audioldm-0.1.1/README.md
+-rwxr-xr-x   0 root         (0) root         (0)    13170 2023-04-12 12:13:35.000000 audioldm-0.1.1/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:44.953972 audioldm-0.1.1/audioldm/
+-rwxrwxrwx   0 root         (0) root         (0)      132 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4748 2023-04-12 12:15:29.000000 audioldm-0.1.1/audioldm/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:44.995543 audioldm-0.1.1/audioldm/audio/
+-rwxrwxrwx   0 root         (0) root         (0)       78 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/audio/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2642 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/audio/audio_processing.py
+-rwxrwxrwx   0 root         (0) root         (0)     6374 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/audio/stft.py
+-rwxrwxrwx   0 root         (0) root         (0)     2759 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/audio/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.003756 audioldm-0.1.1/audioldm/clap/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6318 2023-04-10 07:02:06.000000 audioldm-0.1.1/audioldm/clap/encoders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.086222 audioldm-0.1.1/audioldm/clap/open_clip/
+-rwxrwxrwx   0 root         (0) root         (0)      639 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/bert.py
+-rwxrwxrwx   0 root         (0) root         (0)  1356917 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rwxrwxrwx   0 root         (0) root         (0)    11070 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/factory.py
+-rwxrwxrwx   0 root         (0) root         (0)     7177 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/feature_fusion.py
+-rwxrwxrwx   0 root         (0) root         (0)    48104 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/htsat.py
+-rwxrwxrwx   0 root         (0) root         (0)     2243 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/linear_probe.py
+-rwxrwxrwx   0 root         (0) root         (0)    16143 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/loss.py
+-rwxrwxrwx   0 root         (0) root         (0)    33147 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.182628 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/
+-rwxrwxrwx   0 root         (0) root         (0)      497 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/HTSAT-base.json
+-rwxrwxrwx   0 root         (0) root         (0)      498 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/HTSAT-large.json
+-rwxrwxrwx   0 root         (0) root         (0)      496 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/HTSAT-tiny-win-1536.json
+-rwxrwxrwx   0 root         (0) root         (0)      496 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/HTSAT-tiny.json
+-rwxrwxrwx   0 root         (0) root         (0)      497 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/PANN-10.json
+-rwxrwxrwx   0 root         (0) root         (0)      497 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/PANN-14-fmax-18k.json
+-rwxrwxrwx   0 root         (0) root         (0)      496 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/PANN-14-fmax-8k-20s.json
+-rwxrwxrwx   0 root         (0) root         (0)      496 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/PANN-14-tiny-transformer.json
+-rwxrwxrwx   0 root         (0) root         (0)      497 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/PANN-14-win-1536.json
+-rwxrwxrwx   0 root         (0) root         (0)      497 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/PANN-14.json
+-rwxrwxrwx   0 root         (0) root         (0)      495 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/PANN-6.json
+-rwxrwxrwx   0 root         (0) root         (0)      388 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/RN101-quickgelu.json
+-rwxrwxrwx   0 root         (0) root         (0)      364 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/RN101.json
+-rwxrwxrwx   0 root         (0) root         (0)      389 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/RN50-quickgelu.json
+-rwxrwxrwx   0 root         (0) root         (0)      364 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/RN50.json
+-rwxrwxrwx   0 root         (0) root         (0)      365 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/RN50x16.json
+-rwxrwxrwx   0 root         (0) root         (0)      365 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/RN50x4.json
+-rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/ViT-B-16.json
+-rwxrwxrwx   0 root         (0) root         (0)      318 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rwxrwxrwx   0 root         (0) root         (0)      294 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/ViT-B-32.json
+-rwxrwxrwx   0 root         (0) root         (0)      296 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/model_configs/ViT-L-14.json
+-rwxrwxrwx   0 root         (0) root         (0)     5085 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/openai.py
+-rwxrwxrwx   0 root         (0) root         (0)    23398 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/pann_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     6501 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/pretrained.py
+-rwxrwxrwx   0 root         (0) root         (0)     4337 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/timm_model.py
+-rwxrwxrwx   0 root         (0) root         (0)     6400 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/tokenizer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1051 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/transform.py
+-rwxrwxrwx   0 root         (0) root         (0)    12103 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/open_clip/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.250290 audioldm-0.1.1/audioldm/clap/training/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    84448 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/audioset_textmap.npy
+-rwxrwxrwx   0 root         (0) root         (0)    34417 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/data.py
+-rwxrwxrwx   0 root         (0) root         (0)     5165 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/distributed.py
+-rwxrwxrwx   0 root         (0) root         (0)    22199 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/imagenet_zeroshot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     3208 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/infer_demo.py
+-rwxrwxrwx   0 root         (0) root         (0)      943 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/logger.py
+-rwxrwxrwx   0 root         (0) root         (0)    25459 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/lp_main.py
+-rwxrwxrwx   0 root         (0) root         (0)    10607 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/lp_train.py
+-rwxrwxrwx   0 root         (0) root         (0)    22551 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/main.py
+-rwxrwxrwx   0 root         (0) root         (0)    17283 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/params.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/scheduler.py
+-rwxrwxrwx   0 root         (0) root         (0)    36331 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/train.py
+-rwxrwxrwx   0 root         (0) root         (0)     3429 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/clap/training/zero_shot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.292071 audioldm-0.1.1/audioldm/hifigan/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/hifigan/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5524 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/hifigan/models.py
+-rwxrwxrwx   0 root         (0) root         (0)     2110 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/hifigan/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.358950 audioldm-0.1.1/audioldm/latent_diffusion/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/latent_diffusion/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15343 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/latent_diffusion/attention.py
+-rwxrwxrwx   0 root         (0) root         (0)    13593 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/latent_diffusion/ddim.py
+-rwxrwxrwx   0 root         (0) root         (0)    16399 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/latent_diffusion/ddpm.py
+-rwxrwxrwx   0 root         (0) root         (0)     3066 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/latent_diffusion/ema.py
+-rwxrwxrwx   0 root         (0) root         (0)    39155 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/latent_diffusion/openaimodel.py
+-rwxrwxrwx   0 root         (0) root         (0)     9863 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/latent_diffusion/util.py
+-rwxrwxrwx   0 root         (0) root         (0)    28164 2023-04-10 06:45:17.000000 audioldm-0.1.1/audioldm/ldm.py
+-rwxrwxrwx   0 root         (0) root         (0)    10650 2023-04-12 12:13:19.000000 audioldm-0.1.1/audioldm/pipeline.py
+-rwxrwxrwx   0 root         (0) root         (0)     9803 2023-04-10 13:43:36.000000 audioldm-0.1.1/audioldm/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.376119 audioldm-0.1.1/audioldm/variational_autoencoder/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/variational_autoencoder/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3132 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/variational_autoencoder/autoencoder.py
+-rwxrwxrwx   0 root         (0) root         (0)     3097 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/variational_autoencoder/distributions.py
+-rwxrwxrwx   0 root         (0) root         (0)    34390 2023-04-10 06:44:17.000000 audioldm-0.1.1/audioldm/variational_autoencoder/modules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:44.976301 audioldm-0.1.1/audioldm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11323 2023-04-12 12:39:44.000000 audioldm-0.1.1/audioldm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3310 2023-04-12 12:39:44.000000 audioldm-0.1.1/audioldm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 12:39:44.000000 audioldm-0.1.1/audioldm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-04-12 12:39:44.000000 audioldm-0.1.1/audioldm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-12 12:39:44.000000 audioldm-0.1.1/audioldm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:39:45.387621 audioldm-0.1.1/bin/
+-rwxrwxrwx   0 root         (0) root         (0)     4748 2023-04-12 12:15:43.000000 audioldm-0.1.1/bin/audioldm
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-04-10 06:44:17.000000 audioldm-0.1.1/bin/audioldm.cmd
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 12:39:45.394334 audioldm-0.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     4510 2023-04-12 12:17:26.000000 audioldm-0.1.1/setup.py
```

### Comparing `audioldm-0.1.0/LICENSE` & `audioldm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/PKG-INFO` & `audioldm-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: audioldm
-Version: 0.1.0
-Summary: This package is written for text-to-audio generation.
-Home-page: https://github.com/haoheliu/audioldm
-Author: Haohe Liu
-Author-email: haoheliu@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 # :sound: Audio Generation with AudioLDM
 
 [![arXiv](https://img.shields.io/badge/arXiv-2301.12503-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2301.12503)  [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://audioldm.github.io/)  [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/haoheliu/audioldm-text-to-audio-generation)  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/olaviinha/NeuralTextToAudio/blob/main/AudioLDM_pub.ipynb?force_theme=dark)  [![Replicate](https://replicate.com/jagilley/audio-ldm/badge)](https://replicate.com/jagilley/audio-ldm)
 
 <!-- # [![PyPI version](https://badge.fury.io/py/voicefixer.svg)](https://badge.fury.io/py/voicefixer) -->
 
 **Generate speech, sound effects, music and beyond.**
@@ -101,20 +82,23 @@
 ```
 
 :gear: How to choose between different model checkpoints?
 ```
 # Add the --model_name parameter, choice={audioldm-m-text-ft, audioldm-s-text-ft, audioldm-m-full, audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}
 audioldm --model_name audioldm-s-full
 ```
-- :star: audioldm-m-text-ft (**recommand**, default): the medium large AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
-- :star: audioldm-s-text-ft (**recommand**): the small AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
-- audioldm-m-full: the medium AudioLDM without finetuning and trained with audio embeddings as condition *(added 2023-04-10)*.
-- audioldm-s-full-v2: more training steps comparing with audioldm-s-full *(added 2023-03-04)*.
+
+- :star: audioldm-m-full (default, **recommend**): the medium AudioLDM without finetuning and trained with audio embeddings as condition *(added 2023-04-10)*.
+- :star: audioldm-s-full (**recommend**): the original open-sourced version *(added 2023-02-01)*.
+- :star: audioldm-s-full-v2 (**recommend**): more training steps comparing with audioldm-s-full *(added 2023-03-04)*.
+- audioldm-s-text-ft: the small AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
+- audioldm-m-text-ft: the medium large AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
 - audioldm-l-full: larger model comparing with audioldm-s-full *(added 2023-03-04)*.
-- audioldm-s-full: the original open-sourced version *(added 2023-02-01)*.
+
+> @haoheliu personally did a evaluation regarding the overall quality of the checkpoint, which gives audioldm-m-full (6.85/10), audioldm-s-full (6.62/10), audioldm-s-text-ft (6/10), audioldm-m-text-ft (5.46/10). These score are only for reference and may not reflect the true performance of the checkpoint. Checkpoint performance also varying with different text input as well.
 
 :grey_question: For more options on guidance scale, batchsize, seed, ddim steps, etc., please run
 ```shell
 audioldm -h
 ```
 ```console
 usage: audioldm [-h] [--mode {generation,transfer}] [-t TEXT] [-f FILE_PATH] [--transfer_strength TRANSFER_STRENGTH] [-s SAVE_PATH] [--model_name {audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}] [-ckpt CKPT_PATH]
```

### Comparing `audioldm-0.1.0/README.md` & `audioldm-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: audioldm
+Version: 0.1.1
+Summary: This package is written for text-to-audio generation.
+Home-page: https://github.com/haoheliu/audioldm
+Author: Haohe Liu
+Author-email: haoheliu@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # :sound: Audio Generation with AudioLDM
 
 [![arXiv](https://img.shields.io/badge/arXiv-2301.12503-brightgreen.svg?style=flat-square)](https://arxiv.org/abs/2301.12503)  [![githubio](https://img.shields.io/badge/GitHub.io-Audio_Samples-blue?logo=Github&style=flat-square)](https://audioldm.github.io/)  [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/haoheliu/audioldm-text-to-audio-generation)  [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/olaviinha/NeuralTextToAudio/blob/main/AudioLDM_pub.ipynb?force_theme=dark)  [![Replicate](https://replicate.com/jagilley/audio-ldm/badge)](https://replicate.com/jagilley/audio-ldm)
 
 <!-- # [![PyPI version](https://badge.fury.io/py/voicefixer.svg)](https://badge.fury.io/py/voicefixer) -->
 
 **Generate speech, sound effects, music and beyond.**
@@ -82,20 +101,23 @@
 ```
 
 :gear: How to choose between different model checkpoints?
 ```
 # Add the --model_name parameter, choice={audioldm-m-text-ft, audioldm-s-text-ft, audioldm-m-full, audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}
 audioldm --model_name audioldm-s-full
 ```
-- :star: audioldm-m-text-ft (**recommand**, default): the medium large AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
-- :star: audioldm-s-text-ft (**recommand**): the small AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
-- audioldm-m-full: the medium AudioLDM without finetuning and trained with audio embeddings as condition *(added 2023-04-10)*.
-- audioldm-s-full-v2: more training steps comparing with audioldm-s-full *(added 2023-03-04)*.
+
+- :star: audioldm-m-full (default, **recommend**): the medium AudioLDM without finetuning and trained with audio embeddings as condition *(added 2023-04-10)*.
+- :star: audioldm-s-full (**recommend**): the original open-sourced version *(added 2023-02-01)*.
+- :star: audioldm-s-full-v2 (**recommend**): more training steps comparing with audioldm-s-full *(added 2023-03-04)*.
+- audioldm-s-text-ft: the small AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
+- audioldm-m-text-ft: the medium large AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
 - audioldm-l-full: larger model comparing with audioldm-s-full *(added 2023-03-04)*.
-- audioldm-s-full: the original open-sourced version *(added 2023-02-01)*.
+
+> @haoheliu personally did a evaluation regarding the overall quality of the checkpoint, which gives audioldm-m-full (6.85/10), audioldm-s-full (6.62/10), audioldm-s-text-ft (6/10), audioldm-m-text-ft (5.46/10). These score are only for reference and may not reflect the true performance of the checkpoint. Checkpoint performance also varying with different text input as well.
 
 :grey_question: For more options on guidance scale, batchsize, seed, ddim steps, etc., please run
 ```shell
 audioldm -h
 ```
 ```console
 usage: audioldm [-h] [--mode {generation,transfer}] [-t TEXT] [-f FILE_PATH] [--transfer_strength TRANSFER_STRENGTH] [-s SAVE_PATH] [--model_name {audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}] [-ckpt CKPT_PATH]
```

### Comparing `audioldm-0.1.0/app.py` & `audioldm-0.1.1/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
                     1,
                     5,
                     value=3,
                     step=1,
                     label="Automatic quality control. This number control the number of candidates (e.g., generate three audios and choose the best to show you). A Larger value usually lead to better quality with heavier computation",
                 )
                 model_name = gr.Dropdown(
-                    ["audioldm-s-full", "audioldm-l-full", "audioldm-s-full-v2","audioldm-m-text-ft", "audioldm-s-text-ft", "audioldm-m-full"], value="audioldm-m-text-ft", label="Choose the model to use. audioldm-m-text-ft and audioldm-s-text-ft are recommanded. -s- means small, -m- means medium and -l- means large",
+                    ["audioldm-s-full", "audioldm-l-full", "audioldm-s-full-v2","audioldm-m-text-ft", "audioldm-s-text-ft", "audioldm-m-full"], value="audioldm-m-full", label="Choose the model to use. audioldm-m-text-ft and audioldm-s-text-ft are recommanded. -s- means small, -m- means medium and -l- means large",
                 )
             ############# Output
             # outputs=gr.Audio(label="Output", type="numpy")
             outputs = gr.Video(label="Output", elem_id="output-video")
 
             # with gr.Group(elem_id="container-advanced-btns"):
             #   # advanced_button = gr.Button("Advanced options", elem_id="advanced-btn")
```

### Comparing `audioldm-0.1.0/audioldm/__main__.py` & `audioldm-0.1.1/audioldm/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 )
 
 parser.add_argument(
     "--model_name",
     type=str,
     required=False,
     help="The checkpoint you gonna use",
-    default="audioldm-m-text-ft",
+    default="audioldm-m-full",
     choices=["audioldm-s-full", "audioldm-l-full", "audioldm-s-full-v2","audioldm-m-text-ft", "audioldm-s-text-ft", "audioldm-m-full"]
 )
 
 parser.add_argument(
     "-ckpt",
     "--ckpt_path",
     type=str,
```

### Comparing `audioldm-0.1.0/audioldm/audio/audio_processing.py` & `audioldm-0.1.1/audioldm/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/audio/stft.py` & `audioldm-0.1.1/audioldm/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/audio/tools.py` & `audioldm-0.1.1/audioldm/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/encoders.py` & `audioldm-0.1.1/audioldm/clap/encoders.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/__init__.py` & `audioldm-0.1.1/audioldm/clap/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/bert.py` & `audioldm-0.1.1/audioldm/clap/open_clip/bert.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz` & `audioldm-0.1.1/audioldm/clap/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/factory.py` & `audioldm-0.1.1/audioldm/clap/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/feature_fusion.py` & `audioldm-0.1.1/audioldm/clap/open_clip/feature_fusion.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/htsat.py` & `audioldm-0.1.1/audioldm/clap/open_clip/htsat.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/linear_probe.py` & `audioldm-0.1.1/audioldm/clap/open_clip/linear_probe.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/loss.py` & `audioldm-0.1.1/audioldm/clap/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/model.py` & `audioldm-0.1.1/audioldm/clap/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/openai.py` & `audioldm-0.1.1/audioldm/clap/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/pann_model.py` & `audioldm-0.1.1/audioldm/clap/open_clip/pann_model.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/pretrained.py` & `audioldm-0.1.1/audioldm/clap/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/timm_model.py` & `audioldm-0.1.1/audioldm/clap/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/tokenizer.py` & `audioldm-0.1.1/audioldm/clap/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/transform.py` & `audioldm-0.1.1/audioldm/clap/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/open_clip/utils.py` & `audioldm-0.1.1/audioldm/clap/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/audioset_textmap.npy` & `audioldm-0.1.1/audioldm/clap/training/audioset_textmap.npy`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/data.py` & `audioldm-0.1.1/audioldm/clap/training/data.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/distributed.py` & `audioldm-0.1.1/audioldm/clap/training/distributed.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/imagenet_zeroshot_data.py` & `audioldm-0.1.1/audioldm/clap/training/imagenet_zeroshot_data.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/infer_demo.py` & `audioldm-0.1.1/audioldm/clap/training/infer_demo.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/logger.py` & `audioldm-0.1.1/audioldm/clap/training/logger.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/lp_main.py` & `audioldm-0.1.1/audioldm/clap/training/lp_main.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/lp_train.py` & `audioldm-0.1.1/audioldm/clap/training/lp_train.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/main.py` & `audioldm-0.1.1/audioldm/clap/training/main.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/params.py` & `audioldm-0.1.1/audioldm/clap/training/params.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/scheduler.py` & `audioldm-0.1.1/audioldm/clap/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/train.py` & `audioldm-0.1.1/audioldm/clap/training/train.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/clap/training/zero_shot.py` & `audioldm-0.1.1/audioldm/clap/training/zero_shot.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/hifigan/models.py` & `audioldm-0.1.1/audioldm/hifigan/models.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/hifigan/utilities.py` & `audioldm-0.1.1/audioldm/hifigan/utilities.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/latent_diffusion/attention.py` & `audioldm-0.1.1/audioldm/latent_diffusion/attention.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/latent_diffusion/ddim.py` & `audioldm-0.1.1/audioldm/latent_diffusion/ddim.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/latent_diffusion/ddpm.py` & `audioldm-0.1.1/audioldm/latent_diffusion/ddpm.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/latent_diffusion/ema.py` & `audioldm-0.1.1/audioldm/latent_diffusion/ema.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/latent_diffusion/openaimodel.py` & `audioldm-0.1.1/audioldm/latent_diffusion/openaimodel.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/latent_diffusion/util.py` & `audioldm-0.1.1/audioldm/latent_diffusion/util.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/ldm.py` & `audioldm-0.1.1/audioldm/ldm.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/pipeline.py` & `audioldm-0.1.1/audioldm/pipeline.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/utils.py` & `audioldm-0.1.1/audioldm/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/variational_autoencoder/autoencoder.py` & `audioldm-0.1.1/audioldm/variational_autoencoder/autoencoder.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/variational_autoencoder/distributions.py` & `audioldm-0.1.1/audioldm/variational_autoencoder/distributions.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm/variational_autoencoder/modules.py` & `audioldm-0.1.1/audioldm/variational_autoencoder/modules.py`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/audioldm.egg-info/PKG-INFO` & `audioldm-0.1.1/audioldm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioldm
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package is written for text-to-audio generation.
 Home-page: https://github.com/haoheliu/audioldm
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -101,20 +101,23 @@
 ```
 
 :gear: How to choose between different model checkpoints?
 ```
 # Add the --model_name parameter, choice={audioldm-m-text-ft, audioldm-s-text-ft, audioldm-m-full, audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}
 audioldm --model_name audioldm-s-full
 ```
-- :star: audioldm-m-text-ft (**recommand**, default): the medium large AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
-- :star: audioldm-s-text-ft (**recommand**): the small AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
-- audioldm-m-full: the medium AudioLDM without finetuning and trained with audio embeddings as condition *(added 2023-04-10)*.
-- audioldm-s-full-v2: more training steps comparing with audioldm-s-full *(added 2023-03-04)*.
+
+- :star: audioldm-m-full (default, **recommend**): the medium AudioLDM without finetuning and trained with audio embeddings as condition *(added 2023-04-10)*.
+- :star: audioldm-s-full (**recommend**): the original open-sourced version *(added 2023-02-01)*.
+- :star: audioldm-s-full-v2 (**recommend**): more training steps comparing with audioldm-s-full *(added 2023-03-04)*.
+- audioldm-s-text-ft: the small AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
+- audioldm-m-text-ft: the medium large AudioLDM finetuned with AudioCaps and MusicCaps audio-text pairs *(added 2023-04-10)*.
 - audioldm-l-full: larger model comparing with audioldm-s-full *(added 2023-03-04)*.
-- audioldm-s-full: the original open-sourced version *(added 2023-02-01)*.
+
+> @haoheliu personally did a evaluation regarding the overall quality of the checkpoint, which gives audioldm-m-full (6.85/10), audioldm-s-full (6.62/10), audioldm-s-text-ft (6/10), audioldm-m-text-ft (5.46/10). These score are only for reference and may not reflect the true performance of the checkpoint. Checkpoint performance also varying with different text input as well.
 
 :grey_question: For more options on guidance scale, batchsize, seed, ddim steps, etc., please run
 ```shell
 audioldm -h
 ```
 ```console
 usage: audioldm [-h] [--mode {generation,transfer}] [-t TEXT] [-f FILE_PATH] [--transfer_strength TRANSFER_STRENGTH] [-s SAVE_PATH] [--model_name {audioldm-s-full,audioldm-l-full,audioldm-s-full-v2}] [-ckpt CKPT_PATH]
```

### Comparing `audioldm-0.1.0/audioldm.egg-info/SOURCES.txt` & `audioldm-0.1.1/audioldm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioldm-0.1.0/bin/audioldm` & `audioldm-0.1.1/bin/audioldm`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 )
 
 parser.add_argument(
     "--model_name",
     type=str,
     required=False,
     help="The checkpoint you gonna use",
-    default="audioldm-m-text-ft",
+    default="audioldm-m-full",
     choices=["audioldm-s-full", "audioldm-l-full", "audioldm-s-full-v2","audioldm-m-text-ft", "audioldm-s-text-ft", "audioldm-m-full"]
 )
 
 parser.add_argument(
     "-ckpt",
     "--ckpt_path",
     type=str,
```

### Comparing `audioldm-0.1.0/setup.py` & `audioldm-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audioldm"
 DESCRIPTION = "This package is written for text-to-audio generation."
 URL = "https://github.com/haoheliu/audioldm"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.13.0",
     "torchaudio>=0.13.0",
     "torchvision>=0.14.0",
     "tqdm",
```

