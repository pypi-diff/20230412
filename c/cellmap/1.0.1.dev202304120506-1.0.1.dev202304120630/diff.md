# Comparing `tmp/cellmap-1.0.1.dev202304120506-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304120630-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 8861 bytes, number of entries: 5
+Zip file size: 8794 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    42978 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120506.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120506.dist-info/WHEEL
-?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304120506.dist-info/RECORD
-5 files, 45109 bytes uncompressed, 8107 bytes compressed:  82.0%
+-rw-r--r--  2.0 unx    43229 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1587 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120630.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304120630.dist-info/WHEEL
+?rw-r--r--  2.0 unx      404 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304120630.dist-info/RECORD
+5 files, 45360 bytes uncompressed, 8040 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304120506.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304120630.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304120506.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304120630.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304120506.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304120630.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -70,17 +70,17 @@
                 kwargs['exp_2d_key'] = 'X_tsne'
             elif 'X_pca' in adata.obsm.keys():
                 logger.warning('Warning: The key \"%s\" was not found in adata.obsm, but \"X_pca\" was found insted. \"%s\" was replaced with \"X_tsne\".' % (kwargs['exp_2d_key'],kwargs['exp_2d_key']))
                 kwargs['exp_2d_key'] = 'X_pca'
             else:
                 raise KeyError('The key \"%s\" was not found in adata.obsm.obsm. Please modify the argument \"exp_2d_key\".' % kwargs['exp_2d_key'])
     
-    if 'vel_key' in kwargs.keys():
-        if (kwargs['vel_key'] not in adata.obsm.keys()) and (kwargs['vel_key'] not in adata.layers.keys()):
-            raise KeyError('The key \"%s\" was not found in adata.obsm.obsm. Please modify the argument \"vel_key\".' % kwargs['vel_key'])
+    if 'vkey' in kwargs.keys():
+        if (kwargs['vkey'] not in adata.obsm.keys()) and (kwargs['vkey'] not in adata.layers.keys()):
+            raise KeyError('The key \"%s\" was not found in adata.obsm.obsm. Please modify the argument \"vkey\".' % kwargs['vkey'])
     
     if 'vel_2d_key' in kwargs.keys():
         if (kwargs['vel_2d_key'] not in adata.obsm.keys()) and (kwargs['vel_2d_key'] not in adata.layers.keys()):
             if 'velocity_umap' in adata.obsm.keys():
                 logger.warning('The key \"%s\" was not found in adata.obsm, but \"velocity_umap\" was found insted. \"%s\" was replaced with \"velocity_umap\".' % (kwargs['vel_2d_key'],kwargs['vel_2d_key']))
                 kwargs['vel_2d_key'] = 'velocity_umap'
             elif 'velocity_tsne' in adata.obsm.keys():
