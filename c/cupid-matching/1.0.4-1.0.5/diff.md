# Comparing `tmp/cupid_matching-1.0.4.tar.gz` & `tmp/cupid_matching-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupid_matching-1.0.4.tar", max compression
+gzip compressed data, was "cupid_matching-1.0.5.tar", max compression
```

## Comparing `cupid_matching-1.0.4.tar` & `cupid_matching-1.0.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     2098 2023-04-02 13:26:05.671761 cupid_matching-1.0.4/README.md
--rw-r--r--   0        0        0      176 2023-04-01 13:41:41.834338 cupid_matching-1.0.4/cupid_matching/.idea/.gitignore
--rw-r--r--   0        0        0      539 2023-04-01 14:33:58.454731 cupid_matching-1.0.4/cupid_matching/.idea/cupid_matching.iml
--rw-r--r--   0        0        0     1446 2023-04-01 14:28:21.412476 cupid_matching-1.0.4/cupid_matching/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-04-01 14:28:21.442115 cupid_matching-1.0.4/cupid_matching/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      198 2023-04-01 14:28:21.437713 cupid_matching-1.0.4/cupid_matching/.idea/misc.xml
--rw-r--r--   0        0        0      280 2023-04-01 14:28:21.431899 cupid_matching-1.0.4/cupid_matching/.idea/modules.xml
--rw-r--r--   0        0        0      183 2023-04-01 14:28:21.446055 cupid_matching-1.0.4/cupid_matching/.idea/vcs.xml
--rw-r--r--   0        0        0      368 2023-04-01 14:33:58.460060 cupid_matching-1.0.4/cupid_matching/.idea/webResources.xml
--rw-r--r--   0        0        0       22 2023-04-02 13:24:44.115021 cupid_matching-1.0.4/cupid_matching/__init__.py
--rw-r--r--   0        0        0     7929 2023-04-02 13:02:37.271492 cupid_matching-1.0.4/cupid_matching/choo_siow.py
--rw-r--r--   0        0        0     5656 2023-04-02 13:02:37.271948 cupid_matching-1.0.4/cupid_matching/choo_siow_gender_heteroskedastic.py
--rw-r--r--   0        0        0     6241 2023-04-02 13:02:37.272393 cupid_matching-1.0.4/cupid_matching/choo_siow_heteroskedastic.py
--rw-r--r--   0        0        0    14162 2023-04-02 13:02:37.272889 cupid_matching-1.0.4/cupid_matching/cupid_streamlit.py
--rw-r--r--   0        0        0       51 2023-03-24 00:22:09.620449 cupid_matching-1.0.4/cupid_matching/docs/choo_siow.md
--rw-r--r--   0        0        0       97 2023-03-24 00:21:48.848158 cupid_matching-1.0.4/cupid_matching/docs/choo_siow_gender_heteroskedastic.md
--rw-r--r--   0        0        0       83 2023-03-24 00:22:03.727712 cupid_matching-1.0.4/cupid_matching/docs/choo_siow_heteroskedastic.md
--rw-r--r--   0        0        0      285 2023-03-24 00:22:15.196968 cupid_matching-1.0.4/cupid_matching/docs/cupid_streamlit.md
--rw-r--r--   0        0        0       46 2023-03-24 00:22:19.670499 cupid_matching-1.0.4/cupid_matching/docs/entropy.md
--rw-r--r--   0        0        0       63 2023-04-02 13:02:37.273230 cupid_matching-1.0.4/cupid_matching/docs/example_choosiow.md
--rw-r--r--   0        0        0       69 2023-04-02 13:02:37.273547 cupid_matching-1.0.4/cupid_matching/docs/example_nestedlogit.md
--rw-r--r--   0        0        0     2098 2023-04-02 13:25:13.443717 cupid_matching-1.0.4/cupid_matching/docs/index.md
--rw-r--r--   0        0        0       57 2023-03-24 00:22:52.962261 cupid_matching-1.0.4/cupid_matching/docs/ipfp_solvers.md
--rw-r--r--   0        0        0       61 2023-03-24 00:22:57.157065 cupid_matching-1.0.4/cupid_matching/docs/matching_utils.md
--rw-r--r--   0        0        0       57 2023-03-24 00:23:07.925133 cupid_matching-1.0.4/cupid_matching/docs/min_distance.md
--rw-r--r--   0        0        0       69 2023-03-24 00:23:01.182377 cupid_matching-1.0.4/cupid_matching/docs/min_distance_utils.md
--rw-r--r--   0        0        0       59 2023-03-24 00:27:46.673143 cupid_matching-1.0.4/cupid_matching/docs/model_classes.md
--rw-r--r--   0        0        0       58 2023-03-24 00:23:19.684703 cupid_matching-1.0.4/cupid_matching/docs/nested_logit.md
--rw-r--r--   0        0        0       55 2023-03-24 00:27:33.384226 cupid_matching-1.0.4/cupid_matching/docs/poisson_glm.md
--rw-r--r--   0        0        0       67 2023-03-24 00:27:42.792605 cupid_matching-1.0.4/cupid_matching/docs/poisson_glm_utils.md
--rw-r--r--   0        0        0       43 2023-03-24 00:27:23.096924 cupid_matching-1.0.4/cupid_matching/docs/utils.md
--rw-r--r--   0        0        0    11534 2023-04-02 13:02:37.273872 cupid_matching-1.0.4/cupid_matching/entropy.py
--rw-r--r--   0        0        0     3787 2023-04-02 13:02:37.274156 cupid_matching-1.0.4/cupid_matching/example_choosiow.py
--rw-r--r--   0        0        0     4288 2023-04-02 13:02:37.274484 cupid_matching-1.0.4/cupid_matching/example_nestedlogit.py
--rw-r--r--   0        0        0    26520 2023-04-02 13:02:37.275037 cupid_matching-1.0.4/cupid_matching/ipfp_solvers.py
--rw-r--r--   0        0        0     8743 2023-04-02 13:02:37.290279 cupid_matching-1.0.4/cupid_matching/matching_utils.py
--rw-r--r--   0        0        0    11495 2023-04-02 13:02:37.290650 cupid_matching-1.0.4/cupid_matching/min_distance.py
--rw-r--r--   0        0        0     5216 2023-04-02 13:02:37.290925 cupid_matching-1.0.4/cupid_matching/min_distance_utils.py
--rw-r--r--   0        0        0     1873 2023-04-02 13:02:37.291292 cupid_matching-1.0.4/cupid_matching/mkdocs.yml
--rw-r--r--   0        0        0    16277 2023-04-02 13:02:37.291644 cupid_matching-1.0.4/cupid_matching/model_classes.py
--rw-r--r--   0        0        0      369 2023-03-23 23:43:59.187373 cupid_matching-1.0.4/cupid_matching/mypy.ini
--rw-r--r--   0        0        0     9558 2023-04-02 13:02:37.291920 cupid_matching-1.0.4/cupid_matching/nested_logit.py
--rw-r--r--   0        0        0     7373 2023-04-02 13:02:37.292224 cupid_matching-1.0.4/cupid_matching/poisson_glm.py
--rw-r--r--   0        0        0     6486 2023-04-02 13:02:37.292474 cupid_matching-1.0.4/cupid_matching/poisson_glm_utils.py
--rw-r--r--   0        0        0    17888 2023-04-02 13:25:48.755531 cupid_matching-1.0.4/cupid_matching/site/404.html
--rw-r--r--   0        0        0      704 2023-04-02 13:25:48.697255 cupid_matching-1.0.4/cupid_matching/site/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     1870 2023-04-02 13:25:48.698601 cupid_matching-1.0.4/cupid_matching/site/assets/images/favicon.png
--rw-r--r--   0        0        0    17074 2023-04-02 13:25:48.699536 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2023-04-02 13:25:48.699905 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2023-04-02 13:25:48.700089 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2023-04-02 13:25:48.700244 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2023-04-02 13:25:48.700705 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2023-04-02 13:25:48.701002 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2023-04-02 13:25:48.701180 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     3383 2023-04-02 13:25:48.701489 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2023-04-02 13:25:48.701702 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0    11232 2023-04-02 13:25:48.701863 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2023-04-02 13:25:48.702013 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2023-04-02 13:25:48.702162 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     7973 2023-04-02 13:25:48.702320 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2023-04-02 13:25:48.702472 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2023-04-02 13:25:48.702638 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2023-04-02 13:25:48.702861 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2023-04-02 13:25:48.703035 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2023-04-02 13:25:48.703212 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2023-04-02 13:25:48.703429 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     3647 2023-04-02 13:25:48.703650 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2023-04-02 13:25:48.703834 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2023-04-02 13:25:48.703991 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     1031 2023-04-02 13:25:48.704187 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2023-04-02 13:25:48.704776 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2023-04-02 13:25:48.704982 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2062 2023-04-02 13:25:48.705176 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2023-04-02 13:25:48.705366 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677455 2023-04-02 13:25:48.705679 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    38916 2023-04-02 13:25:48.705864 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js
--rw-r--r--   0        0        0   209901 2023-04-02 13:25:48.706124 cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map
--rw-r--r--   0        0        0    12355 2023-04-02 13:25:48.706743 cupid_matching-1.0.4/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css
--rw-r--r--   0        0        0     3646 2023-04-02 13:25:48.706901 cupid_matching-1.0.4/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
--rw-r--r--   0        0        0    59109 2023-04-02 13:25:48.779193 cupid_matching-1.0.4/cupid_matching/site/choo_siow/index.html
--rw-r--r--   0        0        0    61309 2023-04-02 13:25:48.792943 cupid_matching-1.0.4/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html
--rw-r--r--   0        0        0    67113 2023-04-02 13:25:48.809968 cupid_matching-1.0.4/cupid_matching/site/choo_siow_heteroskedastic/index.html
--rw-r--r--   0        0        0    19453 2023-04-02 13:25:48.810842 cupid_matching-1.0.4/cupid_matching/site/cupid_streamlit/index.html
--rw-r--r--   0        0        0    52734 2023-04-02 13:25:48.820430 cupid_matching-1.0.4/cupid_matching/site/entropy/index.html
--rw-r--r--   0        0        0    23793 2023-04-02 13:25:48.764897 cupid_matching-1.0.4/cupid_matching/site/index.html
--rw-r--r--   0        0        0   171028 2023-04-02 13:25:48.889559 cupid_matching-1.0.4/cupid_matching/site/ipfp_solvers/index.html
--rw-r--r--   0        0        0    33535 2023-04-02 13:25:48.895183 cupid_matching-1.0.4/cupid_matching/site/matching_utils/index.html
--rw-r--r--   0        0        0    73534 2023-04-02 13:25:48.914885 cupid_matching-1.0.4/cupid_matching/site/min_distance/index.html
--rw-r--r--   0        0        0    48446 2023-04-02 13:25:48.926196 cupid_matching-1.0.4/cupid_matching/site/min_distance_utils/index.html
--rw-r--r--   0        0        0   158026 2023-04-02 13:25:48.981428 cupid_matching-1.0.4/cupid_matching/site/model_classes/index.html
--rw-r--r--   0        0        0    80348 2023-04-02 13:25:49.003109 cupid_matching-1.0.4/cupid_matching/site/nested_logit/index.html
--rw-r--r--   0        0        0      864 2023-04-02 13:25:48.697588 cupid_matching-1.0.4/cupid_matching/site/objects.inv
--rw-r--r--   0        0        0    70696 2023-04-02 13:25:49.023137 cupid_matching-1.0.4/cupid_matching/site/poisson_glm/index.html
--rw-r--r--   0        0        0    52535 2023-04-02 13:25:49.035787 cupid_matching-1.0.4/cupid_matching/site/poisson_glm_utils/index.html
--rw-r--r--   0        0        0   180162 2023-04-02 13:25:49.071290 cupid_matching-1.0.4/cupid_matching/site/search/search_index.json
--rw-r--r--   0        0        0     3235 2023-04-02 13:25:48.756744 cupid_matching-1.0.4/cupid_matching/site/sitemap.xml
--rw-r--r--   0        0        0      354 2023-04-02 13:25:48.756898 cupid_matching-1.0.4/cupid_matching/site/sitemap.xml.gz
--rw-r--r--   0        0        0   120234 2023-04-02 13:25:49.070697 cupid_matching-1.0.4/cupid_matching/site/utils/index.html
--rw-r--r--   0        0        0    12373 2023-04-02 13:02:37.292713 cupid_matching-1.0.4/cupid_matching/utils.py
--rw-r--r--   0        0        0      969 2023-04-02 13:24:24.936660 cupid_matching-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 cupid_matching-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2226 2023-04-12 19:22:08.495691 cupid_matching-1.0.5/README.md
+-rw-r--r--   0        0        0      176 2023-04-01 13:41:41.834338 cupid_matching-1.0.5/cupid_matching/.idea/.gitignore
+-rw-r--r--   0        0        0      539 2023-04-01 14:33:58.454731 cupid_matching-1.0.5/cupid_matching/.idea/cupid_matching.iml
+-rw-r--r--   0        0        0     1446 2023-04-01 14:28:21.412476 cupid_matching-1.0.5/cupid_matching/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-04-01 14:28:21.442115 cupid_matching-1.0.5/cupid_matching/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      198 2023-04-01 14:28:21.437713 cupid_matching-1.0.5/cupid_matching/.idea/misc.xml
+-rw-r--r--   0        0        0      280 2023-04-01 14:28:21.431899 cupid_matching-1.0.5/cupid_matching/.idea/modules.xml
+-rw-r--r--   0        0        0      183 2023-04-01 14:28:21.446055 cupid_matching-1.0.5/cupid_matching/.idea/vcs.xml
+-rw-r--r--   0        0        0      368 2023-04-01 14:33:58.460060 cupid_matching-1.0.5/cupid_matching/.idea/webResources.xml
+-rw-r--r--   0        0        0        1 2023-04-02 19:21:40.197779 cupid_matching-1.0.5/cupid_matching/__init__.py
+-rw-r--r--   0        0        0     9374 2023-04-12 19:23:11.716207 cupid_matching-1.0.5/cupid_matching/choo_siow.py
+-rw-r--r--   0        0        0     5656 2023-04-02 13:02:37.271948 cupid_matching-1.0.5/cupid_matching/choo_siow_gender_heteroskedastic.py
+-rw-r--r--   0        0        0     6283 2023-04-02 19:11:25.395323 cupid_matching-1.0.5/cupid_matching/choo_siow_heteroskedastic.py
+-rw-r--r--   0        0        0    14162 2023-04-02 13:02:37.272889 cupid_matching-1.0.5/cupid_matching/cupid_streamlit.py
+-rw-r--r--   0        0        0       51 2023-03-24 00:22:09.620449 cupid_matching-1.0.5/cupid_matching/docs/choo_siow.md
+-rw-r--r--   0        0        0       97 2023-03-24 00:21:48.848158 cupid_matching-1.0.5/cupid_matching/docs/choo_siow_gender_heteroskedastic.md
+-rw-r--r--   0        0        0       83 2023-03-24 00:22:03.727712 cupid_matching-1.0.5/cupid_matching/docs/choo_siow_heteroskedastic.md
+-rw-r--r--   0        0        0      285 2023-03-24 00:22:15.196968 cupid_matching-1.0.5/cupid_matching/docs/cupid_streamlit.md
+-rw-r--r--   0        0        0       46 2023-03-24 00:22:19.670499 cupid_matching-1.0.5/cupid_matching/docs/entropy.md
+-rw-r--r--   0        0        0       63 2023-04-02 13:02:37.273230 cupid_matching-1.0.5/cupid_matching/docs/example_choosiow.md
+-rw-r--r--   0        0        0       69 2023-04-02 13:02:37.273547 cupid_matching-1.0.5/cupid_matching/docs/example_nestedlogit.md
+-rw-r--r--   0        0        0     2226 2023-04-12 19:25:51.647057 cupid_matching-1.0.5/cupid_matching/docs/index.md
+-rw-r--r--   0        0        0       57 2023-03-24 00:22:52.962261 cupid_matching-1.0.5/cupid_matching/docs/ipfp_solvers.md
+-rw-r--r--   0        0        0       61 2023-03-24 00:22:57.157065 cupid_matching-1.0.5/cupid_matching/docs/matching_utils.md
+-rw-r--r--   0        0        0       57 2023-03-24 00:23:07.925133 cupid_matching-1.0.5/cupid_matching/docs/min_distance.md
+-rw-r--r--   0        0        0       69 2023-03-24 00:23:01.182377 cupid_matching-1.0.5/cupid_matching/docs/min_distance_utils.md
+-rw-r--r--   0        0        0       59 2023-03-24 00:27:46.673143 cupid_matching-1.0.5/cupid_matching/docs/model_classes.md
+-rw-r--r--   0        0        0       58 2023-03-24 00:23:19.684703 cupid_matching-1.0.5/cupid_matching/docs/nested_logit.md
+-rw-r--r--   0        0        0       55 2023-03-24 00:27:33.384226 cupid_matching-1.0.5/cupid_matching/docs/poisson_glm.md
+-rw-r--r--   0        0        0       67 2023-03-24 00:27:42.792605 cupid_matching-1.0.5/cupid_matching/docs/poisson_glm_utils.md
+-rw-r--r--   0        0        0       43 2023-03-24 00:27:23.096924 cupid_matching-1.0.5/cupid_matching/docs/utils.md
+-rw-r--r--   0        0        0    11551 2023-04-02 19:15:11.050530 cupid_matching-1.0.5/cupid_matching/entropy.py
+-rw-r--r--   0        0        0     3499 2023-04-02 19:12:57.727887 cupid_matching-1.0.5/cupid_matching/example_choosiow.py
+-rw-r--r--   0        0        0     4133 2023-04-02 19:13:08.597638 cupid_matching-1.0.5/cupid_matching/example_nestedlogit.py
+-rw-r--r--   0        0        0    26548 2023-04-02 19:13:28.516760 cupid_matching-1.0.5/cupid_matching/ipfp_solvers.py
+-rw-r--r--   0        0        0     8743 2023-04-02 13:02:37.290279 cupid_matching-1.0.5/cupid_matching/matching_utils.py
+-rw-r--r--   0        0        0    11551 2023-04-02 19:13:54.856938 cupid_matching-1.0.5/cupid_matching/min_distance.py
+-rw-r--r--   0        0        0     5260 2023-04-02 19:13:40.696373 cupid_matching-1.0.5/cupid_matching/min_distance_utils.py
+-rw-r--r--   0        0        0     1873 2023-04-02 13:02:37.291292 cupid_matching-1.0.5/cupid_matching/mkdocs.yml
+-rw-r--r--   0        0        0    16277 2023-04-02 19:15:11.063645 cupid_matching-1.0.5/cupid_matching/model_classes.py
+-rw-r--r--   0        0        0      369 2023-04-02 19:14:11.059995 cupid_matching-1.0.5/cupid_matching/mypy.ini
+-rw-r--r--   0        0        0     9515 2023-04-02 19:15:11.064847 cupid_matching-1.0.5/cupid_matching/nested_logit.py
+-rw-r--r--   0        0        0     7401 2023-04-02 19:15:11.067470 cupid_matching-1.0.5/cupid_matching/poisson_glm.py
+-rw-r--r--   0        0        0     6544 2023-04-02 19:14:50.571051 cupid_matching-1.0.5/cupid_matching/poisson_glm_utils.py
+-rw-r--r--   0        0        0    17888 2023-04-12 19:26:29.373052 cupid_matching-1.0.5/cupid_matching/site/404.html
+-rw-r--r--   0        0        0      704 2023-04-12 19:26:29.309599 cupid_matching-1.0.5/cupid_matching/site/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     1870 2023-04-12 19:26:29.310373 cupid_matching-1.0.5/cupid_matching/site/assets/images/favicon.png
+-rw-r--r--   0        0        0    17074 2023-04-12 19:26:29.311600 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2023-04-12 19:26:29.312037 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2023-04-12 19:26:29.312251 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2023-04-12 19:26:29.312426 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2023-04-12 19:26:29.312902 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2023-04-12 19:26:29.313341 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2023-04-12 19:26:29.313561 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2023-04-12 19:26:29.314020 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2023-04-12 19:26:29.314355 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0    11232 2023-04-12 19:26:29.314561 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2023-04-12 19:26:29.314763 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2023-04-12 19:26:29.315037 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     7973 2023-04-12 19:26:29.315327 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2023-04-12 19:26:29.315576 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2023-04-12 19:26:29.315839 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2023-04-12 19:26:29.316052 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2023-04-12 19:26:29.316272 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2023-04-12 19:26:29.316522 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2023-04-12 19:26:29.316751 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     3647 2023-04-12 19:26:29.317000 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2023-04-12 19:26:29.317173 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2023-04-12 19:26:29.317357 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     1031 2023-04-12 19:26:29.317572 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2023-04-12 19:26:29.318097 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2023-04-12 19:26:29.318370 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2062 2023-04-12 19:26:29.318588 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2023-04-12 19:26:29.318822 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677455 2023-04-12 19:26:29.319181 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    38916 2023-04-12 19:26:29.319522 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2023-04-12 19:26:29.319816 cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0    12355 2023-04-12 19:26:29.320580 cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css
+-rw-r--r--   0        0        0     3646 2023-04-12 19:26:29.320794 cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map
+-rw-r--r--   0        0        0    56388 2023-04-12 19:26:29.397202 cupid_matching-1.0.5/cupid_matching/site/choo_siow/index.html
+-rw-r--r--   0        0        0    61309 2023-04-12 19:26:29.411120 cupid_matching-1.0.5/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html
+-rw-r--r--   0        0        0    67113 2023-04-12 19:26:29.427864 cupid_matching-1.0.5/cupid_matching/site/choo_siow_heteroskedastic/index.html
+-rw-r--r--   0        0        0    19453 2023-04-12 19:26:29.428738 cupid_matching-1.0.5/cupid_matching/site/cupid_streamlit/index.html
+-rw-r--r--   0        0        0    52734 2023-04-12 19:26:29.439005 cupid_matching-1.0.5/cupid_matching/site/entropy/index.html
+-rw-r--r--   0        0        0    24288 2023-04-12 19:26:29.383321 cupid_matching-1.0.5/cupid_matching/site/index.html
+-rw-r--r--   0        0        0   171028 2023-04-12 19:26:29.510337 cupid_matching-1.0.5/cupid_matching/site/ipfp_solvers/index.html
+-rw-r--r--   0        0        0    33535 2023-04-12 19:26:29.516154 cupid_matching-1.0.5/cupid_matching/site/matching_utils/index.html
+-rw-r--r--   0        0        0    73534 2023-04-12 19:26:29.536810 cupid_matching-1.0.5/cupid_matching/site/min_distance/index.html
+-rw-r--r--   0        0        0    48540 2023-04-12 19:26:29.548044 cupid_matching-1.0.5/cupid_matching/site/min_distance_utils/index.html
+-rw-r--r--   0        0        0   158026 2023-04-12 19:26:29.603190 cupid_matching-1.0.5/cupid_matching/site/model_classes/index.html
+-rw-r--r--   0        0        0    80301 2023-04-12 19:26:29.625018 cupid_matching-1.0.5/cupid_matching/site/nested_logit/index.html
+-rw-r--r--   0        0        0      864 2023-04-12 19:26:29.310029 cupid_matching-1.0.5/cupid_matching/site/objects.inv
+-rw-r--r--   0        0        0    70696 2023-04-12 19:26:29.645184 cupid_matching-1.0.5/cupid_matching/site/poisson_glm/index.html
+-rw-r--r--   0        0        0    52629 2023-04-12 19:26:29.657841 cupid_matching-1.0.5/cupid_matching/site/poisson_glm_utils/index.html
+-rw-r--r--   0        0        0   179908 2023-04-12 19:26:29.695697 cupid_matching-1.0.5/cupid_matching/site/search/search_index.json
+-rw-r--r--   0        0        0     3235 2023-04-12 19:26:29.374434 cupid_matching-1.0.5/cupid_matching/site/sitemap.xml
+-rw-r--r--   0        0        0      354 2023-04-12 19:26:29.374610 cupid_matching-1.0.5/cupid_matching/site/sitemap.xml.gz
+-rw-r--r--   0        0        0   120234 2023-04-12 19:26:29.694954 cupid_matching-1.0.5/cupid_matching/site/utils/index.html
+-rw-r--r--   0        0        0    12373 2023-04-02 19:15:05.244218 cupid_matching-1.0.5/cupid_matching/utils.py
+-rw-r--r--   0        0        0      969 2023-04-12 19:22:27.062349 cupid_matching-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 cupid_matching-1.0.5/PKG-INFO
```

### Comparing `cupid_matching-1.0.4/README.md` & `cupid_matching-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,7 +37,9 @@
 * as a consequence,  the `numeric` versions of the minimum distance estimator (which use numerical derivatives) are not recommended. 
 * the bias-corrected minimum distance estimator (`corrected`) may have a larger mean-squared error and/or introduce numerical instabilities.
 ## Release notes
 ### version 1.0.4
 * added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.
 * added two complete examples: [example_choosiow.py](example_choosiow.md) and [example_nestedlogit.py](example_nestedlogit.md).
 
