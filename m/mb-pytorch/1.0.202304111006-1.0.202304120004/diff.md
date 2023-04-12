# Comparing `tmp/mb_pytorch-1.0.202304111006-py3-none-any.whl.zip` & `tmp/mb_pytorch-1.0.202304120004-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 28563 bytes, number of entries: 36
--rw-rw-r--  2.0 unx     3133 b- defN 23-Apr-10 19:17 mb_pytorch/classification/training.py
+Zip file size: 29032 bytes, number of entries: 36
+-rw-rw-r--  2.0 unx     4990 b- defN 23-Apr-12 00:03 mb_pytorch/classification/training.py
 -rw-rw-r--  2.0 unx       44 b- defN 23-Mar-16 11:39 mb_pytorch/dataloader/__init__.py
 -rw-rw-r--  2.0 unx    11844 b- defN 23-Mar-31 20:26 mb_pytorch/dataloader/loader.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-23 13:56 mb_pytorch/metalearning/__init__.py
 -rw-rw-r--  2.0 unx     1385 b- defN 23-Mar-02 03:28 mb_pytorch/metalearning/meta_utils.py
 -rw-rw-r--  2.0 unx     1030 b- defN 23-Mar-15 02:58 mb_pytorch/metalearning/proto_dataloader.py
 -rw-rw-r--  2.0 unx     2861 b- defN 23-Mar-03 23:55 mb_pytorch/metalearning/prototypical.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-31 19:54 mb_pytorch/models/__init__.py
@@ -19,20 +19,20 @@
 -rw-rw-r--  2.0 unx     1184 b- defN 23-Mar-23 01:40 mb_pytorch/models/blocks/rnn.py
 -rw-rw-r--  2.0 unx     1630 b- defN 23-Mar-17 00:48 mb_pytorch/training/accelerate_train.py
 -rw-rw-r--  2.0 unx     1443 b- defN 23-Apr-08 10:22 mb_pytorch/training/train_params.py
 -rw-rw-r--  2.0 unx      144 b- defN 23-Apr-01 17:43 mb_pytorch/training/training.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-23 13:56 mb_pytorch/utils/__init__.py
 -rw-rw-r--  2.0 unx     1055 b- defN 23-Mar-17 02:23 mb_pytorch/utils/compiler.py
 -rw-rw-r--  2.0 unx      257 b- defN 23-Mar-01 22:55 mb_pytorch/utils/dist.py
--rw-rw-r--  2.0 unx     3391 b- defN 23-Apr-11 10:05 mb_pytorch/utils/extra_utils.py
+-rw-rw-r--  2.0 unx     3391 b- defN 23-Apr-11 23:28 mb_pytorch/utils/extra_utils.py
 -rw-rw-r--  2.0 unx     7178 b- defN 23-Mar-15 02:58 mb_pytorch/utils/generate_emb.py
 -rw-rw-r--  2.0 unx     2582 b- defN 23-Apr-03 19:30 mb_pytorch/utils/losses.py
 -rw-rw-r--  2.0 unx     1199 b- defN 23-Apr-04 20:14 mb_pytorch/utils/metrics.py
 -rw-rw-r--  2.0 unx     5537 b- defN 23-Mar-27 17:38 mb_pytorch/utils/viewer.py
 -rw-rw-r--  2.0 unx      994 b- defN 23-Mar-06 13:11 mb_pytorch/utils/yaml_reader.py
