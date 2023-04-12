# Comparing `tmp/onediff-0.7.0-py3-none-any.whl.zip` & `tmp/onediff-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 57195 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1034 b- defN 23-Mar-27 07:40 onediff/__init__.py
--rw-r--r--  2.0 unx     3350 b- defN 23-Feb-17 07:48 onediff/graph_utils.py
+Zip file size: 56116 bytes, number of entries: 14
+-rw-r--r--  2.0 unx     1034 b- defN 23-Apr-12 01:35 onediff/__init__.py
+-rw-r--r--  2.0 unx     5519 b- defN 23-Apr-12 01:35 onediff/graph_utils.py
 -rw-r--r--  2.0 unx     7755 b- defN 23-Feb-17 07:48 onediff/oneflow_graph_compile_cache.py
--rw-r--r--  2.0 unx    35375 b- defN 23-Mar-06 09:51 onediff/pipeline_alt_diffusion_oneflow.py
+-rw-r--r--  2.0 unx    33943 b- defN 23-Apr-12 01:35 onediff/pipeline_alt_diffusion_oneflow.py
 -rw-r--r--  2.0 unx    39449 b- defN 23-Mar-27 07:40 onediff/pipeline_stable_diffusion_controlnet_oneflow.py
--rw-r--r--  2.0 unx    37667 b- defN 23-Mar-27 07:40 onediff/pipeline_stable_diffusion_img2img_oneflow.py
--rw-r--r--  2.0 unx    43618 b- defN 23-Mar-06 09:51 onediff/pipeline_stable_diffusion_inpaint_oneflow.py
--rw-r--r--  2.0 unx    36140 b- defN 23-Mar-06 09:51 onediff/pipeline_stable_diffusion_oneflow.py
+-rw-r--r--  2.0 unx    36019 b- defN 23-Apr-12 01:35 onediff/pipeline_stable_diffusion_img2img_oneflow.py
+-rw-r--r--  2.0 unx    42338 b- defN 23-Apr-12 01:35 onediff/pipeline_stable_diffusion_inpaint_oneflow.py
+-rw-r--r--  2.0 unx    34444 b- defN 23-Apr-12 01:35 onediff/pipeline_stable_diffusion_oneflow.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-22 07:03 onediff/demo/__init__.py
 -rw-r--r--  2.0 unx     1180 b- defN 23-Feb-17 07:48 onediff/demo/__main__.py
--rw-r--r--  2.0 unx      884 b- defN 23-Mar-27 07:44 onediff-0.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 07:44 onediff-0.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-27 07:44 onediff-0.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1239 b- defN 23-Mar-27 07:44 onediff-0.7.0.dist-info/RECORD
-14 files, 207791 bytes uncompressed, 55111 bytes compressed:  73.5%
+-rw-r--r--  2.0 unx      884 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1239 b- defN 23-Apr-12 01:36 onediff-0.8.0.dist-info/RECORD
+14 files, 203904 bytes uncompressed, 54032 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: onediff/demo/__init__.py
 Comment: 
 
 Filename: onediff/demo/__main__.py
 Comment: 
 
-Filename: onediff-0.7.0.dist-info/METADATA
+Filename: onediff-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: onediff-0.7.0.dist-info/WHEEL
+Filename: onediff-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: onediff-0.7.0.dist-info/top_level.txt
+Filename: onediff-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: onediff-0.7.0.dist-info/RECORD
+Filename: onediff-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## onediff/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 __author__ = "OneFlow"
 __credits__ = "OneFlow contributors"
 import oneflow as flow
 
 
 # monkey patch hacks
 flow.strided = None
```

## onediff/graph_utils.py

```diff
@@ -1,47 +1,61 @@
+import os
 import oneflow as flow