+### version 1,0.5
+* simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.
```

### Comparing `cupid_matching-1.0.4/cupid_matching/.idea/cupid_matching.iml` & `cupid_matching-1.0.5/cupid_matching/.idea/cupid_matching.iml`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/.idea/inspectionProfiles/Project_Default.xml` & `cupid_matching-1.0.5/cupid_matching/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/choo_siow.py` & `cupid_matching-1.0.5/cupid_matching/choo_siow.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """The components of the derivative of the entropy
 for the Choo and Siow homoskedastic model.
 """
-from typing import Any, Literal, Optional, Union, cast, overload
+from typing import Literal, Optional, Union, cast, overload
 
 import numpy as np
 
 from cupid_matching.entropy import EntropyFunctions, EntropyHessians
 from cupid_matching.matching_utils import Matching
-from cupid_matching.utils import FourArrays, ThreeArrays, TwoArrays, bs_error_abort, \
-    npmaxabs, nppow
+from cupid_matching.utils import FourArrays, ThreeArrays, TwoArrays, bs_error_abort
 
 
 @overload
 def _entropy_choo_siow(muhat: Matching, deriv: Literal[0]) -> np.ndarray:
     ...
 
 
@@ -23,15 +22,15 @@
 
 @overload
 def _entropy_choo_siow(muhat: Matching, deriv: Literal[2]) -> FourArrays:
     ...
 
 
 def _entropy_choo_siow(
-        muhat: Matching, deriv: Optional[int] = 0
+    muhat: Matching, deriv: Optional[int] = 0
 ) -> Union[None, np.ndarray, TwoArrays, FourArrays]:
     """Returns the values of $\\mathcal{E}$
     and the first (if `deriv` is 1 or 2) and second (if `deriv` is 2) derivatives
     for the Choo and Siow model
 
     Args:
         muhat: a Matching
@@ -49,19 +48,19 @@
     muxy, mux0, mu0y, n, m = muhat.unpack()
 
     logxy = np.log(muxy)
     logx0 = np.log(mux0)
     log0y = np.log(mu0y)
 
     val_entropy = (
-            -2.0 * np.sum(muxy * logxy)
-            - np.sum(mux0 * logx0)
-            - np.sum(mu0y * log0y)
-            + np.sum(n * np.log(n))
-            + np.sum(m * np.log(m))
+        -2.0 * np.sum(muxy * logxy)
+        - np.sum(mux0 * logx0)
+        - np.sum(mu0y * log0y)
+        + np.sum(n * np.log(n))
+        + np.sum(m * np.log(m))
     )
 
     if deriv == 0:
         return val_entropy
     if deriv in [1, 2]:
         der_xy = -2.0 * logxy + log0y
         der_xy += logx0.reshape((-1, 1))
@@ -86,47 +85,92 @@
                     der2_xyr[x, y, X + y] = derlog0y[y]
             return val_entropy, der_xy, der2_xyzt, der2_xyr
     else:
         bs_error_abort("deriv should be 0, 1, or 2")
         return None
 
 
+def _der_entropy_choo_siow_corrected(
+    muhat: Matching, hessian: Optional[bool] = False
+) -> Union[np.ndarray, ThreeArrays]:
+    """Returns the corrected first derivative of $\\mathcal{E}$
+    and the corrected second derivative (if `hessian` is True) 
+    for the Choo and Siow model
+
+    Args:
+        muhat: a Matching
+        hessian: if `True`, also compute the hessian
+
+    Returns:
+        the (X,Y) matrix of the first derivative of the entropy
+        if hessian is True, the (X,Y,X,Y) array of the second derivative
+            wrt $(\\mu,\\mu)$
+          and the (X,Y,X+Y) second derivatives
+            wrt $(\\mu,(n,m))$
+    """
+    muxy, mux0, mu0y, n, m = muhat.unpack()
+    n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)
+
+    muxy_corr = muxy + (1.0-muxy/n_households)/2.0
+    logxy = np.log(muxy_corr)
+    mux0_corr = mux0 + (1.0-mux0/n_households)/2.0
+    logx0 = np.log(mux0_corr)
+    mu0y_corr = mu0y + (1.0-mu0y/n_households)/2.0
+    log0y = np.log(mu0y_corr)
+
+    der_xy = -2.0 * logxy + log0y
+    der_xy += logx0.reshape((-1, 1))
+    if not hessian:
+        return der_xy
+    else:  # we compute the Hessians
+        X, Y = muxy.shape
+        f_corr = 1.0-1.0/n_households/2.0
+        derlogxy = f_corr / muxy_corr
+        derlogx0 = f_corr / mux0_corr
+        derlog0y = f_corr / mu0y_corr
+        der2_xyzt = np.zeros((X, Y, X, Y))
+        der2_xyr = np.zeros((X, Y, X + Y))
+        for x in range(X):
+            dlogx0 = derlogx0[x]
+            for y in range(Y):
+                d2xy = np.zeros((X, Y))
+                d2xy[x, :] = -dlogx0
+                d2xy[:, y] -= derlog0y[y]
+                d2xy[x, y] -= 2.0 * derlogxy[x, y]
+                der2_xyzt[x, y, :, :] = d2xy
+                der2_xyr[x, y, x] = derlogx0[x]
+                der2_xyr[x, y, X + y] = derlog0y[y]
+        return der_xy, der2_xyzt, der2_xyr
+
+
 def e0_fun_choo_siow(muhat: Matching) -> np.ndarray:
     """Returns the values of $e_0$ for the Choo and Siow model.
 
     Args:
         muhat: a Matching
 
     Returns:
         the (X,Y) matrix of the first derivative of the entropy
     """
     entropy_res = _entropy_choo_siow(muhat, deriv=1)
     return entropy_res[1]
 
 
-def e0_fun_choo_siow_corrected(
-        muhat: Matching
-) -> np.ndarray:
+def e0_fun_choo_siow_corrected(muhat: Matching) -> np.ndarray:
     """Returns the values of $e_0$ for the Choo and Siow model,
-    using the finite-sample correction.
+    using the finite-sample correction log(p+(1-p)/(2N))
 
     Args:
         muhat: a Matching
 
     Returns:
         the (X,Y) matrix of the first derivative of the entropy
     """
-    entropy_res = _entropy_choo_siow(muhat, deriv=1)
-    e0_val = entropy_res[1]
-    muxy, mux0, mu0y, *_ = muhat.unpack()
-    n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)
-    e0_val_corrected = e0_val - (1.0 - muxy / n_households) / muxy
-    e0_val_corrected += ((1.0 - mux0 / n_households) / (2.0 * mux0)).reshape((-1, 1))
-    e0_val_corrected += ((1.0 - mu0y / n_households) / (2.0 * mu0y))
-    # print(f"{npmaxabs(e0_val_corrected/e0_val - 1.0)=}")
+    e0_val_corrected \
+        = _der_entropy_choo_siow_corrected(muhat, hessian=False)
     return e0_val_corrected
 
 
 def hessian_mumu_choo_siow(muhat: Matching) -> ThreeArrays:
     """Returns the derivatives of $e_0$ in $\\mu$
     for the Choo and Siow model.
 
@@ -148,39 +192,37 @@
             d2xy = hessmumu[x, y, :, :]
             hess_x[x, y, :] = d2xy[x, :]
             hess_y[x, y, :] = d2xy[:, y]
             hess_xy[x, y] = d2xy[x, y]
     return hess_x, hess_y, hess_xy
 
 
-def hessian_mumu_choo_siow_corrected(
-        muhat: Matching
-) -> ThreeArrays:
+def hessian_mumu_choo_siow_corrected(muhat: Matching) -> ThreeArrays:
     """Returns the derivatives of $e_0$ in $\\mu$
     for the Choo and Siow model, with the small sample correction
 
     Args:
         muhat: a Matching
 
     Returns:
         the three components of the hessian wrt $(\\mu,\\mu)$ of the entropy
     """
-    hess_x, hess_y, hess_xy = hessian_mumu_choo_siow(muhat)
-    muxy, mux0, mu0y, *_ = muhat.unpack()
-    n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)
-    X, Y = hess_xy.shape
-    corr_x0 = 1.0 / (2.0*mux0*mux0)
-    corr_0y = 1.0 / (2.0*mu0y*mu0y)
-    corr_xy = -1.0 / (muxy*muxy)
+    _, hessmumu, _ \
+        = _der_entropy_choo_siow_corrected(muhat, hessian=True)
+    muxy, *_ = muhat.unpack()
+    X, Y = muxy.shape
+    hess_x = np.zeros((X, Y, Y))
+    hess_y = np.zeros((X, Y, X))
+    hess_xy = np.zeros((X, Y))
     for x in range(X):
         for y in range(Y):
-            hess_x[x, y, y] += corr_x0[x]
-            hess_y[x, y, x] += corr_0y[y]
-            hess_xy[x, y] += corr_xy[x, y]
-
+            d2xy = hessmumu[x, y, :, :]
+            hess_x[x, y, :] = d2xy[x, :]
+            hess_y[x, y, :] = d2xy[:, y]
+            hess_xy[x, y] = d2xy[x, y]
     return hess_x, hess_y, hess_xy
 
 
 def hessian_mur_choo_siow(muhat: Matching) -> TwoArrays:
     """Returns the derivatives of $e_0$ in $r$
     for the Choo and Siow model.
 
@@ -200,35 +242,35 @@
         for y in range(Y):
             d2r = hessmur[x, y, :]
             hess_nx[x, y] = d2r[x]
             hess_my[x, y] = d2r[X + y]
     return hess_nx, hess_my
 
 
-def hessian_mur_choo_siow_corrected(
-        muhat: Matching
-) -> TwoArrays:
+def hessian_mur_choo_siow_corrected(muhat: Matching) -> TwoArrays:
     """Returns the derivatives of $e_0$ in $r$
     for the Choo and Siow model, with the small sample correction
 
     Args:
         muhat: a Matching
 
     Returns:
         the two components of the hessian wrt $(\\mu,r)$ of the entropy
     """
-    hess_nx, hess_my = hessian_mur_choo_siow(muhat)
-    _, mux0, mu0y, *_ = muhat.unpack()
-    corr_nx = 1.0 / (2.0*mux0*mux0)
-    corr_my = 1.0 / (2.0*mu0y*mu0y)
-    X, Y = mux0.size, mu0y.size
+    _, _, hessmur \
+        = _der_entropy_choo_siow_corrected(muhat, hessian=True)
+    muxy, *_ = muhat.unpack()
+    X, Y = muxy.shape
+    hess_nx = np.zeros((X, Y))
+    hess_my = np.zeros((X, Y))
     for x in range(X):
-        hess_my[x, :] += corr_my
-    for y in range(Y):
-        hess_nx[:, y] += corr_nx
+        for y in range(Y):
+            d2r = hessmur[x, y, :]
+            hess_nx[x, y] = d2r[x]
+            hess_my[x, y] = d2r[X + y]
     return hess_nx, hess_my
 
 
 e0_derivative_choo_siow = (hessian_mumu_choo_siow, hessian_mur_choo_siow)
 e0_derivative_choo_siow_corrected = (
     hessian_mumu_choo_siow_corrected,
     hessian_mur_choo_siow_corrected,
```

### Comparing `cupid_matching-1.0.4/cupid_matching/choo_siow_gender_heteroskedastic.py` & `cupid_matching-1.0.5/cupid_matching/choo_siow_gender_heteroskedastic.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/choo_siow_heteroskedastic.py` & `cupid_matching-1.0.5/cupid_matching/choo_siow_heteroskedastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 We normalize the standard error for X=1 at 1, and we estimate the standard errors
 for all other types on the X side and for all types on the Y side.
 """
 from typing import cast
 
 import numpy as np
 
-from .entropy import EntropyFunctions, EntropyHessians
-from .matching_utils import Matching
-from .utils import ThreeArrays, TwoArrays
+from cupid_matching.entropy import EntropyFunctions, EntropyHessians
+from cupid_matching.matching_utils import Matching
+from cupid_matching.utils import ThreeArrays, TwoArrays
 
 
 def e0_choo_siow_heteroskedastic(muhat: Matching) -> np.ndarray:
     """Returns the values of the parameter-independent part $e_0$
     for the Choo and Siow heteroskedastic model;
     we normalized $\\sigma_1=1$
```

### Comparing `cupid_matching-1.0.4/cupid_matching/cupid_streamlit.py` & `cupid_matching-1.0.5/cupid_matching/cupid_streamlit.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/docs/index.md` & `cupid_matching-1.0.5/cupid_matching/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,7 +37,9 @@
 * as a consequence,  the `numeric` versions of the minimum distance estimator (which use numerical derivatives) are not recommended. 
 * the bias-corrected minimum distance estimator (`corrected`) may have a larger mean-squared error and/or introduce numerical instabilities.
 ## Release notes
 ### version 1.0.4
 * added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.
 * added two complete examples: [example_choosiow.py](example_choosiow.md) and [example_nestedlogit.py](example_nestedlogit.md).
 
+### version 1,0.5
+* simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.
```

### Comparing `cupid_matching-1.0.4/cupid_matching/entropy.py` & `cupid_matching-1.0.5/cupid_matching/entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Entropies and their derivatives. """
 from dataclasses import dataclass
 from functools import partial
 from typing import Any, Callable, Literal, Optional, cast
 
 import numpy as np
 
-from cupid_matching.matching_utils import Matching, MatchingFunction, MatchingFunctionParam
+from cupid_matching.matching_utils import (
+    Matching,
+    MatchingFunction,
+    MatchingFunctionParam,
+)
 from cupid_matching.utils import _EPS, _TWO_EPS, ThreeArrays, TwoArrays, bs_error_abort
 
 EntropyHessianMuMu = Callable[[Matching], ThreeArrays]
 """The type of a function that takes in a Matching
    and returns the three components of the hessian of the entropy
    wrt $(\\mu,\\mu)$.
 """
```

### Comparing `cupid_matching-1.0.4/cupid_matching/example_choosiow.py` & `cupid_matching-1.0.5/cupid_matching/example_choosiow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """ example using the Choo and Siow homoskedastic model"""
 
-import numpy as np
 from typing import Optional, Tuple
 
-from cupid_matching.model_classes import ChooSiowPrimitives, Matching
-from cupid_matching.entropy import EntropyFunctions
+import numpy as np
+
 from cupid_matching.choo_siow import (
     entropy_choo_siow,
     entropy_choo_siow_corrected,
-    entropy_choo_siow_numeric,
     entropy_choo_siow_corrected_numeric,
+    entropy_choo_siow_numeric,
 )
+from cupid_matching.entropy import EntropyFunctions
 from cupid_matching.min_distance import estimate_semilinear_mde
+from cupid_matching.model_classes import ChooSiowPrimitives, Matching
 from cupid_matching.poisson_glm import choo_siow_poisson_glm
-from cupid_matching.matching_utils import _variance_muhat, _variance_diagonal
 from cupid_matching.utils import print_stars
 
 
-def create_choosiow_population(X: int, Y: int, K: int,
-                               std_betas: Optional[float] = 1.0) \
-        -> Tuple[ChooSiowPrimitives, np.ndarray, np.ndarray]:
+def create_choosiow_population(
+    X: int, Y: int, K: int, std_betas: Optional[float] = 1.0
+) -> Tuple[ChooSiowPrimitives, np.ndarray, np.ndarray]:
     """
     we simulate a Choo and Siow population
     with equal numbers of men and women of each type
     and random bases dunctions and coefficients
 
         Args:
          X: number of types of men
@@ -40,52 +40,71 @@
     n = np.ones(X)
     m = np.ones(Y)
     Phi = phi_bases @ betas_true
     choo_siow_instance = ChooSiowPrimitives(Phi, n, m)
     return choo_siow_instance, phi_bases, betas_true
 
 
-def mde_estimate(mus_sim: Matching,
-                 phi_bases: np.ndarray,
-                 betas_true: np.ndarray,
-                 entropy: EntropyFunctions,
-                 title: str) -> float:
+def mde_estimate(
+    mus_sim: Matching,
+    phi_bases: np.ndarray,
+    betas_true: np.ndarray,
+    entropy: EntropyFunctions,
+    title: str,
+) -> float:
     """we estimate the parameters using the minimum distance estimator
 
     Args:
         mus_sim: a Choo and Siow Matching
         phi_bases: the basis functions
         betas_true: their true coefficients
         entropy: the entropy functions we use
         title: the name of the estimator
 
     Returns:
         the largest absolute difference between the true and estimated coefficients
     """
     print_stars(f"    {title}")
-    mde_results = estimate_semilinear_mde(
-        mus_sim, phi_bases, entropy
-    )
+    mde_results = estimate_semilinear_mde(mus_sim, phi_bases, entropy)
     mde_discrepancy = mde_results.print_results(true_coeffs=betas_true)
     return mde_discrepancy
 
 
 choo_siow_instance, phi_bases, betas_true = create_choosiow_population(10, 8, 5)
 mus_sim = choo_siow_instance.simulate(1e5)
 
 # we estimate using forur variants of the minimum distance estimator