--rwxrwxr-x  2.0 unx     1304 b- defN 23-Apr-11 10:06 mb_pytorch-1.0.202304111006.data/scripts/dataload_results.py
--rwxrwxr-x  2.0 unx      980 b- defN 23-Mar-15 02:59 mb_pytorch-1.0.202304111006.data/scripts/emb.py
--rw-rw-r--  2.0 unx      329 b- defN 23-Apr-11 10:06 mb_pytorch-1.0.202304111006.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 10:06 mb_pytorch-1.0.202304111006.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Apr-11 10:06 mb_pytorch-1.0.202304111006.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3256 b- defN 23-Apr-11 10:06 mb_pytorch-1.0.202304111006.dist-info/RECORD
-36 files, 82031 bytes uncompressed, 23243 bytes compressed:  71.7%
+-rwxrwxr-x  2.0 unx     1304 b- defN 23-Apr-12 00:04 mb_pytorch-1.0.202304120004.data/scripts/dataload_results.py
+-rwxrwxr-x  2.0 unx      980 b- defN 23-Mar-15 02:59 mb_pytorch-1.0.202304120004.data/scripts/emb.py
+-rw-rw-r--  2.0 unx      329 b- defN 23-Apr-12 00:04 mb_pytorch-1.0.202304120004.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-12 00:04 mb_pytorch-1.0.202304120004.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Apr-12 00:04 mb_pytorch-1.0.202304120004.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3256 b- defN 23-Apr-12 00:04 mb_pytorch-1.0.202304120004.dist-info/RECORD
+36 files, 83888 bytes uncompressed, 23712 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -84,26 +84,26 @@
 
 Filename: mb_pytorch/utils/viewer.py
 Comment: 
 
 Filename: mb_pytorch/utils/yaml_reader.py
 Comment: 
 
-Filename: mb_pytorch-1.0.202304111006.data/scripts/dataload_results.py
+Filename: mb_pytorch-1.0.202304120004.data/scripts/dataload_results.py
 Comment: 
 
-Filename: mb_pytorch-1.0.202304111006.data/scripts/emb.py
+Filename: mb_pytorch-1.0.202304120004.data/scripts/emb.py
 Comment: 
 
-Filename: mb_pytorch-1.0.202304111006.dist-info/METADATA
+Filename: mb_pytorch-1.0.202304120004.dist-info/METADATA
 Comment: 
 
-Filename: mb_pytorch-1.0.202304111006.dist-info/WHEEL
+Filename: mb_pytorch-1.0.202304120004.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pytorch-1.0.202304111006.dist-info/top_level.txt
+Filename: mb_pytorch-1.0.202304120004.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pytorch-1.0.202304111006.dist-info/RECORD
+Filename: mb_pytorch-1.0.202304120004.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pytorch/classification/training.py

