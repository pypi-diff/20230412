# Comparing `tmp/deepchem-2.7.2.dev20230411091951.tar.gz` & `tmp/deepchem-2.7.2.dev20230412020314.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230411091951.tar", last modified: Tue Apr 11 09:19:51 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230412020314.tar", last modified: Wed Apr 12 02:03:15 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230411091951.tar` & `deepchem-2.7.2.dev20230412020314.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.942061 deepchem-2.7.2.dev20230411091951/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 09:19:51.942061 deepchem-2.7.2.dev20230411091951/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.910060 deepchem-2.7.2.dev20230411091951/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.910060 deepchem-2.7.2.dev20230411091951/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67590 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.910060 deepchem-2.7.2.dev20230411091951/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.914060 deepchem-2.7.2.dev20230411091951/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.914060 deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.914060 deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.918060 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.918060 deepchem-2.7.2.dev20230411091951/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.918060 deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.918060 deepchem-2.7.2.dev20230411091951/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.918060 deepchem-2.7.2.dev20230411091951/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.918060 deepchem-2.7.2.dev20230411091951/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.922060 deepchem-2.7.2.dev20230411091951/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.922060 deepchem-2.7.2.dev20230411091951/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.922060 deepchem-2.7.2.dev20230411091951/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.922060 deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.922060 deepchem-2.7.2.dev20230411091951/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    36276 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.922060 deepchem-2.7.2.dev20230411091951/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.926061 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.930061 deepchem-2.7.2.dev20230411091951/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.934061 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.934061 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.934061 deepchem-2.7.2.dev20230411091951/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.934061 deepchem-2.7.2.dev20230411091951/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.934061 deepchem-2.7.2.dev20230411091951/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.934061 deepchem-2.7.2.dev20230411091951/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.938061 deepchem-2.7.2.dev20230411091951/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.942061 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:51.910060 deepchem-2.7.2.dev20230411091951/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 09:19:51.000000 deepchem-2.7.2.dev20230411091951/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-11 09:19:51.000000 deepchem-2.7.2.dev20230411091951/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:19:51.000000 deepchem-2.7.2.dev20230411091951/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-11 09:19:51.000000 deepchem-2.7.2.dev20230411091951/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 09:19:51.000000 deepchem-2.7.2.dev20230411091951/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-11 09:19:51.942061 deepchem-2.7.2.dev20230411091951/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-11 09:19:41.000000 deepchem-2.7.2.dev20230411091951/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.285747 deepchem-2.7.2.dev20230412020314/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-12 02:03:00.000000 deepchem-2.7.2.dev20230412020314/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 02:03:15.285747 deepchem-2.7.2.dev20230412020314/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-12 02:03:00.000000 deepchem-2.7.2.dev20230412020314/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.237743 deepchem-2.7.2.dev20230412020314/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.241744 deepchem-2.7.2.dev20230412020314/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67590 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.241744 deepchem-2.7.2.dev20230412020314/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.241744 deepchem-2.7.2.dev20230412020314/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.245744 deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.245744 deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.245744 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.245744 deepchem-2.7.2.dev20230412020314/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.249744 deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.249744 deepchem-2.7.2.dev20230412020314/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.249744 deepchem-2.7.2.dev20230412020314/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.249744 deepchem-2.7.2.dev20230412020314/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.253744 deepchem-2.7.2.dev20230412020314/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.253744 deepchem-2.7.2.dev20230412020314/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.253744 deepchem-2.7.2.dev20230412020314/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.253744 deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.253744 deepchem-2.7.2.dev20230412020314/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39719 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.253744 deepchem-2.7.2.dev20230412020314/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.261745 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.261745 deepchem-2.7.2.dev20230412020314/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.269746 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.269746 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.269746 deepchem-2.7.2.dev20230412020314/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.269746 deepchem-2.7.2.dev20230412020314/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.273746 deepchem-2.7.2.dev20230412020314/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.273746 deepchem-2.7.2.dev20230412020314/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.277746 deepchem-2.7.2.dev20230412020314/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.285747 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:03:15.237743 deepchem-2.7.2.dev20230412020314/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 02:03:15.000000 deepchem-2.7.2.dev20230412020314/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-12 02:03:15.000000 deepchem-2.7.2.dev20230412020314/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:03:15.000000 deepchem-2.7.2.dev20230412020314/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 02:03:15.000000 deepchem-2.7.2.dev20230412020314/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 02:03:15.000000 deepchem-2.7.2.dev20230412020314/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-12 02:03:15.285747 deepchem-2.7.2.dev20230412020314/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-12 02:03:01.000000 deepchem-2.7.2.dev20230412020314/setup.py
```

### Comparing `deepchem-2.7.2.dev20230411091951/LICENSE` & `deepchem-2.7.2.dev20230412020314/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/PKG-INFO` & `deepchem-2.7.2.dev20230412020314/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230411091951
+Version: 2.7.2.dev20230412020314
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230411091951/README.md` & `deepchem-2.7.2.dev20230412020314/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230412020314/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230412020314/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230412020314/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230412020314/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230412020314/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230412020314/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230412020314/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230412020314/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230412020314/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230412020314/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230412020314/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230412020314/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230412020314/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230412020314/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230412020314/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/losses.py`

 * *Files 9% similar despite different names*

```diff
@@ -905,14 +905,81 @@
             # return overall_loss, av_loss, bv_loss, fg_loss, av_dist_loss, bv_dist_loss, fg_dist_loss
             # We just return overall_loss since TorchModel can handle only a single loss
             return overall_loss
 
         return loss
 
 