-mde_discrepancy = mde_estimate(mus_sim, phi_bases, betas_true, entropy_choo_siow,
-                               "RESULTS FOR MDE WITH ANALYTICAL GRADIENT")
-mde_discrepancy_numeric = mde_estimate(mus_sim, phi_bases, betas_true, entropy_choo_siow_numeric,
-                                       "RESULTS FOR MDE WITH NUMERICAL GRADIENT")
-mde_discrepancy_corrected = mde_estimate(mus_sim, phi_bases, betas_true, entropy_choo_siow_corrected,
-                                         "RESULTS FOR THE CORRECTED MDE WITH ANALYTICAL GRADIENT")
-mde_discrepancy_corrected_numeric = mde_estimate(mus_sim, phi_bases, betas_true,
-                                                 entropy_choo_siow_corrected_numeric,
-                                                 "RESULTS FOR THE CORRECTED MDE WITH NUMERICAL GRADIENT")
+mde_discrepancy = mde_estimate(
+    mus_sim,
+    phi_bases,
+    betas_true,
+    entropy_choo_siow,
+    "RESULTS FOR MDE WITH ANALYTICAL GRADIENT",
+)
+mde_discrepancy_numeric = mde_estimate(
+    mus_sim,
+    phi_bases,
+    betas_true,
+    entropy_choo_siow_numeric,
+    "RESULTS FOR MDE WITH NUMERICAL GRADIENT",
+)
+mde_discrepancy_corrected = mde_estimate(
+    mus_sim,
+    phi_bases,
+    betas_true,
+    entropy_choo_siow_corrected,
+    "RESULTS FOR THE CORRECTED MDE WITH ANALYTICAL GRADIENT",
+)
+mde_discrepancy_corrected_numeric = mde_estimate(
+    mus_sim,
+    phi_bases,
+    betas_true,
+    entropy_choo_siow_corrected_numeric,
+    "RESULTS FOR THE CORRECTED MDE WITH NUMERICAL GRADIENT",
+)
 
 # we also estimate using Poisson GLM
 print_stars("    RESULTS FOR POISSON   ")
 poisson_results = choo_siow_poisson_glm(mus_sim, phi_bases)
 muxy_sim, mux0_sim, mu0y_sim, n_sim, m_sim = mus_sim.unpack()
 poisson_discrepancy = poisson_results.print_results(
     betas_true,
```

### Comparing `cupid_matching-1.0.4/cupid_matching/example_nestedlogit.py` & `cupid_matching-1.0.5/cupid_matching/example_nestedlogit.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,38 @@
 One nest on each side must consist of the 0 option.
 The other nests are specified as nested lists.
 E.g. [[1, 3], [2,4]] describes two nests, one with types 1 and 3,
 and the other with types 2 and 4.
 On each side, the nests are the same for each type, with the same parameters.
 """
 
-import numpy as np
 from typing import Optional, Tuple
 
-from cupid_matching.model_classes import Matching, NestedLogitPrimitives
-from cupid_matching.entropy import EntropyFunctions
-from cupid_matching.nested_logit import setup_standard_nested_logit
+import numpy as np
 
+from cupid_matching.entropy import EntropyFunctions
 from cupid_matching.min_distance import estimate_semilinear_mde
-from cupid_matching.matching_utils import _variance_muhat, _variance_diagonal
+from cupid_matching.model_classes import Matching, NestedLogitPrimitives
+from cupid_matching.nested_logit import setup_standard_nested_logit
 from cupid_matching.utils import print_stars
 
 
-def create_nestedlogit_population(X: int, Y: int, K: int,
-                                  std_alphas: Optional[float] = 0.5,
-                                  std_betas: Optional[float] = 1.0) \
-        -> Tuple[NestedLogitPrimitives, np.ndarray, np.ndarray, EntropyFunctions, EntropyFunctions]:
+def create_nestedlogit_population(
+    X: int,
+    Y: int,
+    K: int,
+    std_alphas: Optional[float] = 0.5,
+    std_betas: Optional[float] = 1.0,
+) -> Tuple[
+    NestedLogitPrimitives,
+    np.ndarray,
+    np.ndarray,
+    EntropyFunctions,
+    EntropyFunctions,
+]:
     """
     we simulate a nested logit population
     with equal numbers of men and women of each type
     and random bases dunctions and coefficients
 
         Args:
          X: number of types of men
@@ -49,58 +57,85 @@
         list(range(X // 2 + 1, X + 1)),
     ]
 
     n = np.ones(X)
     m = np.ones(Y)
     phi_bases = np.random.randn(X, Y, K)
 
-    entropy_nested_logit, entropy_nested_logit_numeric = setup_standard_nested_logit(nests_for_each_x,
-                                                                                     nests_for_each_y)
+    (
+        entropy_nested_logit,
+        entropy_nested_logit_numeric,
+    ) = setup_standard_nested_logit(nests_for_each_x, nests_for_each_y)
     n_rhos, n_deltas = len(nests_for_each_x), len(nests_for_each_y)
     n_alphas = n_rhos + n_deltas
 
     betas_true = std_betas * np.random.randn(K)
     alphas_true = std_alphas * np.random.uniform(size=n_alphas)
 
     Phi = phi_bases @ betas_true
     nested_logit_instance = NestedLogitPrimitives(
         Phi, n, m, nests_for_each_x, nests_for_each_y, alphas_true
     )
     true_coeffs = np.concatenate((alphas_true, betas_true))
-    return nested_logit_instance, phi_bases, true_coeffs, entropy_nested_logit, entropy_nested_logit_numeric
+    return (
+        nested_logit_instance,
+        phi_bases,
+        true_coeffs,
+        entropy_nested_logit,
+        entropy_nested_logit_numeric,
+    )
 
 
-def mde_estimate(mus_sim: Matching,
-                 phi_bases: np.ndarray,
-                 true_coeffs: np.ndarray,
-                 entropy: EntropyFunctions,
-                 title: str) -> float:
+def mde_estimate(
+    mus_sim: Matching,
+    phi_bases: np.ndarray,
+    true_coeffs: np.ndarray,
+    entropy: EntropyFunctions,
+    title: str,
+) -> float:
     """we estimate the parameters using the minimum distance estimator
 
     Args:
         mus_sim: a Choo and Siow Matching
         phi_bases: the basis functions
         true_coeffs: their true coefficients and  the nesting parameters
         entropy: the entropy functions we use
         title: the name of the estimator
 
     Returns:
         the largest absolute difference between the true and estimated coefficients
     """
     print_stars(f"    {title}")
     mde_results = estimate_semilinear_mde(
-        mus_sim, phi_bases, entropy,
+        mus_sim,
+        phi_bases,
+        entropy,
         additional_parameters=entropy.additional_parameters,
     )
     mde_discrepancy = mde_results.print_results(true_coeffs=true_coeffs)
     return mde_discrepancy
 
 
-nested_logit_instance, phi_bases, true_coeffs, entropy_nested_logit, entropy_nested_logit_numeric \
-    = create_nestedlogit_population(20, 18, 6)
+(
+    nested_logit_instance,
+    phi_bases,
+    true_coeffs,
+    entropy_nested_logit,
+    entropy_nested_logit_numeric,
+) = create_nestedlogit_population(20, 18, 6)
 seed = 6475788
 n_households = 1e6
 mus_sim = nested_logit_instance.simulate(n_households, seed)
-mde_discrepancy = mde_estimate(mus_sim, phi_bases, true_coeffs, entropy_nested_logit,
-                               "RESULTS FOR MDE WITH ANALYTICAL GRADIENT")
-mde_discrepancy_numeric = mde_estimate(mus_sim, phi_bases, true_coeffs, entropy_nested_logit_numeric,
-                                       "RESULTS FOR MDE WITH NUMERICAL GRADIENT")
+mde_discrepancy = mde_estimate(
+    mus_sim,
+    phi_bases,
+    true_coeffs,
+    entropy_nested_logit,
+    "RESULTS FOR MDE WITH ANALYTICAL GRADIENT",
+)
+mde_discrepancy_numeric = mde_estimate(
+    mus_sim,
+    phi_bases,
+    true_coeffs,
+    entropy_nested_logit_numeric,
+    "RESULTS FOR MDE WITH NUMERICAL GRADIENT",
+)
```

### Comparing `cupid_matching-1.0.4/cupid_matching/ipfp_solvers.py` & `cupid_matching-1.0.5/cupid_matching/ipfp_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 """
 from math import sqrt
 from typing import Literal, overload
 
 import numpy as np
 import scipy.linalg as spla
 
-from .matching_utils import Matching
-from .utils import (
+from cupid_matching.matching_utils import Matching
+from cupid_matching.utils import (
     bs_error_abort,
     der_nppow,
     npexp,
     npmaxabs,
     nppow,
     nprepeat_col,
     nprepeat_row,
```

### Comparing `cupid_matching-1.0.4/cupid_matching/matching_utils.py` & `cupid_matching-1.0.5/cupid_matching/matching_utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/min_distance.py` & `cupid_matching-1.0.5/cupid_matching/min_distance.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 """
 from typing import Optional, cast
 
 import numpy as np
 import scipy.linalg as spla
 import scipy.stats as sts
 
-from .entropy import (
+from cupid_matching.entropy import (
     EntropyFunctions,
     EntropyHessianMuMu,
     EntropyHessianMuMuParam,
     EntropyHessianMuR,
     EntropyHessianMuRParam,
     EntropyHessians,
     EntropyHessiansParam,
     _fill_hessianMuMu_from_components,
     _fill_hessianMuR_from_components,
     _numeric_hessian,
 )
-from .matching_utils import (
+from cupid_matching.matching_utils import (
     Matching,
     MatchingFunction,
     MatchingFunctionParam,
     _make_XY_K_mat,
     _variance_muhat,
 )
-from .min_distance_utils import MDEResults, _compute_estimates
-from .utils import bs_error_abort, print_stars
+from cupid_matching.min_distance_utils import MDEResults, _compute_estimates
+from cupid_matching.utils import bs_error_abort, print_stars
 
 
 def estimate_semilinear_mde(
     muhat: Matching,
     phi_bases: np.ndarray,
     entropy: EntropyFunctions,
     additional_parameters: Optional[list] = None,
```

### Comparing `cupid_matching-1.0.4/cupid_matching/min_distance_utils.py` & `cupid_matching-1.0.5/cupid_matching/min_distance_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 import scipy.linalg as spla
 
-from .utils import npmaxabs, print_stars
+from cupid_matching.utils import npmaxabs, print_stars
 
 
 def _compute_estimates(
     M: np.ndarray, S_mat: np.ndarray, d: np.ndarray
 ) -> tuple[np.ndarray, np.ndarray]:
     """Returns the QGLS estimates and their variance-covariance.
 
@@ -116,15 +116,17 @@
                 j = n_alpha + i
                 repr_str += (
                     f"   base {i + 1}: {true_coeffs[j]: > 10.3f}  "
                     + f"{coeff: > 10.3f}  ({stderrs[j]: > 10.3f})\n"
                 )
             print_stars(repr_str)
             discrepancy = npmaxabs(true_coeffs - estimates)
-            print_stars(f"The largest difference between true and estimated coefficients is {discrepancy: .2e}")
+            print_stars(
+                f"The largest difference between true and estimated coefficients is {discrepancy: .2e}"
+            )
         else:
             repr_str = (
                 "The estimated coefficients "
                 + "(and their standard errors) are\n\n"
             )
             for i, coeff in enumerate(estimates[:n_alpha]):
                 repr_str + f"{coeff: > 10.3f}  ({stderrs[i]: > 10.3f})\n"
```

### Comparing `cupid_matching-1.0.4/cupid_matching/mkdocs.yml` & `cupid_matching-1.0.5/cupid_matching/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/model_classes.py` & `cupid_matching-1.0.5/cupid_matching/model_classes.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/nested_logit.py` & `cupid_matching-1.0.5/cupid_matching/nested_logit.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 On each side, the nests are the same for each type, with the same parameters.
 """
 from math import log
 from typing import Any, cast
 
 import numpy as np
 
-from cupid_matching.entropy import (
-    EntropyFunctions,
-    EntropyHessianComponents,
-    EntropyHessiansParam,
-)
+from cupid_matching.entropy import EntropyFunctions, EntropyHessiansParam
 from cupid_matching.matching_utils import Matching, _change_indices
 from cupid_matching.utils import NestsList, ThreeArrays, TwoArrays
 
 
 def e0_nested_logit(
     muhat: Matching, additional_parameters: list[Any]
 ) -> np.ndarray:
```

### Comparing `cupid_matching-1.0.4/cupid_matching/poisson_glm.py` & `cupid_matching-1.0.5/cupid_matching/poisson_glm.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from typing import Optional
 
 import numpy as np
 import scipy.linalg as spla
 import scipy.sparse as spr
 from sklearn import linear_model
 
-from .matching_utils import Matching, _make_XY_K_mat, _variance_muhat
-from .poisson_glm_utils import PoissonGLMResults, _prepare_data
+from cupid_matching.matching_utils import Matching, _make_XY_K_mat, _variance_muhat
+from cupid_matching.poisson_glm_utils import PoissonGLMResults, _prepare_data
 
 
 def choo_siow_poisson_glm(
     muhat: Matching,
     phi_bases: np.ndarray,
     tol: Optional[float] = 1e-12,
     max_iter: Optional[int] = 10000,
```

### Comparing `cupid_matching-1.0.4/cupid_matching/poisson_glm_utils.py` & `cupid_matching-1.0.5/cupid_matching/poisson_glm_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 """
 
 from dataclasses import dataclass
 from typing import Optional, Tuple
 
 import numpy as np
 
-from .matching_utils import Matching
-from .utils import npmaxabs, print_stars
+from cupid_matching.matching_utils import Matching
+from cupid_matching.utils import npmaxabs, print_stars
 
 
 @dataclass
 class PoissonGLMResults:
     """Stores and formats the estimation results.
 
     Args:
@@ -134,15 +134,17 @@
                 repr_str += f" {coeff: > 10.3f}  ({stderrs_v[i]: > 10.3f})\n"
             print_stars(repr_str)
 
         if lambda_true is None:
             return None
         else:
             discrepancy = npmaxabs(lambda_true - estimates_beta)
-            print_stars(f"The largest difference between true and estimated coefficients is {discrepancy: .2e}")
+            print_stars(
+                f"The largest difference between true and estimated coefficients is {discrepancy: .2e}"
+            )
             return discrepancy
 
 
 def _prepare_data(
     muhat: Matching,
     var_muhat: np.ndarray,
     var_munm: np.ndarray,
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/404.html` & `cupid_matching-1.0.5/cupid_matching/site/404.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/_mkdocstrings.css` & `cupid_matching-1.0.5/cupid_matching/site/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/images/favicon.png` & `cupid_matching-1.0.5/cupid_matching/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/tinyseg.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/lunr/wordcut.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map` & `cupid_matching-1.0.5/cupid_matching/site/assets/javascripts/workers/search.208ed371.min.js.map`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css` & `cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map` & `cupid_matching-1.0.5/cupid_matching/site/assets/stylesheets/palette.a0c5b2b5.min.css.map`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/choo_siow/index.html` & `cupid_matching-1.0.5/cupid_matching/site/choo_siow/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -777,25 +777,25 @@
           <td><p>the (X,Y) matrix of the first derivative of the entropy</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/choo_siow.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal"> 93</span>
-<span class="normal"> 94</span>
-<span class="normal"> 95</span>
-<span class="normal"> 96</span>
-<span class="normal"> 97</span>
-<span class="normal"> 98</span>
-<span class="normal"> 99</span>
-<span class="normal">100</span>
-<span class="normal">101</span>
-<span class="normal">102</span>
-<span class="normal">103</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_fun_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">:</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">145</span>
+<span class="normal">146</span>
+<span class="normal">147</span>
+<span class="normal">148</span>
+<span class="normal">149</span>
+<span class="normal">150</span>
+<span class="normal">151</span>
+<span class="normal">152</span>
+<span class="normal">153</span>
+<span class="normal">154</span>
+<span class="normal">155</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_fun_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the values of $e_0$ for the Choo and Siow model.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
 
 <span class="sd">    Returns:</span>
 <span class="sd">        the (X,Y) matrix of the first derivative of the entropy</span>
@@ -817,15 +817,15 @@
 
 <a href="#cupid_matching.choo_siow.e0_fun_choo_siow_corrected" class="headerlink" title="Permanent link">&para;</a></h2>
 
 
   <div class="doc doc-contents ">
   
       <p>Returns the values of <span class="arithmatex"><span class="MathJax_Preview">e_0</span><script type="math/tex">e_0</script></span> for the Choo and Siow model,
-using the finite-sample correction.</p>
+using the finite-sample correction log(p+(1-p)/(2N))</p>
 
   <p><strong>Parameters:</strong></p>
   <table>
     <thead>
       <tr>
         <th>Name</th>
         <th>Type</th>
@@ -863,54 +863,38 @@
           <td><p>the (X,Y) matrix of the first derivative of the entropy</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/choo_siow.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">106</span>
-<span class="normal">107</span>
-<span class="normal">108</span>
-<span class="normal">109</span>
-<span class="normal">110</span>
-<span class="normal">111</span>
-<span class="normal">112</span>
-<span class="normal">113</span>
-<span class="normal">114</span>
-<span class="normal">115</span>
-<span class="normal">116</span>
-<span class="normal">117</span>
-<span class="normal">118</span>
-<span class="normal">119</span>
-<span class="normal">120</span>
-<span class="normal">121</span>
-<span class="normal">122</span>
-<span class="normal">123</span>
-<span class="normal">124</span>
-<span class="normal">125</span>
-<span class="normal">126</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_fun_choo_siow_corrected</span><span class="p">(</span>
-        <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span>
-<span class="p">)</span> <span class="o">-&gt;</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">:</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">158</span>
+<span class="normal">159</span>
+<span class="normal">160</span>
+<span class="normal">161</span>
+<span class="normal">162</span>
+<span class="normal">163</span>
+<span class="normal">164</span>
+<span class="normal">165</span>
+<span class="normal">166</span>
+<span class="normal">167</span>
+<span class="normal">168</span>
+<span class="normal">169</span>
+<span class="normal">170</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_fun_choo_siow_corrected</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the values of $e_0$ for the Choo and Siow model,</span>
-<span class="sd">    using the finite-sample correction.</span>
+<span class="sd">    using the finite-sample correction log(p+(1-p)/(2N))</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
 
 <span class="sd">    Returns:</span>
 <span class="sd">        the (X,Y) matrix of the first derivative of the entropy</span>
 <span class="sd">    &quot;&quot;&quot;</span>
-    <span class="n">entropy_res</span> <span class="o">=</span> <span class="n">_entropy_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">,</span> <span class="n">deriv</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
-    <span class="n">e0_val</span> <span class="o">=</span> <span class="n">entropy_res</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
-    <span class="n">muxy</span><span class="p">,</span> <span class="n">mux0</span><span class="p">,</span> <span class="n">mu0y</span><span class="p">,</span> <span class="o">*</span><span class="n">_</span> <span class="o">=</span> <span class="n">muhat</span><span class="o">.</span><span class="n">unpack</span><span class="p">()</span>
-    <span class="n">n_households</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">muxy</span><span class="p">)</span> <span class="o">+</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">mux0</span><span class="p">)</span> <span class="o">+</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">mu0y</span><span class="p">)</span>
-    <span class="n">e0_val_corrected</span> <span class="o">=</span> <span class="n">e0_val</span> <span class="o">-</span> <span class="p">(</span><span class="mf">1.0</span> <span class="o">-</span> <span class="n">muxy</span> <span class="o">/</span> <span class="n">n_households</span><span class="p">)</span> <span class="o">/</span> <span class="n">muxy</span>
-    <span class="n">e0_val_corrected</span> <span class="o">+=</span> <span class="p">((</span><span class="mf">1.0</span> <span class="o">-</span> <span class="n">mux0</span> <span class="o">/</span> <span class="n">n_households</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="mf">2.0</span> <span class="o">*</span> <span class="n">mux0</span><span class="p">))</span><span class="o">.</span><span class="n">reshape</span><span class="p">((</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">))</span>
-    <span class="n">e0_val_corrected</span> <span class="o">+=</span> <span class="p">((</span><span class="mf">1.0</span> <span class="o">-</span> <span class="n">mu0y</span> <span class="o">/</span> <span class="n">n_households</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="mf">2.0</span> <span class="o">*</span> <span class="n">mu0y</span><span class="p">))</span>
-    <span class="c1"># print(f&quot;{npmaxabs(e0_val_corrected/e0_val - 1.0)=}&quot;)</span>
+    <span class="n">e0_val_corrected</span> \
+        <span class="o">=</span> <span class="n">_der_entropy_choo_siow_corrected</span><span class="p">(</span><span class="n">muhat</span><span class="p">,</span> <span class="n">hessian</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
     <span class="k">return</span> <span class="n">e0_val_corrected</span>
 </code></pre></div></td></tr></table></div>
       </details>
   </div>
 
 </div>
 
@@ -969,38 +953,38 @@
           <td><p>the three components of the hessian wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,\mu)</span><script type="math/tex">(\mu,\mu)</script></span> of the entropy</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/choo_siow.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">129</span>
-<span class="normal">130</span>
-<span class="normal">131</span>
-<span class="normal">132</span>
-<span class="normal">133</span>
-<span class="normal">134</span>
-<span class="normal">135</span>
-<span class="normal">136</span>
-<span class="normal">137</span>
-<span class="normal">138</span>
-<span class="normal">139</span>
-<span class="normal">140</span>
-<span class="normal">141</span>
-<span class="normal">142</span>
-<span class="normal">143</span>
-<span class="normal">144</span>
-<span class="normal">145</span>
-<span class="normal">146</span>
-<span class="normal">147</span>
-<span class="normal">148</span>
-<span class="normal">149</span>
-<span class="normal">150</span>
-<span class="normal">151</span>
-<span class="normal">152</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mumu_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ThreeArrays</span><span class="p">:</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">173</span>
+<span class="normal">174</span>
+<span class="normal">175</span>
+<span class="normal">176</span>
+<span class="normal">177</span>
+<span class="normal">178</span>
+<span class="normal">179</span>
+<span class="normal">180</span>
+<span class="normal">181</span>
+<span class="normal">182</span>
+<span class="normal">183</span>
+<span class="normal">184</span>
+<span class="normal">185</span>
+<span class="normal">186</span>
+<span class="normal">187</span>
+<span class="normal">188</span>
+<span class="normal">189</span>
+<span class="normal">190</span>
+<span class="normal">191</span>
+<span class="normal">192</span>
+<span class="normal">193</span>
+<span class="normal">194</span>
+<span class="normal">195</span>
+<span class="normal">196</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mumu_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ThreeArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of $e_0$ in $\\mu$</span>
 <span class="sd">    for the Choo and Siow model.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
 
 <span class="sd">    Returns:</span>
@@ -1081,64 +1065,60 @@
           <td><p>the three components of the hessian wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,\mu)</span><script type="math/tex">(\mu,\mu)</script></span> of the entropy</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/choo_siow.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">155</span>
-<span class="normal">156</span>
-<span class="normal">157</span>
-<span class="normal">158</span>
-<span class="normal">159</span>
-<span class="normal">160</span>
-<span class="normal">161</span>
-<span class="normal">162</span>
-<span class="normal">163</span>
-<span class="normal">164</span>
-<span class="normal">165</span>
-<span class="normal">166</span>
-<span class="normal">167</span>
-<span class="normal">168</span>
-<span class="normal">169</span>
-<span class="normal">170</span>
-<span class="normal">171</span>
-<span class="normal">172</span>
-<span class="normal">173</span>
-<span class="normal">174</span>
-<span class="normal">175</span>
-<span class="normal">176</span>
-<span class="normal">177</span>
-<span class="normal">178</span>
-<span class="normal">179</span>
-<span class="normal">180</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mumu_choo_siow_corrected</span><span class="p">(</span>
-        <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span>
-<span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ThreeArrays</span><span class="p">:</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">199</span>
+<span class="normal">200</span>
+<span class="normal">201</span>
+<span class="normal">202</span>
+<span class="normal">203</span>
+<span class="normal">204</span>
+<span class="normal">205</span>
+<span class="normal">206</span>
+<span class="normal">207</span>
+<span class="normal">208</span>
+<span class="normal">209</span>
+<span class="normal">210</span>
+<span class="normal">211</span>
+<span class="normal">212</span>
+<span class="normal">213</span>
+<span class="normal">214</span>
+<span class="normal">215</span>
+<span class="normal">216</span>
+<span class="normal">217</span>
+<span class="normal">218</span>
+<span class="normal">219</span>
+<span class="normal">220</span>
+<span class="normal">221</span>
+<span class="normal">222</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mumu_choo_siow_corrected</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ThreeArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of $e_0$ in $\\mu$</span>
 <span class="sd">    for the Choo and Siow model, with the small sample correction</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
 
 <span class="sd">    Returns:</span>
 <span class="sd">        the three components of the hessian wrt $(\\mu,\\mu)$ of the entropy</span>
 <span class="sd">    &quot;&quot;&quot;</span>
-    <span class="n">hess_x</span><span class="p">,</span> <span class="n">hess_y</span><span class="p">,</span> <span class="n">hess_xy</span> <span class="o">=</span> <span class="n">hessian_mumu_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">)</span>
-    <span class="n">muxy</span><span class="p">,</span> <span class="n">mux0</span><span class="p">,</span> <span class="n">mu0y</span><span class="p">,</span> <span class="o">*</span><span class="n">_</span> <span class="o">=</span> <span class="n">muhat</span><span class="o">.</span><span class="n">unpack</span><span class="p">()</span>
-    <span class="n">n_households</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">muxy</span><span class="p">)</span> <span class="o">+</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">mux0</span><span class="p">)</span> <span class="o">+</span> <span class="n">np</span><span class="o">.</span><span class="n">sum</span><span class="p">(</span><span class="n">mu0y</span><span class="p">)</span>
-    <span class="n">X</span><span class="p">,</span> <span class="n">Y</span> <span class="o">=</span> <span class="n">hess_xy</span><span class="o">.</span><span class="n">shape</span>
-    <span class="n">corr_x0</span> <span class="o">=</span> <span class="mf">1.0</span> <span class="o">/</span> <span class="p">(</span><span class="mf">2.0</span><span class="o">*</span><span class="n">mux0</span><span class="o">*</span><span class="n">mux0</span><span class="p">)</span>
-    <span class="n">corr_0y</span> <span class="o">=</span> <span class="mf">1.0</span> <span class="o">/</span> <span class="p">(</span><span class="mf">2.0</span><span class="o">*</span><span class="n">mu0y</span><span class="o">*</span><span class="n">mu0y</span><span class="p">)</span>
-    <span class="n">corr_xy</span> <span class="o">=</span> <span class="o">-</span><span class="mf">1.0</span> <span class="o">/</span> <span class="p">(</span><span class="n">muxy</span><span class="o">*</span><span class="n">muxy</span><span class="p">)</span>
+    <span class="n">_</span><span class="p">,</span> <span class="n">hessmumu</span><span class="p">,</span> <span class="n">_</span> \
+        <span class="o">=</span> <span class="n">_der_entropy_choo_siow_corrected</span><span class="p">(</span><span class="n">muhat</span><span class="p">,</span> <span class="n">hessian</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+    <span class="n">muxy</span><span class="p">,</span> <span class="o">*</span><span class="n">_</span> <span class="o">=</span> <span class="n">muhat</span><span class="o">.</span><span class="n">unpack</span><span class="p">()</span>
+    <span class="n">X</span><span class="p">,</span> <span class="n">Y</span> <span class="o">=</span> <span class="n">muxy</span><span class="o">.</span><span class="n">shape</span>
+    <span class="n">hess_x</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">zeros</span><span class="p">((</span><span class="n">X</span><span class="p">,</span> <span class="n">Y</span><span class="p">,</span> <span class="n">Y</span><span class="p">))</span>
+    <span class="n">hess_y</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">zeros</span><span class="p">((</span><span class="n">X</span><span class="p">,</span> <span class="n">Y</span><span class="p">,</span> <span class="n">X</span><span class="p">))</span>
+    <span class="n">hess_xy</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">zeros</span><span class="p">((</span><span class="n">X</span><span class="p">,</span> <span class="n">Y</span><span class="p">))</span>
     <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">X</span><span class="p">):</span>
         <span class="k">for</span> <span class="n">y</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">Y</span><span class="p">):</span>
-            <span class="n">hess_x</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">y</span><span class="p">]</span> <span class="o">+=</span> <span class="n">corr_x0</span><span class="p">[</span><span class="n">x</span><span class="p">]</span>
-            <span class="n">hess_y</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="n">x</span><span class="p">]</span> <span class="o">+=</span> <span class="n">corr_0y</span><span class="p">[</span><span class="n">y</span><span class="p">]</span>
-            <span class="n">hess_xy</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">]</span> <span class="o">+=</span> <span class="n">corr_xy</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">]</span>
-
+            <span class="n">d2xy</span> <span class="o">=</span> <span class="n">hessmumu</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="p">:,</span> <span class="p">:]</span>
+            <span class="n">hess_x</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="p">:]</span> <span class="o">=</span> <span class="n">d2xy</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="p">:]</span>
+            <span class="n">hess_y</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="p">:]</span> <span class="o">=</span> <span class="n">d2xy</span><span class="p">[:,</span> <span class="n">y</span><span class="p">]</span>
+            <span class="n">hess_xy</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">]</span> <span class="o">=</span> <span class="n">d2xy</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">]</span>
     <span class="k">return</span> <span class="n">hess_x</span><span class="p">,</span> <span class="n">hess_y</span><span class="p">,</span> <span class="n">hess_xy</span>
 </code></pre></div></td></tr></table></div>
       </details>
   </div>
 
 </div>
 
@@ -1197,36 +1177,36 @@
           <td><p>the two components of the hessian wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,r)</span><script type="math/tex">(\mu,r)</script></span> of the entropy</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/choo_siow.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">183</span>
-<span class="normal">184</span>
-<span class="normal">185</span>
-<span class="normal">186</span>
-<span class="normal">187</span>
-<span class="normal">188</span>
-<span class="normal">189</span>
-<span class="normal">190</span>
-<span class="normal">191</span>
-<span class="normal">192</span>
-<span class="normal">193</span>
-<span class="normal">194</span>
-<span class="normal">195</span>
-<span class="normal">196</span>
-<span class="normal">197</span>
-<span class="normal">198</span>
-<span class="normal">199</span>
-<span class="normal">200</span>
-<span class="normal">201</span>
-<span class="normal">202</span>
-<span class="normal">203</span>
-<span class="normal">204</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mur_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">TwoArrays</span><span class="p">:</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">225</span>
+<span class="normal">226</span>
+<span class="normal">227</span>
+<span class="normal">228</span>
+<span class="normal">229</span>
+<span class="normal">230</span>
+<span class="normal">231</span>
+<span class="normal">232</span>
+<span class="normal">233</span>
+<span class="normal">234</span>
+<span class="normal">235</span>
+<span class="normal">236</span>
+<span class="normal">237</span>
+<span class="normal">238</span>
+<span class="normal">239</span>
+<span class="normal">240</span>
+<span class="normal">241</span>
+<span class="normal">242</span>
+<span class="normal">243</span>
+<span class="normal">244</span>
+<span class="normal">245</span>
+<span class="normal">246</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mur_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">TwoArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of $e_0$ in $r$</span>
 <span class="sd">    for the Choo and Siow model.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
 
 <span class="sd">    Returns:</span>
@@ -1305,56 +1285,56 @@
           <td><p>the two components of the hessian wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,r)</span><script type="math/tex">(\mu,r)</script></span> of the entropy</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/choo_siow.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">207</span>
-<span class="normal">208</span>
-<span class="normal">209</span>
-<span class="normal">210</span>
-<span class="normal">211</span>
-<span class="normal">212</span>
-<span class="normal">213</span>
-<span class="normal">214</span>
-<span class="normal">215</span>
-<span class="normal">216</span>
-<span class="normal">217</span>
-<span class="normal">218</span>
-<span class="normal">219</span>
-<span class="normal">220</span>
-<span class="normal">221</span>
-<span class="normal">222</span>
-<span class="normal">223</span>
-<span class="normal">224</span>
-<span class="normal">225</span>
-<span class="normal">226</span>
-<span class="normal">227</span>
-<span class="normal">228</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mur_choo_siow_corrected</span><span class="p">(</span>
-        <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span>
-<span class="p">)</span> <span class="o">-&gt;</span> <span class="n">TwoArrays</span><span class="p">:</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">249</span>
+<span class="normal">250</span>
+<span class="normal">251</span>
+<span class="normal">252</span>
+<span class="normal">253</span>
+<span class="normal">254</span>
+<span class="normal">255</span>
+<span class="normal">256</span>
+<span class="normal">257</span>
+<span class="normal">258</span>
+<span class="normal">259</span>
+<span class="normal">260</span>
+<span class="normal">261</span>
+<span class="normal">262</span>
+<span class="normal">263</span>
+<span class="normal">264</span>
+<span class="normal">265</span>
+<span class="normal">266</span>
+<span class="normal">267</span>
+<span class="normal">268</span>
+<span class="normal">269</span>
+<span class="normal">270</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">hessian_mur_choo_siow_corrected</span><span class="p">(</span><span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">TwoArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of $e_0$ in $r$</span>
 <span class="sd">    for the Choo and Siow model, with the small sample correction</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
 
 <span class="sd">    Returns:</span>
 <span class="sd">        the two components of the hessian wrt $(\\mu,r)$ of the entropy</span>
 <span class="sd">    &quot;&quot;&quot;</span>
