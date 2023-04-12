# Comparing `tmp/haruna-0.1.8-py3-none-any.whl.zip` & `tmp/haruna-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 30367 bytes, number of entries: 35
+Zip file size: 30360 bytes, number of entries: 35
 -rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 haruna/__init__.py
 -rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 haruna/agents/__init__.py
 -rw-r--r--  2.0 unx     1764 b- defN 80-Jan-01 00:00 haruna/agents/agent.py
 -rw-r--r--  2.0 unx     5529 b- defN 80-Jan-01 00:00 haruna/agents/categorical_dqn.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 haruna/agents/double_dqn.py
 -rw-r--r--  2.0 unx     2144 b- defN 80-Jan-01 00:00 haruna/agents/dueling_dqn.py
 -rw-r--r--  2.0 unx     3246 b- defN 80-Jan-01 00:00 haruna/agents/noisy_dqn.py
--rw-r--r--  2.0 unx     8645 b- defN 80-Jan-01 00:00 haruna/agents/td3.py
+-rw-r--r--  2.0 unx     8628 b- defN 80-Jan-01 00:00 haruna/agents/td3.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 haruna/common/__init__.py
 -rw-r--r--  2.0 unx      620 b- defN 80-Jan-01 00:00 haruna/common/evaluation.py
 -rw-r--r--  2.0 unx     6553 b- defN 80-Jan-01 00:00 haruna/common/replay_buffer.py
 -rw-r--r--  2.0 unx     3353 b- defN 80-Jan-01 00:00 haruna/common/schedules.py
 -rw-r--r--  2.0 unx     4834 b- defN 80-Jan-01 00:00 haruna/common/segment_tree.py
 -rw-r--r--  2.0 unx     2519 b- defN 80-Jan-01 00:00 haruna/common/utils.py
 -rw-r--r--  2.0 unx       32 b- defN 80-Jan-01 00:00 haruna/envs/__init__.py
@@ -26,12 +26,12 @@
 -rw-r--r--  2.0 unx     1986 b- defN 80-Jan-01 00:00 haruna/optim/rmsprop.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 haruna/transforms/__init__.py
 -rw-r--r--  2.0 unx     2178 b- defN 80-Jan-01 00:00 haruna/transforms/segmentation.py
 -rw-r--r--  2.0 unx      281 b- defN 80-Jan-01 00:00 haruna/utils/__init__.py
 -rw-r--r--  2.0 unx      155 b- defN 80-Jan-01 00:00 haruna/utils/test_timeit.py
 -rw-r--r--  2.0 unx      596 b- defN 80-Jan-01 00:00 haruna/utils/timeit.py
 -rw-r--r--  2.0 unx     1318 b- defN 80-Jan-01 00:00 haruna/utils/utils.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 haruna-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1038 b- defN 80-Jan-01 00:00 haruna-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 haruna-0.1.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2794 b- defN 16-Jan-01 00:00 haruna-0.1.8.dist-info/RECORD
-35 files, 80599 bytes uncompressed, 25931 bytes compressed:  67.8%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 haruna-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1038 b- defN 80-Jan-01 00:00 haruna-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 haruna-0.1.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2794 b- defN 16-Jan-01 00:00 haruna-0.1.9.dist-info/RECORD
+35 files, 80582 bytes uncompressed, 25924 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -87,20 +87,20 @@
 
 Filename: haruna/utils/timeit.py
 Comment: 
 
 Filename: haruna/utils/utils.py
 Comment: 
 
-Filename: haruna-0.1.8.dist-info/LICENSE
+Filename: haruna-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: haruna-0.1.8.dist-info/METADATA
+Filename: haruna-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: haruna-0.1.8.dist-info/WHEEL
+Filename: haruna-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: haruna-0.1.8.dist-info/RECORD
+Filename: haruna-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## haruna/agents/td3.py

```diff
@@ -109,15 +109,15 @@
             raise ValueError("The environment must be set before calling setup_aliases()")
 
         self.setup_aliases()
 
         self.setup_models()
 
         self.replay_buffer = ReplayBuffer(size=self.buffer_size)
-        self.noise = GaussianExploration(self.action_space)
+        self.noise = GaussianExploration()
 
     def setup_aliases(self):
         self.observation_space = self.env.observation_space
         self.action_space = self.env.action_space
         self.obs_dim = self.env.observation_space.shape[0]
         self.action_dim = self.env.action_space.shape[0]
```