-from .oneflow_graph_compile_cache import OneFlowGraphCompileCache
 
 
-class UNetGraph(flow.nn.Graph):
-    def __init__(self, unet):
-        super().__init__()
-        self.unet = unet
-        self.config.enable_cudnn_conv_heuristic_search_algo(False)
-        self.config.allow_fuse_add_to_output(True)
-
-    def build(self, latent_model_input, t, text_embeddings):
-        text_embeddings = flow._C.amp_white_identity(text_embeddings)
-        return self.unet(
-            latent_model_input, t, encoder_hidden_states=text_embeddings
-        ).sample
+def get_unet_graph(cache_size, enable_shared, enable_save, *args, **kwargs):
+    class UNetGraph(flow.nn.Graph):
+        @flow.nn.Graph.with_dynamic_input_shape(
+            enable_shared=enable_shared, size=cache_size
+        )
+        def __init__(self, unet):
+            super().__init__(enable_get_runtime_state_dict=enable_save)
+            self.unet = unet
+            self.config.enable_cudnn_conv_heuristic_search_algo(False)
+            self.config.allow_fuse_add_to_output(True)
+
+        def build(self, latent_model_input, t, text_embeddings):
+            text_embeddings = flow._C.amp_white_identity(text_embeddings)
+            return self.unet(
+                latent_model_input, t, encoder_hidden_states=text_embeddings
+            ).sample
+
+    return UNetGraph(*args, **kwargs)
+
+
+def get_vae_graph(cache_size, enable_shared, enable_save, *args, **kwargs):
+    class VaeGraph(flow.nn.Graph):
+        @flow.nn.Graph.with_dynamic_input_shape(
+            enable_shared=enable_shared, size=cache_size
+        )
+        def __init__(self, vae_post_process) -> None:
+            super().__init__(enable_get_runtime_state_dict=enable_save)
+            self.vae_post_process = vae_post_process
+            self.config.enable_cudnn_conv_heuristic_search_algo(False)
+            self.config.allow_fuse_add_to_output(True)
+
+        def build(self, latents):
+            return self.vae_post_process(latents)
+
+    return VaeGraph(*args, **kwargs)
 
 
 class VaePostProcess(flow.nn.Module):
     def __init__(self, vae) -> None:
         super().__init__()
         self.vae = vae
 
     def forward(self, latents):
         latents = 1 / 0.18215 * latents
         image = self.vae.decode(latents).sample
         image = (image / 2 + 0.5).clamp(0, 1)
         return image
 
 
-class VaeGraph(flow.nn.Graph):
-    def __init__(self, vae_post_process) -> None:
-        super().__init__()
-        self.vae_post_process = vae_post_process
-
-    def build(self, latents):
-        return self.vae_post_process(latents)
-
-
-class GraphCacheMixin:
+class GraphCacheMixin(object):
     r"""
     Base class for all models.
 
     [`DiffusionPipeline`] takes care of storing all components (models, schedulers, processors) for diffusion pipelines
     and handles methods for loading, downloading and saving models as well as a few methods common to all pipelines to:
 
         - move all PyTorch modules to the device of your choice
@@ -50,44 +64,82 @@
     Class attributes:
 
         - **config_name** (`str`) -- name of the config file that will store the class and module names of all
           components of the diffusion pipeline.
         - **_optional_components** (List[`str`]) -- list of all components that are optional so they don't have to be
           passed for the pipeline to function (should be overridden by subclasses).
     """
-    config_name = "model_index.json"
-    _optional_components = []
 
-    def init_graph_compile_cache(self, cache_size, enable_graph_share_mem=False):
-        self.graph_compile_cache = OneFlowGraphCompileCache(
-            cache_size, enable_graph_share_mem
-        )
+    def __init__(self) -> None:
+        self.graph_dict = dict()
+        self.cache_size = 10
+        self.enable_shared = True
+        self.enable_save = True
 
     def set_graph_compile_cache_size(self, cache_size):
-        self.graph_compile_cache.set_cache_size(cache_size)
+        self.cache_size = cache_size
 
-    def enable_graph_share_mem(self, enabled=True):
-        self.graph_compile_cache.enable_share_mem(enabled)
+    def enable_save_graph(self, mode=True):
+        self.enable_save = mode
 
