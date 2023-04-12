# Comparing `tmp/ipydrawio-mathjax-1.2.2.tar.gz` & `tmp/ipydrawio-mathjax-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipydrawio-mathjax-1.2.2.tar", last modified: Tue Nov  8 14:39:15 2022, max compression
+gzip compressed data, was "ipydrawio-mathjax-1.3.0.tar", last modified: Tue Apr 11 21:51:00 2023, max compression
```

## Comparing `ipydrawio-mathjax-1.2.2.tar` & `ipydrawio-mathjax-1.3.0.tar`

### file list

```diff
@@ -1,267 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2262 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/_/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.387107 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/0105afb2a7b1cb48786a.js
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/01469e75839bfe3b3ea2.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/05c8c84c55e4ca878d75.js
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/0c41a0e14993bf9b20b0.js
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/13ce6053d320a2f64a91.woff
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/1a232c5da5da0c37d68f.js
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/1a477f517908731b09d9.woff
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/1b3b2a6e8e3f5c268a18.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/1ba2702b534636b4c952.json
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/1f0ab91aad9a7eb0a172.js
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/22646e62c22f8063eb42.woff
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/23a843f419122319cd9d.js
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/24957464d4cff9554f73.js
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/25e1367d3691f645c8bc.woff
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/2613b5b1da6a860bd53d.json
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/27d385ccf2f4ea7008f4.js
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/297fd0f2e5e05a4c3084.js
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/299228230cfccc0b8f0c.woff
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/2ad11906aa6ee804ee8e.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/2bbaf7e49edc89f3838c.json
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/35345eb9b2212be313e0.woff
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/3751cbd01fd90a4afe57.js
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/39bf15c765b08ae85b12.js
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/3a020ff978296a1cdd1b.js
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/3a7f99cb9d515034bb6c.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/3f5a4f4c715413f84537.js
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/3f857597b016cafd0b3e.woff
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/40708d53def0402dd528.json
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/446e5c8b02734312f3fc.js
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/46ddbbade4b8b1a8db9c.js
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/474850fe2e03410434a1.woff
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/480.3f50ce7358e02e2ef38b.js
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/4a494eedd8fc00eaafd7.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/4afd3bf2bc0ed1f42e8a.json
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/4b3395175f9e53a548c0.woff
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/54a37771d1dd11e353d5.js
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/560b148048d4008d044c.woff
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/568.7226bc506cb1dc5c99c7.js
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/58c102189b297eb4464f.js
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/5b8bda2222239e331bdf.js
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/5d115f578491d9cc141b.json
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/5e2495e69252853d5cfc.js
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/5f41784627299ade1edb.js
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/62696a7f39d413bd9627.woff
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/6344bfadbad62079ecc8.json
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/692e6db1b2c51cc55375.json
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/69987877f7e1acc37a5a.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/6bb8ecb25b0058d55085.json
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/6e147198914185dcafb0.woff
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/6f692024f3b5acd65f50.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/7016fb9e84037c36f872.json
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/70efd429a87509bc539c.js
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/7167e618c0b4bf456bab.js
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/727d6ab819bf2176a997.js
--rw-r--r--   0 runner    (1001) docker     (121)    25664 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/799.edc688f162b17cb84c84.js
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/7c908ef0e17849b942d2.woff
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/83e5ee6851b26a27999c.js
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/873f01ea7bb5fd439fb6.js
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/9111db760ee9c385d639.woff
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/951da76598f17b4929ff.woff
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/994270bdcba004153f9f.woff
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/9a486c5aea255bd7a495.woff
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/9ba44918776a7dedbab5.js
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/a00cd7232feaabf5bec3.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/a77db5a8a2ba17b432cd.json
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/a8677266500942fdad59.js
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ac037a6239911775cb0f.js
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ac0ec3a957245780bc87.js
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ac3678b875c9788b0ba8.js
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ac8c31b136c23d37af5b.js
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ad3ab81edad23a1a9a03.js
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ad95f6159a20b67d4dea.js
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/af06b9cab204027e6b8d.js
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/af45b01c70b757c28b00.js
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/af526d140a0fcfd0dbb7.js
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/b694016f93d93fb7ed7e.woff
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/b6e5e9fc75f074b7ba29.js
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/b90c7601b5b16f9e687e.js
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ba9736e904da2083bc88.js
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/bc22034776fbb4602766.js
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/bd73c9bdce1b564a034c.js
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/bdfb824546533e75cd55.woff
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/c433eff89a4a0cc3d6a0.js
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d09e363046fabceb7553.js
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d199b80c3dad1a721cac.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d21c6040db5534085cc4.json
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d3ce3863e49e333d5140.js
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d58529242e68f73984da.js
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d64c5b1829abb4116d04.js
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d6c5e65d60817508188e.js
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d705ea1e9f09e39aa938.woff
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/d7841a6907f74607a691.woff
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dad65891a048937689de.json
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dbbf84e2698ad2b20665.js
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dbd74f6f71046a665a45.js
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/de168eb349ee32238963.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.387107 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.403108 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.407108 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/assistive-mml.js
--rw-r--r--   0 runner    (1001) docker     (121)    18034 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/complexity.js
--rw-r--r--   0 runner    (1001) docker     (121)    36348 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/explorer.js
--rw-r--r--   0 runner    (1001) docker     (121)     8084 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/semantic-enrich.js
--rw-r--r--   0 runner    (1001) docker     (121)   337064 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/sre.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.407108 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/adaptors/
--rw-r--r--   0 runner    (1001) docker     (121)    22827 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/adaptors/liteDOM.js
--rw-r--r--   0 runner    (1001) docker     (121)   218533 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/core.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.407108 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/
--rw-r--r--   0 runner    (1001) docker     (121)   107781 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/asciimath.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.407108 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/
--rw-r--r--   0 runner    (1001) docker     (121)    51126 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/entities.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.407108 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)    28862 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.js
--rw-r--r--   0 runner    (1001) docker     (121)   199492 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.sef.json
--rw-r--r--   0 runner    (1001) docker     (121)    14583 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.415109 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/
--rw-r--r--   0 runner    (1001) docker     (121)     2611 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/action.js
--rw-r--r--   0 runner    (1001) docker     (121)   215178 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/all-packages.js
--rw-r--r--   0 runner    (1001) docker     (121)    29459 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/ams.js
--rw-r--r--   0 runner    (1001) docker     (121)     6769 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/amscd.js
--rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/autoload.js
--rw-r--r--   0 runner    (1001) docker     (121)     3006 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bbox.js
--rw-r--r--   0 runner    (1001) docker     (121)     4056 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/boldsymbol.js
--rw-r--r--   0 runner    (1001) docker     (121)     6729 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/braket.js
--rw-r--r--   0 runner    (1001) docker     (121)    18344 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bussproofs.js
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cancel.js
--rw-r--r--   0 runner    (1001) docker     (121)     7064 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cases.js
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/centernot.js
--rw-r--r--   0 runner    (1001) docker     (121)     8627 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/color.js
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colortbl.js
--rw-r--r--   0 runner    (1001) docker     (121)     1998 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colorv2.js
--rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/configmacros.js
--rw-r--r--   0 runner    (1001) docker     (121)    11100 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/empheq.js
--rw-r--r--   0 runner    (1001) docker     (121)     2387 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/enclose.js
--rw-r--r--   0 runner    (1001) docker     (121)     3451 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/extpfeil.js
--rw-r--r--   0 runner    (1001) docker     (121)     2104 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/gensymb.js
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/html.js
--rw-r--r--   0 runner    (1001) docker     (121)    31845 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mathtools.js
--rw-r--r--   0 runner    (1001) docker     (121)    38270 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mhchem.js
--rw-r--r--   0 runner    (1001) docker     (121)    11768 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/newcommand.js
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noerrors.js
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noundefined.js
--rw-r--r--   0 runner    (1001) docker     (121)    24029 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/physics.js
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/require.js
--rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/setoptions.js
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/tagformat.js
--rw-r--r--   0 runner    (1001) docker     (121)     6808 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textcomp.js
--rw-r--r--   0 runner    (1001) docker     (121)    16138 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textmacros.js
--rw-r--r--   0 runner    (1001) docker     (121)     3450 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/unicode.js
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/upgreek.js
--rw-r--r--   0 runner    (1001) docker     (121)     2562 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/verb.js
--rw-r--r--   0 runner    (1001) docker     (121)   135594 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-base.js
--rw-r--r--   0 runner    (1001) docker     (121)   345624 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-full.js
--rw-r--r--   0 runner    (1001) docker     (121)   179888 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex.js
--rw-r--r--   0 runner    (1001) docker     (121)     5090 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/latest.js
--rw-r--r--   0 runner    (1001) docker     (121)    18439 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/loader.js
--rw-r--r--   0 runner    (1001) docker     (121)   997633 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/mml-chtml.js
--rw-r--r--   0 runner    (1001) docker     (121)  1945224 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/mml-svg.js
--rw-r--r--   0 runner    (1001) docker     (121)   265880 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/node-main.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.415109 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.415109 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)   104800 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/tex.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.419109 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/
--rw-r--r--   0 runner    (1001) docker     (121)    40808 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_AMS-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)     9908 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)     9600 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    22340 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    21480 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    34464 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    20832 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    34160 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    19776 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    19360 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    19288 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    15944 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    14628 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)    12660 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    11852 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)     5792 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)     5148 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    17604 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Zero.woff
--rw-r--r--   0 runner    (1001) docker     (121)   221887 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.419109 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)  1065875 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/fonts/tex.js
--rw-r--r--   0 runner    (1001) docker     (121)   208515 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/svg.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.423110 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/
--rw-r--r--   0 runner    (1001) docker     (121)   115025 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/base.json
--rw-r--r--   0 runner    (1001) docker     (121)   296176 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/ca.json
--rw-r--r--   0 runner    (1001) docker     (121)   294956 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/da.json
--rw-r--r--   0 runner    (1001) docker     (121)   329805 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/de.json
--rw-r--r--   0 runner    (1001) docker     (121)   409173 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/en.json
--rw-r--r--   0 runner    (1001) docker     (121)   298556 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/es.json
--rw-r--r--   0 runner    (1001) docker     (121)   322917 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/fr.json
--rw-r--r--   0 runner    (1001) docker     (121)   440548 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/hi.json
--rw-r--r--   0 runner    (1001) docker     (121)   328235 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/it.json
--rw-r--r--   0 runner    (1001) docker     (121)   307312 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nb.json
--rw-r--r--   0 runner    (1001) docker     (121)   224008 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nemeth.json
--rw-r--r--   0 runner    (1001) docker     (121)   308992 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nn.json
--rw-r--r--   0 runner    (1001) docker     (121)   317841 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/sv.json
--rw-r--r--   0 runner    (1001) docker     (121)    29566 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/startup.js
--rw-r--r--   0 runner    (1001) docker     (121)  2091263 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full-speech.js
--rw-r--r--   0 runner    (1001) docker     (121)  1327522 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full.js
--rw-r--r--   0 runner    (1001) docker     (121)  1160989 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml.js
--rw-r--r--   0 runner    (1001) docker     (121)  1173007 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-chtml.js
--rw-r--r--   0 runner    (1001) docker     (121)  2120598 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-svg.js
--rw-r--r--   0 runner    (1001) docker     (121)  2275113 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg-full.js
--rw-r--r--   0 runner    (1001) docker     (121)  2108580 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/ui/
--rw-r--r--   0 runner    (1001) docker     (121)    11148 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/ui/lazy.js
--rw-r--r--   0 runner    (1001) docker     (121)   425918 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/ui/menu.js
--rw-r--r--   0 runner    (1001) docker     (121)    11189 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/ui/safe.js
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/package.json
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/e21f10a35be70062bd52.js
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/e28ce8d8788f1c481c94.js
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/e34e1eea962d106ac9f7.js
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/e9742b45b7f18586fbfc.js
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/f018740ba126b768ba78.woff
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/f2bbf41c400f22c7be3e.js
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/f3ab53586fa196f69840.js
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/f848df2e7ed3efa15a23.woff
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/f9da71e65171af2f166e.js
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/f9e999ca21af13e9af38.json
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/fb1b139080c47e548597.js
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/fb1e0d7cdde5dd7da606.json
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/fc58ec940d60e00df5c8.js
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/ffc48ea13dc24dd37689.js
--rw-r--r--   0 runner    (1001) docker     (121)    26735 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/remoteEntry.787652ab34540ecbe077.js
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-08 14:38:52.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/style.js
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-11-08 14:38:53.000000 ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1589 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.375106 ipydrawio-mathjax-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax/
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax/etc/
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax/etc/install.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-11-08 14:39:15.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13911 2022-11-08 14:39:15.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 14:39:15.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-08 14:39:15.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-08 14:39:15.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-08 14:39:15.000000 ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-08 14:39:15.427110 ipydrawio-mathjax-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-11-08 14:37:20.000000 ipydrawio-mathjax-1.2.2/tests/test_labextensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.924615 ipydrawio-mathjax-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-11 21:51:00.924615 ipydrawio-mathjax-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.568612 ipydrawio-mathjax-1.3.0/_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.596612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.608612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/480.4e5821ae6810e33f4c3b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/568.6474bf67e268a15a4277.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.576612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.608612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.692613 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.724613 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/assistive-mml.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/complexity.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36348 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/semantic-enrich.js
+-rw-r--r--   0 runner    (1001) docker     (123)   337064 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/sre.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.724613 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)    22827 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/adaptors/liteDOM.js
+-rw-r--r--   0 runner    (1001) docker     (123)   218533 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/core.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.736613 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/
+-rw-r--r--   0 runner    (1001) docker     (123)   107781 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/asciimath.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.736613 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/
+-rw-r--r--   0 runner    (1001) docker     (123)    51126 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/entities.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.736613 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)    28862 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   199492 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.sef.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.580612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.804614 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/action.js
+-rw-r--r--   0 runner    (1001) docker     (123)   215178 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/all-packages.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/ams.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/amscd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/autoload.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bbox.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/boldsymbol.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/braket.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bussproofs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cancel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cases.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/centernot.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/color.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colortbl.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colorv2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/configmacros.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/empheq.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/enclose.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/extpfeil.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/gensymb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/html.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31845 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mathtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)    38270 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mhchem.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/newcommand.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noerrors.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noundefined.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/physics.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/require.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/setoptions.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/tagformat.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textcomp.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textmacros.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/unicode.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/upgreek.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/verb.js
+-rw-r--r--   0 runner    (1001) docker     (123)   135594 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-base.js
+-rw-r--r--   0 runner    (1001) docker     (123)   345624 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-full.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179888 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/latest.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/loader.js
+-rw-r--r--   0 runner    (1001) docker     (123)   997633 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/mml-chtml.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1945224 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/mml-svg.js
+-rw-r--r--   0 runner    (1001) docker     (123)   265880 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/node-main.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.804614 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.580612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.808614 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   104800 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/tex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.856614 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)    40808 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_AMS-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    21480 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34464 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34160 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19776 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19360 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    19288 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14628 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Zero.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   221887 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.588612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.856614 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)  1065875 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/fonts/tex.js
+-rw-r--r--   0 runner    (1001) docker     (123)   208515 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/svg.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.588612 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.896614 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)   115025 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/base.json
+-rw-r--r--   0 runner    (1001) docker     (123)   296176 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/ca.json
+-rw-r--r--   0 runner    (1001) docker     (123)   294956 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/da.json
+-rw-r--r--   0 runner    (1001) docker     (123)   329805 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/de.json
+-rw-r--r--   0 runner    (1001) docker     (123)   409173 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)   298556 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/es.json
+-rw-r--r--   0 runner    (1001) docker     (123)   322917 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/fr.json
+-rw-r--r--   0 runner    (1001) docker     (123)   440548 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/hi.json
+-rw-r--r--   0 runner    (1001) docker     (123)   328235 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/it.json
+-rw-r--r--   0 runner    (1001) docker     (123)   307312 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nb.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224008 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nemeth.json
+-rw-r--r--   0 runner    (1001) docker     (123)   308992 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nn.json
+-rw-r--r--   0 runner    (1001) docker     (123)   317841 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/sv.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29566 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/startup.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2091263 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full-speech.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1327522 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1160989 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1173007 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-chtml.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2120598 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-svg.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2275113 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg-full.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2108580 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.908614 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/ui/lazy.js
+-rw-r--r--   0 runner    (1001) docker     (123)   425918 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/ui/menu.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11189 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/ui/safe.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26657 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/remoteEntry.6abe8eb6564d5e102902.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-11 21:50:55.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 21:50:58.000000 ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-11 21:51:00.928615 ipydrawio-mathjax-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.588612 ipydrawio-mathjax-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.908614 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.924615 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax/etc/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.924615 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-04-11 21:51:00.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-04-11 21:51:00.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:00.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:51:00.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-11 21:51:00.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 21:51:00.000000 ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:51:00.924615 ipydrawio-mathjax-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-11 21:49:16.000000 ipydrawio-mathjax-1.3.0/tests/test_labextensions.py
```

### Comparing `ipydrawio-mathjax-1.2.2/LICENSE.txt` & `ipydrawio-mathjax-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/PKG-INFO` & `ipydrawio-mathjax-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ipydrawio-mathjax
-Version: 1.2.2
+Version: 1.3.0
 Summary: MathJax for ipydrawio
 Home-page: https://ipydrawio.rtfd.io
 Author: ipydrawio Contributors
 Author-email: ripxl@example.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/deathbeds/ipydrawio/issues
-Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://app.codecov.io/gh/deathbeds/ipydrawio
 Project-URL: Documentation, https://ipydrawio.rtfd.io
 Project-URL: Source Code, https://github.com/deathbeds/ipydrawio
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # IPyDrawio Math
 
 [![docs][docs-badge]][docs] [![binder-badge][]][binder]
@@ -55,15 +54,15 @@
 ```
 
 ## Open Source
 
 This work is licensed under the [Apache-2.0] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -71,24 +70,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-mathjax/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-mathjax/LICENSE.txt
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-mathjax
 [pypi]: https://pypi.org/project/ipydrawio-mathjax
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-mathjax
 [conda]: https://anaconda.org/conda-forge/ipydrawio-mathjax
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-mathjax-1.2.2/README.md` & `ipydrawio-mathjax-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```
 
 ## Open Source
 
 This work is licensed under the [Apache-2.0] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -36,24 +36,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-mathjax/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-mathjax/LICENSE.txt
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-mathjax
 [pypi]: https://pypi.org/project/ipydrawio-mathjax
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-mathjax
 [conda]: https://anaconda.org/conda-forge/ipydrawio-mathjax
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/package.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9366071428571429%*

 * *Differences: {"'dependencies'": "{'@deathbeds/ipydrawio-webpack': '^21.1.600'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^3.6.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.6abe8eb6564d5e102902.js'}}",*

 * * "'version'": "'1.3.0'"}*