-    <span class="n">hess_nx</span><span class="p">,</span> <span class="n">hess_my</span> <span class="o">=</span> <span class="n">hessian_mur_choo_siow</span><span class="p">(</span><span class="n">muhat</span><span class="p">)</span>
-    <span class="n">_</span><span class="p">,</span> <span class="n">mux0</span><span class="p">,</span> <span class="n">mu0y</span><span class="p">,</span> <span class="o">*</span><span class="n">_</span> <span class="o">=</span> <span class="n">muhat</span><span class="o">.</span><span class="n">unpack</span><span class="p">()</span>
-    <span class="n">corr_nx</span> <span class="o">=</span> <span class="mf">1.0</span> <span class="o">/</span> <span class="p">(</span><span class="mf">2.0</span><span class="o">*</span><span class="n">mux0</span><span class="o">*</span><span class="n">mux0</span><span class="p">)</span>
-    <span class="n">corr_my</span> <span class="o">=</span> <span class="mf">1.0</span> <span class="o">/</span> <span class="p">(</span><span class="mf">2.0</span><span class="o">*</span><span class="n">mu0y</span><span class="o">*</span><span class="n">mu0y</span><span class="p">)</span>
-    <span class="n">X</span><span class="p">,</span> <span class="n">Y</span> <span class="o">=</span> <span class="n">mux0</span><span class="o">.</span><span class="n">size</span><span class="p">,</span> <span class="n">mu0y</span><span class="o">.</span><span class="n">size</span>
+    <span class="n">_</span><span class="p">,</span> <span class="n">_</span><span class="p">,</span> <span class="n">hessmur</span> \
+        <span class="o">=</span> <span class="n">_der_entropy_choo_siow_corrected</span><span class="p">(</span><span class="n">muhat</span><span class="p">,</span> <span class="n">hessian</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+    <span class="n">muxy</span><span class="p">,</span> <span class="o">*</span><span class="n">_</span> <span class="o">=</span> <span class="n">muhat</span><span class="o">.</span><span class="n">unpack</span><span class="p">()</span>
+    <span class="n">X</span><span class="p">,</span> <span class="n">Y</span> <span class="o">=</span> <span class="n">muxy</span><span class="o">.</span><span class="n">shape</span>
+    <span class="n">hess_nx</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">zeros</span><span class="p">((</span><span class="n">X</span><span class="p">,</span> <span class="n">Y</span><span class="p">))</span>
+    <span class="n">hess_my</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">zeros</span><span class="p">((</span><span class="n">X</span><span class="p">,</span> <span class="n">Y</span><span class="p">))</span>
     <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">X</span><span class="p">):</span>
-        <span class="n">hess_my</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="p">:]</span> <span class="o">+=</span> <span class="n">corr_my</span>
-    <span class="k">for</span> <span class="n">y</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">Y</span><span class="p">):</span>
-        <span class="n">hess_nx</span><span class="p">[:,</span> <span class="n">y</span><span class="p">]</span> <span class="o">+=</span> <span class="n">corr_nx</span>
+        <span class="k">for</span> <span class="n">y</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">Y</span><span class="p">):</span>
+            <span class="n">d2r</span> <span class="o">=</span> <span class="n">hessmur</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">,</span> <span class="p">:]</span>
+            <span class="n">hess_nx</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">]</span> <span class="o">=</span> <span class="n">d2r</span><span class="p">[</span><span class="n">x</span><span class="p">]</span>
+            <span class="n">hess_my</span><span class="p">[</span><span class="n">x</span><span class="p">,</span> <span class="n">y</span><span class="p">]</span> <span class="o">=</span> <span class="n">d2r</span><span class="p">[</span><span class="n">X</span> <span class="o">+</span> <span class="n">y</span><span class="p">]</span>
     <span class="k">return</span> <span class="n">hess_nx</span><span class="p">,</span> <span class="n">hess_my</span>
 </code></pre></div></td></tr></table></div>
       </details>
   </div>
 
 </div>
```

#### html2text {}

```diff
@@ -67,196 +67,186 @@
 Parameters:
 Name  Type     Description Default
 muhat Matching a Matching  required
 Returns:
 Type       Description
 np.ndarray the (X,Y) matrix of the first derivative of the entropy
  Source code in cupid_matching/choo_siow.py
- 93 def e0_fun_choo_siow(muhat: Matching) -> np.ndarray:
- 94     """Returns the values of $e_0$ for the Choo and Siow model.
- 95
- 96     Args:
- 97         muhat: a Matching
- 98
- 99     Returns:
-100         the (X,Y) matrix of the first derivative of the entropy
-101     """
-102     entropy_res = _entropy_choo_siow(muhat, deriv=1)
-103     return entropy_res[1]
+145 def e0_fun_choo_siow(muhat: Matching) -> np.ndarray:
+146     """Returns the values of $e_0$ for the Choo and Siow model.
+147
+148     Args:
+149         muhat: a Matching
+150
+151     Returns:
+152         the (X,Y) matrix of the first derivative of the entropy
+153     """
+154     entropy_res = _entropy_choo_siow(muhat, deriv=1)
+155     return entropy_res[1]
 ***** e0_fun_choo_siow_corrected(muhat) ¶ *****
 Returns the values of e_0
- for the Choo and Siow model, using the finite-sample correction.
+ for the Choo and Siow model, using the finite-sample correction log(p+(1-p)/
+(2N))
 Parameters:
 Name  Type     Description Default
 muhat Matching a Matching  required
 Returns:
 Type       Description
 np.ndarray the (X,Y) matrix of the first derivative of the entropy
  Source code in cupid_matching/choo_siow.py
-106 def e0_fun_choo_siow_corrected(
-107         muhat: Matching
-108 ) -> np.ndarray:
-109     """Returns the values of $e_0$ for the Choo and Siow model,
-110     using the finite-sample correction.
-111
-112     Args:
-113         muhat: a Matching
-114
-115     Returns:
-116         the (X,Y) matrix of the first derivative of the entropy
-117     """
-118     entropy_res = _entropy_choo_siow(muhat, deriv=1)
-119     e0_val = entropy_res[1]
-120     muxy, mux0, mu0y, *_ = muhat.unpack()
-121     n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)
-122     e0_val_corrected = e0_val - (1.0 - muxy / n_households) / muxy
-123     e0_val_corrected += ((1.0 - mux0 / n_households) / (2.0 *
-124 mux0)).reshape((-1, 1))
-125     e0_val_corrected += ((1.0 - mu0y / n_households) / (2.0 * mu0y))
-126     # print(f"{npmaxabs(e0_val_corrected/e0_val - 1.0)=}")
-        return e0_val_corrected
+158 def e0_fun_choo_siow_corrected(muhat: Matching) -> np.ndarray:
+159     """Returns the values of $e_0$ for the Choo and Siow model,
+160     using the finite-sample correction log(p+(1-p)/(2N))
+161
+162     Args:
+163         muhat: a Matching
+164
+165     Returns:
+166         the (X,Y) matrix of the first derivative of the entropy
+167     """
+168     e0_val_corrected \
+169         = _der_entropy_choo_siow_corrected(muhat, hessian=False)
+170     return e0_val_corrected
 ***** hessian_mumu_choo_siow(muhat) ¶ *****
 Returns the derivatives of e_0
  in \mu
  for the Choo and Siow model.
 Parameters:
 Name  Type     Description Default
 muhat Matching a Matching  required
 Returns:
 Type        Description
 ThreeArrays the three components of the hessian wrt (\mu,\mu)
              of the entropy
  Source code in cupid_matching/choo_siow.py
-129 def hessian_mumu_choo_siow(muhat: Matching) -> ThreeArrays:
-130     """Returns the derivatives of $e_0$ in $\\mu$
-131     for the Choo and Siow model.
-132
-133     Args:
-134         muhat: a Matching
-135
-136     Returns:
-137         the three components of the hessian wrt $(\\mu,\\mu)$ of the
-138 entropy
-139     """
-140     entropy_res = _entropy_choo_siow(muhat, deriv=2)
-141     hessmumu = entropy_res[2]
-142     muxy, *_ = muhat.unpack()
-143     X, Y = muxy.shape
-144     hess_x = np.zeros((X, Y, Y))
-145     hess_y = np.zeros((X, Y, X))
-146     hess_xy = np.zeros((X, Y))
-147     for x in range(X):
-148         for y in range(Y):
-149             d2xy = hessmumu[x, y, :, :]
-150             hess_x[x, y, :] = d2xy[x, :]
-151             hess_y[x, y, :] = d2xy[:, y]
-152             hess_xy[x, y] = d2xy[x, y]
+173 def hessian_mumu_choo_siow(muhat: Matching) -> ThreeArrays:
+174     """Returns the derivatives of $e_0$ in $\\mu$
+175     for the Choo and Siow model.
+176
+177     Args:
+178         muhat: a Matching
+179
+180     Returns:
+181         the three components of the hessian wrt $(\\mu,\\mu)$ of the
+182 entropy
+183     """
+184     entropy_res = _entropy_choo_siow(muhat, deriv=2)
+185     hessmumu = entropy_res[2]
+186     muxy, *_ = muhat.unpack()
+187     X, Y = muxy.shape
+188     hess_x = np.zeros((X, Y, Y))
+189     hess_y = np.zeros((X, Y, X))
+190     hess_xy = np.zeros((X, Y))
+191     for x in range(X):
+192         for y in range(Y):
+193             d2xy = hessmumu[x, y, :, :]
+194             hess_x[x, y, :] = d2xy[x, :]
+195             hess_y[x, y, :] = d2xy[:, y]
+196             hess_xy[x, y] = d2xy[x, y]
         return hess_x, hess_y, hess_xy
 ***** hessian_mumu_choo_siow_corrected(muhat) ¶ *****
 Returns the derivatives of e_0
  in \mu
  for the Choo and Siow model, with the small sample correction
 Parameters:
 Name  Type     Description Default
 muhat Matching a Matching  required
 Returns:
 Type        Description
 ThreeArrays the three components of the hessian wrt (\mu,\mu)
              of the entropy
  Source code in cupid_matching/choo_siow.py
-155 def hessian_mumu_choo_siow_corrected(
-156         muhat: Matching
-157 ) -> ThreeArrays:
-158     """Returns the derivatives of $e_0$ in $\\mu$
-159     for the Choo and Siow model, with the small sample correction
-160
-161     Args:
-162         muhat: a Matching
-163
-164     Returns:
-165         the three components of the hessian wrt $(\\mu,\\mu)$ of the
-166 entropy
-167     """
-168     hess_x, hess_y, hess_xy = hessian_mumu_choo_siow(muhat)
-169     muxy, mux0, mu0y, *_ = muhat.unpack()
-170     n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)
-171     X, Y = hess_xy.shape
-172     corr_x0 = 1.0 / (2.0*mux0*mux0)
-173     corr_0y = 1.0 / (2.0*mu0y*mu0y)
-174     corr_xy = -1.0 / (muxy*muxy)
-175     for x in range(X):
-176         for y in range(Y):
-177             hess_x[x, y, y] += corr_x0[x]
-178             hess_y[x, y, x] += corr_0y[y]
-179             hess_xy[x, y] += corr_xy[x, y]
-180
+199 def hessian_mumu_choo_siow_corrected(muhat: Matching) -> ThreeArrays:
+200     """Returns the derivatives of $e_0$ in $\\mu$
+201     for the Choo and Siow model, with the small sample correction
+202
+203     Args:
+204         muhat: a Matching
+205
+206     Returns:
+207         the three components of the hessian wrt $(\\mu,\\mu)$ of the
+208 entropy
+209     """
+210     _, hessmumu, _ \
+211         = _der_entropy_choo_siow_corrected(muhat, hessian=True)
+212     muxy, *_ = muhat.unpack()
+213     X, Y = muxy.shape
+214     hess_x = np.zeros((X, Y, Y))
+215     hess_y = np.zeros((X, Y, X))
+216     hess_xy = np.zeros((X, Y))
+217     for x in range(X):
+218         for y in range(Y):
+219             d2xy = hessmumu[x, y, :, :]
+220             hess_x[x, y, :] = d2xy[x, :]
+221             hess_y[x, y, :] = d2xy[:, y]
+222             hess_xy[x, y] = d2xy[x, y]
         return hess_x, hess_y, hess_xy
 ***** hessian_mur_choo_siow(muhat) ¶ *****
 Returns the derivatives of e_0
  in r
  for the Choo and Siow model.
 Parameters:
 Name  Type     Description Default
 muhat Matching a Matching  required
 Returns:
 Type      Description
 TwoArrays the two components of the hessian wrt (\mu,r)
            of the entropy
  Source code in cupid_matching/choo_siow.py
-183 def hessian_mur_choo_siow(muhat: Matching) -> TwoArrays:
-184     """Returns the derivatives of $e_0$ in $r$
-185     for the Choo and Siow model.
-186
-187     Args:
-188         muhat: a Matching
-189
-190     Returns:
-191         the two components of the hessian wrt $(\\mu,r)$ of the entropy
-192     """
-193     entropy_res = _entropy_choo_siow(muhat, deriv=2)
-194     hessmur = entropy_res[3]
-195     muxy, *_ = muhat.unpack()
-196     X, Y = muxy.shape
-197     hess_nx = np.zeros((X, Y))
-198     hess_my = np.zeros((X, Y))
-199     for x in range(X):
-200         for y in range(Y):
-201             d2r = hessmur[x, y, :]
-202             hess_nx[x, y] = d2r[x]
-203             hess_my[x, y] = d2r[X + y]
-204     return hess_nx, hess_my
+225 def hessian_mur_choo_siow(muhat: Matching) -> TwoArrays:
+226     """Returns the derivatives of $e_0$ in $r$
+227     for the Choo and Siow model.
+228
+229     Args:
+230         muhat: a Matching
+231
+232     Returns:
+233         the two components of the hessian wrt $(\\mu,r)$ of the entropy
+234     """
+235     entropy_res = _entropy_choo_siow(muhat, deriv=2)
+236     hessmur = entropy_res[3]
+237     muxy, *_ = muhat.unpack()
+238     X, Y = muxy.shape
+239     hess_nx = np.zeros((X, Y))
+240     hess_my = np.zeros((X, Y))
+241     for x in range(X):
+242         for y in range(Y):
+243             d2r = hessmur[x, y, :]
+244             hess_nx[x, y] = d2r[x]
+245             hess_my[x, y] = d2r[X + y]
+246     return hess_nx, hess_my
 ***** hessian_mur_choo_siow_corrected(muhat) ¶ *****
 Returns the derivatives of e_0
  in r
  for the Choo and Siow model, with the small sample correction
 Parameters:
 Name  Type     Description Default
 muhat Matching a Matching  required
 Returns:
 Type      Description
 TwoArrays the two components of the hessian wrt (\mu,r)
            of the entropy
  Source code in cupid_matching/choo_siow.py
-207 def hessian_mur_choo_siow_corrected(
-208         muhat: Matching
-209 ) -> TwoArrays:
-210     """Returns the derivatives of $e_0$ in $r$
-211     for the Choo and Siow model, with the small sample correction
-212
-213     Args:
-214         muhat: a Matching
-215
-216     Returns:
-217         the two components of the hessian wrt $(\\mu,r)$ of the entropy
-218     """
-219     hess_nx, hess_my = hessian_mur_choo_siow(muhat)
-220     _, mux0, mu0y, *_ = muhat.unpack()
-221     corr_nx = 1.0 / (2.0*mux0*mux0)
-222     corr_my = 1.0 / (2.0*mu0y*mu0y)
-223     X, Y = mux0.size, mu0y.size
-224     for x in range(X):
-225         hess_my[x, :] += corr_my
-226     for y in range(Y):
-227         hess_nx[:, y] += corr_nx
-228     return hess_nx, hess_my
+249 def hessian_mur_choo_siow_corrected(muhat: Matching) -> TwoArrays:
+250     """Returns the derivatives of $e_0$ in $r$
+251     for the Choo and Siow model, with the small sample correction
+252
+253     Args:
+254         muhat: a Matching
+255
+256     Returns:
+257         the two components of the hessian wrt $(\\mu,r)$ of the entropy
+258     """
+259     _, _, hessmur \
+260         = _der_entropy_choo_siow_corrected(muhat, hessian=True)
+261     muxy, *_ = muhat.unpack()
+262     X, Y = muxy.shape
+263     hess_nx = np.zeros((X, Y))
+264     hess_my = np.zeros((X, Y))
+265     for x in range(X):
+266         for y in range(Y):
+267             d2r = hessmur[x, y, :]
+268             hess_nx[x, y] = d2r[x]
+269             hess_my[x, y] = d2r[X + y]
+270     return hess_nx, hess_my
 
 Made with Material_for_MkDocs
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html` & `cupid_matching-1.0.5/cupid_matching/site/choo_siow_gender_heteroskedastic/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/choo_siow_heteroskedastic/index.html` & `cupid_matching-1.0.5/cupid_matching/site/choo_siow_heteroskedastic/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/cupid_streamlit/index.html` & `cupid_matching-1.0.5/cupid_matching/site/cupid_streamlit/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/entropy/index.html` & `cupid_matching-1.0.5/cupid_matching/site/entropy/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1022,19 +1022,15 @@
 
 <p><strong>Examples:</strong></p>
     <p>See <code>entropy_choo_siow</code> in <code>choo_siow.py</code></p>
 
 
         <details class="quote">
           <summary>Source code in <code>cupid_matching/entropy.py</code></summary>
-          <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal"> 50</span>
-<span class="normal"> 51</span>
-<span class="normal"> 52</span>
-<span class="normal"> 53</span>
-<span class="normal"> 54</span>
+          <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal"> 54</span>
 <span class="normal"> 55</span>
 <span class="normal"> 56</span>
 <span class="normal"> 57</span>
 <span class="normal"> 58</span>
 <span class="normal"> 59</span>
 <span class="normal"> 60</span>
 <span class="normal"> 61</span>
@@ -1076,15 +1072,19 @@
 <span class="normal"> 97</span>
 <span class="normal"> 98</span>
 <span class="normal"> 99</span>
 <span class="normal">100</span>
 <span class="normal">101</span>
 <span class="normal">102</span>
 <span class="normal">103</span>
-<span class="normal">104</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="nd">@dataclass</span>
+<span class="normal">104</span>
+<span class="normal">105</span>
+<span class="normal">106</span>
+<span class="normal">107</span>
+<span class="normal">108</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="nd">@dataclass</span>
 <span class="k">class</span> <span class="nc">EntropyFunctions</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Defines the entropy used, via the derivative $e_0 + e \\cdot \\alpha$</span>
 
 <span class="sd">    Attributes:</span>
 <span class="sd">        e0_fun: required</span>
 <span class="sd">        parameter_dependent:  if `True`, the entropy depends on parameters.</span>
 <span class="sd">            Defaults to `False`</span>
@@ -1250,19 +1250,15 @@
           <td><p>at <span class="arithmatex"><span class="MathJax_Preview">(\mu, n, m, \alpha, p)</span><script type="math/tex">(\mu, n, m, \alpha, p)</script></span>.</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/entropy.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">107</span>
-<span class="normal">108</span>
-<span class="normal">109</span>
-<span class="normal">110</span>
-<span class="normal">111</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">111</span>
 <span class="normal">112</span>
 <span class="normal">113</span>
 <span class="normal">114</span>
 <span class="normal">115</span>
 <span class="normal">116</span>
 <span class="normal">117</span>
 <span class="normal">118</span>
@@ -1292,15 +1288,19 @@
 <span class="normal">142</span>
 <span class="normal">143</span>
 <span class="normal">144</span>
 <span class="normal">145</span>
 <span class="normal">146</span>
 <span class="normal">147</span>
 <span class="normal">148</span>
-<span class="normal">149</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">entropy_gradient</span><span class="p">(</span>
+<span class="normal">149</span>
+<span class="normal">150</span>
+<span class="normal">151</span>
+<span class="normal">152</span>
+<span class="normal">153</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">entropy_gradient</span><span class="p">(</span>
     <span class="n">entropy</span><span class="p">:</span> <span class="n">EntropyFunctions</span><span class="p">,</span>
     <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">,</span>
     <span class="n">alpha</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
     <span class="n">additional_parameters</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">list</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
 <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Computes the derivative of the entropy wrt $\\mu$</span>
 <span class="sd">     at $(\\mu, n, m, \\alpha, p)$</span>
```

#### html2text {}

```diff
@@ -123,69 +123,69 @@
 additional_parameters Optional[list]              define the distribution of
                                                   errors. Defaults to None
 description           Optional[str]               some text describing the
                                                   model. Defaults to None
 Examples:
 See entropy_choo_siow in choo_siow.py
  Source code in cupid_matching/entropy.py
- 50 @dataclass
- 51 class EntropyFunctions:
- 52     """Defines the entropy used, via the derivative $e_0 + e \\cdot
- 53 \\alpha$
- 54
- 55     Attributes:
- 56         e0_fun: required
- 57         parameter_dependent:  if `True`, the entropy depends on parameters.
- 58             Defaults to `False`
- 59         e_fun: only in entropies that depend on parameters.
- 60             Defaults to `None`
- 61         hessian: defaults to `"numeric"`
- 62             * if `"provided"`, we provide the hessian of the entropy.
- 63             * if `"numerical"`, it is computed by central differences.
- 64         e0_derivative: the derivative of `e0_fun`, if available.
- 65             Defaults to `None`
- 66         e_derivative: the derivative of `e_fun`, if available.
- 67             Defaults to `None`
- 68         additional_parameters: additional parameters
- 69             that define the distribution of errors.
- 70             Defaults to `None`
- 71         description: some text describing the model.
- 72             Defaults to `None`
- 73
- 74     Examples:
- 75         See `entropy_choo_siow` in `choo_siow.py`
- 76     """
+ 54 @dataclass
+ 55 class EntropyFunctions:
+ 56     """Defines the entropy used, via the derivative $e_0 + e \\cdot
+ 57 \\alpha$
+ 58
+ 59     Attributes:
+ 60         e0_fun: required
+ 61         parameter_dependent:  if `True`, the entropy depends on parameters.
+ 62             Defaults to `False`
+ 63         e_fun: only in entropies that depend on parameters.
+ 64             Defaults to `None`
+ 65         hessian: defaults to `"numeric"`
+ 66             * if `"provided"`, we provide the hessian of the entropy.
+ 67             * if `"numerical"`, it is computed by central differences.
+ 68         e0_derivative: the derivative of `e0_fun`, if available.
+ 69             Defaults to `None`
+ 70         e_derivative: the derivative of `e_fun`, if available.
+ 71             Defaults to `None`
+ 72         additional_parameters: additional parameters
+ 73             that define the distribution of errors.
+ 74             Defaults to `None`
+ 75         description: some text describing the model.
+ 76             Defaults to `None`
  77
- 78     e0_fun: MatchingFunction | MatchingFunctionParam
- 79     e0_derivative: Optional[EntropyHessians | EntropyHessiansParam] = None
- 80     additional_parameters: Optional[list] = None
- 81     description: Optional[str] = None
- 82     e_fun: Optional[MatchingFunction | MatchingFunctionParam] = None
- 83     e_derivative: Optional[EntropyHessians | EntropyHessiansParam] = None
- 84     hessian: Optional[str] = "numerical"
- 85     parameter_dependent: bool = False
- 86
- 87     def __post_init__(self):
- 88         if not self.parameter_dependent:
- 89             if self.hessian == "provided" and self.e0_derivative is None:
- 90                 bs_error_abort(
- 91                     "You claim to provide the hessian "
- 92                     + "but you did not provide the e0_derivative."
- 93                 )
- 94         else:
- 95             if self.e_fun is None:
- 96                 bs_error_abort(
- 97                     "Your entropy is parameter dependent "
- 98                     + " but you did not provide the e_fun."
- 99                 )
-100             if self.hessian == "provided" and self.e_derivative is None:
-101                 bs_error_abort(
-102                     "Your entropy is parameter dependent, "
-103                     + "you claim to provide the hessian,\n"
-104                     + " but I do not see the e_derivative."
+ 78     Examples:
+ 79         See `entropy_choo_siow` in `choo_siow.py`
+ 80     """
+ 81
+ 82     e0_fun: MatchingFunction | MatchingFunctionParam
+ 83     e0_derivative: Optional[EntropyHessians | EntropyHessiansParam] = None
+ 84     additional_parameters: Optional[list] = None
+ 85     description: Optional[str] = None
+ 86     e_fun: Optional[MatchingFunction | MatchingFunctionParam] = None
+ 87     e_derivative: Optional[EntropyHessians | EntropyHessiansParam] = None
+ 88     hessian: Optional[str] = "numerical"
+ 89     parameter_dependent: bool = False
+ 90
+ 91     def __post_init__(self):
+ 92         if not self.parameter_dependent:
+ 93             if self.hessian == "provided" and self.e0_derivative is None:
+ 94                 bs_error_abort(
+ 95                     "You claim to provide the hessian "
+ 96                     + "but you did not provide the e0_derivative."
+ 97                 )
+ 98         else:
+ 99             if self.e_fun is None:
+100                 bs_error_abort(
+101                     "Your entropy is parameter dependent "
+102                     + " but you did not provide the e_fun."
+103                 )
+104             if self.hessian == "provided" and self.e_derivative is None:
+105                 bs_error_abort(
+106                     "Your entropy is parameter dependent, "
+107                     + "you claim to provide the hessian,\n"
+108                     + " but I do not see the e_derivative."
                     )
 ***** entropy_gradient(entropy, muhat, alpha=None, additional_parameters=None)
 ¶ *****
 Computes the derivative of the entropy wrt \mu
  at (\mu, n, m, \alpha, p)
 Parameters:
 Name                  Type                 Description                 Default
@@ -198,53 +198,53 @@
                                            parameters p, if any
 Returns:
 Type       Description
 np.ndarray the derivative of the entropy wrt \mu
 np.ndarray at (\mu, n, m, \alpha, p)
            .
  Source code in cupid_matching/entropy.py