-    def enable_save_graph(self, enabled=True):
-        self.graph_compile_cache.enable_save_graph(enabled)
+    def enable_graph_share_mem(self, mode=True):
+        self.enable_shared = mode
 
     def save_graph(self, path):
-        self.graph_compile_cache.save_graph(path)
+        if self.enable_save:
+            os.makedirs(path, exist_ok=True)
+            for graph_class_name, graph in self.graph_dict.items():
+                state_dict = graph.runtime_state_dict()
+                flow.save(
+                    state_dict, os.path.join(path, graph_class_name),
+                )
 
     def load_graph(self, path, compile_unet: bool = True, compile_vae: bool = True):
-        graph_class2init_args = dict()
         # compile vae graph
         vae_graph = None
         if compile_vae:
             vae_post_process = VaePostProcess(self.vae)
             vae_post_process.eval()
-            vae_graph_args = (VaeGraph, vae_post_process)
-            graph_class2init_args[VaeGraph.__name__] = vae_graph_args
+            state_dict = flow.load(os.path.join(path, "vae"))
+            vae_graph = get_vae_graph(
+                cache_size=self.cache_size,
+                enable_shared=self.enable_shared,
+                enable_save=self.enable_save,
+                vae_post_process=vae_post_process,
+            )
+            vae_graph.load_runtime_state_dict(state_dict)
+            self.graph_dict["vae"] = vae_graph
 
         # compile unet graph
         unet_graph = None
         if compile_unet:
-            unet_graph_args = (UNetGraph, self.unet)
-            graph_class2init_args[UNetGraph.__name__] = unet_graph_args
-
-        self.graph_compile_cache.load_graph(path, graph_class2init_args)
+            state_dict = flow.load(os.path.join(path, "unet"))
+            unet_graph = get_unet_graph(
+                cache_size=self.cache_size,
+                enable_shared=self.enable_shared,
+                enable_save=self.enable_save,
+                unet=self.unet,
+            )
+            unet_graph.load_runtime_state_dict(state_dict)
+            self.graph_dict["unet"] = unet_graph
+
+    def get_graph(self, graph_class, graph):
+        if graph_class == "unet":
+            if graph_class not in self.graph_dict:
+                self.graph_dict[graph_class] = get_unet_graph(
+                    cache_size=self.cache_size,
+                    enable_shared=self.enable_shared,
+                    enable_save=self.enable_save,
+                    unet=graph,
+                )
+            return self.graph_dict[graph_class]
+        elif graph_class == "vae":
+            if graph_class not in self.graph_dict:
+                vae_post_process = VaePostProcess(graph)
+                vae_post_process.eval()
+                self.graph_dict[graph_class] = get_vae_graph(
+                    cache_size=self.cache_size,
+                    enable_shared=self.enable_shared,
+                    enable_save=self.enable_save,
+                    vae_post_process=vae_post_process,
+                )
+            return self.graph_dict[graph_class]
```

## onediff/pipeline_alt_diffusion_oneflow.py

```diff
@@ -38,47 +38,14 @@
 from diffusers.pipelines.alt_diffusion import AltDiffusionPipelineOutput
 from diffusers.pipelines.alt_diffusion import RobertaSeriesModelWithTransformation
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-class UNetGraph(flow.nn.Graph):
-    def __init__(self, unet):
-        super().__init__()
-        self.unet = unet
-        self.config.enable_cudnn_conv_heuristic_search_algo(False)
-        self.config.allow_fuse_add_to_output(True)
-
-    def build(self, latent_model_input, t, text_embeddings):
-        text_embeddings = flow._C.amp_white_identity(text_embeddings)
-        return self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
-
-
-class VaePostProcess(flow.nn.Module):
-    def __init__(self, vae) -> None:
-        super().__init__()
-        self.vae = vae
-
-    def forward(self, latents):
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-        image = (image / 2 + 0.5).clamp(0, 1)
-        return image
-
-
-class VaeGraph(flow.nn.Graph):
-    def __init__(self, vae_post_process) -> None:
-        super().__init__()
-        self.vae_post_process = vae_post_process
-
-    def build(self, latents):
-        return self.vae_post_process(latents)
-
-
 # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline with Stable->Alt, CLIPTextModel->RobertaSeriesModelWithTransformation, CLIPTokenizer->XLMRobertaTokenizer, AltDiffusionSafetyChecker->StableDiffusionSafetyChecker
 class OneFlowAltDiffusionPipeline(DiffusionPipeline, GraphCacheMixin):
     r"""
     Pipeline for text-to-image generation using Alt Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
@@ -218,15 +185,14 @@
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
         self.register_to_config(requires_safety_checker=requires_safety_checker)
-        self.init_graph_compile_cache(1)
 
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
@@ -631,42 +597,37 @@
         )
 
         # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
         extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
         # compile vae graph
         if compile_vae:
-            cache_key = (height, width, num_images_per_prompt)
-            vae_post_process = VaePostProcess(self.vae)
-            vae_post_process.eval()
-            vae_post_process_graph = self.graph_compile_cache.get_graph(VaeGraph, cache_key, vae_post_process)
-            vae_post_process_graph.compile(latents)
+            vae_post_process_graph = self.get_graph("vae", self.vae)
+            if vae_post_process_graph.is_compiled is False:
+                vae_post_process_graph._compile(latents)
 
         # compile unet graph
         if compile_unet:
-            cache_key = (height, width, num_images_per_prompt)
-            unet_graph = self.graph_compile_cache.get_graph(UNetGraph, cache_key, self.unet)
+            unet_graph = self.get_graph("unet", self.unet)
             if unet_graph.is_compiled is False:
                 latent_model_input = flow.cat([latents] * 2) if do_classifier_free_guidance else latents
                 _, t = list(enumerate(self.scheduler.timesteps))[0]
-                unet_graph.compile(latent_model_input, t, text_embeddings)
+                unet_graph._compile(latent_model_input, t, text_embeddings)
 
         # 7. Denoising loop
         num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
         with self.progress_bar(total=num_inference_steps) as progress_bar:
             for i, t in enumerate(timesteps):
                 # expand the latents if we are doing classifier free guidance
                 latent_model_input = flow.cat([latents] * 2) if do_classifier_free_guidance else latents
                 latent_model_input = self.scheduler.scale_model_input(latent_model_input, t)
 
                 # predict the noise residual
                 if compile_unet:
-                    flow._oneflow_internal.profiler.RangePush(f"denoise-{i}-unet-graph")
                     noise_pred = unet_graph(latent_model_input, t, text_embeddings)
-                    flow._oneflow_internal.profiler.RangePop()
                 else:
                     noise_pred = self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
 
                 # perform guidance
                 if do_classifier_free_guidance:
                     noise_pred_uncond, noise_pred_text = noise_pred.chunk(2)
                     noise_pred = noise_pred_uncond + guidance_scale * (noise_pred_text - noise_pred_uncond)
```

## onediff/pipeline_stable_diffusion_img2img_oneflow.py

```diff
@@ -48,25 +48,14 @@
 
 from timeit import default_timer as timer
 import os
 
 import oneflow as flow
 
 
-class UNetGraph(flow.nn.Graph):
-    def __init__(self, unet):
-        super().__init__()
-        self.unet = unet
-        self.config.enable_cudnn_conv_heuristic_search_algo(False)
-
-    def build(self, latent_model_input, t, text_embeddings):
-        text_embeddings = torch._C.amp_white_identity(text_embeddings)
-        return self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
-
-
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 def preprocess(image):
     w, h = image.size
     w, h = map(lambda x: x - x % 32, (w, h))  # resize to integer multiple of 32
     image = image.resize((w, h), resample=PIL_INTERPOLATION["lanczos"])
@@ -218,19 +207,14 @@
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
         self.register_to_config(requires_safety_checker=requires_safety_checker)
-        self.unet_graphs = dict()
-        self.unet_graphs_cache_size = 1
-        self.unet_graphs_lru_cache_time = 0
-        # solve AttributeError: 'OneFlowStableDiffusionImg2ImgPipeline' object has no attribute 'graph_compile_cache'
-        self.init_graph_compile_cache(self.unet_graphs_cache_size)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
@@ -637,41 +621,27 @@
         latent_timestep = timesteps[:1].repeat(batch_size * num_images_per_prompt)
 
         # 6. Prepare latent variables
         latents = self.prepare_latents(
             image, latent_timestep, batch_size, num_images_per_prompt, text_embeddings.dtype, device, generator
         )
 
-        compilation_start = timer()
-        compilation_time = 0
+        # compile vae graph
+        if compile_vae:
+            vae_post_process_graph = self.get_graph("vae", self.vae)
+            if vae_post_process_graph.is_compiled is False:
+                vae_post_process_graph._compile(latents)
+        
+        # compile unet graph
         if compile_unet:
-            self.unet_graphs_lru_cache_time += 1
-            (_, _, height, width) = latents.shape
-            if (height, width) in self.unet_graphs:
-                _, unet_graph = self.unet_graphs[height, width]
-                self.unet_graphs[height, width] = (self.unet_graphs_lru_cache_time, unet_graph)
-            else:
-                while len(self.unet_graphs) >= self.unet_graphs_cache_size:
-                    shape_to_del = min(self.unet_graphs.keys(), key=lambda shape: self.unet_graphs[shape][0])
-                    print(
-                        "[oneflow]",
-                        f"a compiled unet (height={shape_to_del[0]}, width={shape_to_del[1]}) "
-                        "is deleted according to the LRU policy",
-                    )
-                    print("[oneflow]", "cache size can be changed by `pipeline.set_unet_graphs_cache_size`")
-                    del self.unet_graphs[shape_to_del]
-                print("[oneflow]", "compiling unet beforehand to make sure the progress bar is more accurate")
-                i, t = list(enumerate(self.scheduler.timesteps))[0]
+            unet_graph = self.get_graph("unet", self.unet)
+            if unet_graph.is_compiled is False:
+                _, t = list(enumerate(self.scheduler.timesteps))[0]
                 latent_model_input = torch.cat([latents] * 2) if do_classifier_free_guidance else latents
-                unet_graph = UNetGraph(self.unet)
                 unet_graph._compile(latent_model_input, t, text_embeddings)
-                unet_graph(latent_model_input, t, text_embeddings)  # warmup
-                compilation_time = timer() - compilation_start
-                print("[oneflow]", "[elapsed(s)]", "[unet compilation]", compilation_time)
-                self.unet_graphs[height, width] = (self.unet_graphs_lru_cache_time, unet_graph)
 
         # 7. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
         extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
         # 8. Denoising loop
         num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
         with self.progress_bar(total=num_inference_steps) as progress_bar:
@@ -697,15 +667,19 @@
                 # call the callback, if provided
                 if (i + 1) > num_warmup_steps and (i + 1) % self.scheduler.order == 0:
                     progress_bar.update()
                     if callback is not None and i % callback_steps == 0:
                         callback(i, t, latents)
 
         # 9. Post-processing
-        image = self.decode_latents(latents)
+        if compile_vae:
+            image = vae_post_process_graph(latents)
+            image = image.cpu().permute(0, 2, 3, 1).float().numpy()
+        else:
+            image = self.decode_latents(latents)
 
         # 10. Run safety checker
         image, has_nsfw_concept = self.run_safety_checker(image, device, text_embeddings.dtype)
 
         # 11. Convert to PIL
         if output_type == "pil":
             image = self.numpy_to_pil(image)
```

## onediff/pipeline_stable_diffusion_inpaint_oneflow.py

```diff
@@ -33,47 +33,14 @@
 from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
 from diffusers.pipelines.stable_diffusion.safety_checker import StableDiffusionSafetyChecker
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
-class UNetGraph(flow.nn.Graph):
-    def __init__(self, unet):
-        super().__init__()
-        self.unet = unet
-        self.config.enable_cudnn_conv_heuristic_search_algo(False)
-        self.config.allow_fuse_add_to_output(True)
-
-    def build(self, latent_model_input, t, text_embeddings):
-        text_embeddings = flow._C.amp_white_identity(text_embeddings)
-        return self.unet(latent_model_input, t, encoder_hidden_states=text_embeddings).sample
-
-
-class VaePostProcess(flow.nn.Module):
-    def __init__(self, vae) -> None:
-        super().__init__()
-        self.vae = vae
-
-    def forward(self, latents):
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-        image = (image / 2 + 0.5).clamp(0, 1)
-        return image
-
-
-class VaeGraph(flow.nn.Graph):
-    def __init__(self, vae_post_process) -> None:
-        super().__init__()
-        self.vae_post_process = vae_post_process
-
-    def build(self, latents):
-        return self.vae_post_process(latents)
-
-
 def prepare_mask_and_masked_image(image, mask):
     """
     Prepares a pair (image, mask) to be consumed by the Stable Diffusion pipeline. This means that those inputs will be
     converted to ``flow.Tensor`` with shapes ``batch x channels x height x width`` where ``channels`` is ``3`` for the
     ``image`` and ``1`` for the ``mask``.
 
     The ``image`` will be converted to ``flow.float32`` and normalized to be in ``[-1, 1]``. The ``mask`` will be