```diff
@@ -1,25 +1,25 @@
 {
     "author": "IPyDrawio Contributors",
     "bugs": {
         "url": "https://github.com/deathbeds/ipydrawio/issues"
     },
     "dependencies": {
-        "@deathbeds/ipydrawio-webpack": "^20.5.300",
+        "@deathbeds/ipydrawio-webpack": "^21.1.600",
         "@jupyterlab/application": "^3.1.0"
     },
     "description": "MathJax for ipydrawio",
     "devDependencies": {
-        "@jupyterlab/builder": "^3.4.0"
+        "@jupyterlab/builder": "^3.6.1"
     },
     "homepage": "https://ipydrawio.rtfd.io",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.787652ab34540ecbe077.js"
+            "load": "static/remoteEntry.6abe8eb6564d5e102902.js"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "ipydrawio-mathjax"
                 },
                 "managers": [
@@ -40,9 +40,9 @@
     "main": "lib/index.js",
     "name": "@deathbeds/ipydrawio-mathjax",
     "repository": {
         "type": "git",
         "url": "https://github.com/deathbeds/ipydrawio.git"
     },
     "types": "lib/index.d.ts",
-    "version": "1.2.2"
+    "version": "1.3.0"
 }
```

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/480.3f50ce7358e02e2ef38b.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/480.4e5821ae6810e33f4c3b.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,45 +1,41 @@
 "use strict";
 (self["webpackChunk_deathbeds_ipydrawio_mathjax"] = self["webpackChunk_deathbeds_ipydrawio_mathjax"] || []).push([
     [480], {
 
         /***/
-        4480:
+        480:
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
                     "default": () => (__WEBPACK_DEFAULT_EXPORT__)
                     /* harmony export */
                 });
-                // Copyright 2022 ipydrawio contributors
+                // Copyright 2023 ipydrawio contributors
                 //
                 // Licensed under the Apache License, Version 2.0 (the "License");
                 // you may not use this file except in compliance with the License.
                 // You may obtain a copy of the License at
                 //
                 //     http://www.apache.org/licenses/LICENSE-2.0
                 //
                 // Unless required by applicable law or agreed to in writing, software
                 // distributed under the License is distributed on an "AS IS" BASIS,
                 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
                 // See the License for the specific language governing permissions and
                 // limitations under the License.
 
-                let DEBUG = false;
-
                 const plugin = {
                     id: '@deathbeds/ipydrawio-mathjax:plugin',
                     activate: async () => {
-                        if (DEBUG) {
-                            await __webpack_require__.e( /* import() */ 799).then(__webpack_require__.bind(__webpack_require__, 9462));
-                        }
+                        //
                     },
                     autoStart: true,
                 };
 
                 /* harmony default export */
                 const __WEBPACK_DEFAULT_EXPORT__ = (plugin);
```

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/568.7226bc506cb1dc5c99c7.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/568.6474bf67e268a15a4277.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,25 +1,25 @@
 "use strict";
 (self["webpackChunk_deathbeds_ipydrawio_mathjax"] = self["webpackChunk_deathbeds_ipydrawio_mathjax"] || []).push([
     [568], {
 
         /***/
-        1568:
+        568:
             /***/
             ((__unused_webpack_module, __webpack_exports__, __webpack_require__) => {
 
                 __webpack_require__.r(__webpack_exports__);
                 /* harmony export */
                 __webpack_require__.d(__webpack_exports__, {
                     /* harmony export */
                     "DRAWIO_MATHJAX_URL": () => ( /* binding */ DRAWIO_MATHJAX_URL)
                     /* harmony export */
                 });
                 /* harmony import */
-                var _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(1019);
+                var _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(142);
                 /* harmony import */
                 var _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/ __webpack_require__.n(_jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__);
 
                 /**
                  * The path on the server to base application HTML, to be served in an iframe
                  */
                 const DRAWIO_MATHJAX_URL = _jupyterlab_coreutils__WEBPACK_IMPORTED_MODULE_0__.URLExt.join(
```

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/assistive-mml.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/assistive-mml.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/complexity.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/complexity.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/explorer.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/explorer.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/semantic-enrich.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/semantic-enrich.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/a11y/sre.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/a11y/sre.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/adaptors/liteDOM.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/adaptors/liteDOM.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/core.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/core.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/asciimath.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/asciimath.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/entities.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/entities.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.sef.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml/extensions/mml3.sef.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/mml.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/mml.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/action.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/action.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/all-packages.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/all-packages.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/ams.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/ams.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/amscd.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/amscd.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/autoload.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/autoload.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bbox.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bbox.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/boldsymbol.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/boldsymbol.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/braket.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/braket.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bussproofs.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/bussproofs.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cancel.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cancel.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cases.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/cases.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/centernot.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/centernot.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/color.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/color.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colortbl.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colortbl.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colorv2.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/colorv2.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/configmacros.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/configmacros.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/empheq.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/empheq.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/enclose.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/enclose.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/extpfeil.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/extpfeil.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/gensymb.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/gensymb.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/html.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/html.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mathtools.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mathtools.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mhchem.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/mhchem.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/newcommand.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/newcommand.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noerrors.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noerrors.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noundefined.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/noundefined.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/physics.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/physics.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/require.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/require.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/setoptions.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/setoptions.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/tagformat.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/tagformat.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textcomp.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textcomp.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textmacros.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/textmacros.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/unicode.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/unicode.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/upgreek.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/upgreek.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/verb.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex/extensions/verb.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-base.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-base.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-full.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex-full.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/input/tex.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/input/tex.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/latest.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/latest.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/loader.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/loader.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/mml-chtml.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/mml-chtml.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/mml-svg.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/mml-svg.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/node-main.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/node-main.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/tex.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/tex.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_AMS-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Bold.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Calligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Bold.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Bold.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Italic.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-BoldItalic.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Italic.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Math-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Bold.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Italic.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Script-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size1-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size2-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size3-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size4-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Typewriter-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Bold.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Bold.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Regular.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Vector-Regular.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Zero.woff` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml/fonts/woff-v2/MathJax_Zero.woff`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/chtml.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/fonts/tex.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/svg/fonts/tex.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/output/svg.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/output/svg.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/base.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/base.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/ca.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/ca.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/da.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/da.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/de.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/de.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/en.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/en.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/es.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/es.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/fr.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/fr.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/hi.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/hi.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/it.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/it.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nb.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nb.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nemeth.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nemeth.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nn.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/nn.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/sv.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/sre/mathmaps/sv.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/startup.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/startup.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full-speech.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full-speech.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml-full.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-chtml.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-chtml.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-chtml.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-svg.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-mml-svg.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg-full.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg-full.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/tex-svg.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/ui/lazy.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/ui/lazy.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/ui/menu.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/ui/menu.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/es5/ui/safe.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/es5/ui/safe.js`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/dio/math/package.json` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/dio/math/package.json`

 * *Files identical despite different names*

### Comparing `ipydrawio-mathjax-1.2.2/_/ipydrawio-mathjax/static/remoteEntry.787652ab34540ecbe077.js` & `ipydrawio-mathjax-1.3.0/_/ipydrawio-mathjax/static/remoteEntry.6abe8eb6564d5e102902.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -3,24 +3,24 @@
 (() => { // webpackBootstrap
     /******/
     "use strict";
     /******/
     var __webpack_modules__ = ({
 
         /***/
-        3950:
+        950:
             /***/
             ((__unused_webpack_module, exports, __webpack_require__) => {
 
                 var moduleMap = {
                     "./index": () => {
-                        return __webpack_require__.e(568).then(() => (() => ((__webpack_require__(1568)))));
+                        return __webpack_require__.e(568).then(() => (() => ((__webpack_require__(568)))));
                     },
                     "./extension": () => {
-                        return __webpack_require__.e(480).then(() => (() => ((__webpack_require__(4480)))));
+                        return __webpack_require__.e(480).then(() => (() => ((__webpack_require__(480)))));
                     }
                 };
                 var get = (module, getScope) => {
                     __webpack_require__.R = getScope;
                     getScope = (
                         __webpack_require__.o(moduleMap, module) ?
                         moduleMap[module]() :
@@ -175,21 +175,19 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "480": "3f50ce7358e02e2ef38b",
-                "568": "7226bc506cb1dc5c99c7",
-                "799": "edc688f162b17cb84c84"
+                "480": "4e5821ae6810e33f4c3b",
+                "568": "6474bf67e268a15a4277"
             } [chunkId] + ".js?v=" + {
-                "480": "3f50ce7358e02e2ef38b",
-                "568": "7226bc506cb1dc5c99c7",
-                "799": "edc688f162b17cb84c84"
+                "480": "4e5821ae6810e33f4c3b",
+                "568": "6474bf67e268a15a4277"
             } [chunkId] + "";
             /******/
         };
         /******/
     })();
     /******/
     /******/
@@ -300,16 +298,14 @@
                 /******/
                 doneFns && doneFns.forEach((fn) => (fn(event)));
                 /******/
                 if (prev) return prev(event);
                 /******/
             }
             /******/
-            ;
-            /******/
             var timeout = setTimeout(onScriptComplete.bind(null, undefined, {
                 type: 'timeout',
                 target: script
             }), 120000);
             /******/
             script.onerror = onScriptComplete.bind(null, script.onerror);
             /******/
@@ -422,15 +418,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("@deathbeds/ipydrawio-mathjax", "1.2.2", () => (__webpack_require__.e(568).then(() => (() => (__webpack_require__(1568))))));
+                    register("@deathbeds/ipydrawio-mathjax", "1.3.0", () => (__webpack_require__.e(568).then(() => (() => (__webpack_require__(568))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -453,15 +449,15 @@
         /******/
         var document = __webpack_require__.g.document;
         /******/
         if (!scriptUrl && document) {
             /******/
             if (document.currentScript)
                 /******/
-                scriptUrl = document.currentScript.src
+                scriptUrl = document.currentScript.src;
             /******/
             if (!scriptUrl) {
                 /******/
                 var scripts = document.getElementsByTagName("script");
                 /******/
                 if (scripts.length) scriptUrl = scripts[scripts.length - 1].src
                 /******/
@@ -811,24 +807,24 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            1019: () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 5, 0]))
+            142: () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 5, 6, 3]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "568": [
                 /******/
-                1019
+                142
                 /******/
             ]
             /******/
         };
         /******/
         __webpack_require__.f.consumes = (chunkId, promises) => {
             /******/
@@ -1040,13 +1036,13 @@
     /******/
     /************************************************************************/
     /******/
     /******/ // module cache are used so entry inlining is disabled
     /******/ // startup
     /******/ // Load entry module and return exports
     /******/
-    var __webpack_exports__ = __webpack_require__(3950);
+    var __webpack_exports__ = __webpack_require__(950);
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["@deathbeds/ipydrawio-mathjax"] = __webpack_exports__;
     /******/
     /******/
 })();
```

### Comparing `ipydrawio-mathjax-1.2.2/setup.cfg` & `ipydrawio-mathjax-1.3.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -6,70 +6,61 @@
 url = https://ipydrawio.rtfd.io
 author = ipydrawio Contributors
 author_email = ripxl@example.com
 license = Apache-2.0
 license_files = LICENSE.txt
 project_urls = 
 	Bug Tracker = https://github.com/deathbeds/ipydrawio/issues
-	Changelog = https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+	Changelog = https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 	Coverage = https://app.codecov.io/gh/deathbeds/ipydrawio
 	Documentation = https://ipydrawio.rtfd.io
 	Source Code = https://github.com/deathbeds/ipydrawio
 classifiers = 
 	Development Status :: 4 - Beta
 	Framework :: Jupyter
 	Framework :: Jupyter :: JupyterLab :: 3
 	Framework :: Jupyter :: JupyterLab :: Extensions
 	Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 	Topic :: Multimedia :: Graphics :: Presentation
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 package_dir = 
 	= src
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
-	ipydrawio ==1.2.2
+	ipydrawio ==1.3.0
 
 [options.packages.find]
 where = 
 	src
 
 [options.extras_require]
 test = 
 	pytest
 
-[flake8]
-exclude = .git,__pycache__,envs,.ipynb_checkpoints,.mypy_cache
-max-line-length = 88
-ignore = E203
-
-[isort]
-combine_as_imports = True
-include_trailing_comma = True
-line_length = 88
-multi_line_output = 3
-
 [coverage:run]
 branch = True
 source_pkgs = 
 	ipydrawio_mathjax
 concurrency = multiprocessing
 parallel = True
 
+[coverage:html]
+show_contexts = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ipydrawio-mathjax-1.2.2/setup.py` & `ipydrawio-mathjax-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""dynamic setup information for setuptools, also see package.json and setup.cfg"""
+"""dynamic setup information for setuptools, also see package.json and setup.cfg."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -28,26 +28,26 @@
 
 FILES = []
 
 for package_json in EXT.glob("*/package.json"):
     pkg = json.loads(package_json.read_text(encoding="utf-8"))
 
     FILES += [
-        (f"""{SHARE}/{pkg["name"]}""", ["src/ipydrawio_mathjax/etc/install.json"])
+        (f"""{SHARE}/{pkg["name"]}""", ["src/ipydrawio_mathjax/etc/install.json"]),
     ]
 
     for path in package_json.parent.rglob("*"):
         if path.is_dir():
             continue
         parent = path.parent.relative_to(package_json.parent).as_posix()
         FILES += [
             (
                 f"""{SHARE}/{pkg["name"]}/{parent}""",
                 [str(path.relative_to(HERE).as_posix())],
-            )
+            ),
         ]
 
 
 if __name__ == "__main__":
     import setuptools
 
     setuptools.setup(version=__js__["version"], data_files=FILES)
```

### Comparing `ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax/__init__.py` & `ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""MathJax for ipydrawio"""
+"""MathJax for ipydrawio."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,17 +16,16 @@
 
 from ipydrawio import _ipydrawio_labextension_paths
 
 from ._version import __ext__, __js__, __prefix__, __version__
 
 
 def _jupyter_labextension_paths():
-    """static paths to link for interactive installation"""
-    exts = _ipydrawio_labextension_paths(prefix=__prefix__, extensions=__ext__)
-    return exts
+    """Static paths to link for interactive installation."""
+    return _ipydrawio_labextension_paths(prefix=__prefix__, extensions=__ext__)
 
 
 __all__ = [
     "__js__",
     "__version__",
     "_jupyter_labextension_paths",
 ]
```

### Comparing `ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax/_version.py` & `ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""source of truth for ipydrawio version"""
+"""source of truth for ipydrawio version."""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 # Copyright 2020 jupyterlab-drawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `ipydrawio-mathjax-1.2.2/src/ipydrawio_mathjax.egg-info/PKG-INFO` & `ipydrawio-mathjax-1.3.0/src/ipydrawio_mathjax.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: ipydrawio-mathjax
-Version: 1.2.2
+Version: 1.3.0
 Summary: MathJax for ipydrawio
 Home-page: https://ipydrawio.rtfd.io
 Author: ipydrawio Contributors
 Author-email: ripxl@example.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/deathbeds/ipydrawio/issues
-Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/master/CHANGELOG.md
+Project-URL: Changelog, https://github.com/deathbeds/ipydrawio/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://app.codecov.io/gh/deathbeds/ipydrawio
 Project-URL: Documentation, https://ipydrawio.rtfd.io
 Project-URL: Source Code, https://github.com/deathbeds/ipydrawio
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # IPyDrawio Math
 
 [![docs][docs-badge]][docs] [![binder-badge][]][binder]
@@ -55,15 +54,15 @@
 ```
 
 ## Open Source
 
 This work is licensed under the [Apache-2.0] License.
 
 ```
-Copyright 2022 ipydrawio contributors
+Copyright 2023 ipydrawio contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
   http://www.apache.org/licenses/LICENSE-2.0
 
@@ -71,24 +70,24 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 
 [apache-2.0]:
-  https://github.com/deathbeds/ipydrawio/blob/master/py_packages/ipydrawio-mathjax/LICENSE.txt
+  https://github.com/deathbeds/ipydrawio/blob/main/py_packages/ipydrawio-mathjax/LICENSE.txt
 [binder]:
-  http://mybinder.org/v2/gh/deathbeds/ipydrawio/master?urlpath=lab/tree/docs/Poster.dio.svg
+  http://mybinder.org/v2/gh/deathbeds/ipydrawio/main?urlpath=lab/tree/docs/Poster.dio.svg
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [pypi-badge]: https://img.shields.io/pypi/v/ipydrawio-mathjax
 [pypi]: https://pypi.org/project/ipydrawio-mathjax
 [conda-badge]: https://img.shields.io/conda/vn/conda-forge/ipydrawio-mathjax
 [conda]: https://anaconda.org/conda-forge/ipydrawio-mathjax
 [workflow-badge]:
   https://github.com/deathbeds/ipydrawio/workflows/.github/workflows/ci.yml/badge.svg
 [workflow]:
-  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amaster+workflow%3A.github%2Fworkflows%2Fci.yml
+  https://github.com/deathbeds/ipydrawio/actions?query=branch%3Amain+workflow%3A.github%2Fworkflows%2Fci.yml
 [cov-badge]:
-  https://codecov.io/gh/deathbeds/ipydrawio/branch/master/graph/badge.svg?token=9B74VKHQDK
+  https://codecov.io/gh/deathbeds/ipydrawio/branch/main/graph/badge.svg?token=9B74VKHQDK
 [cov]: https://codecov.io/gh/deathbeds/ipydrawio
 [docs-badge]: https://readthedocs.org/projects/ipydrawio/badge/?version=latest
 [docs]: https://ipydrawio.rtfd.io
```

### Comparing `ipydrawio-mathjax-1.2.2/tests/test_labextensions.py` & `ipydrawio-mathjax-1.3.0/tests/test_labextensions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """minimal tests of metadata"""
 
-# Copyright 2022 ipydrawio contributors
+# Copyright 2023 ipydrawio contributors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