-107 def entropy_gradient(
-108     entropy: EntropyFunctions,
-109     muhat: Matching,
-110     alpha: Optional[np.ndarray] = None,
-111     additional_parameters: Optional[list] = None,
-112 ) -> np.ndarray:
-113     """Computes the derivative of the entropy wrt $\\mu$
-114      at $(\\mu, n, m, \\alpha, p)$
-115
-116     Args:
-117         entropy: the `EntropyFunctions` object
-118         muhat: a Matching
-119         alpha: a vector of parameters of the derivative of the entropy, if
-120 any
-121         additional_parameters: a list of additional parameters `p`, if any
-122
-123     Returns:
-124         the derivative of the entropy wrt $\\mu$
-125         at $(\\mu, n, m, \\alpha, p)$.
-126     """
-127     e0_fun = entropy.e0_fun
-128     if additional_parameters is not None:
-129         e0_fun = cast(MatchingFunctionParam, e0_fun)
-130         e0_vals = e0_fun(muhat, additional_parameters)
-131     else:
-132         e0_fun = cast(MatchingFunction, e0_fun)
-133         e0_vals = e0_fun(muhat)
-134     parameter_dependent = entropy.parameter_dependent
-135     if parameter_dependent:
-136         if alpha is None:
-137             bs_error_abort("alpha should be specified for this model")
-138         e_fun = entropy.e_fun
-139         if e_fun is None:
-140             bs_error_abort("we should have an e_fun in this model")
-141         else:
-142             if additional_parameters is not None:
-143                 e_fun = cast(MatchingFunctionParam, e_fun)
-144                 e_vals = e_fun(muhat, additional_parameters)
-145             else:
-146                 e_fun = cast(MatchingFunction, e_fun)
-147                 e_vals = e_fun(muhat)
-148         return e0_vals + e_vals @ alpha
-149     else:
+111 def entropy_gradient(
+112     entropy: EntropyFunctions,
+113     muhat: Matching,
+114     alpha: Optional[np.ndarray] = None,
+115     additional_parameters: Optional[list] = None,
+116 ) -> np.ndarray:
+117     """Computes the derivative of the entropy wrt $\\mu$
+118      at $(\\mu, n, m, \\alpha, p)$
+119
+120     Args:
+121         entropy: the `EntropyFunctions` object
+122         muhat: a Matching
+123         alpha: a vector of parameters of the derivative of the entropy, if
+124 any
+125         additional_parameters: a list of additional parameters `p`, if any
+126
+127     Returns:
+128         the derivative of the entropy wrt $\\mu$
+129         at $(\\mu, n, m, \\alpha, p)$.
+130     """
+131     e0_fun = entropy.e0_fun
+132     if additional_parameters is not None:
+133         e0_fun = cast(MatchingFunctionParam, e0_fun)
+134         e0_vals = e0_fun(muhat, additional_parameters)
+135     else:
+136         e0_fun = cast(MatchingFunction, e0_fun)
+137         e0_vals = e0_fun(muhat)
+138     parameter_dependent = entropy.parameter_dependent
+139     if parameter_dependent:
+140         if alpha is None:
+141             bs_error_abort("alpha should be specified for this model")
+142         e_fun = entropy.e_fun
+143         if e_fun is None:
+144             bs_error_abort("we should have an e_fun in this model")
+145         else:
+146             if additional_parameters is not None:
+147                 e_fun = cast(MatchingFunctionParam, e_fun)
+148                 e_vals = e_fun(muhat, additional_parameters)
+149             else:
+150                 e_fun = cast(MatchingFunction, e_fun)
+151                 e_vals = e_fun(muhat)
+152         return e0_vals + e_vals @ alpha
+153     else:
             return e0_vals
 
 Made with Material_for_MkDocs
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/index.html` & `cupid_matching-1.0.5/cupid_matching/site/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,21 @@
           <li class="md-nav__item">
   <a href="#version-104" class="md-nav__link">
     version 1.0.4
   </a>
   
 </li>
         
+          <li class="md-nav__item">
+  <a href="#version-105" class="md-nav__link">
+    version 1,0.5
+  </a>
+  
+</li>
+        
       </ul>
     </nav>
   
 </li>
       
     </ul>
   
@@ -668,14 +675,21 @@
           <li class="md-nav__item">
   <a href="#version-104" class="md-nav__link">
     version 1.0.4
   </a>
   
 </li>
         
+          <li class="md-nav__item">
+  <a href="#version-105" class="md-nav__link">
+    version 1,0.5
+  </a>
+  
+</li>
+        
       </ul>
     </nav>
   
 </li>
       
     </ul>
   
@@ -729,14 +743,18 @@
 </ul>
 <h2 id="release-notes">Release notes<a class="headerlink" href="#release-notes" title="Permanent link">&para;</a></h2>
 <h3 id="version-104">version 1.0.4<a class="headerlink" href="#version-104" title="Permanent link">&para;</a></h3>
 <ul>
 <li>added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.</li>
 <li>added two complete examples: <a href="example_choosiow/">example_choosiow.py</a> and <a href="example_nestedlogit/">example_nestedlogit.py</a>.</li>
 </ul>
+<h3 id="version-105">version 1,0.5<a class="headerlink" href="#version-105" title="Permanent link">&para;</a></h3>
+<ul>
+<li>simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.</li>
+</ul>
 
 
 
 
 
                 
               </article>
```

#### html2text {}

```diff
@@ -26,14 +26,15 @@
     * ⁰  Home   Home    Table of contents
           o Installation
           o Importing_functions_from_the_package
           o Examples
           o Warnings
           o Release_notes
                 # version_1.0.4
+                # version_1,0.5
     * ⁰  API Reference      API Reference
           o Minimum_Distance_Estimator
           o Utilities_for_MDE
           o Poisson_estimator
           o Utilities_for_Poisson
           o Entropy_utilities
           o Choo-Siow_homoskedastic
@@ -50,14 +51,15 @@
    Table of contents
     * Installation
     * Importing_functions_from_the_package
     * Examples
     * Warnings
     * Release_notes
           o version_1.0.4
+          o version_1,0.5
 ****** cupid_matching¶ ******
 
 A Python package to solve, simulate and estimate separable matching models
     * Free software: MIT license
     * Documentation: https://bsalanie.github.io/cupid_matching
     * See also: An_interactive_Streamlit_app
 ***** Installation¶ *****
@@ -81,9 +83,12 @@
 ***** Release notes¶ *****
 **** version 1.0.4¶ ****
     * added an optional bias-correction for the minimum distance estimator in
       the Choo and Siow homoskedastic model, to help with cases when the
       matching patterns vary a lot across cells.
     * added two complete examples: example_choosiow.py and
       example_nestedlogit.py.
+**** version 1,0.5¶ ****
+    * simplified the bias-correction for the minimum distance estimator in the
+      Choo and Siow homoskedastic model.
 
 Made with Material_for_MkDocs
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/ipfp_solvers/index.html` & `cupid_matching-1.0.5/cupid_matching/site/ipfp_solvers/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/matching_utils/index.html` & `cupid_matching-1.0.5/cupid_matching/site/matching_utils/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/min_distance/index.html` & `cupid_matching-1.0.5/cupid_matching/site/min_distance/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/min_distance_utils/index.html` & `cupid_matching-1.0.5/cupid_matching/site/min_distance_utils/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -920,15 +920,17 @@
 <span class="normal">142</span>
 <span class="normal">143</span>
 <span class="normal">144</span>
 <span class="normal">145</span>
 <span class="normal">146</span>
 <span class="normal">147</span>
 <span class="normal">148</span>
-<span class="normal">149</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="nd">@dataclass</span>
+<span class="normal">149</span>
+<span class="normal">150</span>
+<span class="normal">151</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="nd">@dataclass</span>
 <span class="k">class</span> <span class="nc">MDEResults</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    The results from minimum-distance estimation and testing.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        X: int</span>
 <span class="sd">        Y: int</span>
@@ -1010,15 +1012,17 @@
                 <span class="n">j</span> <span class="o">=</span> <span class="n">n_alpha</span> <span class="o">+</span> <span class="n">i</span>
                 <span class="n">repr_str</span> <span class="o">+=</span> <span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;   base </span><span class="si">{</span><span class="n">i</span><span class="w"> </span><span class="o">+</span><span class="w"> </span><span class="mi">1</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">true_coeffs</span><span class="p">[</span><span class="n">j</span><span class="p">]</span><span class="si">:</span><span class="s2"> &gt; 10.3f</span><span class="si">}</span><span class="s2">  &quot;</span>
                     <span class="o">+</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">coeff</span><span class="si">:</span><span class="s2"> &gt; 10.3f</span><span class="si">}</span><span class="s2">  (</span><span class="si">{</span><span class="n">stderrs</span><span class="p">[</span><span class="n">j</span><span class="p">]</span><span class="si">:</span><span class="s2"> &gt; 10.3f</span><span class="si">}</span><span class="s2">)</span><span class="se">\n</span><span class="s2">&quot;</span>
                 <span class="p">)</span>
             <span class="n">print_stars</span><span class="p">(</span><span class="n">repr_str</span><span class="p">)</span>
             <span class="n">discrepancy</span> <span class="o">=</span> <span class="n">npmaxabs</span><span class="p">(</span><span class="n">true_coeffs</span> <span class="o">-</span> <span class="n">estimates</span><span class="p">)</span>
-            <span class="n">print_stars</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The largest difference between true and estimated coefficients is </span><span class="si">{</span><span class="n">discrepancy</span><span class="si">:</span><span class="s2"> .2e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <span class="n">print_stars</span><span class="p">(</span>
+                <span class="sa">f</span><span class="s2">&quot;The largest difference between true and estimated coefficients is </span><span class="si">{</span><span class="n">discrepancy</span><span class="si">:</span><span class="s2"> .2e</span><span class="si">}</span><span class="s2">&quot;</span>
+            <span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">repr_str</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="s2">&quot;The estimated coefficients &quot;</span>
                 <span class="o">+</span> <span class="s2">&quot;(and their standard errors) are</span><span class="se">\n\n</span><span class="s2">&quot;</span>
             <span class="p">)</span>
             <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">coeff</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">estimates</span><span class="p">[:</span><span class="n">n_alpha</span><span class="p">]):</span>
                 <span class="n">repr_str</span> <span class="o">+</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">coeff</span><span class="si">:</span><span class="s2"> &gt; 10.3f</span><span class="si">}</span><span class="s2">  (</span><span class="si">{</span><span class="n">stderrs</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="si">:</span><span class="s2"> &gt; 10.3f</span><span class="si">}</span><span class="s2">)</span><span class="se">\n</span><span class="s2">&quot;</span>
```

#### html2text {}

```diff
@@ -156,37 +156,39 @@
 118                 j = n_alpha + i
 119                 repr_str += (
 120                     f"   base {i + 1}: {true_coeffs[j]: > 10.3f}  "
 121                     + f"{coeff: > 10.3f}  ({stderrs[j]: > 10.3f})\n"
 122                 )
 123             print_stars(repr_str)
 124             discrepancy = npmaxabs(true_coeffs - estimates)
-125             print_stars(f"The largest difference between true and estimated
-126 coefficients is {discrepancy: .2e}")
-127         else:
-128             repr_str = (
-129                 "The estimated coefficients "
-130                 + "(and their standard errors) are\n\n"
-131             )
-132             for i, coeff in enumerate(estimates[:n_alpha]):
-133                 repr_str + f"{coeff: > 10.3f}  ({stderrs[i]: > 10.3f})\n"
-134                 repr_str += "\n"
-135             for i, coeff in enumerate(estimates[n_alpha:]):
-136                 j = n_alpha + i
-137                 repr_str += f"{coeff: > 10.3f}  ({stderrs[j]: > 10.3f})\n"
-138             print_stars(repr_str)
-139
-140         repr_str = "\nSpecification test:\n"
-141         repr_str += (
-142             "   the value of the test statistic is "
-143             + f"{self.test_statistic: > 10.3f}\n"
-144         )
-145         repr_str += (
-146             f"     for a chi2({self.ndf}), "
-147             + f"the p-value is {self.test_pvalue: > 10.3f}\n"
-148         )
-149         print_stars(repr_str)
+125             print_stars(
+126                 f"The largest difference between true and estimated
+127 coefficients is {discrepancy: .2e}"
+128             )
+129         else:
+130             repr_str = (
+131                 "The estimated coefficients "
+132                 + "(and their standard errors) are\n\n"
+133             )
+134             for i, coeff in enumerate(estimates[:n_alpha]):
+135                 repr_str + f"{coeff: > 10.3f}  ({stderrs[i]: > 10.3f})\n"
+136                 repr_str += "\n"
+137             for i, coeff in enumerate(estimates[n_alpha:]):
+138                 j = n_alpha + i
+139                 repr_str += f"{coeff: > 10.3f}  ({stderrs[j]: > 10.3f})\n"
+140             print_stars(repr_str)
+141
+142         repr_str = "\nSpecification test:\n"
+143         repr_str += (
+144             "   the value of the test statistic is "
+145             + f"{self.test_statistic: > 10.3f}\n"
+146         )
+147         repr_str += (
+148             f"     for a chi2({self.ndf}), "
+149             + f"the p-value is {self.test_pvalue: > 10.3f}\n"
+150         )
+151         print_stars(repr_str)
             if true_coeffs is not None:
                 return discrepancy
             return None
 
 Made with Material_for_MkDocs
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/model_classes/index.html` & `cupid_matching-1.0.5/cupid_matching/site/model_classes/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/nested_logit/index.html` & `cupid_matching-1.0.5/cupid_matching/site/nested_logit/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -808,61 +808,61 @@
           <td><p>wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,\mu)</span><script type="math/tex">(\mu,\mu)</script></span>.</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/nested_logit.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal"> 56</span>