@@ -180,17 +180,17 @@
     colornorm[-1][0] = 1
     cmap = matplotlib.colors.LinearSegmentedColormap.from_list('earth', colornorm, N=hight.max()-hight.min()+1)
     return cmap
 
 
 def Hodge_decomposition(
     adata,
-    exp_key = None,
-    vel_key  = 'velocity',
     basis = 'umap',
+    vkey  = 'velocity',
+    exp_key = None,
     potential_key = 'Hodge_potential',
     potential_vkey = 'potential_velocity',
     rotation_key = 'Hodge_rotation',
     rotation_vkey = 'rotation_velocity',
     graph_key = 'CM_graph',
     graph_method = 'Delauney',
     HD_rate = 0.2,
@@ -207,37 +207,37 @@
     Parameters
     ----------
     adata: anndata (n_samples, n_features)
     
     exp_key: None or string
     """
     
-    kwargs_arg = check_arguments(adata, verbose = True, exp_key=exp_key, vel_key = vel_key, basis=basis, graph_method=graph_method)
-    exp_key,vel_key,basis = kwargs_arg['exp_key'],kwargs_arg['vel_key'],kwargs_arg['basis']
+    kwargs_arg = check_arguments(adata, verbose = True, exp_key=exp_key, vkey = vkey, basis=basis, graph_method=graph_method)
+    exp_key,vkey,basis = kwargs_arg['exp_key'],kwargs_arg['vkey'],kwargs_arg['basis']
     
-    exp_2d_key = 'X_%s' % basis
-    vel_2d_key = 'velocity_%s' % basis
+    exp_2d_key_ = 'X_%s' % basis
+    vel_2d_key_ = '%s_%s' % (vkey,basis)
     pot_vkey_ = '%s_%s' % (potential_vkey,basis)
     rot_vkey_ = '%s_%s' % (rotation_vkey,basis)
     
     if exp_key == None:
         if scipy.sparse.issparse(adata.X):
             exp_HD = adata.X.toarray()
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
         exp_HD = adata.obsm[exp_key]
     else:
         exp_HD = adata.layers[exp_key]
     
-    vel_HD = adata.obsm[vel_key] if vel_key in adata.obsm.keys() else adata.layers[vel_key]
+    vel_HD = adata.obsm[vkey] if vkey in adata.obsm.keys() else adata.layers[vkey]
     if logscale_vel:
         vel_HD = (adata.obs['n_counts'].values*vel_HD.T).T/np.exp(exp_HD)
-    exp_LD = adata.obsm[exp_2d_key][:,:2] if exp_2d_key in adata.obsm.keys() else adata.layers[exp_2d_key][:,:2]
-    vel_LD = adata.obsm[vel_2d_key][:,:2] if vel_2d_key in adata.obsm.keys() else adata.layers[vel_2d_key][:,:2]
+    exp_LD = adata.obsm[exp_2d_key_][:,:2] if exp_2d_key_ in adata.obsm.keys() else adata.layers[exp_2d_key_][:,:2]
+    vel_LD = adata.obsm[vel_2d_key_][:,:2] if vel_2d_key_ in adata.obsm.keys() else adata.layers[vel_2d_key_][:,:2]
     
     ## Compute graph and edge velocities
     n_node_ = exp_HD.shape[0]
     if graph_method == 'Delauney':
         tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
         source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
     elif graph_method == 'knn':
@@ -251,17 +251,21 @@
         source = np.ravel(np.repeat(np.arange(exp_HD.shape[0]).reshape((-1, 1)),n_neighbors,axis=1))
         target = np.ravel(indices)
     
     if HD_rate > 0:
         idx_vel_HD = np.isnan(vel_HD[0])==False
         X1,X2 = exp_HD[:,idx_vel_HD][source],exp_HD[:,idx_vel_HD][target]
         V1,V2 = vel_HD[:,idx_vel_HD][source],vel_HD[:,idx_vel_HD][target]
+        V1_p,V2_p = V1*(X2-X1),V2*(X2-X1)
+        V1_p[V1_p<0] = 0
+        V2_p[V2_p<0] = 0
         Dis = np.linalg.norm(X2-X1,axis=1)
         Dis[Dis==0] = 1
-        edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis/np.sum(idx_vel_HD)
+        # edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis/np.sum(idx_vel_HD)
+        edge_vel_HD = np.sum(0.5*(V1_p+V2_p),axis=1)/Dis/np.sum(idx_vel_HD)
         # edge_vel_HD = np.sum(0.5*(V1+V2)*(X2-X1),axis=1)/Dis
         edge_vel_HD_norm = np.linalg.norm(edge_vel_HD)
         if edge_vel_HD_norm > 0: edge_vel_HD = edge_vel_HD/edge_vel_HD_norm
     else:
         edge_vel_HD = 0
     
     if HD_rate < 1:
@@ -303,25 +307,25 @@
             idx_s = source == i
             idx_t = target == i
             ex_s = -(exp_LD[source[idx_s]]-exp_LD[target[idx_s]])/np.linalg.norm(exp_LD[source[idx_s]]-exp_LD[target[idx_s]],ord=2)
             ex_t = -(exp_LD[target[idx_t]]-exp_LD[source[idx_t]])/np.linalg.norm(exp_LD[target[idx_t]]-exp_LD[source[idx_t]],ord=2)
             vel_potential[i] = 2*(np.sum((adata.obs[potential_key][source[idx_s]].values-adata.obs[potential_key][target[idx_s]].values)*ex_s.T,axis=1) + \
                                 np.sum((adata.obs[potential_key][target[idx_t]].values-adata.obs[potential_key][source[idx_t]].values)*ex_t.T,axis=1))
         adata.obsm[pot_vkey_] = vel_potential
-        adata.obsm[rot_vkey_]  = adata.obsm[pot_vkey_]-vel_potential
+        adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
     elif graph_method == 'knn':
         knn = sklearn.neighbors.NearestNeighbors(n_neighbors=n_neighbors+1, algorithm='kd_tree')
         knn.fit(exp_LD)
         distances, indices = knn.kneighbors(exp_LD)
         distances, indices = distances[:,1:], indices[:,1:]
         for i in range(adata.shape[0]):
             ex_s = (exp_LD[indices[i]]-exp_LD[i])/np.linalg.norm(exp_LD[indices[i]]-exp_LD[i],ord=2)
             vel_potential[i] = -2*np.sum((adata.obs[potential_key].values[indices[i]]-adata.obs[potential_key].values[i])*ex_s.T,axis=1)
         adata.obsm[pot_vkey_] = vel_potential
-        adata.obsm[rot_vkey_]  = adata.obsm[pot_vkey_]-vel_potential
+        adata.obsm[rot_vkey_] = adata.obsm[vel_2d_key_]-vel_potential
 
     ## Contribution ratio
     log_ = {}
     log_["Contribution_ratio"] = {}
     norm_grad = np.linalg.norm(pot_flow)
     norm_curl = np.linalg.norm(rot_flow)
     log_["Contribution_ratio"]['Potential'] = '{:.2%}'.format(norm_grad/(norm_grad+norm_curl))
@@ -330,60 +334,64 @@
     if verbose: print(adata.uns['CellMap_log'])
 
     if graph_key not in adata.uns.keys(): adata.uns[graph_key] = np.vstack((source,target))
 
 def Hodge_decomposition_genes(
     adata,
     genes,
+    basis = 'umap',
+    vkey  = 'velocity',
     exp_key = None,
-    vel_key  = 'velocity',
-    exp_2d_key = 'X_umap',
-    vel_2d_key = 'velocity_umap',
     potential_key = 'Hodge_potential',
+    potential_vkey = 'potential_velocity',
     rotation_key = 'Hodge_rotation',
+    rotation_vkey = 'rotation_velocity',
     graph_key = 'CM_graph',
     graph_method = 'Delauney',
-    alpha = 0.2,
+    HD_rate = 0.2,
     n_neighbors = 10,
-    contribution_rate = 0.95,
+    contribution_rate_pca = 0.95,
     cutedge_vol  = None,
     cutedge_length = None,
     verbose = True,
-    use_HVG = True,
     logscale_vel = True,
-    n_HVG = 10,
     ):
     """
     Hodge decomposition
 
     Parameters
     ----------
     adata: anndata (n_samples, n_features)
     
     exp_key: None or string
     """
     
-    kwargs_arg = check_arguments(adata, exp_key=exp_key, vel_key = vel_key, exp_2d_key=exp_2d_key, vel_2d_key=vel_2d_key, graph_method=graph_method)
-    exp_key,vel_key,exp_2d_key,vel_2d_key = kwargs_arg['exp_key'],kwargs_arg['vel_key'],kwargs_arg['exp_2d_key'],kwargs_arg['vel_2d_key']
+    kwargs_arg = check_arguments(adata, verbose = True, exp_key=exp_key, vkey = vkey, basis=basis, graph_method=graph_method)
+    exp_key,vkey,basis = kwargs_arg['exp_key'],kwargs_arg['vkey'],kwargs_arg['basis']
+    
+    exp_2d_key_ = 'X_%s' % basis
+    vel_2d_key_ = '%s_%s' % (vkey,basis)
+    pot_vkey_ = '%s_%s' % (potential_vkey,basis)
+    rot_vkey_ = '%s_%s' % (rotation_vkey,basis)
     
     
     if exp_key == None:
         if scipy.sparse.issparse(adata.X):
             exp_HD = adata.X.toarray()
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
         exp_HD = adata.obsm[exp_key]
     else:
         exp_HD = adata.layers[exp_key]
     
-    vel_HD = adata.obsm[vel_key] if vel_key in adata.obsm.keys() else adata.layers[vel_key]
+    vel_HD = adata.obsm[vkey] if vkey in adata.obsm.keys() else adata.layers[vkey]
     if logscale_vel:
         vel_HD = (1e+4*vel_HD.T/adata.obs['n_counts'].values).T/np.power(2,exp_HD)
-    exp_LD = adata.obsm[exp_2d_key][:,:2] if exp_2d_key in adata.obsm.keys() else adata.layers[exp_2d_key][:,:2]
+    exp_LD = adata.obsm[exp_2d_key_][:,:2] if exp_2d_key_ in adata.obsm.keys() else adata.layers[exp_2d_key_][:,:2]
     
     n_node_ = exp_HD.shape[0]
     if graph_method == 'Delauney':
         tri_,idx_tri = create_graph(exp_LD[:,0],exp_LD[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
         source, target = np.ravel(tri_.triangles[idx_tri][:,[0,1,2]]),np.ravel(tri_.triangles[idx_tri][:,[1,2,0]])
     elif graph_method == 'knn':
         pca = sklearn.decomposition.PCA()
@@ -588,14 +596,15 @@
     basis = 'umap',
     vkey = 'velocity',
     potential_vkey = 'potential_velocity',
     rotation_vkey = 'rotation_velocity',
     cluster_key='clusters',
     alpha=0.3,
     fontsize = 18,
+    scale=1,
     **kwargs
     ):
     
     kwargs_arg = check_arguments(adata,basis = basis)
     basis = kwargs_arg['basis']
     basis_key = 'X_%s' % basis
     vkey_ = '%s_%s' % (vkey,basis)
@@ -610,30 +619,30 @@
     fig,ax = plt.subplots(1,3,figsize=(24,8),tight_layout=True)
     for i in range(3):
         for j in range(len(cluster_set)):
             idx = adata.obs[cluster_key] == cluster_set[j]
             ax[i].scatter(adata.obsm[basis_key][idx,0],adata.obsm[basis_key][idx,1],s=200,alpha=alpha,label=cluster_set[j],color=cmap(j),zorder=0)
             ax[i].text(np.mean(adata.obsm[basis_key][idx,0]),np.mean(adata.obsm[basis_key][idx,1]),cluster_set[j],fontsize=fontsize,
                        ha='center',va='center',weight='bold')
-    ax[0].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[vkey_][:,0],adata.obsm[vkey_][:,1],scale=1,zorder=1)
+    ax[0].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[vkey_][:,0],adata.obsm[vkey_][:,1],scale=scale,zorder=1,**kwargs)
     ax[0].set_title('RNA velocity',fontsize=fontsize)
     ax[0].axis('off')
-    ax[1].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[pot_vkey_][:,0],adata.obsm[pot_vkey_][:,1],scale=1,zorder=1,**kwargs)
+    ax[1].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[pot_vkey_][:,0],adata.obsm[pot_vkey_][:,1],scale=scale,zorder=1,**kwargs)
     ax[1].set_title('Potential flow',fontsize=fontsize)
     ax[1].axis('off')
-    ax[2].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[rot_vkey_][:,0],adata.obsm[rot_vkey_][:,1],scale=1,zorder=1,**kwargs)
+    ax[2].quiver(adata.obsm[basis_key][:,0],adata.obsm[basis_key][:,1],adata.obsm[rot_vkey_][:,0],adata.obsm[rot_vkey_][:,1],scale=scale,zorder=1,**kwargs)
     ax[2].set_title('Rotational flow',fontsize=fontsize)
     ax[2].axis('off')
 
 def view_surface_genes(
     adata,
     genes,
     exp_key = None,
     basis = 'umap',
-    vel_key  = 'velocity',
+    vkey  = 'velocity',
     potential_key = 'Hodge_potential',
     graph_key = 'CM_graph',
     cluster_key = None,
     show_graph = False,
     cutedge_vol  = None,
     cutedge_length = None,
     logscale_vel = True,
@@ -654,15 +663,15 @@
         else:
             exp_HD = adata.X
     elif exp_key in adata.obsm.keys():
         exp_HD = adata.obsm[exp_key]
     else:
         exp_HD = adata.layers[exp_key]
     
-    vel_HD = adata.obsm[vel_key] if vel_key in adata.obsm.keys() else adata.layers[vel_key]
+    vel_HD = adata.obsm[vkey] if vkey in adata.obsm.keys() else adata.layers[vkey]
     if logscale_vel:
         vel_HD = (1e+4*vel_HD.T/adata.obs['n_counts'].values).T/np.power(2,exp_HD)
     if 'cmap' not in kwargs:
         kwargs['cmap'] = cmap_earth(adata.obs[potential_key])
     
     data_pos = adata.obsm[basis_key]
     tri_ = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length)
@@ -899,15 +908,15 @@
         graph_[tuple(triangles[weight<-min_weight][:,[id_y,id_x]].T[::-1])] = 1
     return scipy.sparse.coo_matrix(graph_)
 
 
 def create_dgraph(
     adata,
     basis = 'umap',
-    vel_key  = 'velocity',
+    vkey  = 'velocity',
     cutedge_vol  = None,
     cutedge_length = None,
     ):
     """
     Hodge decomposition
 
     Parameters
@@ -915,22 +924,22 @@
     adata: anndata (n_samples, n_features)
     
     basis: ndarray or string
     """
     
     kwargs_arg = check_arguments(adata,
                              basis = basis,
-                             vel_key = vel_key,
+                             vkey = vkey,
                              map_key = map_key
                             )
-    basis,vel_key,map_key = kwargs_arg['basis'],kwargs_arg['vel_key'],kwargs_arg['map_key']
+    basis,vkey,map_key = kwargs_arg['basis'],kwargs_arg['vkey'],kwargs_arg['map_key']
     basis_key = 'X_%s' % basis
     
     data_pos = adata.obsm[basis_key]
-    data_vel = adata.obsm['%s_%s' % (vel_key,basis)]
+    data_vel = adata.obsm['%s_%s' % (vkey,basis)]
     triangles = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length).triangles
     tri_,idx_tri = create_graph(data_pos[:,0],data_pos[:,1],cutedge_vol=cutedge_vol,cutedge_length=cutedge_length,return_mask = True)
     triangles = tri_.triangles[idx_tri]
     n_node_ = data_pos.shape[0]
     graph_ = scipy.sparse.lil_matrix(np.zeros([n_node_,n_node_]))
     idx_set = [[0,1],[1,2],[2,0]]
     idx = np.isnan(data_vel[0])==False
```

## Comparing `cellmap-1.0.1.dev202304120506.dist-info/METADATA` & `cellmap-1.0.1.dev202304120630.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304120506
+Version: 1.0.1.dev202304120630
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