+class EdgePredictionLoss(Loss):
+    """
+    EdgePredictionLoss is an unsupervised graph edge prediction loss function that calculates the loss based on the similarity between node embeddings for positive and negative edge pairs. This loss function is designed for graph neural networks and is particularly useful for pre-training tasks.
+
+    This loss function encourages the model to learn node embeddings that can effectively distinguish between true edges (positive samples) and false edges (negative samples) in the graph.
+
+    The loss is computed by comparing the similarity scores (dot product) of node embeddings for positive and negative edge pairs. The goal is to maximize the similarity for positive pairs and minimize it for negative pairs.
+
+    To use this loss function, the input must be a BatchGraphData object transformed by the negative_edge_sampler. The loss function takes the node embeddings and the input graph data (with positive and negative edge pairs) as inputs and returns the edge prediction loss.
+
+    Examples
+    --------
+    >>> from deepchem.models.losses import EdgePredictionLoss
+    >>> from deepchem.feat.graph_data import BatchGraphData, GraphData
+    >>> from deepchem.models.torch_models.gnn import negative_edge_sampler
+    >>> import torch
+    >>> import numpy as np
+    >>> emb_dim = 8
+    >>> num_nodes_list, num_edge_list = [3, 4, 5], [2, 4, 5]
+    >>> num_node_features, num_edge_features = 32, 32
+    >>> edge_index_list = [
+    ...     np.array([[0, 1], [1, 2]]),
+    ...     np.array([[0, 1, 2, 3], [1, 2, 0, 2]]),
+    ...     np.array([[0, 1, 2, 3, 4], [1, 2, 3, 4, 0]]),
+    ... ]
+    >>> graph_list = [
+    ...     GraphData(node_features=np.random.random_sample(
+    ...         (num_nodes_list[i], num_node_features)),
+    ...               edge_index=edge_index_list[i],
+    ...               edge_features=np.random.random_sample(
+    ...                   (num_edge_list[i], num_edge_features)),
+    ...               node_pos_features=None) for i in range(len(num_edge_list))
+    ... ]
+    >>> batched_graph = BatchGraphData(graph_list)
+    >>> batched_graph = batched_graph.numpy_to_torch()
+    >>> neg_sampled = negative_edge_sampler(batched_graph)
+    >>> embedding = np.random.random((sum(num_nodes_list), emb_dim))
+    >>> embedding = torch.from_numpy(embedding)
+    >>> loss_func = EdgePredictionLoss()._create_pytorch_loss()
+    >>> loss = loss_func(embedding, neg_sampled)
+
+    References
+    ----------
+    .. [1] Hu, W. et al. Strategies for Pre-training Graph Neural Networks. Preprint at https://doi.org/10.48550/arXiv.1905.12265 (2020).
+    """
+
+    def _create_pytorch_loss(self):
+        import torch
+        self.criterion = torch.nn.BCEWithLogitsLoss()
+
+        def loss(node_emb, inputs):
+            positive_score = torch.sum(node_emb[inputs.edge_index[0, ::2]] *
+                                       node_emb[inputs.edge_index[1, ::2]],
+                                       dim=1)
+            negative_score = torch.sum(node_emb[inputs.negative_edge_index[0]] *
+                                       node_emb[inputs.negative_edge_index[1]],
+                                       dim=1)
+
+            edge_pred_loss = self.criterion(
+                positive_score,
+                torch.ones_like(positive_score)) + self.criterion(
+                    negative_score, torch.zeros_like(negative_score))
+            return edge_pred_loss
+
+        return loss
+
+
 def _make_tf_shapes_consistent(output, labels):
     """Try to make inputs have the same shape by adding dimensions of size 1."""
     import tensorflow as tf
     shape1 = output.shape
     shape2 = labels.shape
     len1 = len(shape1)
     len2 = len(shape2)