@@ -296,15 +263,14 @@
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
         self.register_to_config(requires_safety_checker=requires_safety_checker)
-        self.init_graph_compile_cache(1)
 
     # Copied from diffusers.pipelines.stable_diffusion.pipeline_stable_diffusion.StableDiffusionPipeline.enable_attention_slicing
     def enable_attention_slicing(self, slice_size: Optional[Union[str, int]] = "auto"):
         r"""
         Enable sliced attention computation.
 
         When this option is enabled, the attention module will split the input tensor in slices, to compute attention
@@ -774,29 +740,26 @@
             )
 
         # 9. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
         extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
         # compile vae graph
         if compile_vae:
-            cache_key = (height, width, num_images_per_prompt)
-            vae_post_process = VaePostProcess(self.vae)
-            vae_post_process.eval()
-            vae_post_process_graph = self.graph_compile_cache.get_graph(VaeGraph, cache_key, vae_post_process)
-            vae_post_process_graph.compile(latents)
+            vae_post_process_graph = self.get_graph("vae", self.vae)
+            if vae_post_process_graph.is_compiled is False:
+                vae_post_process_graph._compile(latents)
 
         # compile unet graph
         if compile_unet:
-            cache_key = (height, width, num_images_per_prompt)
-            unet_graph = self.graph_compile_cache.get_graph(UNetGraph, cache_key, self.unet)
+            unet_graph = self.get_graph("unet", self.unet)
             if unet_graph.is_compiled is False:
                 latent_model_input = flow.cat([latents] * 2) if do_classifier_free_guidance else latents
                 _, t = list(enumerate(self.scheduler.timesteps))[0]
                 latent_model_input = flow.cat([latent_model_input, mask, masked_image_latents], dim=1)
-                unet_graph.compile(latent_model_input, t, text_embeddings)
+                unet_graph._compile(latent_model_input, t, text_embeddings)
 
         # 10. Denoising loop
         num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
         with self.progress_bar(total=num_inference_steps) as progress_bar:
             for i, t in enumerate(timesteps):
                 # expand the latents if we are doing classifier free guidance
                 latent_model_input = flow.cat([latents] * 2) if do_classifier_free_guidance else latents
```

## onediff/pipeline_stable_diffusion_oneflow.py

```diff
@@ -31,58 +31,14 @@
 
 from timeit import default_timer as timer
 import os
 import oneflow as flow
 from .graph_utils import GraphCacheMixin
 
 
-class UNetGraph(flow.nn.Graph):
-    def __init__(self, unet):
-        super().__init__()
-        self.unet = unet
-        self.config.enable_cudnn_conv_heuristic_search_algo(False)
-        self.config.allow_fuse_add_to_output(True)
-
-    def build(self, latent_model_input, t, text_embeddings):
-        text_embeddings = flow._C.amp_white_identity(text_embeddings)
-        return self.unet(
-            latent_model_input, t, encoder_hidden_states=text_embeddings
-        ).sample
-
-
-class VaePostProcess(flow.nn.Module):
-    def __init__(self, vae) -> None:
-        super().__init__()
-        self.vae = vae
-
-    def forward(self, latents):
-        latents = 1 / 0.18215 * latents
-        image = self.vae.decode(latents).sample
-        image = (image / 2 + 0.5).clamp(0, 1)
-        return image
-
-
-class VaeGraph(flow.nn.Graph):
-    def __init__(self, vae_post_process) -> None:
-        super().__init__()
-        self.vae_post_process = vae_post_process
-
-    def build(self, latents):
-        return self.vae_post_process(latents)
-
-
-class TextEncoderGraph(flow.nn.Graph):
-    def __init__(self, text_encoder) -> None:
-        super().__init__()
-        self.text_encoder = text_encoder
-
-    def build(self, text_input, attention_mask):
-        return self.text_encoder(text_input, attention_mask)[0]
-
-
 class OneFlowStableDiffusionPipeline(DiffusionPipeline, GraphCacheMixin):
     r"""
     Pipeline for text-to-image generation using Stable Diffusion.
 
     This model inherits from [`DiffusionPipeline`]. Check the superclass documentation for the generic methods the
     library implements for all the pipelines (such as downloading or saving, running on a particular device, etc.)
 