-<span class="normal"> 57</span>
-<span class="normal"> 58</span>
-<span class="normal"> 59</span>
-<span class="normal"> 60</span>
-<span class="normal"> 61</span>
-<span class="normal"> 62</span>
-<span class="normal"> 63</span>
-<span class="normal"> 64</span>
-<span class="normal"> 65</span>
-<span class="normal"> 66</span>
-<span class="normal"> 67</span>
-<span class="normal"> 68</span>
-<span class="normal"> 69</span>
-<span class="normal"> 70</span>
-<span class="normal"> 71</span>
-<span class="normal"> 72</span>
-<span class="normal"> 73</span>
-<span class="normal"> 74</span>
-<span class="normal"> 75</span>
-<span class="normal"> 76</span>
-<span class="normal"> 77</span>
-<span class="normal"> 78</span>
-<span class="normal"> 79</span>
-<span class="normal"> 80</span>
-<span class="normal"> 81</span>
-<span class="normal"> 82</span>
-<span class="normal"> 83</span>
-<span class="normal"> 84</span>
-<span class="normal"> 85</span>
-<span class="normal"> 86</span>
-<span class="normal"> 87</span>
-<span class="normal"> 88</span>
-<span class="normal"> 89</span>
-<span class="normal"> 90</span>
-<span class="normal"> 91</span>
-<span class="normal"> 92</span>
-<span class="normal"> 93</span>
-<span class="normal"> 94</span>
-<span class="normal"> 95</span>
-<span class="normal"> 96</span>
-<span class="normal"> 97</span>
-<span class="normal"> 98</span>
-<span class="normal"> 99</span>
-<span class="normal">100</span>
-<span class="normal">101</span>
-<span class="normal">102</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_derivative_mu_nested_logit</span><span class="p">(</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">52</span>
+<span class="normal">53</span>
+<span class="normal">54</span>
+<span class="normal">55</span>
+<span class="normal">56</span>
+<span class="normal">57</span>
+<span class="normal">58</span>
+<span class="normal">59</span>
+<span class="normal">60</span>
+<span class="normal">61</span>
+<span class="normal">62</span>
+<span class="normal">63</span>
+<span class="normal">64</span>
+<span class="normal">65</span>
+<span class="normal">66</span>
+<span class="normal">67</span>
+<span class="normal">68</span>
+<span class="normal">69</span>
+<span class="normal">70</span>
+<span class="normal">71</span>
+<span class="normal">72</span>
+<span class="normal">73</span>
+<span class="normal">74</span>
+<span class="normal">75</span>
+<span class="normal">76</span>
+<span class="normal">77</span>
+<span class="normal">78</span>
+<span class="normal">79</span>
+<span class="normal">80</span>
+<span class="normal">81</span>
+<span class="normal">82</span>
+<span class="normal">83</span>
+<span class="normal">84</span>
+<span class="normal">85</span>
+<span class="normal">86</span>
+<span class="normal">87</span>
+<span class="normal">88</span>
+<span class="normal">89</span>
+<span class="normal">90</span>
+<span class="normal">91</span>
+<span class="normal">92</span>
+<span class="normal">93</span>
+<span class="normal">94</span>
+<span class="normal">95</span>
+<span class="normal">96</span>
+<span class="normal">97</span>
+<span class="normal">98</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_derivative_mu_nested_logit</span><span class="p">(</span>
     <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">,</span> <span class="n">additional_parameters</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span>
 <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ThreeArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of the parameter-independent part $e_0$</span>
 <span class="sd">    wrt $\\mu$ for the nested logit.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
@@ -982,15 +982,19 @@
           <td><p>wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,r)</span><script type="math/tex">(\mu,r)</script></span>.</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/nested_logit.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">105</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">101</span>
+<span class="normal">102</span>
+<span class="normal">103</span>
+<span class="normal">104</span>
+<span class="normal">105</span>
 <span class="normal">106</span>
 <span class="normal">107</span>
 <span class="normal">108</span>
 <span class="normal">109</span>
 <span class="normal">110</span>
 <span class="normal">111</span>
 <span class="normal">112</span>
@@ -1014,19 +1018,15 @@
 <span class="normal">130</span>
 <span class="normal">131</span>
 <span class="normal">132</span>
 <span class="normal">133</span>
 <span class="normal">134</span>
 <span class="normal">135</span>
 <span class="normal">136</span>
-<span class="normal">137</span>
-<span class="normal">138</span>
-<span class="normal">139</span>
-<span class="normal">140</span>
-<span class="normal">141</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_derivative_r_nested_logit</span><span class="p">(</span>
+<span class="normal">137</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_derivative_r_nested_logit</span><span class="p">(</span>
     <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">,</span> <span class="n">additional_parameters</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span>
 <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">TwoArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of the parameter-independent part $e_0$</span>
 <span class="sd">    wrt $r$ for the nested logit.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
@@ -1136,15 +1136,19 @@
           <td><p>of the first derivative of the entropy.</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/nested_logit.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">22</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">18</span>
+<span class="normal">19</span>
+<span class="normal">20</span>
+<span class="normal">21</span>
+<span class="normal">22</span>
 <span class="normal">23</span>
 <span class="normal">24</span>
 <span class="normal">25</span>
 <span class="normal">26</span>
 <span class="normal">27</span>
 <span class="normal">28</span>
 <span class="normal">29</span>
@@ -1163,19 +1167,15 @@
 <span class="normal">42</span>
 <span class="normal">43</span>
 <span class="normal">44</span>
 <span class="normal">45</span>
 <span class="normal">46</span>
 <span class="normal">47</span>
 <span class="normal">48</span>
-<span class="normal">49</span>
-<span class="normal">50</span>
-<span class="normal">51</span>
-<span class="normal">52</span>
-<span class="normal">53</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_nested_logit</span><span class="p">(</span>
+<span class="normal">49</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e0_nested_logit</span><span class="p">(</span>
     <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">,</span> <span class="n">additional_parameters</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span>
 <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the values of the parameter-independent part $e_0$</span>
 <span class="sd">    for the nested logit.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
@@ -1280,15 +1280,19 @@
           <td><p>wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,\mu)</span><script type="math/tex">(\mu,\mu)</script></span>.</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/nested_logit.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">191</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">187</span>
+<span class="normal">188</span>
+<span class="normal">189</span>
+<span class="normal">190</span>
+<span class="normal">191</span>
 <span class="normal">192</span>
 <span class="normal">193</span>
 <span class="normal">194</span>
 <span class="normal">195</span>
 <span class="normal">196</span>
 <span class="normal">197</span>
 <span class="normal">198</span>
@@ -1324,19 +1328,15 @@
 <span class="normal">228</span>
 <span class="normal">229</span>
 <span class="normal">230</span>
 <span class="normal">231</span>
 <span class="normal">232</span>
 <span class="normal">233</span>
 <span class="normal">234</span>
-<span class="normal">235</span>
-<span class="normal">236</span>
-<span class="normal">237</span>
-<span class="normal">238</span>
-<span class="normal">239</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e_derivative_mu_nested_logit</span><span class="p">(</span>
+<span class="normal">235</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e_derivative_mu_nested_logit</span><span class="p">(</span>
     <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">,</span> <span class="n">additional_parameters</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span>
 <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">ThreeArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of the parameter-dependent part $e$</span>
 <span class="sd">     wrt $\\mu$ for the nested logit.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
@@ -1458,15 +1458,19 @@
           <td><p>wrt <span class="arithmatex"><span class="MathJax_Preview">(\mu,r)</span><script type="math/tex">(\mu,r)</script></span>.</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/nested_logit.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">242</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">238</span>
+<span class="normal">239</span>
+<span class="normal">240</span>
+<span class="normal">241</span>
+<span class="normal">242</span>
 <span class="normal">243</span>
 <span class="normal">244</span>
 <span class="normal">245</span>
 <span class="normal">246</span>
 <span class="normal">247</span>
 <span class="normal">248</span>
 <span class="normal">249</span>
@@ -1479,19 +1483,15 @@
 <span class="normal">256</span>
 <span class="normal">257</span>
 <span class="normal">258</span>
 <span class="normal">259</span>
 <span class="normal">260</span>
 <span class="normal">261</span>
 <span class="normal">262</span>
-<span class="normal">263</span>
-<span class="normal">264</span>
-<span class="normal">265</span>
-<span class="normal">266</span>
-<span class="normal">267</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e_derivative_r_nested_logit</span><span class="p">(</span>
+<span class="normal">263</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e_derivative_r_nested_logit</span><span class="p">(</span>
     <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">,</span> <span class="n">additional_parameters</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span>
 <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">TwoArrays</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the derivatives of the parameter-dependent part $e$</span>
 <span class="sd">     wrt $r$ for the nested logit.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
@@ -1590,15 +1590,19 @@
           <td><p>of the first derivative of the entropy.</p></td>
         </tr>
     </tbody>
   </table>
 
       <details class="quote">
         <summary>Source code in <code>cupid_matching/nested_logit.py</code></summary>
-        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">150</span>
+        <div class="highlight"><table class="highlighttable"><tr><td class="linenos"><div class="linenodiv"><pre><span></span><span class="normal">146</span>
+<span class="normal">147</span>
+<span class="normal">148</span>
+<span class="normal">149</span>
+<span class="normal">150</span>
 <span class="normal">151</span>
 <span class="normal">152</span>
 <span class="normal">153</span>
 <span class="normal">154</span>
 <span class="normal">155</span>
 <span class="normal">156</span>
 <span class="normal">157</span>
@@ -1624,19 +1628,15 @@
 <span class="normal">177</span>
 <span class="normal">178</span>
 <span class="normal">179</span>
 <span class="normal">180</span>
 <span class="normal">181</span>
 <span class="normal">182</span>
 <span class="normal">183</span>
-<span class="normal">184</span>
-<span class="normal">185</span>
-<span class="normal">186</span>
-<span class="normal">187</span>
-<span class="normal">188</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e_nested_logit</span><span class="p">(</span>
+<span class="normal">184</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="k">def</span> <span class="nf">e_nested_logit</span><span class="p">(</span>
     <span class="n">muhat</span><span class="p">:</span> <span class="n">Matching</span><span class="p">,</span> <span class="n">additional_parameters</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]</span>
 <span class="p">)</span> <span class="o">-&gt;</span> <span class="n">np</span><span class="o">.</span><span class="n">ndarray</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Returns the values of the parameter-dependent part  $e$</span>
 <span class="sd">    for the nested logit.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        muhat: a Matching</span>
```

#### html2text {}

```diff
@@ -76,305 +76,305 @@
 additional_parameters list[Any] a list with the nest structure required
 Returns:
 Type        Description
 ThreeArrays the parameter-independent part of the hessian of the entropy
 ThreeArrays wrt (\mu,\mu)
             .
  Source code in cupid_matching/nested_logit.py
- 56 def e0_derivative_mu_nested_logit(
- 57     muhat: Matching, additional_parameters: list[Any]
- 58 ) -> ThreeArrays:
- 59     """Returns the derivatives of the parameter-independent part $e_0$
- 60     wrt $\\mu$ for the nested logit.
- 61
- 62     Args:
- 63         muhat: a Matching
- 64         additional_parameters: a list with the nest structure
- 65
- 66     Returns:
- 67         the parameter-independent part of the hessian of the entropy
- 68         wrt $(\\mu,\\mu)$.
- 69     """
- 70     nests_for_each_x, nests_for_each_y = additional_parameters
- 71     nests_x = _change_indices(nests_for_each_x)
- 72     nests_y = _change_indices(nests_for_each_y)
- 73     muxy, mux0, mu0y, *_ = muhat.unpack()
- 74     X, Y = muxy.shape
- 75
- 76     hess_x = np.zeros((X, Y, Y))
- 77     hess_y = np.zeros((X, Y, X))
- 78     hess_xy = np.zeros((X, Y))
- 79     der_logx0 = 1.0 / mux0
- 80     der_log0y = 1.0 / mu0y
- 81
- 82     for x in range(X):
- 83         dlogx0 = der_logx0[x]
- 84         for nest in nests_x:
- 85             mu_xn = np.sum(muxy[x, nest])
- 86             der_logxn = 1.0 / mu_xn
- 87             for y in nest:
- 88                 hess_x[x, y, :] = -dlogx0
- 89                 hess_x[x, y, nest] -= der_logxn
- 90     for y in range(Y):
- 91         dlog0y = der_log0y[y]
- 92         for nest in nests_y:
- 93             mu_ny = np.sum(muxy[nest, y])
- 94             der_logny = 1.0 / mu_ny
- 95             for x in nest:
- 96                 hess_y[x, y, :] = -dlog0y
- 97                 hess_y[x, y, nest] -= der_logny
- 98     for x in range(X):
- 99         for y in range(Y):
-100             hess_xy[x, y] = hess_x[x, y, y] + hess_y[x, y, x]
-101
-102     return hess_x, hess_y, hess_xy
+52 def e0_derivative_mu_nested_logit(
+53     muhat: Matching, additional_parameters: list[Any]
+54 ) -> ThreeArrays:
+55     """Returns the derivatives of the parameter-independent part $e_0$
+56     wrt $\\mu$ for the nested logit.
+57
+58     Args:
+59         muhat: a Matching
+60         additional_parameters: a list with the nest structure
+61
+62     Returns:
+63         the parameter-independent part of the hessian of the entropy
+64         wrt $(\\mu,\\mu)$.
+65     """
+66     nests_for_each_x, nests_for_each_y = additional_parameters
+67     nests_x = _change_indices(nests_for_each_x)
+68     nests_y = _change_indices(nests_for_each_y)
+69     muxy, mux0, mu0y, *_ = muhat.unpack()
+70     X, Y = muxy.shape
+71
+72     hess_x = np.zeros((X, Y, Y))
+73     hess_y = np.zeros((X, Y, X))
+74     hess_xy = np.zeros((X, Y))
+75     der_logx0 = 1.0 / mux0
+76     der_log0y = 1.0 / mu0y
+77
+78     for x in range(X):
+79         dlogx0 = der_logx0[x]
+80         for nest in nests_x:
+81             mu_xn = np.sum(muxy[x, nest])
+82             der_logxn = 1.0 / mu_xn
+83             for y in nest:
+84                 hess_x[x, y, :] = -dlogx0
+85                 hess_x[x, y, nest] -= der_logxn
+86     for y in range(Y):
+87         dlog0y = der_log0y[y]
+88         for nest in nests_y:
+89             mu_ny = np.sum(muxy[nest, y])
+90             der_logny = 1.0 / mu_ny
+91             for x in nest:
+92                 hess_y[x, y, :] = -dlog0y
+93                 hess_y[x, y, nest] -= der_logny
+94     for x in range(X):
+95         for y in range(Y):
+96             hess_xy[x, y] = hess_x[x, y, y] + hess_y[x, y, x]
+97
+98     return hess_x, hess_y, hess_xy
 ***** e0_derivative_r_nested_logit(muhat, additional_parameters) ¶ *****
 Returns the derivatives of the parameter-independent part e_0
  wrt r
  for the nested logit.
 Parameters:
 Name                  Type      Description                    Default
 muhat                 Matching  a Matching                     required
 additional_parameters list[Any] a list with the nest structure required
 Returns:
 Type      Description
 TwoArrays the parameter-independent part of the hessian of the entropy
 TwoArrays wrt (\mu,r)
           .
  Source code in cupid_matching/nested_logit.py
-105 def e0_derivative_r_nested_logit(
-106     muhat: Matching, additional_parameters: list[Any]
-107 ) -> TwoArrays:
-108     """Returns the derivatives of the parameter-independent part $e_0$
-109     wrt $r$ for the nested logit.
+101 def e0_derivative_r_nested_logit(
+102     muhat: Matching, additional_parameters: list[Any]
+103 ) -> TwoArrays:
+104     """Returns the derivatives of the parameter-independent part $e_0$
+105     wrt $r$ for the nested logit.
+106
+107     Args:
+108         muhat: a Matching
+109         additional_parameters: a list with the nest structure
 110
-111     Args:
-112         muhat: a Matching
-113         additional_parameters: a list with the nest structure
-114
-115     Returns:
-116         the parameter-independent part of the hessian of the entropy
-117         wrt $(\\mu,r)$.
-118     """
-119     nests_for_each_x, nests_for_each_y = additional_parameters
-120     nests_x = _change_indices(nests_for_each_x)
-121     nests_y = _change_indices(nests_for_each_y)
-122     muxy, mux0, mu0y, n, m = muhat.unpack()
-123     X, Y = muxy.shape
-124
-125     hess_n = np.zeros((X, Y))
-126     hess_m = np.zeros((X, Y))
-127     der_logx0 = 1.0 / mux0
-128     der_log0y = 1.0 / mu0y
-129
-130     for x in range(X):
-131         dlogx0 = der_logx0[x]
-132         for nest in nests_x:
-133             for y in nest:
-134                 hess_n[x, y] = dlogx0
-135     for y in range(Y):
-136         dlog0y = der_log0y[y]
-137         for nest in nests_y:
-138             for x in nest:
-139                 hess_m[x, y] = dlog0y
-140
-141     return hess_n, hess_m
+111     Returns:
+112         the parameter-independent part of the hessian of the entropy
+113         wrt $(\\mu,r)$.
+114     """
+115     nests_for_each_x, nests_for_each_y = additional_parameters
+116     nests_x = _change_indices(nests_for_each_x)
+117     nests_y = _change_indices(nests_for_each_y)
+118     muxy, mux0, mu0y, n, m = muhat.unpack()
+119     X, Y = muxy.shape
+120
+121     hess_n = np.zeros((X, Y))
+122     hess_m = np.zeros((X, Y))
+123     der_logx0 = 1.0 / mux0
+124     der_log0y = 1.0 / mu0y
+125
+126     for x in range(X):
+127         dlogx0 = der_logx0[x]
+128         for nest in nests_x:
+129             for y in nest:
+130                 hess_n[x, y] = dlogx0
+131     for y in range(Y):
+132         dlog0y = der_log0y[y]
+133         for nest in nests_y:
+134             for x in nest:
+135                 hess_m[x, y] = dlog0y
+136
+137     return hess_n, hess_m
 ***** e0_nested_logit(muhat, additional_parameters) ¶ *****
 Returns the values of the parameter-independent part e_0
  for the nested logit.
 Parameters:
 Name                  Type      Description                    Default
 muhat                 Matching  a Matching                     required
 additional_parameters list[Any] a list with the nest structure required
 Returns:
 Type       Description
 np.ndarray the (X,Y) matrix of the parameter-independent part
 np.ndarray of the first derivative of the entropy.
  Source code in cupid_matching/nested_logit.py
-22 def e0_nested_logit(
-23     muhat: Matching, additional_parameters: list[Any]
-24 ) -> np.ndarray:
-25     """Returns the values of the parameter-independent part $e_0$
-26     for the nested logit.
+18 def e0_nested_logit(
+19     muhat: Matching, additional_parameters: list[Any]
+20 ) -> np.ndarray:
+21     """Returns the values of the parameter-independent part $e_0$
+22     for the nested logit.
+23
+24     Args:
+25         muhat: a Matching
+26         additional_parameters: a list with the nest structure
 27
-28     Args:
-29         muhat: a Matching
-30         additional_parameters: a list with the nest structure
-31
-32     Returns:
-33         the (X,Y) matrix of the parameter-independent part
-34         of the first derivative of the entropy.
-35     """
-36     nests_for_each_x, nests_for_each_y = additional_parameters
-37     nests_x = _change_indices(nests_for_each_x)
-38     nests_y = _change_indices(nests_for_each_y)
-39     muxy, mux0, mu0y, *_ = muhat.unpack()
-40     X, Y = muxy.shape
-41     e0_vals = np.zeros((X, Y))
-42
-43     for x in range(X):
-44         mux0_x = mux0[x]
-45         for nest in nests_x:
-46             mu_xn = np.sum(muxy[x, nest])
-47             e0_vals[x, nest] = -log(mu_xn / mux0_x)
-48     for y in range(Y):
-49         mu0y_y = mu0y[y]
-50         for nest in nests_y:
-51             mu_ny = np.sum(muxy[nest, y])
-52             e0_vals[nest, y] -= log(mu_ny / mu0y_y)
-53     return e0_vals
+28     Returns:
+29         the (X,Y) matrix of the parameter-independent part
+30         of the first derivative of the entropy.
+31     """
+32     nests_for_each_x, nests_for_each_y = additional_parameters
+33     nests_x = _change_indices(nests_for_each_x)
+34     nests_y = _change_indices(nests_for_each_y)
+35     muxy, mux0, mu0y, *_ = muhat.unpack()
+36     X, Y = muxy.shape
+37     e0_vals = np.zeros((X, Y))
+38
+39     for x in range(X):
+40         mux0_x = mux0[x]
+41         for nest in nests_x:
+42             mu_xn = np.sum(muxy[x, nest])
+43             e0_vals[x, nest] = -log(mu_xn / mux0_x)
+44     for y in range(Y):
+45         mu0y_y = mu0y[y]
+46         for nest in nests_y:
+47             mu_ny = np.sum(muxy[nest, y])
+48             e0_vals[nest, y] -= log(mu_ny / mu0y_y)
+49     return e0_vals
 ***** e_derivative_mu_nested_logit(muhat, additional_parameters) ¶ *****
 Returns the derivatives of the parameter-dependent part e
  wrt \mu
  for the nested logit.
 Parameters:
 Name                  Type      Description                    Default
 muhat                 Matching  a Matching                     required
 additional_parameters list[Any] a list with the nest structure required
 Returns:
 Type        Description
 ThreeArrays the parameter-dependent part of the hessian of the entropy
 ThreeArrays wrt (\mu,\mu)
             .
  Source code in cupid_matching/nested_logit.py
-191 def e_derivative_mu_nested_logit(
-192     muhat: Matching, additional_parameters: list[Any]
-193 ) -> ThreeArrays:
-194     """Returns the derivatives of the parameter-dependent part $e$
-195      wrt $\\mu$ for the nested logit.
+187 def e_derivative_mu_nested_logit(
+188     muhat: Matching, additional_parameters: list[Any]
+189 ) -> ThreeArrays:
+190     """Returns the derivatives of the parameter-dependent part $e$
+191      wrt $\\mu$ for the nested logit.
+192
+193     Args:
+194         muhat: a Matching
+195         additional_parameters: a list with the nest structure
 196
-197     Args:
-198         muhat: a Matching
-199         additional_parameters: a list with the nest structure
-200
-201     Returns:
-202         the parameter-dependent part of the hessian of the entropy
-203         wrt $(\\mu,\\mu)$.
-204     """
-205     nests_for_each_x, nests_for_each_y = additional_parameters
-206     nests_x = _change_indices(nests_for_each_x)
-207     nests_y = _change_indices(nests_for_each_y)
-208     n_rhos = len(nests_for_each_x)
-209     n_deltas = len(nests_for_each_y)
-210     n_alpha = n_rhos + n_deltas
-211
-212     muxy, *_ = muhat.unpack()
-213     X, Y = muxy.shape
-214
-215     hess_x = np.zeros((X, Y, Y, n_alpha))
-216     hess_y = np.zeros((X, Y, X, n_alpha))
-217     hess_xy = np.zeros((X, Y, n_alpha))
-218     der_logxy = 1.0 / muxy
-219
-220     for x in range(X):
-221         for i_n, nest in enumerate(nests_x):
-222             mux_nest_n = muxy[x, nest]
-223             mu_xn = np.sum(mux_nest_n)
-224             der_logxn = 1.0 / mu_xn
-225             for t in nest:
-226                 hess_x[x, nest, t, i_n] = der_logxn
-227             hess_xy[x, nest, i_n] = der_logxn - der_logxy[x, nest]
-228
-229     for y in range(Y):
-230         for i_n, nest in enumerate(nests_y):
-231             muy_nest_n = muxy[nest, y]
-232             mu_ny = np.sum(muy_nest_n)
-233             der_logny = 1.0 / mu_ny
-234             i_n2 = i_n + n_rhos
-235             for z in nest:
-236                 hess_y[nest, y, z, i_n2] = der_logny
-237             hess_xy[nest, y, i_n2] = der_logny - der_logxy[nest, y]
-238
-239     return hess_x, hess_y, hess_xy
+197     Returns:
+198         the parameter-dependent part of the hessian of the entropy
+199         wrt $(\\mu,\\mu)$.
+200     """
+201     nests_for_each_x, nests_for_each_y = additional_parameters
+202     nests_x = _change_indices(nests_for_each_x)
+203     nests_y = _change_indices(nests_for_each_y)
+204     n_rhos = len(nests_for_each_x)
+205     n_deltas = len(nests_for_each_y)
+206     n_alpha = n_rhos + n_deltas
+207
+208     muxy, *_ = muhat.unpack()
+209     X, Y = muxy.shape
+210
+211     hess_x = np.zeros((X, Y, Y, n_alpha))
+212     hess_y = np.zeros((X, Y, X, n_alpha))
+213     hess_xy = np.zeros((X, Y, n_alpha))
+214     der_logxy = 1.0 / muxy
+215
+216     for x in range(X):
+217         for i_n, nest in enumerate(nests_x):
+218             mux_nest_n = muxy[x, nest]
+219             mu_xn = np.sum(mux_nest_n)
+220             der_logxn = 1.0 / mu_xn
+221             for t in nest:
+222                 hess_x[x, nest, t, i_n] = der_logxn
+223             hess_xy[x, nest, i_n] = der_logxn - der_logxy[x, nest]
+224
+225     for y in range(Y):
+226         for i_n, nest in enumerate(nests_y):
+227             muy_nest_n = muxy[nest, y]
+228             mu_ny = np.sum(muy_nest_n)
+229             der_logny = 1.0 / mu_ny
+230             i_n2 = i_n + n_rhos
+231             for z in nest:
+232                 hess_y[nest, y, z, i_n2] = der_logny
+233             hess_xy[nest, y, i_n2] = der_logny - der_logxy[nest, y]
+234
+235     return hess_x, hess_y, hess_xy
 ***** e_derivative_r_nested_logit(muhat, additional_parameters) ¶ *****
 Returns the derivatives of the parameter-dependent part e
  wrt r
  for the nested logit.
 Parameters:
 Name                  Type      Description                    Default
 muhat                 Matching  a Matching                     required
 additional_parameters list[Any] a list with the nest structure required
 Returns:
 Type      Description
 TwoArrays the parameter-dependent part of the hessian of the entropy
 TwoArrays wrt (\mu,r)
           .
  Source code in cupid_matching/nested_logit.py
-242 def e_derivative_r_nested_logit(
-243     muhat: Matching, additional_parameters: list[Any]
-244 ) -> TwoArrays:
-245     """Returns the derivatives of the parameter-dependent part $e$
-246      wrt $r$ for the nested logit.
+238 def e_derivative_r_nested_logit(
+239     muhat: Matching, additional_parameters: list[Any]
+240 ) -> TwoArrays:
+241     """Returns the derivatives of the parameter-dependent part $e$
+242      wrt $r$ for the nested logit.
+243
+244     Args:
+245         muhat: a Matching
+246         additional_parameters: a list with the nest structure
 247
-248     Args:
-249         muhat: a Matching
-250         additional_parameters: a list with the nest structure
-251
-252     Returns:
-253         the parameter-dependent part of the hessian of the entropy
-254         wrt $(\\mu,r)$.
-255     """
-256     nests_for_each_x, nests_for_each_y = additional_parameters
-257     n_rhos = len(nests_for_each_x)
-258     n_deltas = len(nests_for_each_y)
-259     n_alpha = n_rhos + n_deltas
-260
-261     muxy, *_ = muhat.unpack()
-262     X, Y = muxy.shape
-263
-264     hess_n = np.zeros((X, Y, n_alpha))
-265     hess_m = np.zeros((X, Y, n_alpha))
-266
-267     return hess_n, hess_m
+248     Returns:
+249         the parameter-dependent part of the hessian of the entropy
+250         wrt $(\\mu,r)$.
+251     """
+252     nests_for_each_x, nests_for_each_y = additional_parameters
+253     n_rhos = len(nests_for_each_x)
+254     n_deltas = len(nests_for_each_y)
+255     n_alpha = n_rhos + n_deltas
+256
+257     muxy, *_ = muhat.unpack()
+258     X, Y = muxy.shape
+259
+260     hess_n = np.zeros((X, Y, n_alpha))
+261     hess_m = np.zeros((X, Y, n_alpha))
+262
+263     return hess_n, hess_m
 ***** e_nested_logit(muhat, additional_parameters) ¶ *****
 Returns the values of the parameter-dependent part e
  for the nested logit.
 Parameters:
 Name                  Type      Description                    Default
 muhat                 Matching  a Matching                     required
 additional_parameters list[Any] a list with the nest structure required
 Returns:
 Type       Description
 np.ndarray the (X,Y,n_alpha) array of the parameter-dependent part
 np.ndarray of the first derivative of the entropy.
  Source code in cupid_matching/nested_logit.py
-150 def e_nested_logit(
-151     muhat: Matching, additional_parameters: list[Any]
-152 ) -> np.ndarray:
-153     """Returns the values of the parameter-dependent part  $e$
-154     for the nested logit.
+146 def e_nested_logit(
+147     muhat: Matching, additional_parameters: list[Any]
+148 ) -> np.ndarray:
+149     """Returns the values of the parameter-dependent part  $e$
+150     for the nested logit.
+151
+152     Args:
+153         muhat: a Matching
+154         additional_parameters: a list with the nest structure
 155
-156     Args:
-157         muhat: a Matching
-158         additional_parameters: a list with the nest structure
-159
-160     Returns:
-161         the (X,Y,n_alpha) array of the parameter-dependent part
-162         of the first derivative of the entropy.
-163     """
-164     nests_for_each_x, nests_for_each_y = additional_parameters
-165     nests_x = _change_indices(nests_for_each_x)
-166     nests_y = _change_indices(nests_for_each_y)
-167     n_rhos = len(nests_for_each_x)
-168     n_deltas = len(nests_for_each_y)
-169     n_alpha = n_rhos + n_deltas
-170
-171     muxy, *_ = muhat.unpack()
-172     X, Y = muxy.shape
-173
-174     e_vals = np.zeros((X, Y, n_alpha))
-175
-176     for x in range(X):
-177         for i_n, nest in enumerate(nests_x):
-178             mux_nest_n = muxy[x, nest]
-179             mu_xn = np.sum(mux_nest_n)
-180             e_vals[x, nest, i_n] = -np.log(mux_nest_n / mu_xn)
-181
-182     for y in range(Y):
-183         for i_n, nest in enumerate(nests_y):
-184             muy_nest_n = muxy[nest, y]
-185             mu_ny = np.sum(muy_nest_n)
-186             e_vals[nest, y, (i_n + n_rhos)] -= np.log(muy_nest_n / mu_ny)
-187
-188     return e_vals
+156     Returns:
+157         the (X,Y,n_alpha) array of the parameter-dependent part
+158         of the first derivative of the entropy.
+159     """
+160     nests_for_each_x, nests_for_each_y = additional_parameters
+161     nests_x = _change_indices(nests_for_each_x)
+162     nests_y = _change_indices(nests_for_each_y)
+163     n_rhos = len(nests_for_each_x)
+164     n_deltas = len(nests_for_each_y)
+165     n_alpha = n_rhos + n_deltas
+166
+167     muxy, *_ = muhat.unpack()
+168     X, Y = muxy.shape
+169
+170     e_vals = np.zeros((X, Y, n_alpha))
+171
+172     for x in range(X):
+173         for i_n, nest in enumerate(nests_x):
+174             mux_nest_n = muxy[x, nest]
+175             mu_xn = np.sum(mux_nest_n)
+176             e_vals[x, nest, i_n] = -np.log(mux_nest_n / mu_xn)
+177
+178     for y in range(Y):
+179         for i_n, nest in enumerate(nests_y):
+180             muy_nest_n = muxy[nest, y]
+181             mu_ny = np.sum(muy_nest_n)
+182             e_vals[nest, y, (i_n + n_rhos)] -= np.log(muy_nest_n / mu_ny)
+183
+184     return e_vals
 
 Made with Material_for_MkDocs
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/objects.inv` & `cupid_matching-1.0.5/cupid_matching/site/objects.inv`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/poisson_glm/index.html` & `cupid_matching-1.0.5/cupid_matching/site/poisson_glm/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/site/poisson_glm_utils/index.html` & `cupid_matching-1.0.5/cupid_matching/site/poisson_glm_utils/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -973,15 +973,17 @@
 <span class="normal">135</span>
 <span class="normal">136</span>
 <span class="normal">137</span>
 <span class="normal">138</span>
 <span class="normal">139</span>
 <span class="normal">140</span>
 <span class="normal">141</span>
-<span class="normal">142</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="nd">@dataclass</span>
+<span class="normal">142</span>
+<span class="normal">143</span>
+<span class="normal">144</span></pre></div></td><td class="code"><div><pre><span></span><code><span class="nd">@dataclass</span>
 <span class="k">class</span> <span class="nc">PoissonGLMResults</span><span class="p">:</span>
 <span class="w">    </span><span class="sd">&quot;&quot;&quot;Stores and formats the estimation results.</span>
 
 <span class="sd">    Args:</span>
 <span class="sd">        X: int</span>
 <span class="sd">        Y: int</span>
 <span class="sd">        K: int</span>
@@ -1101,15 +1103,17 @@
                 <span class="n">repr_str</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; </span><span class="si">{</span><span class="n">coeff</span><span class="si">:</span><span class="s2"> &gt; 10.3f</span><span class="si">}</span><span class="s2">  (</span><span class="si">{</span><span class="n">stderrs_v</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="si">:</span><span class="s2"> &gt; 10.3f</span><span class="si">}</span><span class="s2">)</span><span class="se">\n</span><span class="s2">&quot;</span>
             <span class="n">print_stars</span><span class="p">(</span><span class="n">repr_str</span><span class="p">)</span>
 
         <span class="k">if</span> <span class="n">lambda_true</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="n">discrepancy</span> <span class="o">=</span> <span class="n">npmaxabs</span><span class="p">(</span><span class="n">lambda_true</span> <span class="o">-</span> <span class="n">estimates_beta</span><span class="p">)</span>
-            <span class="n">print_stars</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;The largest difference between true and estimated coefficients is </span><span class="si">{</span><span class="n">discrepancy</span><span class="si">:</span><span class="s2"> .2e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <span class="n">print_stars</span><span class="p">(</span>
+                <span class="sa">f</span><span class="s2">&quot;The largest difference between true and estimated coefficients is </span><span class="si">{</span><span class="n">discrepancy</span><span class="si">:</span><span class="s2"> .2e</span><span class="si">}</span><span class="s2">&quot;</span>
+            <span class="p">)</span>
             <span class="k">return</span> <span class="n">discrepancy</span>
 </code></pre></div></td></tr></table></div>
         </details>
 
   
 
   <div class="doc doc-children">
```

#### html2text {}

```diff
@@ -202,14 +202,16 @@
 136                 repr_str += f"   v_{i + 1}: {v_true[i]: > 10.3f} "
 137                 repr_str += f" {coeff: > 10.3f}  ({stderrs_v[i]: >
 138 10.3f})\n"
 139             print_stars(repr_str)
 140
 141         if lambda_true is None:
 142             return None
-            else:
-                discrepancy = npmaxabs(lambda_true - estimates_beta)
-                print_stars(f"The largest difference between true and estimated
-    coefficients is {discrepancy: .2e}")
+143         else:
+144             discrepancy = npmaxabs(lambda_true - estimates_beta)
+                print_stars(
+                    f"The largest difference between true and estimated
+    coefficients is {discrepancy: .2e}"
+                )
                 return discrepancy
 
 Made with Material_for_MkDocs
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/search/search_index.json` & `cupid_matching-1.0.5/cupid_matching/site/search/search_index.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'docs'": "{10: {'text': '<p>Returns the values of e_0 for the Choo and Siow model, using the "*

 * *           'finite-sample correction log(p+(1-p)/(2N))</p> <p>Parameters:</p> Name Type '*

 * *           'Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> '*

 * *           'required <p>Returns:</p> Type Description <code>np.ndarray</code> <p>the (X,Y) matrix '*

 * *           'of the first derivative of the entropy</p> Source code in '*

 * *           '<code>cupid_matching/choo_siow.py</code> <pre><c […]*

```diff
@@ -41,46 +41,51 @@
         },
         {
             "location": "#version-104",
             "text": "<ul> <li>added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.</li> <li>added two complete examples: example_choosiow.py and example_nestedlogit.py.</li> </ul>",
             "title": "version 1.0.4"
         },
         {
+            "location": "#version-105",
+            "text": "<ul> <li>simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.</li> </ul>",
+            "title": "version 1,0.5"
+        },
+        {
             "location": "choo_siow/",
             "text": "<p>The components of the derivative of the entropy for the Choo and Siow homoskedastic model.</p>",
             "title": "<code>choo_siow</code> module"
         },
         {
             "location": "choo_siow/#cupid_matching.choo_siow.e0_fun_choo_siow",
             "text": "<p>Returns the values of e_0 for the Choo and Siow model.</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>np.ndarray</code> <p>the (X,Y) matrix of the first derivative of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def e0_fun_choo_siow(muhat: Matching) -&gt; np.ndarray:\n\"\"\"Returns the values of $e_0$ for the Choo and Siow model.\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the (X,Y) matrix of the first derivative of the entropy\n    \"\"\"\n    entropy_res = _entropy_choo_siow(muhat, deriv=1)\n    return entropy_res[1]\n</code></pre>",
             "title": "<code>e0_fun_choo_siow(muhat)</code>"
         },
         {
             "location": "choo_siow/#cupid_matching.choo_siow.e0_fun_choo_siow_corrected",
-            "text": "<p>Returns the values of e_0 for the Choo and Siow model, using the finite-sample correction.</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>np.ndarray</code> <p>the (X,Y) matrix of the first derivative of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def e0_fun_choo_siow_corrected(\n        muhat: Matching\n) -&gt; np.ndarray:\n\"\"\"Returns the values of $e_0$ for the Choo and Siow model,\n    using the finite-sample correction.\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the (X,Y) matrix of the first derivative of the entropy\n    \"\"\"\n    entropy_res = _entropy_choo_siow(muhat, deriv=1)\n    e0_val = entropy_res[1]\n    muxy, mux0, mu0y, *_ = muhat.unpack()\n    n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)\n    e0_val_corrected = e0_val - (1.0 - muxy / n_households) / muxy\n    e0_val_corrected += ((1.0 - mux0 / n_households) / (2.0 * mux0)).reshape((-1, 1))\n    e0_val_corrected += ((1.0 - mu0y / n_households) / (2.0 * mu0y))\n    # print(f\"{npmaxabs(e0_val_corrected/e0_val - 1.0)=}\")\n    return e0_val_corrected\n</code></pre>",
+            "text": "<p>Returns the values of e_0 for the Choo and Siow model, using the finite-sample correction log(p+(1-p)/(2N))</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>np.ndarray</code> <p>the (X,Y) matrix of the first derivative of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def e0_fun_choo_siow_corrected(muhat: Matching) -&gt; np.ndarray:\n\"\"\"Returns the values of $e_0$ for the Choo and Siow model,\n    using the finite-sample correction log(p+(1-p)/(2N))\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the (X,Y) matrix of the first derivative of the entropy\n    \"\"\"\n    e0_val_corrected \\\n        = _der_entropy_choo_siow_corrected(muhat, hessian=False)\n    return e0_val_corrected\n</code></pre>",
             "title": "<code>e0_fun_choo_siow_corrected(muhat)</code>"
         },
         {
             "location": "choo_siow/#cupid_matching.choo_siow.hessian_mumu_choo_siow",
             "text": "<p>Returns the derivatives of e_0 in \\mu for the Choo and Siow model.</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>ThreeArrays</code> <p>the three components of the hessian wrt (\\mu,\\mu) of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def hessian_mumu_choo_siow(muhat: Matching) -&gt; ThreeArrays:\n\"\"\"Returns the derivatives of $e_0$ in $\\\\mu$\n    for the Choo and Siow model.\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the three components of the hessian wrt $(\\\\mu,\\\\mu)$ of the entropy\n    \"\"\"\n    entropy_res = _entropy_choo_siow(muhat, deriv=2)\n    hessmumu = entropy_res[2]\n    muxy, *_ = muhat.unpack()\n    X, Y = muxy.shape\n    hess_x = np.zeros((X, Y, Y))\n    hess_y = np.zeros((X, Y, X))\n    hess_xy = np.zeros((X, Y))\n    for x in range(X):\n        for y in range(Y):\n            d2xy = hessmumu[x, y, :, :]\n            hess_x[x, y, :] = d2xy[x, :]\n            hess_y[x, y, :] = d2xy[:, y]\n            hess_xy[x, y] = d2xy[x, y]\n    return hess_x, hess_y, hess_xy\n</code></pre>",
             "title": "<code>hessian_mumu_choo_siow(muhat)</code>"
         },
         {
             "location": "choo_siow/#cupid_matching.choo_siow.hessian_mumu_choo_siow_corrected",
-            "text": "<p>Returns the derivatives of e_0 in \\mu for the Choo and Siow model, with the small sample correction</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>ThreeArrays</code> <p>the three components of the hessian wrt (\\mu,\\mu) of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def hessian_mumu_choo_siow_corrected(\n        muhat: Matching\n) -&gt; ThreeArrays:\n\"\"\"Returns the derivatives of $e_0$ in $\\\\mu$\n    for the Choo and Siow model, with the small sample correction\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the three components of the hessian wrt $(\\\\mu,\\\\mu)$ of the entropy\n    \"\"\"\n    hess_x, hess_y, hess_xy = hessian_mumu_choo_siow(muhat)\n    muxy, mux0, mu0y, *_ = muhat.unpack()\n    n_households = np.sum(muxy) + np.sum(mux0) + np.sum(mu0y)\n    X, Y = hess_xy.shape\n    corr_x0 = 1.0 / (2.0*mux0*mux0)\n    corr_0y = 1.0 / (2.0*mu0y*mu0y)\n    corr_xy = -1.0 / (muxy*muxy)\n    for x in range(X):\n        for y in range(Y):\n            hess_x[x, y, y] += corr_x0[x]\n            hess_y[x, y, x] += corr_0y[y]\n            hess_xy[x, y] += corr_xy[x, y]\n\n    return hess_x, hess_y, hess_xy\n</code></pre>",
+            "text": "<p>Returns the derivatives of e_0 in \\mu for the Choo and Siow model, with the small sample correction</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>ThreeArrays</code> <p>the three components of the hessian wrt (\\mu,\\mu) of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def hessian_mumu_choo_siow_corrected(muhat: Matching) -&gt; ThreeArrays:\n\"\"\"Returns the derivatives of $e_0$ in $\\\\mu$\n    for the Choo and Siow model, with the small sample correction\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the three components of the hessian wrt $(\\\\mu,\\\\mu)$ of the entropy\n    \"\"\"\n    _, hessmumu, _ \\\n        = _der_entropy_choo_siow_corrected(muhat, hessian=True)\n    muxy, *_ = muhat.unpack()\n    X, Y = muxy.shape\n    hess_x = np.zeros((X, Y, Y))\n    hess_y = np.zeros((X, Y, X))\n    hess_xy = np.zeros((X, Y))\n    for x in range(X):\n        for y in range(Y):\n            d2xy = hessmumu[x, y, :, :]\n            hess_x[x, y, :] = d2xy[x, :]\n            hess_y[x, y, :] = d2xy[:, y]\n            hess_xy[x, y] = d2xy[x, y]\n    return hess_x, hess_y, hess_xy\n</code></pre>",
             "title": "<code>hessian_mumu_choo_siow_corrected(muhat)</code>"
         },
         {
             "location": "choo_siow/#cupid_matching.choo_siow.hessian_mur_choo_siow",
             "text": "<p>Returns the derivatives of e_0 in r for the Choo and Siow model.</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>TwoArrays</code> <p>the two components of the hessian wrt (\\mu,r) of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def hessian_mur_choo_siow(muhat: Matching) -&gt; TwoArrays:\n\"\"\"Returns the derivatives of $e_0$ in $r$\n    for the Choo and Siow model.\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the two components of the hessian wrt $(\\\\mu,r)$ of the entropy\n    \"\"\"\n    entropy_res = _entropy_choo_siow(muhat, deriv=2)\n    hessmur = entropy_res[3]\n    muxy, *_ = muhat.unpack()\n    X, Y = muxy.shape\n    hess_nx = np.zeros((X, Y))\n    hess_my = np.zeros((X, Y))\n    for x in range(X):\n        for y in range(Y):\n            d2r = hessmur[x, y, :]\n            hess_nx[x, y] = d2r[x]\n            hess_my[x, y] = d2r[X + y]\n    return hess_nx, hess_my\n</code></pre>",
             "title": "<code>hessian_mur_choo_siow(muhat)</code>"
         },
         {
             "location": "choo_siow/#cupid_matching.choo_siow.hessian_mur_choo_siow_corrected",
-            "text": "<p>Returns the derivatives of e_0 in r for the Choo and Siow model, with the small sample correction</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>TwoArrays</code> <p>the two components of the hessian wrt (\\mu,r) of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def hessian_mur_choo_siow_corrected(\n        muhat: Matching\n) -&gt; TwoArrays:\n\"\"\"Returns the derivatives of $e_0$ in $r$\n    for the Choo and Siow model, with the small sample correction\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the two components of the hessian wrt $(\\\\mu,r)$ of the entropy\n    \"\"\"\n    hess_nx, hess_my = hessian_mur_choo_siow(muhat)\n    _, mux0, mu0y, *_ = muhat.unpack()\n    corr_nx = 1.0 / (2.0*mux0*mux0)\n    corr_my = 1.0 / (2.0*mu0y*mu0y)\n    X, Y = mux0.size, mu0y.size\n    for x in range(X):\n        hess_my[x, :] += corr_my\n    for y in range(Y):\n        hess_nx[:, y] += corr_nx\n    return hess_nx, hess_my\n</code></pre>",
+            "text": "<p>Returns the derivatives of e_0 in r for the Choo and Siow model, with the small sample correction</p> <p>Parameters:</p> Name Type Description Default <code>muhat</code> <code>Matching</code> <p>a Matching</p> required <p>Returns:</p> Type Description <code>TwoArrays</code> <p>the two components of the hessian wrt (\\mu,r) of the entropy</p> Source code in <code>cupid_matching/choo_siow.py</code> <pre><code>def hessian_mur_choo_siow_corrected(muhat: Matching) -&gt; TwoArrays:\n\"\"\"Returns the derivatives of $e_0$ in $r$\n    for the Choo and Siow model, with the small sample correction\n\n    Args:\n        muhat: a Matching\n\n    Returns:\n        the two components of the hessian wrt $(\\\\mu,r)$ of the entropy\n    \"\"\"\n    _, _, hessmur \\\n        = _der_entropy_choo_siow_corrected(muhat, hessian=True)\n    muxy, *_ = muhat.unpack()\n    X, Y = muxy.shape\n    hess_nx = np.zeros((X, Y))\n    hess_my = np.zeros((X, Y))\n    for x in range(X):\n        for y in range(Y):\n            d2r = hessmur[x, y, :]\n            hess_nx[x, y] = d2r[x]\n            hess_my[x, y] = d2r[X + y]\n    return hess_nx, hess_my\n</code></pre>",
             "title": "<code>hessian_mur_choo_siow_corrected(muhat)</code>"
         },
         {
             "location": "choo_siow_gender_heteroskedastic/",
             "text": "<p>The components of the derivative of the entropy for the Choo and Siow gender-heteroskedastic model.</p> <p>We normalize the standard error for the X side at 1, and we estimate the standard error on the Y side.</p>",
             "title": "<code>choo_siow_gender_heteroskedastic</code> module"
         },
@@ -207,35 +212,35 @@
         {
             "location": "example_choosiow/",
             "text": "<p>example using the Choo and Siow homoskedastic model</p>",
             "title": "<code>example_choosiow</code> module"
         },
         {
             "location": "example_choosiow/#cupid_matching.example_choosiow.create_choosiow_population",
-            "text": "<p>we simulate a Choo and Siow population with equal numbers of men and women of each type and random bases dunctions and coefficients</p> <pre><code>Args:\n X: number of types of men\n Y: number of types of women\n K: random basis functions\n std_betas: the coefficients are drawn from a centered normal\n             with this standard deviation\n\nReturns:\n    a ChooSiowPrimitives instance, the basis functions, and the coefficients\n</code></pre> Source code in <code>cupid_matching/example_choosiow.py</code> <pre><code>def create_choosiow_population(X: int, Y: int, K: int,\n                               std_betas: Optional[float] = 1.0) \\\n        -&gt; Tuple[ChooSiowPrimitives, np.ndarray, np.ndarray]:\n\"\"\"\n    we simulate a Choo and Siow population\n    with equal numbers of men and women of each type\n    and random bases dunctions and coefficients\n\n        Args:\n         X: number of types of men\n         Y: number of types of women\n         K: random basis functions\n         std_betas: the coefficients are drawn from a centered normal\n                     with this standard deviation\n\n        Returns:\n            a ChooSiowPrimitives instance, the basis functions, and the coefficients\n    \"\"\"\n    betas_true = std_betas * np.random.randn(K)\n    phi_bases = np.random.randn(X, Y, K)\n    n = np.ones(X)\n    m = np.ones(Y)\n    Phi = phi_bases @ betas_true\n    choo_siow_instance = ChooSiowPrimitives(Phi, n, m)\n    return choo_siow_instance, phi_bases, betas_true\n</code></pre>",
+            "text": "<p>we simulate a Choo and Siow population with equal numbers of men and women of each type and random bases dunctions and coefficients</p> <pre><code>Args:\n X: number of types of men\n Y: number of types of women\n K: random basis functions\n std_betas: the coefficients are drawn from a centered normal\n             with this standard deviation\n\nReturns:\n    a ChooSiowPrimitives instance, the basis functions, and the coefficients\n</code></pre> Source code in <code>cupid_matching/example_choosiow.py</code> <pre><code>def create_choosiow_population(\n    X: int, Y: int, K: int, std_betas: Optional[float] = 1.0\n) -&gt; Tuple[ChooSiowPrimitives, np.ndarray, np.ndarray]:\n\"\"\"\n    we simulate a Choo and Siow population\n    with equal numbers of men and women of each type\n    and random bases dunctions and coefficients\n\n        Args:\n         X: number of types of men\n         Y: number of types of women\n         K: random basis functions\n         std_betas: the coefficients are drawn from a centered normal\n                     with this standard deviation\n\n        Returns:\n            a ChooSiowPrimitives instance, the basis functions, and the coefficients\n    \"\"\"\n    betas_true = std_betas * np.random.randn(K)\n    phi_bases = np.random.randn(X, Y, K)\n    n = np.ones(X)\n    m = np.ones(Y)\n    Phi = phi_bases @ betas_true\n    choo_siow_instance = ChooSiowPrimitives(Phi, n, m)\n    return choo_siow_instance, phi_bases, betas_true\n</code></pre>",
             "title": "<code>create_choosiow_population(X, Y, K, std_betas=1.0)</code>"
         },
         {
             "location": "example_choosiow/#cupid_matching.example_choosiow.mde_estimate",
-            "text": "<p>we estimate the parameters using the minimum distance estimator</p> <p>Parameters:</p> Name Type Description Default <code>mus_sim</code> <code>Matching</code> <p>a Choo and Siow Matching</p> required <code>phi_bases</code> <code>np.ndarray</code> <p>the basis functions</p> required <code>betas_true</code> <code>np.ndarray</code> <p>their true coefficients</p> required <code>entropy</code> <code>EntropyFunctions</code> <p>the entropy functions we use</p> required <code>title</code> <code>str</code> <p>the name of the estimator</p> required <p>Returns:</p> Type Description <code>float</code> <p>the largest absolute difference between the true and estimated coefficients</p> Source code in <code>cupid_matching/example_choosiow.py</code> <pre><code>def mde_estimate(mus_sim: Matching,\n                 phi_bases: np.ndarray,\n                 betas_true: np.ndarray,\n                 entropy: EntropyFunctions,\n                 title: str) -&gt; float:\n\"\"\"we estimate the parameters using the minimum distance estimator\n\n    Args:\n        mus_sim: a Choo and Siow Matching\n        phi_bases: the basis functions\n        betas_true: their true coefficients\n        entropy: the entropy functions we use\n        title: the name of the estimator\n\n    Returns:\n        the largest absolute difference between the true and estimated coefficients\n    \"\"\"\n    print_stars(f\"    {title}\")\n    mde_results = estimate_semilinear_mde(\n        mus_sim, phi_bases, entropy\n    )\n    mde_discrepancy = mde_results.print_results(true_coeffs=betas_true)\n    return mde_discrepancy\n</code></pre>",
+            "text": "<p>we estimate the parameters using the minimum distance estimator</p> <p>Parameters:</p> Name Type Description Default <code>mus_sim</code> <code>Matching</code> <p>a Choo and Siow Matching</p> required <code>phi_bases</code> <code>np.ndarray</code> <p>the basis functions</p> required <code>betas_true</code> <code>np.ndarray</code> <p>their true coefficients</p> required <code>entropy</code> <code>EntropyFunctions</code> <p>the entropy functions we use</p> required <code>title</code> <code>str</code> <p>the name of the estimator</p> required <p>Returns:</p> Type Description <code>float</code> <p>the largest absolute difference between the true and estimated coefficients</p> Source code in <code>cupid_matching/example_choosiow.py</code> <pre><code>def mde_estimate(\n    mus_sim: Matching,\n    phi_bases: np.ndarray,\n    betas_true: np.ndarray,\n    entropy: EntropyFunctions,\n    title: str,\n) -&gt; float:\n\"\"\"we estimate the parameters using the minimum distance estimator\n\n    Args:\n        mus_sim: a Choo and Siow Matching\n        phi_bases: the basis functions\n        betas_true: their true coefficients\n        entropy: the entropy functions we use\n        title: the name of the estimator\n\n    Returns:\n        the largest absolute difference between the true and estimated coefficients\n    \"\"\"\n    print_stars(f\"    {title}\")\n    mde_results = estimate_semilinear_mde(mus_sim, phi_bases, entropy)\n    mde_discrepancy = mde_results.print_results(true_coeffs=betas_true)\n    return mde_discrepancy\n</code></pre>",
             "title": "<code>mde_estimate(mus_sim, phi_bases, betas_true, entropy, title)</code>"
         },
         {
             "location": "example_nestedlogit/",
             "text": "<p>example using a simple two-layer nested logit model One nest on each side must consist of the 0 option. The other nests are specified as nested lists. E.g. [[1, 3], [2,4]] describes two nests, one with types 1 and 3, and the other with types 2 and 4. On each side, the nests are the same for each type, with the same parameters.</p>",
             "title": "<code>example_nestedlogit</code> module"
         },
         {
             "location": "example_nestedlogit/#cupid_matching.example_nestedlogit.create_nestedlogit_population",
-            "text": "<p>we simulate a nested logit population with equal numbers of men and women of each type and random bases dunctions and coefficients</p> <pre><code>Args:\n X: number of types of men\n Y: number of types of women\n K: random basis functions\n std_alphas: the nest parameters are drawn from a U[0, std_alphas] distribution\n std_betas: the coefficients of the bases are drawn from a centered normal\n             with this standard deviation\n\nReturns:\n    a NestedLogitPrimitives instance, the basis functions, the true coefficients,\n    and the entropy functions\n</code></pre> Source code in <code>cupid_matching/example_nestedlogit.py</code> <pre><code>def create_nestedlogit_population(X: int, Y: int, K: int,\n                                  std_alphas: Optional[float] = 0.5,\n                                  std_betas: Optional[float] = 1.0) \\\n        -&gt; Tuple[NestedLogitPrimitives, np.ndarray, np.ndarray, EntropyFunctions, EntropyFunctions]:\n\"\"\"\n    we simulate a nested logit population\n    with equal numbers of men and women of each type\n    and random bases dunctions and coefficients\n\n        Args:\n         X: number of types of men\n         Y: number of types of women\n         K: random basis functions\n         std_alphas: the nest parameters are drawn from a U[0, std_alphas] distribution\n         std_betas: the coefficients of the bases are drawn from a centered normal\n                     with this standard deviation\n\n        Returns:\n            a NestedLogitPrimitives instance, the basis functions, the true coefficients,\n            and the entropy functions\n    \"\"\"\n    X, Y, K = 10, 12, 5\n    nests_for_each_x = [\n        list(range(1, Y // 2 + 1)),\n        list(range(Y // 2 + 1, Y + 1)),\n    ]\n    nests_for_each_y = [\n        list(range(1, X // 2 + 1)),\n        list(range(X // 2 + 1, X + 1)),\n    ]\n\n    n = np.ones(X)\n    m = np.ones(Y)\n    phi_bases = np.random.randn(X, Y, K)\n\n    entropy_nested_logit, entropy_nested_logit_numeric = setup_standard_nested_logit(nests_for_each_x,\n                                                                                     nests_for_each_y)\n    n_rhos, n_deltas = len(nests_for_each_x), len(nests_for_each_y)\n    n_alphas = n_rhos + n_deltas\n\n    betas_true = std_betas * np.random.randn(K)\n    alphas_true = std_alphas * np.random.uniform(size=n_alphas)\n\n    Phi = phi_bases @ betas_true\n    nested_logit_instance = NestedLogitPrimitives(\n        Phi, n, m, nests_for_each_x, nests_for_each_y, alphas_true\n    )\n    true_coeffs = np.concatenate((alphas_true, betas_true))\n    return nested_logit_instance, phi_bases, true_coeffs, entropy_nested_logit, entropy_nested_logit_numeric\n</code></pre>",
+            "text": "<p>we simulate a nested logit population with equal numbers of men and women of each type and random bases dunctions and coefficients</p> <pre><code>Args:\n X: number of types of men\n Y: number of types of women\n K: random basis functions\n std_alphas: the nest parameters are drawn from a U[0, std_alphas] distribution\n std_betas: the coefficients of the bases are drawn from a centered normal\n             with this standard deviation\n\nReturns:\n    a NestedLogitPrimitives instance, the basis functions, the true coefficients,\n    and the entropy functions\n</code></pre> Source code in <code>cupid_matching/example_nestedlogit.py</code> <pre><code>def create_nestedlogit_population(\n    X: int,\n    Y: int,\n    K: int,\n    std_alphas: Optional[float] = 0.5,\n    std_betas: Optional[float] = 1.0,\n) -&gt; Tuple[\n    NestedLogitPrimitives,\n    np.ndarray,\n    np.ndarray,\n    EntropyFunctions,\n    EntropyFunctions,\n]:\n\"\"\"\n    we simulate a nested logit population\n    with equal numbers of men and women of each type\n    and random bases dunctions and coefficients\n\n        Args:\n         X: number of types of men\n         Y: number of types of women\n         K: random basis functions\n         std_alphas: the nest parameters are drawn from a U[0, std_alphas] distribution\n         std_betas: the coefficients of the bases are drawn from a centered normal\n                     with this standard deviation\n\n        Returns:\n            a NestedLogitPrimitives instance, the basis functions, the true coefficients,\n            and the entropy functions\n    \"\"\"\n    X, Y, K = 10, 12, 5\n    nests_for_each_x = [\n        list(range(1, Y // 2 + 1)),\n        list(range(Y // 2 + 1, Y + 1)),\n    ]\n    nests_for_each_y = [\n        list(range(1, X // 2 + 1)),\n        list(range(X // 2 + 1, X + 1)),\n    ]\n\n    n = np.ones(X)\n    m = np.ones(Y)\n    phi_bases = np.random.randn(X, Y, K)\n\n    (\n        entropy_nested_logit,\n        entropy_nested_logit_numeric,\n    ) = setup_standard_nested_logit(nests_for_each_x, nests_for_each_y)\n    n_rhos, n_deltas = len(nests_for_each_x), len(nests_for_each_y)\n    n_alphas = n_rhos + n_deltas\n\n    betas_true = std_betas * np.random.randn(K)\n    alphas_true = std_alphas * np.random.uniform(size=n_alphas)\n\n    Phi = phi_bases @ betas_true\n    nested_logit_instance = NestedLogitPrimitives(\n        Phi, n, m, nests_for_each_x, nests_for_each_y, alphas_true\n    )\n    true_coeffs = np.concatenate((alphas_true, betas_true))\n    return (\n        nested_logit_instance,\n        phi_bases,\n        true_coeffs,\n        entropy_nested_logit,\n        entropy_nested_logit_numeric,\n    )\n</code></pre>",
             "title": "<code>create_nestedlogit_population(X, Y, K, std_alphas=0.5, std_betas=1.0)</code>"
         },
         {
             "location": "example_nestedlogit/#cupid_matching.example_nestedlogit.mde_estimate",
-            "text": "<p>we estimate the parameters using the minimum distance estimator</p> <p>Parameters:</p> Name Type Description Default <code>mus_sim</code> <code>Matching</code> <p>a Choo and Siow Matching</p> required <code>phi_bases</code> <code>np.ndarray</code> <p>the basis functions</p> required <code>true_coeffs</code> <code>np.ndarray</code> <p>their true coefficients and  the nesting parameters</p> required <code>entropy</code> <code>EntropyFunctions</code> <p>the entropy functions we use</p> required <code>title</code> <code>str</code> <p>the name of the estimator</p> required <p>Returns:</p> Type Description <code>float</code> <p>the largest absolute difference between the true and estimated coefficients</p> Source code in <code>cupid_matching/example_nestedlogit.py</code> <pre><code>def mde_estimate(mus_sim: Matching,\n                 phi_bases: np.ndarray,\n                 true_coeffs: np.ndarray,\n                 entropy: EntropyFunctions,\n                 title: str) -&gt; float:\n\"\"\"we estimate the parameters using the minimum distance estimator\n\n    Args:\n        mus_sim: a Choo and Siow Matching\n        phi_bases: the basis functions\n        true_coeffs: their true coefficients and  the nesting parameters\n        entropy: the entropy functions we use\n        title: the name of the estimator\n\n    Returns:\n        the largest absolute difference between the true and estimated coefficients\n    \"\"\"\n    print_stars(f\"    {title}\")\n    mde_results = estimate_semilinear_mde(\n        mus_sim, phi_bases, entropy,\n        additional_parameters=entropy.additional_parameters,\n    )\n    mde_discrepancy = mde_results.print_results(true_coeffs=true_coeffs)\n    return mde_discrepancy\n</code></pre>",
+            "text": "<p>we estimate the parameters using the minimum distance estimator</p> <p>Parameters:</p> Name Type Description Default <code>mus_sim</code> <code>Matching</code> <p>a Choo and Siow Matching</p> required <code>phi_bases</code> <code>np.ndarray</code> <p>the basis functions</p> required <code>true_coeffs</code> <code>np.ndarray</code> <p>their true coefficients and  the nesting parameters</p> required <code>entropy</code> <code>EntropyFunctions</code> <p>the entropy functions we use</p> required <code>title</code> <code>str</code> <p>the name of the estimator</p> required <p>Returns:</p> Type Description <code>float</code> <p>the largest absolute difference between the true and estimated coefficients</p> Source code in <code>cupid_matching/example_nestedlogit.py</code> <pre><code>def mde_estimate(\n    mus_sim: Matching,\n    phi_bases: np.ndarray,\n    true_coeffs: np.ndarray,\n    entropy: EntropyFunctions,\n    title: str,\n) -&gt; float:\n\"\"\"we estimate the parameters using the minimum distance estimator\n\n    Args:\n        mus_sim: a Choo and Siow Matching\n        phi_bases: the basis functions\n        true_coeffs: their true coefficients and  the nesting parameters\n        entropy: the entropy functions we use\n        title: the name of the estimator\n\n    Returns:\n        the largest absolute difference between the true and estimated coefficients\n    \"\"\"\n    print_stars(f\"    {title}\")\n    mde_results = estimate_semilinear_mde(\n        mus_sim,\n        phi_bases,\n        entropy,\n        additional_parameters=entropy.additional_parameters,\n    )\n    mde_discrepancy = mde_results.print_results(true_coeffs=true_coeffs)\n    return mde_discrepancy\n</code></pre>",
             "title": "<code>mde_estimate(mus_sim, phi_bases, true_coeffs, entropy, title)</code>"
         },
         {
             "location": "ipfp_solvers/",
             "text": "<p>Implementations of the IPFP algorithm to solve for equilibrium and do comparative statics in several variants of the <code>Choo and Siow 2006 &lt;https://www.jstor.org/stable/10.1086/498585?seq=1&gt;</code>_ model:</p> <ul> <li>homoskedastic with singles (as in Choo and Siow 2006)</li> <li>homoskedastic without singles</li> <li>gender-heteroskedastic: with a scale parameter on the error term for women</li> <li>gender- and type-heteroskedastic: with a scale parameter on the error term    for each gender and type</li> <li>two-level nested logit, with nests and nest parameters that do not depend on the type,    and {0} as the first nest</li> </ul> <p>Each solver, when fed the joint surplus and margins, returns the equilibrium matching patterns, the adding-up errors on the margins, and if requested (using <code>gr=True</code>) the derivatives of the matching patterns in all primitives.</p>",
             "title": "<code>ipfp_solvers</code> module"
         },
@@ -287,15 +292,15 @@
         {
             "location": "min_distance_utils/",
             "text": "<p>Utility programs used in <code>min_distance.py</code>.</p>",
             "title": "<code>min_distance_utils</code> module"
         },
         {
             "location": "min_distance_utils/#cupid_matching.min_distance_utils.MDEResults",
-            "text": "<p>The results from minimum-distance estimation and testing.</p> <p>Parameters:</p> Name Type Description Default <code>X</code> <code>int</code> <p>int</p> required <code>Y</code> <code>int</code> <p>int</p> required <code>K</code> <code>int</code> <p>int</p> required <code>number_households</code> <code>int</code> <p>int</p> required <code>estimated_coefficients</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>varcov_coefficients</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_coefficients</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_Phi</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>test_statistic</code> <code>float</code> <p>float</p> required <code>test_pvalue</code> <code>float</code> <p>float</p> required <code>ndf</code> <code>int</code> <p>int</p> required <code>parameterized_entropy</code> <code>Optional[bool]</code> <p>Optional[bool] = False</p> <code>False</code> Source code in <code>cupid_matching/min_distance_utils.py</code> <pre><code>@dataclass\nclass MDEResults:\n\"\"\"\n    The results from minimum-distance estimation and testing.\n\n    Args:\n        X: int\n        Y: int\n        K: int\n        number_households: int\n        estimated_coefficients: np.ndarray\n        varcov_coefficients: np.ndarray\n        stderrs_coefficients: np.ndarray\n        estimated_Phi: np.ndarray\n        test_statistic: float\n        test_pvalue: float\n        ndf: int\n        parameterized_entropy: Optional[bool] = False\n    \"\"\"\n\n    X: int\n    Y: int\n    K: int\n    number_households: int\n    estimated_coefficients: np.ndarray\n    varcov_coefficients: np.ndarray\n    stderrs_coefficients: np.ndarray\n    estimated_Phi: np.ndarray\n    test_statistic: float\n    test_pvalue: float\n    ndf: int\n    parameterized_entropy: Optional[bool] = False\n\n    def __str__(self):\n        line_stars = \"*\" * 80 + \"\\n\"\n        if self.parameterized_entropy:\n            n_alpha = self.estimated_coefficients.size - self.K\n            entropy_str = f\"     The entropy has {n_alpha} parameters.\"\n        else:\n            entropy_str = \"     The entropy is parameter-free.\"\n            n_alpha = 0\n        model_str = f\"The data has {self.number_households} households\\n\\n\"\n        model_str += (\n            f\"The model has {self.X}x{self.Y} margins\\n {entropy_str} \\n\"\n        )\n        model_str += f\"We use {self.K} basis functions.\\n\\n\"\n        repr_str = line_stars + model_str\n        repr_str += (\n            \"The estimated coefficients (and their standard errors) are\\n\\n\"\n        )\n        if self.parameterized_entropy:\n            for i, coeff in enumerate(self.estimated_coefficients[:n_alpha]):\n                repr_str += (\n                    f\"   alpha({i + 1}): {coeff: &gt; 10.3f}  \"\n                    + f\"({self.stderrs_coefficients[i]: .3f})\\n\"\n                )\n            repr_str += \"\\n\"\n        for i, coeff in enumerate(self.estimated_coefficients[n_alpha:]):\n            repr_str += (\n                f\"   base {i + 1}: {coeff: &gt; 10.3f} \"\n                + f\"({self.stderrs_coefficients[n_alpha + i]: .3f})\\n\"\n            )\n        repr_str += \"\\nSpecification test:\\n\"\n        repr_str += f\"   the value of the test statistic is {self.test_statistic: &gt; 10.3f}\\n\"\n        repr_str += f\"     for a chi2({self.ndf}), the p-value is {self.test_pvalue: &gt; 10.3f}\\n\"\n        return repr_str + line_stars\n\n    def print_results(\n        self, true_coeffs: Optional[np.ndarray] = None, n_alpha: int = 0\n    ) -&gt; None | float:\n        estimates = self.estimated_coefficients\n        stderrs = self.stderrs_coefficients\n\n        if true_coeffs is not None:\n            repr_str = (\n                \"The true and estimated coefficients \"\n                + \"(and their standard errors) are\\n\\n\"\n            )\n            for i, coeff in enumerate(estimates[:n_alpha]):\n                repr_str += f\"   alpha({i + 1}): {true_coeffs[i]: &gt; 10.3f}\"\n                repr_str += f\"{coeff: &gt; 10.3f}  ({stderrs[i]: &gt; 10.3f})\\n\"\n                repr_str += \"\\n\"\n            for i, coeff in enumerate(estimates[n_alpha:]):\n                j = n_alpha + i\n                repr_str += (\n                    f\"   base {i + 1}: {true_coeffs[j]: &gt; 10.3f}  \"\n                    + f\"{coeff: &gt; 10.3f}  ({stderrs[j]: &gt; 10.3f})\\n\"\n                )\n            print_stars(repr_str)\n            discrepancy = npmaxabs(true_coeffs - estimates)\n            print_stars(f\"The largest difference between true and estimated coefficients is {discrepancy: .2e}\")\n        else:\n            repr_str = (\n                \"The estimated coefficients \"\n                + \"(and their standard errors) are\\n\\n\"\n            )\n            for i, coeff in enumerate(estimates[:n_alpha]):\n                repr_str + f\"{coeff: &gt; 10.3f}  ({stderrs[i]: &gt; 10.3f})\\n\"\n                repr_str += \"\\n\"\n            for i, coeff in enumerate(estimates[n_alpha:]):\n                j = n_alpha + i\n                repr_str += f\"{coeff: &gt; 10.3f}  ({stderrs[j]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        repr_str = \"\\nSpecification test:\\n\"\n        repr_str += (\n            \"   the value of the test statistic is \"\n            + f\"{self.test_statistic: &gt; 10.3f}\\n\"\n        )\n        repr_str += (\n            f\"     for a chi2({self.ndf}), \"\n            + f\"the p-value is {self.test_pvalue: &gt; 10.3f}\\n\"\n        )\n        print_stars(repr_str)\n        if true_coeffs is not None:\n            return discrepancy\n        return None\n</code></pre>",
+            "text": "<p>The results from minimum-distance estimation and testing.</p> <p>Parameters:</p> Name Type Description Default <code>X</code> <code>int</code> <p>int</p> required <code>Y</code> <code>int</code> <p>int</p> required <code>K</code> <code>int</code> <p>int</p> required <code>number_households</code> <code>int</code> <p>int</p> required <code>estimated_coefficients</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>varcov_coefficients</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_coefficients</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_Phi</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>test_statistic</code> <code>float</code> <p>float</p> required <code>test_pvalue</code> <code>float</code> <p>float</p> required <code>ndf</code> <code>int</code> <p>int</p> required <code>parameterized_entropy</code> <code>Optional[bool]</code> <p>Optional[bool] = False</p> <code>False</code> Source code in <code>cupid_matching/min_distance_utils.py</code> <pre><code>@dataclass\nclass MDEResults:\n\"\"\"\n    The results from minimum-distance estimation and testing.\n\n    Args:\n        X: int\n        Y: int\n        K: int\n        number_households: int\n        estimated_coefficients: np.ndarray\n        varcov_coefficients: np.ndarray\n        stderrs_coefficients: np.ndarray\n        estimated_Phi: np.ndarray\n        test_statistic: float\n        test_pvalue: float\n        ndf: int\n        parameterized_entropy: Optional[bool] = False\n    \"\"\"\n\n    X: int\n    Y: int\n    K: int\n    number_households: int\n    estimated_coefficients: np.ndarray\n    varcov_coefficients: np.ndarray\n    stderrs_coefficients: np.ndarray\n    estimated_Phi: np.ndarray\n    test_statistic: float\n    test_pvalue: float\n    ndf: int\n    parameterized_entropy: Optional[bool] = False\n\n    def __str__(self):\n        line_stars = \"*\" * 80 + \"\\n\"\n        if self.parameterized_entropy:\n            n_alpha = self.estimated_coefficients.size - self.K\n            entropy_str = f\"     The entropy has {n_alpha} parameters.\"\n        else:\n            entropy_str = \"     The entropy is parameter-free.\"\n            n_alpha = 0\n        model_str = f\"The data has {self.number_households} households\\n\\n\"\n        model_str += (\n            f\"The model has {self.X}x{self.Y} margins\\n {entropy_str} \\n\"\n        )\n        model_str += f\"We use {self.K} basis functions.\\n\\n\"\n        repr_str = line_stars + model_str\n        repr_str += (\n            \"The estimated coefficients (and their standard errors) are\\n\\n\"\n        )\n        if self.parameterized_entropy:\n            for i, coeff in enumerate(self.estimated_coefficients[:n_alpha]):\n                repr_str += (\n                    f\"   alpha({i + 1}): {coeff: &gt; 10.3f}  \"\n                    + f\"({self.stderrs_coefficients[i]: .3f})\\n\"\n                )\n            repr_str += \"\\n\"\n        for i, coeff in enumerate(self.estimated_coefficients[n_alpha:]):\n            repr_str += (\n                f\"   base {i + 1}: {coeff: &gt; 10.3f} \"\n                + f\"({self.stderrs_coefficients[n_alpha + i]: .3f})\\n\"\n            )\n        repr_str += \"\\nSpecification test:\\n\"\n        repr_str += f\"   the value of the test statistic is {self.test_statistic: &gt; 10.3f}\\n\"\n        repr_str += f\"     for a chi2({self.ndf}), the p-value is {self.test_pvalue: &gt; 10.3f}\\n\"\n        return repr_str + line_stars\n\n    def print_results(\n        self, true_coeffs: Optional[np.ndarray] = None, n_alpha: int = 0\n    ) -&gt; None | float:\n        estimates = self.estimated_coefficients\n        stderrs = self.stderrs_coefficients\n\n        if true_coeffs is not None:\n            repr_str = (\n                \"The true and estimated coefficients \"\n                + \"(and their standard errors) are\\n\\n\"\n            )\n            for i, coeff in enumerate(estimates[:n_alpha]):\n                repr_str += f\"   alpha({i + 1}): {true_coeffs[i]: &gt; 10.3f}\"\n                repr_str += f\"{coeff: &gt; 10.3f}  ({stderrs[i]: &gt; 10.3f})\\n\"\n                repr_str += \"\\n\"\n            for i, coeff in enumerate(estimates[n_alpha:]):\n                j = n_alpha + i\n                repr_str += (\n                    f\"   base {i + 1}: {true_coeffs[j]: &gt; 10.3f}  \"\n                    + f\"{coeff: &gt; 10.3f}  ({stderrs[j]: &gt; 10.3f})\\n\"\n                )\n            print_stars(repr_str)\n            discrepancy = npmaxabs(true_coeffs - estimates)\n            print_stars(\n                f\"The largest difference between true and estimated coefficients is {discrepancy: .2e}\"\n            )\n        else:\n            repr_str = (\n                \"The estimated coefficients \"\n                + \"(and their standard errors) are\\n\\n\"\n            )\n            for i, coeff in enumerate(estimates[:n_alpha]):\n                repr_str + f\"{coeff: &gt; 10.3f}  ({stderrs[i]: &gt; 10.3f})\\n\"\n                repr_str += \"\\n\"\n            for i, coeff in enumerate(estimates[n_alpha:]):\n                j = n_alpha + i\n                repr_str += f\"{coeff: &gt; 10.3f}  ({stderrs[j]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        repr_str = \"\\nSpecification test:\\n\"\n        repr_str += (\n            \"   the value of the test statistic is \"\n            + f\"{self.test_statistic: &gt; 10.3f}\\n\"\n        )\n        repr_str += (\n            f\"     for a chi2({self.ndf}), \"\n            + f\"the p-value is {self.test_pvalue: &gt; 10.3f}\\n\"\n        )\n        print_stars(repr_str)\n        if true_coeffs is not None:\n            return discrepancy\n        return None\n</code></pre>",
             "title": "<code>MDEResults</code>  <code>dataclass</code>"
         },
         {
             "location": "model_classes/",
             "text": "",
             "title": "<code>model_classes</code> module"
         },
@@ -367,15 +372,15 @@
         {
             "location": "poisson_glm_utils/",
             "text": "<p>Utilities for Poisson GLM.</p>",
             "title": "<code>poisson_glm_utils</code> module"
         },
         {
             "location": "poisson_glm_utils/#cupid_matching.poisson_glm_utils.PoissonGLMResults",
-            "text": "<p>Stores and formats the estimation results.</p> <p>Parameters:</p> Name Type Description Default <code>X</code> <code>int</code> <p>int</p> required <code>Y</code> <code>int</code> <p>int</p> required <code>K</code> <code>int</code> <p>int</p> required <code>number_households</code> <code>int</code> <p>int</p> required <code>number_individuals</code> <code>int</code> <p>int</p> required <code>estimated_gamma</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>varcov_gamma</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_gamma</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_beta</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_u</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_v</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>varcov_beta</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_beta</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_u</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_v</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_Phi</code> <code>np.ndarray</code> <p>np.ndarray</p> required Source code in <code>cupid_matching/poisson_glm_utils.py</code> <pre><code>@dataclass\nclass PoissonGLMResults:\n\"\"\"Stores and formats the estimation results.\n\n    Args:\n        X: int\n        Y: int\n        K: int\n        number_households: int\n        number_individuals: int\n        estimated_gamma: np.ndarray\n        varcov_gamma: np.ndarray\n        stderrs_gamma: np.ndarray\n        estimated_beta: np.ndarray\n        estimated_u: np.ndarray\n        estimated_v: np.ndarray\n        varcov_beta: np.ndarray\n        stderrs_beta: np.ndarray\n        stderrs_u: np.ndarray\n        stderrs_v: np.ndarray\n        estimated_Phi: np.ndarray\n    \"\"\"\n\n    X: int\n    Y: int\n    K: int\n    number_households: int\n    number_individuals: int\n    estimated_gamma: np.ndarray\n    varcov_gamma: np.ndarray\n    stderrs_gamma: np.ndarray\n    estimated_beta: np.ndarray\n    varcov_beta: np.ndarray\n    estimated_u: np.ndarray\n    estimated_v: np.ndarray\n    stderrs_beta: np.ndarray\n    stderrs_u: np.ndarray\n    stderrs_v: np.ndarray\n    estimated_Phi: np.ndarray\n\n    def __str__(self):\n        line_stars = \"*\" * 80 + \"\\n\"\n        print_stars(\"Estimating a Choo and Siow model by Poisson GLM.\")\n        model_str = f\"The data has {self.number_households} households\\n\\n\"\n        model_str += f\"We use {self.K} basis functions.\\n\\n\"\n        repr_str = line_stars + model_str\n        repr_str += \"The estimated basis coefficients (and their standard errors) are\\n\\n\"\n        for i in range(self.K):\n            repr_str += (\n                f\"   base_{i + 1}: {self.estimated_beta[i]: &gt; 10.3f}  \"\n                + f\"({self.stderrs_beta[i]: .3f})\\n\"\n            )\n        repr_str += (\n            \"The estimated utilities of men (and their standard errors) are\\n\\n\"\n        )\n        for i in range(self.X):\n            repr_str += (\n                f\"   u_{i + 1}: {self.estimated_u[i]: &gt; 10.3f}  \"\n                + f\"({self.stderrs_u[i]: .3f})\\n\"\n            )\n        repr_str += \"The estimated utilities of women (and their standard errors) are\\n\\n\"\n        for i in range(self.Y):\n            repr_str += (\n                f\"   v {i + 1}: {self.estimated_v[i]: &gt; 10.3f}  \"\n                + f\"({self.stderrs_v[i]: .3f})\\n\"\n            )\n        return repr_str + line_stars\n\n    def print_results(\n        self,\n        lambda_true: Optional[np.ndarray] = None,\n        u_true: Optional[np.ndarray] = None,\n        v_true: Optional[np.ndarray] = None,\n    ) -&gt; float | None:\n        estimates_beta = self.estimated_beta\n        stderrs_beta = self.stderrs_beta\n\n        if lambda_true is None:\n            repr_str = \"The  estimated coefficients \"\n            repr_str += \"(and their standard errors) are\\n\\n\"\n            for i, coeff in enumerate(estimates_beta):\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_beta[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n        else:\n            repr_str = \"The  true and estimated coefficients \"\n            repr_str += \"(and their standard errors) are\\n\\n\"\n            for i, coeff in enumerate(estimates_beta):\n                repr_str += f\"   base {i + 1}: {lambda_true[i]: &gt; 10.3f} \"\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_beta[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        estimates_u = self.estimated_u\n        stderrs_u = self.stderrs_u\n\n        if u_true is None:\n            repr_str = \"The estimated utilities for men  \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_u):\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_u[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n        else:\n            repr_str = \"The true and estimated utilities for men \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_u):\n                repr_str += f\"   u_{i + 1}: {u_true[i]: &gt; 10.3f} \"\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_u[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        estimates_v = self.estimated_v\n        stderrs_v = self.stderrs_v\n        if v_true is None:\n            repr_str = \"The estimated utilities for women \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_v):\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_v[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n        else:\n            repr_str = \"The true and estimated utilities for women \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_v):\n                repr_str += f\"   v_{i + 1}: {v_true[i]: &gt; 10.3f} \"\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_v[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        if lambda_true is None:\n            return None\n        else:\n            discrepancy = npmaxabs(lambda_true - estimates_beta)\n            print_stars(f\"The largest difference between true and estimated coefficients is {discrepancy: .2e}\")\n            return discrepancy\n</code></pre>",
+            "text": "<p>Stores and formats the estimation results.</p> <p>Parameters:</p> Name Type Description Default <code>X</code> <code>int</code> <p>int</p> required <code>Y</code> <code>int</code> <p>int</p> required <code>K</code> <code>int</code> <p>int</p> required <code>number_households</code> <code>int</code> <p>int</p> required <code>number_individuals</code> <code>int</code> <p>int</p> required <code>estimated_gamma</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>varcov_gamma</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_gamma</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_beta</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_u</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_v</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>varcov_beta</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_beta</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_u</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>stderrs_v</code> <code>np.ndarray</code> <p>np.ndarray</p> required <code>estimated_Phi</code> <code>np.ndarray</code> <p>np.ndarray</p> required Source code in <code>cupid_matching/poisson_glm_utils.py</code> <pre><code>@dataclass\nclass PoissonGLMResults:\n\"\"\"Stores and formats the estimation results.\n\n    Args:\n        X: int\n        Y: int\n        K: int\n        number_households: int\n        number_individuals: int\n        estimated_gamma: np.ndarray\n        varcov_gamma: np.ndarray\n        stderrs_gamma: np.ndarray\n        estimated_beta: np.ndarray\n        estimated_u: np.ndarray\n        estimated_v: np.ndarray\n        varcov_beta: np.ndarray\n        stderrs_beta: np.ndarray\n        stderrs_u: np.ndarray\n        stderrs_v: np.ndarray\n        estimated_Phi: np.ndarray\n    \"\"\"\n\n    X: int\n    Y: int\n    K: int\n    number_households: int\n    number_individuals: int\n    estimated_gamma: np.ndarray\n    varcov_gamma: np.ndarray\n    stderrs_gamma: np.ndarray\n    estimated_beta: np.ndarray\n    varcov_beta: np.ndarray\n    estimated_u: np.ndarray\n    estimated_v: np.ndarray\n    stderrs_beta: np.ndarray\n    stderrs_u: np.ndarray\n    stderrs_v: np.ndarray\n    estimated_Phi: np.ndarray\n\n    def __str__(self):\n        line_stars = \"*\" * 80 + \"\\n\"\n        print_stars(\"Estimating a Choo and Siow model by Poisson GLM.\")\n        model_str = f\"The data has {self.number_households} households\\n\\n\"\n        model_str += f\"We use {self.K} basis functions.\\n\\n\"\n        repr_str = line_stars + model_str\n        repr_str += \"The estimated basis coefficients (and their standard errors) are\\n\\n\"\n        for i in range(self.K):\n            repr_str += (\n                f\"   base_{i + 1}: {self.estimated_beta[i]: &gt; 10.3f}  \"\n                + f\"({self.stderrs_beta[i]: .3f})\\n\"\n            )\n        repr_str += (\n            \"The estimated utilities of men (and their standard errors) are\\n\\n\"\n        )\n        for i in range(self.X):\n            repr_str += (\n                f\"   u_{i + 1}: {self.estimated_u[i]: &gt; 10.3f}  \"\n                + f\"({self.stderrs_u[i]: .3f})\\n\"\n            )\n        repr_str += \"The estimated utilities of women (and their standard errors) are\\n\\n\"\n        for i in range(self.Y):\n            repr_str += (\n                f\"   v {i + 1}: {self.estimated_v[i]: &gt; 10.3f}  \"\n                + f\"({self.stderrs_v[i]: .3f})\\n\"\n            )\n        return repr_str + line_stars\n\n    def print_results(\n        self,\n        lambda_true: Optional[np.ndarray] = None,\n        u_true: Optional[np.ndarray] = None,\n        v_true: Optional[np.ndarray] = None,\n    ) -&gt; float | None:\n        estimates_beta = self.estimated_beta\n        stderrs_beta = self.stderrs_beta\n\n        if lambda_true is None:\n            repr_str = \"The  estimated coefficients \"\n            repr_str += \"(and their standard errors) are\\n\\n\"\n            for i, coeff in enumerate(estimates_beta):\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_beta[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n        else:\n            repr_str = \"The  true and estimated coefficients \"\n            repr_str += \"(and their standard errors) are\\n\\n\"\n            for i, coeff in enumerate(estimates_beta):\n                repr_str += f\"   base {i + 1}: {lambda_true[i]: &gt; 10.3f} \"\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_beta[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        estimates_u = self.estimated_u\n        stderrs_u = self.stderrs_u\n\n        if u_true is None:\n            repr_str = \"The estimated utilities for men  \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_u):\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_u[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n        else:\n            repr_str = \"The true and estimated utilities for men \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_u):\n                repr_str += f\"   u_{i + 1}: {u_true[i]: &gt; 10.3f} \"\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_u[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        estimates_v = self.estimated_v\n        stderrs_v = self.stderrs_v\n        if v_true is None:\n            repr_str = \"The estimated utilities for women \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_v):\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_v[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n        else:\n            repr_str = \"The true and estimated utilities for women \"\n            repr_str += \"(and their standard errors) are:\\n\\n\"\n            for i, coeff in enumerate(estimates_v):\n                repr_str += f\"   v_{i + 1}: {v_true[i]: &gt; 10.3f} \"\n                repr_str += f\" {coeff: &gt; 10.3f}  ({stderrs_v[i]: &gt; 10.3f})\\n\"\n            print_stars(repr_str)\n\n        if lambda_true is None:\n            return None\n        else:\n            discrepancy = npmaxabs(lambda_true - estimates_beta)\n            print_stars(\n                f\"The largest difference between true and estimated coefficients is {discrepancy: .2e}\"\n            )\n            return discrepancy\n</code></pre>",
             "title": "<code>PoissonGLMResults</code>  <code>dataclass</code>"
         },
         {
             "location": "utils/",
             "text": "<p>This module contains some utility programs used by the package.</p>",
             "title": "<code>utils</code> module"
         },
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/sitemap.xml` & `cupid_matching-1.0.5/cupid_matching/site/sitemap.xml`

 * *Files 2% similar despite different names*

#### Comparing `cupid_matching-1.0.4/cupid_matching/site/sitemap.xml` & `cupid_matching-1.0.5/cupid_matching/site/sitemap.xml`

```diff
@@ -1,88 +1,88 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/choo_siow/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/choo_siow_gender_heteroskedastic/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/choo_siow_heteroskedastic/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/cupid_streamlit/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/entropy/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/example_choosiow/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/example_nestedlogit/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/ipfp_solvers/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/matching_utils/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/min_distance/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/min_distance_utils/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/model_classes/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/nested_logit/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/poisson_glm/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/poisson_glm_utils/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://github.pages.io/bsalanie/cupid_matching/utils/</loc>
-    <lastmod>2023-04-02</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `cupid_matching-1.0.4/cupid_matching/site/utils/index.html` & `cupid_matching-1.0.5/cupid_matching/site/utils/index.html`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/cupid_matching/utils.py` & `cupid_matching-1.0.5/cupid_matching/utils.py`

 * *Files identical despite different names*

### Comparing `cupid_matching-1.0.4/pyproject.toml` & `cupid_matching-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cupid_matching"
-version = "1.0.4"
+version = "1.0.5"
 description = "Solves, simulates, and estimates separable matching TU models"
 authors = ["Bernard Salanie <bsalanie@columbia.edu>"]
 readme = "README.md"
 packages = [{include = "cupid_matching"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cupid_matching-1.0.4/PKG-INFO` & `cupid_matching-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupid-matching
-Version: 1.0.4
+Version: 1.0.5
 Summary: Solves, simulates, and estimates separable matching TU models
 Author: Bernard Salanie
 Author-email: bsalanie@columbia.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -58,8 +58,10 @@
 * as a consequence,  the `numeric` versions of the minimum distance estimator (which use numerical derivatives) are not recommended. 
 * the bias-corrected minimum distance estimator (`corrected`) may have a larger mean-squared error and/or introduce numerical instabilities.
 ## Release notes
 ### version 1.0.4
 * added an optional bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model, to help with cases when the matching patterns vary a lot across cells.
 * added two complete examples: [example_choosiow.py](example_choosiow.md) and [example_nestedlogit.py](example_nestedlogit.md).
 
+### version 1,0.5
+* simplified the bias-correction for the minimum distance estimator in the Choo and Siow homoskedastic model.
```