```diff
@@ -2,14 +2,19 @@
 from ..dataloader.loader import DataLoader
 import torch
 from ..training.train_params import train_helper
 import tqdm
 from torch.utils.tensorboard import SummaryWriter
 import os
 from mb_utils.src.logging import logger
+from pytorch_grad_cam import GradCAM
+from pytorch_grad_cam.utils.image import show_cam_on_image
+
+
+__all__ = ['train_loop']
 
 yaml_file = '/home/malav/mb_pytorch/scripts/models/loader_y.yaml'
 data = DataLoader(yaml_file,logger=None)
 data_model = data.data_dict['model']
 train_loader, val_loader,_,_ = data.data_load(logger=None)
 model = ModelLoader(data_model,logger=None)
 
@@ -25,69 +30,109 @@
 
 path_logs = os.path.join(data['data']['work_dir'], 'logs')
 writer = SummaryWriter(log_dir=path_logs)
 
 logger = logger
 
 
-for i in tqdm.tqdm(range(data_model['model_epochs'])):
-    ##train loop
-    model.train()
-    train_loss = 0
-    logger.info('Training Started')
-    for j,(x,y) in enumerate(train_loader):
-        x,y = x.to(device),y.to(device)
-        optimizer.zero_grad()
-        y_pred = model(x)
-        current_loss = loss_attr()(y_pred,y)
-        current_loss.backward()    
-        optimizer.step()
-        train_loss += current_loss.item()
-        logger.info(f'Epoch {i+1} - Batch {j+1} - Train Loss: {current_loss.item()}')
-
-    avg_train_loss = train_loss / len(train_loader)
-    logger.info(f'Epoch {i+1} - Train Loss: {avg_train_loss}')
-    
-    writer.add_scalar('Loss/train', loss_attr().item(), global_step=i)
-    
-    if scheduler is not None:
-        scheduler.step()
-    
-    for name, param in model.named_parameters():
-        writer.add_histogram(name, param, global_step=i)
+def train_loop( data,data_model,model,train_loader,val_loader,loss_attr,optimizer,scheduler=None,writer=None,logger=None,gradcam=None,device='cpu'):
+    """
+    Function to train the model
+    Args:
+        data: data dictionary YAML of DataLoader
+        data_model: model parameters - data.data_dict['model']
+        model: model to be trained
+        train_loader: train dataloader
+        val_loader: validation dataloader
+        loss_attr: loss function
+        optimizer: optimizer
+        scheduler: scheduler
+        writer: tensorboard writer
+        logger: logger
+        gradcam: gradcam layers to be visulized
+        device: default is cpu
+    output:
+        None
+    """
+
+    for i in tqdm.tqdm(range(data_model['model_epochs'])):
+        ##train loop
+        model.train()
+        train_loss = 0
+        if logger:
+            logger.info('Training Started')
+    
+        for j,(x,y) in enumerate(train_loader):
+            x,y = x.to(device),y.to(device)
+            optimizer.zero_grad()
+            y_pred = model(x)
+            current_loss = loss_attr()(y_pred,y)
+            current_loss.backward()    
+            optimizer.step()
+            train_loss += current_loss.item()
+            if logger:
+                logger.info(f'Epoch {i+1} - Batch {j+1} - Train Loss: {current_loss.item()}')
+
+        avg_train_loss = train_loss / len(train_loader)
+        if logger:
+            logger.info(f'Epoch {i+1} - Train Loss: {avg_train_loss}')
+    
+        if writer is not None:
+            writer.add_scalar('Loss/train', loss_attr().item(), global_step=i)
+    
+        if scheduler is not None:
+            scheduler.step()
+    
+        if writer is not None:
+            for name, param in model.named_parameters():
+                writer.add_histogram(name, param, global_step=i)
+        
+        #get grad cam images
+        if gradcam and writer is not None:
+            for cam_layers in gradcam:
+                if getattr(model,cam_layers) is None:
+                    if logger:
+                        logger.info(f'Layer {cam_layers} not found in model') 
+                else:
+                    with GradCAM(model=model,target_layers=cam_layers,use_cuda=False) as cm: 
+                        cr = cm(input_tensor=x)[0,:]
+                        writer.add_image(f'Gradcam/{cam_layers}',show_cam_on_image(x[0].cpu().numpy(),cr.cpu().numpy(),use_rgb=True),global_step=i)
         
-    #get grad cam images
         
-    #validation loop
-    val_loss = 0
-    val_acc = 0
-    num_samples = 0
-    
-    model.eval()
-    with torch.no_grad():
-        for x_val, y_val in val_loader:
-            x_val, y_val = x_val.to(device), y_val.to(device)
-            output = model(x_val)
-            val_loss += loss_attr()(output, y_val).item() * x_val.size(0)
-            _, preds = torch.max(output, 1)
-            val_acc += torch.sum(preds == y_val.data)
-            num_samples += x_val.size(0)
-            logger.info(f'Epoch {i+1} - Batch {j+1} - Val Loss: {val_loss}')
+        #validation loop
+        val_loss = 0
+        val_acc = 0
+        num_samples = 0
+    
+        model.eval()
+        with torch.no_grad():
+            for x_val, y_val in val_loader:
+                x_val, y_val = x_val.to(device), y_val.to(device)
+                output = model(x_val)
+                val_loss += loss_attr()(output, y_val).item() * x_val.size(0)
+                _, preds = torch.max(output, 1)
+                val_acc += torch.sum(preds == y_val.data)
+                num_samples += x_val.size(0)
+                if logger: 
+                    logger.info(f'Epoch {i+1} - Batch {j+1} - Val Loss: {val_loss}')
             
-        val_loss /= num_samples
-        val_acc = val_acc.double() / num_samples
-        logger.info(f'Epoch {i+1} - Val Loss: {val_loss}', f'Epoch {i+1} - Val Accuracy: {val_acc}')
-    
-    writer.add_scalar('Loss/val', val_loss, global_step=i)
-    writer.add_scalar('Accuracy/val', val_acc, global_step=i)
-    
-    # save best model
-    if val_loss < best_val_loss:
-        best_val_loss = val_loss
-        best_model = model.state_dict()
-
-        path = os.path.join(data['data']['work_dir'], 'best_model.pth')
-        torch.save(best_model, path)
-        logger.info(f'Epoch {i+1} - Best Model Saved')
+            val_loss /= num_samples
+            val_acc = val_acc.double() / num_samples
+            if logger:
+                logger.info(f'Epoch {i+1} - Val Loss: {val_loss}', f'Epoch {i+1} - Val Accuracy: {val_acc}')
+    
+        if writer is not None:
+            writer.add_scalar('Loss/val', val_loss, global_step=i)
+            writer.add_scalar('Accuracy/val', val_acc, global_step=i)
+    
+        # save best model
+        if val_loss < best_val_loss:
+            best_val_loss = val_loss
+            best_model = model.state_dict()
+
+            path = os.path.join(data['data']['work_dir'], 'best_model.pth')
+            torch.save(best_model, path)
+            if logger:
+                logger.info(f'Epoch {i+1} - Best Model Saved')
         
-    model.train()
+        model.train()
```