```

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/models.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/gnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import torch
 from torch_geometric.nn import GINEConv, global_add_pool, global_mean_pool, global_max_pool
 from torch_geometric.nn.aggr import AttentionalAggregation, Set2Set
 from torch.functional import F
+from deepchem.data import Dataset
+from deepchem.models.losses import SoftmaxCrossEntropy, EdgePredictionLoss
 from deepchem.models.torch_models import ModularTorchModel
 from deepchem.feat.graph_data import BatchGraphData
+from typing import Iterable, List, Tuple
+from deepchem.metrics import to_one_hot
 
 num_atom_type = 120
 num_chirality_tag = 3
 # Relevant in future PRs
 # num_bond_type = 6
 # num_bond_direction = 3
 
@@ -48,18 +52,18 @@
     >>> from deepchem.models.torch_models.gnn import GNNModular
     >>> from deepchem.feat.graph_data import BatchGraphData
     >>> from deepchem.feat.molecule_featurizers import SNAPFeaturizer
     >>> featurizer = SNAPFeaturizer()
     >>> smiles = ["C1=CC=CC=C1", "C1=CC=CC=C1C=O", "C1=CC=CC=C1C(=O)O"]
     >>> features = featurizer.featurize(smiles)
     >>> batched_graph = BatchGraphData(features).numpy_to_torch(device="cuda")
-    >>> modular = model = GNNModular("gin", 3, 64, 1, "attention", 0, "last", "edge_pred")
+    >>> modular = GNNModular(emb_dim = 8, task = "edge_pred")
     >>> gnnmodel = modular.gnn
     >>> print(gnnmodel(batched_graph)[0].shape)
-    torch.Size([23, 64])
+    torch.Size([23, 32])
 
     """
 
     def __init__(self,
                  atom_type_embedding,
                  chirality_embedding,
                  gconvs,
@@ -105,27 +109,27 @@
             if i == self.num_layer - 1:
                 # remove relu for the last layer
                 h = F.dropout(h, self.dropout, training=self.training)
             else:
                 h = F.dropout(F.relu(h), self.dropout, training=self.training)
             h_list.append(h)
 
-        # Different implementations of JK
+        # Different implementations of jump_knowledge
         if self.jump_knowledge == "concat":
             node_representation = torch.cat(h_list, dim=1)
         elif self.jump_knowledge == "last":
             node_representation = h_list[-1]
         elif self.jump_knowledge == "max":
             h_list = [h.unsqueeze_(0) for h in h_list]
             node_representation = torch.max(torch.cat(h_list, dim=0), dim=0)[0]
         elif self.jump_knowledge == "sum":
             h_list = [h.unsqueeze_(0) for h in h_list]
             node_representation = torch.sum(torch.cat(h_list, dim=0), dim=0)[0]
 
-        return node_representation, data
+        return (node_representation, data)
 
 
 class GNNHead(torch.nn.Module):
     """
     Prediction head module for the GNNModular model.
 
     Parameters
@@ -138,33 +142,39 @@
         The type of task. Must be one of "regression", "classification".
     num_tasks: int
         Number of tasks.
     num_classes: int
         Number of classes for classification.
     """
 
-    def __init__(self, pool, head):
+    def __init__(self, pool, head, task, num_tasks, num_classes):
         super().__init__()
         self.pool = pool
         self.head = head
+        self.task = task
+        self.num_tasks = num_tasks
+        self.num_classes = num_classes
 
-    def forward(self, node_representation, data):
+    def forward(self, data):
         """
         Forward pass for the GNN head module.
 
         Parameters
         ----------
-        node_representation: torch.Tensor
-            The node representations after passing through the GNN layers.
-        data: BatchGraphData
-            The original input graph data.
+        data: tuple
+            A tuple containing the node representations and the input graph data.
+            node_representation is a torch.Tensor created after passing input through the GNN layers.
+            input_batch is the original input BatchGraphData.
         """
+        node_representation, input_batch = data
 
-        pooled = self.pool(node_representation, data.graph_index)
+        pooled = self.pool(node_representation, input_batch.graph_index)
         out = self.head(pooled)
+        if self.task == "classification":
+            out = torch.reshape(out, (-1, self.num_tasks, self.num_classes))
         return out
 
 
 class GNNModular(ModularTorchModel):
     """
     Modular GNN which allows for easy swapping of GNN layers.
 
@@ -211,28 +221,40 @@
     """
 
     def __init__(self,
                  gnn_type: str = "gin",
                  num_layer: int = 3,
                  emb_dim: int = 64,
                  num_tasks: int = 1,
+                 num_classes: int = 2,
                  graph_pooling: str = "attention",
                  dropout: int = 0,
                  jump_knowledge: str = "concat",
                  task: str = "edge_pred",
                  **kwargs):
         self.gnn_type = gnn_type
         self.num_layer = num_layer
         self.emb_dim = emb_dim
+
         self.num_tasks = num_tasks
+        self.num_classes = num_classes
+        if task == "classification":
+            self.output_dim = num_classes * num_tasks
+            self.criterion = SoftmaxCrossEntropy()._create_pytorch_loss()
+        elif task == "regression":
+            self.output_dim = num_tasks
+            self.criterion = F.mse_loss
+        elif task == "edge_pred":
+            self.output_dim = num_tasks
+            self.edge_pred_loss = EdgePredictionLoss()._create_pytorch_loss()
+
         self.graph_pooling = graph_pooling
         self.dropout = dropout
         self.jump_knowledge = jump_knowledge
         self.task = task
-        self.criterion = torch.nn.BCEWithLogitsLoss()
 
         self.components = self.build_components()
         self.model = self.build_model()
         super().__init__(self.model, self.components, **kwargs)
 
     def build_components(self):
         """
@@ -298,17 +320,17 @@
         if self.graph_pooling == "set2set":
             mult = 2
         else:
             mult = 1
 
         if self.jump_knowledge == "concat":
             head = torch.nn.Linear(mult * (self.num_layer + 1) * self.emb_dim,
-                                   self.num_tasks)
+                                   self.output_dim)
         else:
-            head = torch.nn.Linear(mult * self.emb_dim, self.num_tasks)
+            head = torch.nn.Linear(mult * self.emb_dim, self.output_dim)
 
         components = {
             'atom_type_embedding':
                 torch.nn.Embedding(num_atom_type, self.emb_dim),
             'chirality_embedding':
                 torch.nn.Embedding(num_chirality_tag, self.emb_dim),
             'gconvs':
@@ -320,58 +342,57 @@
             'head':
                 head
         }
         self.gnn = GNN(components['atom_type_embedding'],
                        components['chirality_embedding'], components['gconvs'],
                        components['batch_norms'], self.dropout,
                        self.jump_knowledge)
-        self.gnn_head = GNNHead(components['pool'], components['head'])
+        self.gnn_head = GNNHead(components['pool'], components['head'],
+                                self.task, self.num_tasks, self.num_classes)
         return components
 
     def build_model(self):
         """
         Builds the appropriate model based on the specified task.
 
         For the edge prediction task, the model is simply the GNN module because it is an unsupervised task and does not require a prediction head.
 
         Supervised tasks such as node classification and graph regression require a prediction head, so the model is a sequential module consisting of the GNN module followed by the GNN_head module.
         """
 
         if self.task == "edge_pred":  # unsupervised task, does not need pred head
             return self.gnn
-        else:
+        elif self.task in ("regression", "classification"):
             return torch.nn.Sequential(self.gnn, self.gnn_head)
+        else:
+            raise ValueError(f"Task {self.task} is not supported.")
 
     def loss_func(self, inputs, labels, weights):
         """
         The loss function executed in the training loop, which is based on the specified task.
         """
         if self.task == "edge_pred":
-            return self.edge_pred_loss(inputs, labels, weights)
-
-    def edge_pred_loss(self, inputs, labels, weights):
-        """
-        The loss function for the graph edge prediction task.
-
-        The inputs in this loss must be a BatchGraphData object transformed by the NegativeEdge molecule feature utility.
-        """
-        node_emb, _ = self.model(
-            inputs)  # node_emb shape == [num_nodes x emb_dim]
-
-        positive_score = torch.sum(node_emb[inputs.edge_index[0, ::2]] *
-                                   node_emb[inputs.edge_index[1, ::2]],
-                                   dim=1)
-        negative_score = torch.sum(node_emb[inputs.negative_edge_index[0]] *
-                                   node_emb[inputs.negative_edge_index[1]],
-                                   dim=1)
-
-        loss = self.criterion(
-            positive_score, torch.ones_like(positive_score)) + self.criterion(
-                negative_score, torch.zeros_like(negative_score))
-        return (loss * weights[0]).mean()
+            node_emb, inputs = self.model(inputs)
+            loss = self.edge_pred_loss(node_emb, inputs)
+        elif self.task == "regression":
+            loss = self.regression_loss(inputs, labels)
+        elif self.task == "classification":
+            loss = self.classification_loss(inputs, labels)
+        return (loss * weights).mean()
+
+    def regression_loss(self, inputs, labels):
+        out = self.model(inputs)
+        reg_loss = self.criterion(out, labels)
+        return reg_loss
+
+    def classification_loss(self, inputs, labels):
+        out = self.model(inputs)
+        out = F.softmax(out, dim=2)
+        class_loss = self.criterion(out, labels)
+        return class_loss
 
     def _prepare_batch(self, batch):
         """
         Prepares the batch for the model by converting the GraphData numpy arrays to BatchedGraphData torch tensors and moving them to the device, then transforming the input to the appropriate format for the task.
 
         Parameters
         ----------
@@ -396,14 +417,35 @@
 
         if (len(labels) != 0) and (len(weights) != 0):
             labels = labels[0]
             weights = weights[0]
 
         return inputs, labels, weights
 
+    def default_generator(
+            self,
+            dataset: Dataset,
+            epochs: int = 1,
+            mode: str = 'fit',
+            deterministic: bool = True,
+            pad_batches: bool = True) -> Iterable[Tuple[List, List, List]]:
+        """
+        This default generator is modified from the default generator in dc.models.tensorgraph.tensor_graph.py to support multitask classification. If the task is classification, the labels y_b are converted to a one-hot encoding and reshaped according to the number of tasks and classes.
+        """
+
+        for epoch in range(epochs):
+            for (X_b, y_b, w_b,
+                 ids_b) in dataset.iterbatches(batch_size=self.batch_size,
+                                               deterministic=deterministic,
+                                               pad_batches=pad_batches):
+                if self.task == 'classification' and y_b is not None:
+                    y_b = to_one_hot(y_b.flatten(), self.num_classes).reshape(
+                        -1, self.num_tasks, self.num_classes)
+                yield ([X_b], [y_b], [w_b])
+
 
 def negative_edge_sampler(data: BatchGraphData):
     """
     NegativeEdge is a function that adds negative edges to the input graph data. It randomly samples negative edges (edges that do not exist in the original graph) and adds them to the input graph data.
     The number of negative edges added is equal to half the number of edges in the original graph. This is useful for tasks like edge prediction, where the model needs to learn to differentiate between existing and non-existing edges.
 
     Parameters
```

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230412020314/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230412020314/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230412020314/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230412020314/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230412020314/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230412020314/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230412020314/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230412020314/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230412020314/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230412020314/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230412020314/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230411091951
+Version: 2.7.2.dev20230412020314
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230411091951/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230412020314/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/setup.cfg` & `deepchem-2.7.2.dev20230412020314/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230411091951/setup.py` & `deepchem-2.7.2.dev20230412020314/setup.py`

 * *Files identical despite different names*

