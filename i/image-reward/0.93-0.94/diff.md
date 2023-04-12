# Comparing `tmp/image-reward-0.93.tar.gz` & `tmp/image-reward-0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-reward-0.93.tar", last modified: Sun Apr  9 02:43:26 2023, max compression
+gzip compressed data, was "image-reward-0.94.tar", last modified: Wed Apr 12 13:38:56 2023, max compression
```

## Comparing `image-reward-0.93.tar` & `image-reward-0.94.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-09 02:43:26.507453 image-reward-0.93/
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-09 02:43:26.503453 image-reward-0.93/ImageReward/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5231 2023-04-08 13:28:23.000000 image-reward-0.93/ImageReward/ImageReward.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       20 2023-04-08 13:29:13.000000 image-reward-0.93/ImageReward/__init__.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     6322 2023-04-08 14:46:39.000000 image-reward-0.93/ImageReward/utils.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-09 02:43:26.503453 image-reward-0.93/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3010 2023-04-09 02:36:32.000000 image-reward-0.93/README.md
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-09 02:43:26.503453 image-reward-0.93/image_reward.egg-info/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      269 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/SOURCES.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/dependency_links.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       52 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/requires.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-09 02:43:26.000000 image-reward-0.93/image_reward.egg-info/top_level.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-09 02:43:26.507453 image-reward-0.93/setup.cfg
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      972 2023-04-09 02:43:06.000000 image-reward-0.93/setup.py
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-12 13:38:56.484947 image-reward-0.94/
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-12 13:38:56.484947 image-reward-0.94/ImageReward/
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5231 2023-04-08 13:28:23.000000 image-reward-0.94/ImageReward/ImageReward.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       20 2023-04-08 13:29:13.000000 image-reward-0.94/ImageReward/__init__.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5868 2023-04-12 12:22:50.000000 image-reward-0.94/ImageReward/utils.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-12 13:38:56.484947 image-reward-0.94/PKG-INFO
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3492 2023-04-12 13:21:16.000000 image-reward-0.94/README.md
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-12 13:38:56.484947 image-reward-0.94/image_reward.egg-info/
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/PKG-INFO
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      269 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       52 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/requires.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/top_level.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-12 13:38:56.488947 image-reward-0.94/setup.cfg
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      972 2023-04-12 13:31:46.000000 image-reward-0.94/setup.py
```

### Comparing `image-reward-0.93/ImageReward/ImageReward.py` & `image-reward-0.94/ImageReward/ImageReward.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.93/ImageReward/utils.py` & `image-reward-0.94/ImageReward/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,39 +94,32 @@
     return list(_SCORES.keys())
 
 
 def _download(url: str, root: str):
     os.makedirs(root, exist_ok=True)
     filename = os.path.basename(url)
 
-    expected_sha256 = url.split("/")[-2]
     download_target = os.path.join(root, filename)
 
     if os.path.exists(download_target) and not os.path.isfile(download_target):
         raise RuntimeError(f"{download_target} exists and is not a regular file")
 
     if os.path.isfile(download_target):
-        if hashlib.sha256(open(download_target, "rb").read()).hexdigest() == expected_sha256:
-            return download_target
-        else:
-            warnings.warn(f"{download_target} exists, but the SHA256 checksum does not match; re-downloading the file")
+        return download_target
 
     with urllib.request.urlopen(url) as source, open(download_target, "wb") as output:
         with tqdm(total=int(source.info().get("Content-Length")), ncols=80, unit='iB', unit_scale=True, unit_divisor=1024) as loop:
             while True:
                 buffer = source.read(8192)
                 if not buffer:
                     break
 
                 output.write(buffer)
                 loop.update(len(buffer))
 