## Comparing `haruna-0.1.8.dist-info/LICENSE` & `haruna-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `haruna-0.1.8.dist-info/METADATA` & `haruna-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruna
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: なるみ
 Author-email: 4680567+narumiruna@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `haruna-0.1.8.dist-info/RECORD` & `haruna-0.1.9.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 haruna/__init__.py,sha256=wbJZXPnCf43jgs0T0dG31E02lxqGmruEff7Q7_VQkp8,65
 haruna/agents/__init__.py,sha256=wT80xdmzfd5wIrwTTGH94baapuJdZ9qaqkaUpEsOCDo,192
 haruna/agents/agent.py,sha256=Ps_d5uBNscGRJ0FovGxl5yPLM6r82CCO-EEsjKv6Zfg,1764
 haruna/agents/categorical_dqn.py,sha256=TgLiiLWEbMhZNHboArU-v1rX7siTpNWLUeltq5iVFl4,5529
 haruna/agents/double_dqn.py,sha256=uNC1PqlDZWM-NZmRxqOROEpywzJRDEwkz6Vww76n6cE,7466
 haruna/agents/dueling_dqn.py,sha256=O3uDqnRFgqQIV5MOi6gYW747cCqdqLuhCLg02u-kDyI,2144
 haruna/agents/noisy_dqn.py,sha256=nvgwGaHheC4mNPFJ1_yqCgCqyYdf3OrsVnkaYe-iCFg,3246
-haruna/agents/td3.py,sha256=M2xu2KhWABqV7kpr_01_4iBPuP94vOC72Eao1Ox7MpY,8645
+haruna/agents/td3.py,sha256=h7F0CShpx4zdvnyDSYVXrQDIS9ZVBqZ_Avz0rwIV4EM,8628
 haruna/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 haruna/common/evaluation.py,sha256=aDNXz18IDyX7ous5-KGeu5RNVHCzN43Zw7yVciAa3sk,620
 haruna/common/replay_buffer.py,sha256=7aKpiXkBGGGPv0Jy-BvGpkZoDMZjL1eF9iG2l4mBqiQ,6553
 haruna/common/schedules.py,sha256=pA7xAtLuB0r70M2x6dHC4a_KdUCLRm_Y4Ybb2M_SE38,3353
 haruna/common/segment_tree.py,sha256=9WIP38-wOA-WSKsIayJlyXv-AmleF8rjF-ez49S4438,4834
 haruna/common/utils.py,sha256=BeKz01RRekFcAQdmxhVyF9YvPn3JkBasIINDEjsSnGY,2519
 haruna/envs/__init__.py,sha256=sHMYGAVeO_bGgTCLNYRsAXPiPtblLbE0GhdHGjQs9UM,32
@@ -25,11 +25,11 @@
 haruna/optim/rmsprop.py,sha256=10Q_34ibycJm3u-V67IxA2DpofT9jErqqUBGMHtjors,1986
 haruna/transforms/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 haruna/transforms/segmentation.py,sha256=DX4QTDRkRUaa5ZsRdr-NoQ50gpR1l_qJTRJaWNNY_5w,2178
 haruna/utils/__init__.py,sha256=027akLwMXmlqP3_gqzRnEHlS-Euuf_OCgQRU0oFl0UE,281
 haruna/utils/test_timeit.py,sha256=ZqM_wmOlz6JLh0mmVt543jPNrWte47yxj45sfDpcxd8,155
 haruna/utils/timeit.py,sha256=IR-I2Dom4L5H630HulSi9vzx3EMX7w9QnRfFGbYbKPU,596
 haruna/utils/utils.py,sha256=yZel8aE6JcZ1nE7zEgCDm256x_RFeG_8-yyk_uo3X2k,1318
-haruna-0.1.8.dist-info/LICENSE,sha256=vK26DADDD3vPEl4y8fDmCE1Ub_iX3vSP4APVkSiROZs,1066
-haruna-0.1.8.dist-info/METADATA,sha256=DHaCeTdNrlyTTOVWHCvlpjn-tw7kN_m63yyFtQDTBgQ,1038
-haruna-0.1.8.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-haruna-0.1.8.dist-info/RECORD,,
+haruna-0.1.9.dist-info/LICENSE,sha256=vK26DADDD3vPEl4y8fDmCE1Ub_iX3vSP4APVkSiROZs,1066
+haruna-0.1.9.dist-info/METADATA,sha256=OmXiP8v6Cbhxzz-S5Cj6z-ajgYZ5XFECJIZLD7ptBOs,1038
+haruna-0.1.9.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+haruna-0.1.9.dist-info/RECORD,,
```