@@ -239,15 +195,14 @@
             unet=unet,
             scheduler=scheduler,
             safety_checker=safety_checker,
             feature_extractor=feature_extractor,
         )
         self.vae_scale_factor = 2 ** (len(self.vae.config.block_out_channels) - 1)
         self.register_to_config(requires_safety_checker=requires_safety_checker)
-        self.init_graph_compile_cache(1)
 
     def enable_xformers_memory_efficient_attention(self):
         r"""
         Enable memory efficient attention as implemented in xformers.
 
         When this option is enabled, you should observe lower GPU memory usage and a potential speed up at inference
         time. Speed up at training time is not guaranteed.
@@ -709,36 +664,27 @@
             device,
             generator,
             latents,
         )
 
         # compile vae graph
         if compile_vae:
-            cache_key = (height, width, num_images_per_prompt)
-            vae_post_process = VaePostProcess(self.vae)
-            vae_post_process.eval()
-            vae_post_process_graph = self.graph_compile_cache.get_graph(
-                VaeGraph, cache_key, vae_post_process
-            )
+            vae_post_process_graph = self.get_graph("vae", self.vae)
             if vae_post_process_graph.is_compiled is False:
-                vae_post_process_graph.compile(latents)
+                vae_post_process_graph._compile(latents)
 
         # compile unet graph
         if compile_unet:
-            cache_key = (height, width, num_images_per_prompt)
-            unet_graph = self.graph_compile_cache.get_graph(
-                UNetGraph, cache_key, self.unet
-            )
+            unet_graph = self.get_graph("unet", self.unet)
             if unet_graph.is_compiled is False:
                 latent_model_input = (
                     flow.cat([latents] * 2) if do_classifier_free_guidance else latents
                 )
                 _, t = list(enumerate(self.scheduler.timesteps))[0]
-                unet_graph.compile(latent_model_input, t, text_embeddings)
-
+                unet_graph._compile(latent_model_input, t, text_embeddings)
         # 6. Prepare extra step kwargs. TODO: Logic should ideally just be moved out of the pipeline
         extra_step_kwargs = self.prepare_extra_step_kwargs(generator, eta)
 
         # 7. Denoising loop
         num_warmup_steps = len(timesteps) - num_inference_steps * self.scheduler.order
         with self.progress_bar(total=num_inference_steps) as progress_bar:
             for i, t in enumerate(timesteps):
```

## Comparing `onediff-0.7.0.dist-info/METADATA` & `onediff-0.8.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 0.7.0
+Version: 0.8.0
 Summary: OneFlow backend for diffusers
 Home-page: https://github.com/Oneflow-Inc/oneflow
 Author: OneFlow contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