-    if hashlib.sha256(open(download_target, "rb").read()).hexdigest() != expected_sha256:
-        raise RuntimeError("Model has been downloaded but the SHA256 checksum does not not match")
-
     return download_target
 
 
 def load_score(name: str = "CLIP", device: Union[str, torch.device] = "cuda" if torch.cuda.is_available() else "cpu", download_root: str = None):
     """Load a ImageReward model
 
     Parameters
@@ -153,15 +146,15 @@
         raise RuntimeError(f"Score {name} not found; available scores = {available_scores()}")
 
     print('load checkpoint from %s'%model_path)
     if name == "BLIP":
         state_dict = torch.load(model_path, map_location='cpu')
         med_config = ImageReward_download("https://huggingface.co/THUDM/ImageReward/blob/main/med_config.json", model_download_root)
         model = BLIPScore(med_config=med_config, device=device).to(device)
-        model.blip.load_state_dict(state_dict,strict=False)
+        model.blip.load_state_dict(state_dict['model'],strict=False)
     elif name == "CLIP":
         model = CLIPScore(download_root=model_download_root, device=device).to(device)
     elif name == "Aesthetic":
         state_dict = torch.load(model_path, map_location='cpu')
         model = AestheticScore(download_root=model_download_root, device=device).to(device)
         model.mlp.load_state_dict(state_dict,strict=False)
     else:
```

### Comparing `image-reward-0.93/PKG-INFO` & `image-reward-0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.93
+Version: 0.94
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.93/README.md` & `image-reward-0.94/image_reward.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+Metadata-Version: 2.1
+Name: image-reward
+Version: 0.94
+Summary: ImageReward
+Author: xujz18
+Author-email: <xjz22@mails.tsinghua.edu.cn>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 # ImageReward-Pypi
 
 ImageReward is the first general-purpose text-to-image human preference RM which is trained on in total 137k pairs of expert comparisons, based on text prompts and corresponding model outputs from DiffusionDB. We demonstrate that ImageReward outperforms existing text-image scoring methods, such as CLIP, Aesthetic, and BLIP, in terms of understanding human preference in text-to-image synthesis through extensive analysis and experiments.
 
-## Approach
-
-![ImageReward](ImageReward.png)
-
-## Setup
-
-* Environment: install dependencies via `pip install -r requirements.txt`. 
-
 ## Usage
 
 ```python
 import os
 import torch
 import ImageReward as reward
 
@@ -43,57 +46,7 @@
 ranking = [1, 2, 3, 4]
 rewards = [[0.5811622738838196], [0.2745276093482971], [-1.4131819009780884], [-2.029569625854492]]
           1.webp: 0.58
           2.webp: 0.27
           3.webp: -1.41
           4.webp: -2.03
 ```
-
-## Test (One Step)
-
-```bash
-$ bash ./scripts/test.sh
-```
-
-## Test
-
-### Setup for baselines
-
-#### Environment
-
-```bash
-$ pip install git+https://github.com/openai/CLIP.git
-```
-
-#### Checkpoint
-
-* Download checkpoints to checkpoint/
-
-Models | Download Links
---- | :---: 
-ImageReward | <a href="https://huggingface.co/THUDM/ImageReward/blob/main/ImageReward.pt">Download</a>
-CLIP Score | <a href="https://openaipublic.azureedge.net/clip/models/b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836/ViT-L-14.pt">Download</a>
-BLIP Score | <a href="https://storage.googleapis.com/sfr-vision-language-research/BLIP/models/model_large.pth">Download</a>
-Aesthetic | <a href="https://github.com/christophschuhmann/improved-aesthetic-predictor/raw/main/sac%2Blogos%2Bava1-l14-linearMSE.pth">Download</a>
-
-#### Data
-
-Data | File Paths | Download Links
---- | :---: | :---: 
-test_images | data/ | <a href="https://huggingface.co/THUDM/ImageReward/blob/main/test_images.zip">Download</a>
-
-Download `test_images.zip` and unzip it to `data/test_images/`
-
-### One step for test
-
-```bash
-$ python test.py
-```
-
-The test result is:
-
-Models | Preference Acc.
---- | :---:
-CLIP Score | 54.82
-Aesthetic Score | 57.35
-BLIP Score | 57.76
-ImageReward (Ours) | **65.14**
```

### Comparing `image-reward-0.93/setup.py` & `image-reward-0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (Path(__file__).parent / "README-pypi.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="0.93",
+        version="0.94",
         author="xujz18",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
```