## mb_pytorch/utils/extra_utils.py

```diff
@@ -79,16 +79,16 @@
     Output:
         feature_view: Feature view from the model
     """
     out_list = []
     for j in data:
         for i in range(len(layer_names)):
             layer = layer_names[i]
-            #features = feature_extractor(model,layer)
-            features = getattr(model,layer)
+            features = feature_extractor(model,layer)
+            #features = getattr(model,layer)
             output = features(j)
             output = output.squeeze(0).detach().numpy()
             out_list.append(output)
         fig, axs = plt.subplots(1, len(layer_names), figsize=(12, 12))
         for i in range(len(layer_names)):
             if len(out_list[i].shape) > 2:
                 out_map = np.sum(out_list[i], axis=0)
```

## Comparing `mb_pytorch-1.0.202304111006.data/scripts/dataload_results.py` & `mb_pytorch-1.0.202304120004.data/scripts/dataload_results.py`

 * *Files identical despite different names*

## Comparing `mb_pytorch-1.0.202304111006.data/scripts/emb.py` & `mb_pytorch-1.0.202304120004.data/scripts/emb.py`

 * *Files identical despite different names*

## Comparing `mb_pytorch-1.0.202304111006.dist-info/RECORD` & `mb_pytorch-1.0.202304120004.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mb_pytorch/classification/training.py,sha256=YSNb0UCcAyTy68qRxztNTuKXfqUl8mwwziwtJ0Ed-og,3133
+mb_pytorch/classification/training.py,sha256=EIXYP8coQc0ovULifcrsUl69ip7U0Z5XgeXUYLJ1PK0,4990
 mb_pytorch/dataloader/__init__.py,sha256=nB0xPAHbI91Ra1dDkWR1l4td5A4k9xko-I5Jdgv5apI,44
 mb_pytorch/dataloader/loader.py,sha256=NQMZszSD8WN0Ile1NY9BlpgjXmNxUm86H9KefxwKUJM,11844
 mb_pytorch/metalearning/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mb_pytorch/metalearning/meta_utils.py,sha256=mgHYiQIIcYQ1pVTJcrjquSXpQstdYD1q8iXO09Zao1s,1385
 mb_pytorch/metalearning/proto_dataloader.py,sha256=WvrfZYkYMxorocCkR_zHS_AC8W_ML9YndB-P6evkdcc,1030
 mb_pytorch/metalearning/prototypical.py,sha256=qFVf6VF3s8zskGqbM3geJV-dfkdO3tRaf3P8U_KR-cE,2861
 mb_pytorch/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -18,19 +18,19 @@
 mb_pytorch/models/blocks/rnn.py,sha256=DpEgvmK5Eh4HOQaF1Uk-tZFcocDkZhZxO08EALY1_Bs,1184
 mb_pytorch/training/accelerate_train.py,sha256=aozId-qro7FzfjxbqCW09PWGUBphZxEIicF_gYyhQG8,1630
 mb_pytorch/training/train_params.py,sha256=Algc1WIhyD11cRod7ZvBVdofKFCFzVI_D3dd4YAAPYg,1443
 mb_pytorch/training/training.py,sha256=3zRnYRKMO0K0VxgZEjf3p1b0mMLGVwZb5pDNGskjovY,144
 mb_pytorch/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mb_pytorch/utils/compiler.py,sha256=ixu-wc--ykhsjXTZINw34MLmZFg7L-dLkYs7p-nn6i4,1055
 mb_pytorch/utils/dist.py,sha256=7-ZdntmiugRWYnT5wileo8mYTuV1dbjVl4ffJsfnfAw,257
-mb_pytorch/utils/extra_utils.py,sha256=78BBueVea9Gqx2cPLlg1xmfFVi8VVLRsypmv3mRsDi0,3391
+mb_pytorch/utils/extra_utils.py,sha256=-MaT-x3gwgEOVLpg-tWm5yLFtI0CxpV0QUlXx-rqu08,3391
 mb_pytorch/utils/generate_emb.py,sha256=2iK8wRIrYfaLpEgjdbFnDqGU5ux-1JhncQoeboW_6LQ,7178
 mb_pytorch/utils/losses.py,sha256=OLCPLkJH46IofSSVly2xdcklVv7Q5OFFEGtVrJcV7V0,2582
 mb_pytorch/utils/metrics.py,sha256=Kqmdu9llSjR8aRp3IVlmy6PqeQexf0ZXjTJUcEtvcfI,1199
 mb_pytorch/utils/viewer.py,sha256=vMV9YiwTqFNvgFtQ-dOCtmwAtDgKomDzFzicVFLmQhc,5537
 mb_pytorch/utils/yaml_reader.py,sha256=Azgr_5qttsH_BBVsCtfccFMvK6IEjTRYhd5qp4S5uzk,994
-mb_pytorch-1.0.202304111006.data/scripts/dataload_results.py,sha256=8IFAH7WX-nSJ7V532rr3Cl7R37v0jhSakw0JCd9dalE,1304
-mb_pytorch-1.0.202304111006.data/scripts/emb.py,sha256=5jSbTGNOhusDTvHZeaTwk4pmJa4HIdkRGd98s0L4Rl0,980
-mb_pytorch-1.0.202304111006.dist-info/METADATA,sha256=qs9HYnzts8XB2wrwvRmR55tCtdUVEhS6kcgzEoWO1ew,329
-mb_pytorch-1.0.202304111006.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pytorch-1.0.202304111006.dist-info/top_level.txt,sha256=2m_aBiEfjq3pZM2NtYSlTqlgoQxH6WaK8_8SsRicIvg,11
-mb_pytorch-1.0.202304111006.dist-info/RECORD,,
+mb_pytorch-1.0.202304120004.data/scripts/dataload_results.py,sha256=8IFAH7WX-nSJ7V532rr3Cl7R37v0jhSakw0JCd9dalE,1304
+mb_pytorch-1.0.202304120004.data/scripts/emb.py,sha256=5jSbTGNOhusDTvHZeaTwk4pmJa4HIdkRGd98s0L4Rl0,980
+mb_pytorch-1.0.202304120004.dist-info/METADATA,sha256=omyF25rfUBdfGJQJJmJZby9iSB7Lr322h4FqqrJJIxg,329
+mb_pytorch-1.0.202304120004.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pytorch-1.0.202304120004.dist-info/top_level.txt,sha256=2m_aBiEfjq3pZM2NtYSlTqlgoQxH6WaK8_8SsRicIvg,11
+mb_pytorch-1.0.202304120004.dist-info/RECORD,,
```

