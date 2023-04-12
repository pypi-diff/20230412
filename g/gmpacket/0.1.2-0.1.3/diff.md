# Comparing `tmp/gmpacket-0.1.2.tar.gz` & `tmp/gmpacket-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmpacket-0.1.2.tar", last modified: Tue Mar  7 19:34:44 2023, max compression
+gzip compressed data, was "gmpacket-0.1.3.tar", last modified: Wed Apr 12 17:47:41 2023, max compression
```

## Comparing `gmpacket-0.1.2.tar` & `gmpacket-0.1.3.tar`

### file list

```diff
@@ -1,177 +1,121 @@
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      167 2023-03-06 22:17:53.000000 gmpacket-0.1.2/.gitignore
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      761 2023-03-06 22:17:53.000000 gmpacket-0.1.2/DISCLAIMER.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      179 2023-03-06 22:17:53.000000 gmpacket-0.1.2/LICENSE.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2041 2023-03-07 19:34:44.321607 gmpacket-0.1.2/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1312 2023-03-06 22:17:53.000000 gmpacket-0.1.2/README.md
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/doc_source/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/doc_source/.bundle/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       33 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/.bundle/config
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       61 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/.gitignore
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      634 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/Makefile
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/doc_source/_static/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    53968 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/_static/GMP.png
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/doc_source/_static/css/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       65 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/_static/css/custom.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   476986 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/_static/demo-dark.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   452305 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/_static/demo-light.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   775827 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/_static/demo.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2110 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/_static/pied-piper-admonition.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      182 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/_static/readthedocs-dummy.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1455 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/cli.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3919 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/conf.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1628 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/demo.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      885 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/dev.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2374 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/examples.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1449 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/geojson.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2009 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/index.md
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)       98 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/makedocs.sh
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4736 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/pydantic_demo.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      174 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/requirements.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/doc_source/specification/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1323 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/base.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1970 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/event.md
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/doc_source/specification/features/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      128 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/features/index.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3727 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/features/metrics_dict.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1976 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/features/station.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5818 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/features/streams_traces.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      151 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/index.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4562 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/specification/provenance.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2096 2023-03-06 22:17:53.000000 gmpacket-0.1.2/doc_source/terms.md
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/docs/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      230 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/.buildinfo
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/.nojekyll
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/_sources/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1455 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/cli.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1628 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/demo.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      885 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/dev.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2374 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/examples.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1449 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/geojson.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2009 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/index.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4736 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/pydantic_demo.md.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/_sources/specification/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1323 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/base.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1970 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/event.md.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/_sources/specification/features/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      128 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/features/index.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3727 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/features/metrics_dict.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1976 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/features/station.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5818 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/features/streams_traces.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      151 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/index.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4562 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/specification/provenance.md.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2096 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_sources/terms.md.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/_static/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    53968 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/GMP.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4418 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    14810 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/basic.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      313 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/check-solid.svg
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     9031 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/clipboard.min.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      411 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/copy-button.svg
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2060 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/copybutton.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8472 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/copybutton.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2698 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/copybutton_funcs.js
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/_static/css/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       65 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/css/custom.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1266 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/debug.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   476986 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/demo-dark.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   452305 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/demo-light.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   775827 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/demo.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4472 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/doctools.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      444 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/documentation_options.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      286 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/file.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)   288580 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/jquery-3.6.0.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    89501 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/jquery.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4758 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/language_data.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       90 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/minus.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    39364 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2110 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/pied-piper-admonition.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       90 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/plus.png
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    21072 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/pygments.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      182 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/readthedocs-dummy.js
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/_static/scripts/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/scripts/furo-extensions.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5265 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/scripts/furo.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      187 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/scripts/furo.js.LICENSE.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    28242 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/scripts/furo.js.map
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    18215 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/searchtools.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6034 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/skeleton.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4712 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/sphinx_highlight.js
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/_static/styles/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5529 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/styles/furo-extensions.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     7809 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/styles/furo-extensions.css.map
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    48512 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/styles/furo.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    73326 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/styles/furo.css.map
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2589 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/tabs.css
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      551 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/tabs.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    68420 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/underscore-1.13.1.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    19530 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/_static/underscore.js
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    18056 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/cli.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    21354 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/demo.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    16760 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/dev.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    16922 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/examples.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13161 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/genindex.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    18838 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/geojson.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    15908 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/index.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      991 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/objects.inv
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    53740 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/pydantic_demo.html
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/reports/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2449 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/reports/demo.err.log
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    13389 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/search.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    16484 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/searchindex.js
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/specification/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    16823 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/base.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    18499 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/event.html
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/docs/specification/features/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    14706 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/features/index.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    23056 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/features/metrics_dict.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    19137 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/features/station.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    26841 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/features/streams_traces.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    15051 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/index.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    29832 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/specification/provenance.html
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    16729 2023-03-06 22:17:53.000000 gmpacket-0.1.2/docs/terms.html
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/gmpacket/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    15084 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/GMP-demo.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       42 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/README.md
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/__init__.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/gmpacket/bin/
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)      168 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/bin/gmpformat.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/gmpacket/data/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/gmpacket/data/examples/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    19404 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/data/examples/borehole_example.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    10956 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/data/examples/example1.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    14499 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/data/examples/multichannel_example.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    32064 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/data/examples/sps-100-200-example.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6059 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/feature.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1894 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/gmpformat.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6268 2023-03-06 22:45:40.000000 gmpacket-0.1.2/gmpacket/packet.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     5155 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/provenance.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     9164 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/scan.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      123 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/utils.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8719 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket/validate.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/gmpacket.egg-info/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     2041 2023-03-07 19:34:44.000000 gmpacket-0.1.2/gmpacket.egg-info/PKG-INFO
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4292 2023-03-07 19:34:44.000000 gmpacket-0.1.2/gmpacket.egg-info/SOURCES.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        1 2023-03-07 19:34:44.000000 gmpacket-0.1.2/gmpacket.egg-info/dependency_links.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       58 2023-03-07 19:34:44.000000 gmpacket-0.1.2/gmpacket.egg-info/entry_points.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      381 2023-03-07 19:34:44.000000 gmpacket-0.1.2/gmpacket.egg-info/requires.txt
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        9 2023-03-07 19:34:44.000000 gmpacket-0.1.2/gmpacket.egg-info/top_level.txt
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/gmpacket2/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)        0 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket2/__init__.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1055 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket2/feature.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3746 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket2/provenance.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      123 2023-03-06 22:17:53.000000 gmpacket-0.1.2/gmpacket2/utils.py
--rwxr-xr-x   0 mhearne   (1000) mhearne   (1000)     2604 2023-03-06 22:17:53.000000 gmpacket-0.1.2/install.sh
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/notebooks/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)    26271 2023-03-06 22:17:53.000000 gmpacket-0.1.2/notebooks/pydantic_demo.ipynb
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     1327 2023-03-07 19:28:02.000000 gmpacket-0.1.2/pyproject.toml
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)       38 2023-03-07 19:34:44.321607 gmpacket-0.1.2/setup.cfg
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      603 2023-03-06 22:17:53.000000 gmpacket-0.1.2/setup.py
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.311607 gmpacket-0.1.2/tests/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/tests/gmpacket/
-drwxr-xr-x   0 mhearne   (1000) mhearne   (1000)        0 2023-03-07 19:34:44.321607 gmpacket-0.1.2/tests/gmpacket/data/
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     6752 2023-03-06 22:17:53.000000 gmpacket-0.1.2/tests/gmpacket/data/full_packet.json
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     3603 2023-03-06 22:17:53.000000 gmpacket-0.1.2/tests/gmpacket/test_feature.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     8027 2023-03-07 19:26:37.000000 gmpacket-0.1.2/tests/gmpacket/test_packet.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)     4480 2023-03-06 22:17:53.000000 gmpacket-0.1.2/tests/gmpacket/test_provenance.py
--rw-r--r--   0 mhearne   (1000) mhearne   (1000)      225 2023-03-06 22:17:53.000000 gmpacket-0.1.2/tests/gmpacket/test_utils.py
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.960767 gmpacket-0.1.3/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      155 2023-04-12 17:41:09.000000 gmpacket-0.1.3/.gitignore
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      761 2023-04-10 20:24:32.000000 gmpacket-0.1.3/DISCLAIMER.md
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      179 2023-04-10 20:24:32.000000 gmpacket-0.1.3/LICENSE.md
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       63 2023-04-12 17:23:01.000000 gmpacket-0.1.3/MANIFEST.in
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2083 2023-04-12 17:47:41.959819 gmpacket-0.1.3/PKG-INFO
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1312 2023-04-10 20:24:32.000000 gmpacket-0.1.3/README.md
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.474021 gmpacket-0.1.3/docs/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      230 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/.buildinfo
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-11 20:38:42.000000 gmpacket-0.1.3/docs/.nojekyll
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.494982 gmpacket-0.1.3/docs/_sources/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      892 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/dev.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2377 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/examples.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1449 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_sources/geojson.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1229 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/getting_started.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2014 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/index.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4864 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/pydantic_demo.md.txt
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.543528 gmpacket-0.1.3/docs/_sources/specification/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1322 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/base.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1969 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/event.md.txt
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.556911 gmpacket-0.1.3/docs/_sources/specification/features/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      123 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/index.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     3722 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/metrics_dict.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1975 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/station.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5817 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/features/streams_traces.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      150 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/index.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4561 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_sources/specification/provenance.md.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2096 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_sources/terms.md.txt
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.792101 gmpacket-0.1.3/docs/_static/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    53968 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/GMP.png
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4418 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14810 2023-04-11 20:38:41.000000 gmpacket-0.1.3/docs/_static/basic.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      313 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/check-solid.svg
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     9031 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/clipboard.min.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      411 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/copy-button.svg
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2060 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/copybutton.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     8472 2023-04-11 20:38:41.000000 gmpacket-0.1.3/docs/_static/copybutton.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2698 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/copybutton_funcs.js
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.794758 gmpacket-0.1.3/docs/_static/css/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       65 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/css/custom.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1266 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/debug.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   476986 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/demo-dark.png
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   452305 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/demo-light.png
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   775827 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/demo.png
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4472 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/doctools.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      444 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/documentation_options.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      286 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/file.png
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)   288580 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/jquery-3.6.0.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    89501 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/jquery.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4758 2023-04-11 20:38:41.000000 gmpacket-0.1.3/docs/_static/language_data.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       90 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/minus.png
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    39364 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2110 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/pied-piper-admonition.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       90 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/plus.png
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    21072 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/pygments.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      182 2023-04-10 20:24:32.000000 gmpacket-0.1.3/docs/_static/readthedocs-dummy.js
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.816776 gmpacket-0.1.3/docs/_static/scripts/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo-extensions.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5265 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      187 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo.js.LICENSE.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    28242 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/scripts/furo.js.map
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18215 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/searchtools.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     6034 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/skeleton.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     4712 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/sphinx_highlight.js
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.847359 gmpacket-0.1.3/docs/_static/styles/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5529 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/styles/furo-extensions.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     7809 2023-04-11 19:40:39.000000 gmpacket-0.1.3/docs/_static/styles/furo-extensions.css.map
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    48697 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/styles/furo.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    73615 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/_static/styles/furo.css.map
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2589 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/tabs.css
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      551 2023-04-11 19:40:37.000000 gmpacket-0.1.3/docs/_static/tabs.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    68420 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/underscore-1.13.1.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    19530 2023-04-11 19:40:31.000000 gmpacket-0.1.3/docs/_static/underscore.js
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16698 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/dev.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16877 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/examples.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    13090 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/genindex.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18777 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/geojson.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18471 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/getting_started.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    15851 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/index.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      963 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/objects.inv
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    53563 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/pydantic_demo.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    13318 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/search.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    15652 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/searchindex.js
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.878280 gmpacket-0.1.3/docs/specification/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16749 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/specification/base.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    18425 2023-04-11 21:09:33.000000 gmpacket-0.1.3/docs/specification/event.html
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.904471 gmpacket-0.1.3/docs/specification/features/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14629 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/index.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    22987 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/metrics_dict.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    19060 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/station.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    26764 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/features/streams_traces.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14977 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/index.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    29758 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/specification/provenance.html
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    16658 2023-04-11 21:09:34.000000 gmpacket-0.1.3/docs/terms.html
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.915513 gmpacket-0.1.3/gmpacket/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       42 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/README.md
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/__init__.py
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.236879 gmpacket-0.1.3/gmpacket/data/
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.954565 gmpacket-0.1.3/gmpacket/data/examples/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    19404 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/borehole_example.json
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    10956 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/example1.json
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    14499 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/multichannel_example.json
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    32064 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/data/examples/sps-100-200-example.json
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     6059 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/feature.py
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     6268 2023-04-11 15:22:05.000000 gmpacket-0.1.3/gmpacket/packet.py
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     5155 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/provenance.py
+-rwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)     9164 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/scan.py
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      123 2023-04-10 20:24:32.000000 gmpacket-0.1.3/gmpacket/utils.py
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     8719 2023-04-11 15:21:44.000000 gmpacket-0.1.3/gmpacket/validate.py
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.920894 gmpacket-0.1.3/gmpacket.egg-info/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     2083 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/PKG-INFO
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     3030 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/SOURCES.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        1 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/dependency_links.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      383 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/requires.txt
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)        9 2023-04-12 17:47:41.000000 gmpacket-0.1.3/gmpacket.egg-info/top_level.txt
+-rwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)     2604 2023-04-10 20:24:32.000000 gmpacket-0.1.3/install.sh
+drwxr-xr-x   0 gferragut (1707185330) GS\Domain Users (346589396)        0 2023-04-12 17:47:41.958476 gmpacket-0.1.3/notebooks/
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)    26271 2023-04-10 20:24:32.000000 gmpacket-0.1.3/notebooks/pydantic_demo.ipynb
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)     1256 2023-04-12 17:28:33.000000 gmpacket-0.1.3/pyproject.toml
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)       38 2023-04-12 17:47:41.960991 gmpacket-0.1.3/setup.cfg
+-rw-r--r--   0 gferragut (1707185330) GS\Domain Users (346589396)      483 2023-04-12 17:20:26.000000 gmpacket-0.1.3/setup.py
```

### Comparing `gmpacket-0.1.2/DISCLAIMER.md` & `gmpacket-0.1.3/DISCLAIMER.md`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/PKG-INFO` & `gmpacket-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmpacket
-Version: 0.1.2
+Version: 0.1.3
 Summary: ANSS Ground Motion Packet
 Home-page: https://github.com/SCEDC/ground-motion-packet
 Author: Ellen Yu, Lijam Hagos, Jamie Steidl, Eric Thompson, Bruce Worden
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>, Ellen Yu <eyu@caltech.edu>
 License: License
         =======
         
@@ -13,14 +13,16 @@
         http://unlicense.org/
         
 Keywords: ground motion,earthquake
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: build
 License-File: LICENSE.md
 
 # Description of GMP —A GeoJSON Specification for Ground Motion Metrics
 
 Here we present a specification for a GeoJSON (https://geojson.org/) format for 
 unassociated and event-associated ground motion metrics—that is, quantities 
 derived from ground motion records (e.g., accelerograms, velocity recordings).
```

### Comparing `gmpacket-0.1.2/README.md` & `gmpacket-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/doc_source/_static/GMP.png` & `gmpacket-0.1.3/docs/_static/GMP.png`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/doc_source/_static/demo-dark.png` & `gmpacket-0.1.3/docs/_static/demo-dark.png`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/doc_source/_static/demo-light.png` & `gmpacket-0.1.3/docs/_static/demo-light.png`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/doc_source/_static/demo.png` & `gmpacket-0.1.3/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/doc_source/_static/pied-piper-admonition.css` & `gmpacket-0.1.3/docs/_static/pied-piper-admonition.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/doc_source/dev.md` & `gmpacket-0.1.3/docs/_sources/dev.md.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-## Developer Notes
+# Developer Notes
 
 We welcome comments and contributions through github issues.
 
-### Documentation
+## Documentation
 
 Never edit the contents of the `docs` directory, only edit files in the `doc_source`
 directory.
 
 To build this documentation, it is convenient to create a conda virtual environment
 with [mamba](https://github.com/mamba-org/mamba) (note that mamba can be installed 
 with [conda](https://docs.conda.io/en/latest/)).
@@ -14,15 +14,15 @@
 ```
 cd doc_source
 mamba create -n gmpdocs python=3.9 --file requirements.txt
 conda activate gmpdocs
 ```
 
 Then install the python packages as described  in the 
-[Command Line Tools](cli) section. For the demo, we'll also need
+[Getting Started](getting_started) section. For the demo, we'll also need
 
 ```
 pip install ipyleaflet
 jupyter nbextension enable --py widgetsnbextension
 ```
 
 ```
```

### Comparing `gmpacket-0.1.2/doc_source/examples.md` & `gmpacket-0.1.3/docs/_sources/examples.md.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Examples
+# GMP Examples
 
 Examples **with fake data** can be found in this repository 
 [here](https://github.com/SCEDC/ground-motion-packet/tree/main/gmpacket/data/examples).
 These examples are selected to illustrate a number of different possible
 instrument configurations and to highlight the value of sensible grouping
 of traces into streams.
```

### Comparing `gmpacket-0.1.2/doc_source/geojson.md` & `gmpacket-0.1.3/docs/_sources/geojson.md.txt`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/doc_source/index.md` & `gmpacket-0.1.3/docs/_sources/index.md.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 hide-toc: true
 ---
 
-## Earthquake Ground Motion Data Packet 
+# Earthquake Ground Motion Data Packet 
 
 Here we present a specification for a [GeoJSON](https://geojson.org/) format 
 for unassociated and event-associated ground motion metrics—that is, quantities
 derived from ground motion records (e.g., accelerograms, velocity recordings).
 We refer to this specification as a Ground Motion Packet (GMP). Common example
 metrics include peak ground acceleration (PGA), peak ground velocity (PGV), and
 spectral acceleration (SA). This format is designed so that it can also include
@@ -34,17 +34,15 @@
 not stored in the format presented here. 
 ```
 
 
 
 ```{toctree}
 :hidden:
-
+getting_started
 geojson
 terms
 specification/index
 examples
-cli
-demo
 pydantic_demo
 dev
 ```
```

### Comparing `gmpacket-0.1.2/doc_source/pydantic_demo.md` & `gmpacket-0.1.3/docs/_sources/pydantic_demo.md.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 kernelspec:
   display_name: Python 3
   language: python
   name: python3
 ---
 # Pydantic Demo
 
+Before starting, ensure you have installed the python packages as described in the [Getting Started](getting_started) section.
+
 We will start with the necessary imports 
 
 ```{code-cell} ipython3
 from datetime import datetime, timedelta
 from gmpacket.provenance import SoftwareAgent, PersonAgent, OrganizationAgent, Website, Provenance
 from gmpacket.feature import (
     Feature,
```

### Comparing `gmpacket-0.1.2/doc_source/specification/base.md` & `gmpacket-0.1.3/docs/_sources/specification/base.md.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Base Dictionary
+# Base Dictionary
 
 For the base GeoJSON dictionary, the GMP specification adds four additional
 keys:
 
 **version**
 :  The version of the ground motion packet *(string; required)*.
```

### Comparing `gmpacket-0.1.2/doc_source/specification/event.md` & `gmpacket-0.1.3/docs/_sources/specification/event.md.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Event
+# Event
 
 The event dictionary contains the following keys. Note that the event parameters listed
 here can become outdated as new information becomes available. For anyone using these
 data we strongly encourage you to retrieve updated event information from the USGS
 [Comcat](https://earthquake.usgs.gov/earthquakes/search/) database 
 ([Comcat API documentation](https://earthquake.usgs.gov/fdsnws/event/1/)).
```

### Comparing `gmpacket-0.1.2/doc_source/specification/features/metrics_dict.md` & `gmpacket-0.1.3/docs/_sources/specification/features/metrics_dict.md.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-## Metrics Dictionary
+# Metrics Dictionary
 
 The "metrics" dictionary contains the values and metadata relevant for the 
 metrics associated with the parent trace. One challenge with ground motion
 metric data is that different metrics exhibit very different structure. For
 example, some metrics are simply scalars (e.g., PGA) while others are arrays
 (e.g., response spectra, which are a function of both oscillator period and
 the assumed percent of critical damping).
 
 While it is possible to list each metric as a separate element in a list, there
 are two main drawbacks to doing so:
-  1. It is inefficient from a file size perspective, and 
+
+  1. It is inefficient from a file size perspective, and
   2. It is difficult to parse because the properties will be different for each
      metric.
 
 Thus, we have designed a general metrics data structure with the goals of
 being easy to extend to a wide range of metric data structures, consistency in
-how the metrics are stored to make parsing the data more straight-forward, and 
-minimizing the file size. 
+how the metrics are stored to make parsing the data more straight-forward, and minimizing the file size.
 
 The dictionary has the following required keys:
 
 **properties**
 :  A dictionary with the following keys *(dictionary; required)*:
 
    **description**
@@ -109,9 +109,7 @@
                   ]
               }
           ]
       }
   ]
 
 ```
-
-
```

### Comparing `gmpacket-0.1.2/doc_source/specification/features/station.md` & `gmpacket-0.1.3/docs/_sources/specification/features/station.md.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Stations
+# Stations
 
 The GeoJSON features represent seismic stations in the GMP specification. 
 Station metadata is included in the GeoJSON feature "properties" dictionary. 
 Requited properties include:
 
 **type**
 :  Must be "Feature" *(string; required)*.
```

### Comparing `gmpacket-0.1.2/doc_source/specification/features/streams_traces.md` & `gmpacket-0.1.3/docs/_sources/specification/features/streams_traces.md.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Streams and Traces
+# Streams and Traces
 
 For the purposes of the GMP format, we require that the traces be grouped into
 streams for which their corresponding properties (i.e., metadata) are consistent.
 Since a station may include traces from different locations or with different sample
 rates, a single station feature may contain multiple streams. The GMP format requires
 a "streams" key for each station dictionary. The streams key gives a list of
 dictionaries, and each dictionary represents a unique stream at that station.
```

### Comparing `gmpacket-0.1.2/doc_source/specification/provenance.md` & `gmpacket-0.1.3/docs/_sources/specification/provenance.md.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Provenance 
+# Provenance 
 
 The provenance document is meant to inform the user about the provider, source, 
 distributor, and processing of the data in this file. The provenance should 
 meet the requirements of 
 [SEIS-PROV](http://seismicdata.github.io/SEIS-PROV/index.html).
 
 ```{code-block} json
```

### Comparing `gmpacket-0.1.2/doc_source/terms.md` & `gmpacket-0.1.3/docs/_sources/terms.md.txt`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/_sphinx_javascript_frameworks_compat.js` & `gmpacket-0.1.3/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/basic.css` & `gmpacket-0.1.3/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/clipboard.min.js` & `gmpacket-0.1.3/docs/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/copybutton.css` & `gmpacket-0.1.3/docs/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/copybutton.js` & `gmpacket-0.1.3/docs/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/copybutton_funcs.js` & `gmpacket-0.1.3/docs/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/debug.css` & `gmpacket-0.1.3/docs/_static/debug.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/doctools.js` & `gmpacket-0.1.3/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/jquery-3.6.0.js` & `gmpacket-0.1.3/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/jquery.js` & `gmpacket-0.1.3/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/language_data.js` & `gmpacket-0.1.3/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css` & `gmpacket-0.1.3/docs/_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/pygments.css` & `gmpacket-0.1.3/docs/_static/pygments.css`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 body[data-theme="dark"] .highlight .l { color: #d0d0d0 } /* Literal */
 body[data-theme="dark"] .highlight .n { color: #d0d0d0 } /* Name */
 body[data-theme="dark"] .highlight .o { color: #d0d0d0 } /* Operator */
 body[data-theme="dark"] .highlight .x { color: #d0d0d0 } /* Other */
 body[data-theme="dark"] .highlight .p { color: #d0d0d0 } /* Punctuation */
 body[data-theme="dark"] .highlight .ch { color: #ababab; font-style: italic } /* Comment.Hashbang */
 body[data-theme="dark"] .highlight .cm { color: #ababab; font-style: italic } /* Comment.Multiline */
-body[data-theme="dark"] .highlight .cp { color: #cd2828; font-weight: bold } /* Comment.Preproc */
+body[data-theme="dark"] .highlight .cp { color: #ff3a3a; font-weight: bold } /* Comment.Preproc */
 body[data-theme="dark"] .highlight .cpf { color: #ababab; font-style: italic } /* Comment.PreprocFile */
 body[data-theme="dark"] .highlight .c1 { color: #ababab; font-style: italic } /* Comment.Single */
 body[data-theme="dark"] .highlight .cs { color: #e50808; font-weight: bold; background-color: #520000 } /* Comment.Special */
 body[data-theme="dark"] .highlight .gd { color: #d22323 } /* Generic.Deleted */
 body[data-theme="dark"] .highlight .ge { color: #d0d0d0; font-style: italic } /* Generic.Emph */
 body[data-theme="dark"] .highlight .gr { color: #d22323 } /* Generic.Error */
 body[data-theme="dark"] .highlight .gh { color: #ffffff; font-weight: bold } /* Generic.Heading */
@@ -182,15 +182,15 @@
 body:not([data-theme="light"]) .highlight .l { color: #d0d0d0 } /* Literal */
 body:not([data-theme="light"]) .highlight .n { color: #d0d0d0 } /* Name */
 body:not([data-theme="light"]) .highlight .o { color: #d0d0d0 } /* Operator */
 body:not([data-theme="light"]) .highlight .x { color: #d0d0d0 } /* Other */
 body:not([data-theme="light"]) .highlight .p { color: #d0d0d0 } /* Punctuation */
 body:not([data-theme="light"]) .highlight .ch { color: #ababab; font-style: italic } /* Comment.Hashbang */
 body:not([data-theme="light"]) .highlight .cm { color: #ababab; font-style: italic } /* Comment.Multiline */
-body:not([data-theme="light"]) .highlight .cp { color: #cd2828; font-weight: bold } /* Comment.Preproc */
+body:not([data-theme="light"]) .highlight .cp { color: #ff3a3a; font-weight: bold } /* Comment.Preproc */
 body:not([data-theme="light"]) .highlight .cpf { color: #ababab; font-style: italic } /* Comment.PreprocFile */
 body:not([data-theme="light"]) .highlight .c1 { color: #ababab; font-style: italic } /* Comment.Single */
 body:not([data-theme="light"]) .highlight .cs { color: #e50808; font-weight: bold; background-color: #520000 } /* Comment.Special */
 body:not([data-theme="light"]) .highlight .gd { color: #d22323 } /* Generic.Deleted */
 body:not([data-theme="light"]) .highlight .ge { color: #d0d0d0; font-style: italic } /* Generic.Emph */
 body:not([data-theme="light"]) .highlight .gr { color: #d22323 } /* Generic.Error */
 body:not([data-theme="light"]) .highlight .gh { color: #ffffff; font-weight: bold } /* Generic.Heading */
```

### Comparing `gmpacket-0.1.2/docs/_static/scripts/furo.js` & `gmpacket-0.1.3/docs/_static/scripts/furo.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/scripts/furo.js.map` & `gmpacket-0.1.3/docs/_static/scripts/furo.js.map`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/searchtools.js` & `gmpacket-0.1.3/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/skeleton.css` & `gmpacket-0.1.3/docs/_static/skeleton.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/sphinx_highlight.js` & `gmpacket-0.1.3/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/styles/furo-extensions.css` & `gmpacket-0.1.3/docs/_static/styles/furo-extensions.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/styles/furo-extensions.css.map` & `gmpacket-0.1.3/docs/_static/styles/furo-extensions.css.map`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/styles/furo.css` & `gmpacket-0.1.3/docs/_static/styles/furo.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */html{-webkit-text-size-adjust:100%;line-height:1.15}body{margin:0}main{display:block}h1{font-size:2em;margin:.67em 0}hr{box-sizing:content-box;height:0;overflow:visible}pre{font-family:monospace,monospace;font-size:1em}a{background-color:transparent}abbr[title]{border-bottom:none;text-decoration:underline;text-decoration:underline dotted}b,strong{font-weight:bolder}code,kbd,samp{font-family:monospace,monospace;font-size:1em}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}img{border-style:none}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;line-height:1.15;margin:0}button,input{overflow:visible}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner,button::-moz-focus-inner{border-style:none;padding:0}[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring,button:-moz-focusring{outline:1px dotted ButtonText}fieldset{padding:.35em .75em .625em}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal}progress{vertical-align:baseline}textarea{overflow:auto}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}[type=search]::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}details{display:block}summary{display:list-item}[hidden],template{display:none}@media print{.content-icon-container,.headerlink,.mobile-header,.related-pages{display:none!important}.highlight{border:.1pt solid var(--color-foreground-border)}a,blockquote,dl,ol,pre,table,ul{page-break-inside:avoid}caption,figure,h1,h2,h3,h4,h5,h6,img{page-break-after:avoid;page-break-inside:avoid}dl,ol,ul{page-break-before:avoid}}.visually-hidden{clip:rect(0,0,0,0)!important;border:0!important;height:1px!important;margin:-1px!important;overflow:hidden!important;padding:0!important;position:absolute!important;white-space:nowrap!important;width:1px!important}:-moz-focusring{outline:auto}body{--font-stack:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;--font-stack--monospace:"SFMono-Regular",Menlo,Consolas,Monaco,Liberation Mono,Lucida Console,monospace;--font-size--normal:100%;--font-size--small:87.5%;--font-size--small--2:81.25%;--font-size--small--3:75%;--font-size--small--4:62.5%;--sidebar-caption-font-size:var(--font-size--small--2);--sidebar-item-font-size:var(--font-size--small);--sidebar-search-input-font-size:var(--font-size--small);--toc-font-size:var(--font-size--small--3);--toc-font-size--mobile:var(--font-size--normal);--toc-title-font-size:var(--font-size--small--4);--admonition-font-size:0.8125rem;--admonition-title-font-size:0.8125rem;--code-font-size:var(--font-size--small--2);--api-font-size:var(--font-size--small);--header-height:calc(var(--sidebar-item-line-height) + var(--sidebar-item-spacing-vertical)*4);--header-padding:0.5rem;--sidebar-tree-space-above:1.5rem;--sidebar-caption-space-above:1rem;--sidebar-item-line-height:1rem;--sidebar-item-spacing-vertical:0.5rem;--sidebar-item-spacing-horizontal:1rem;--sidebar-item-height:calc(var(--sidebar-item-line-height) + var(--sidebar-item-spacing-vertical)*2);--sidebar-expander-width:var(--sidebar-item-height);--sidebar-search-space-above:0.5rem;--sidebar-search-input-spacing-vertical:0.5rem;--sidebar-search-input-spacing-horizontal:0.5rem;--sidebar-search-input-height:1rem;--sidebar-search-icon-size:var(--sidebar-search-input-height);--toc-title-padding:0.25rem 0;--toc-spacing-vertical:1.5rem;--toc-spacing-horizontal:1.5rem;--toc-item-spacing-vertical:0.4rem;--toc-item-spacing-horizontal:1rem;--icon-search:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M0 0h24v24H0z" stroke="none"/><circle cx="10" cy="10" r="7"/><path d="m21 21-6-6"/></svg>');--icon-pencil:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20.71 7.04c.39-.39.39-1.04 0-1.41l-2.34-2.34c-.37-.39-1.02-.39-1.41 0l-1.84 1.83 3.75 3.75M3 17.25V21h3.75L17.81 9.93l-3.75-3.75L3 17.25z"/></svg>');--icon-abstract:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 5h16v2H4V5m0 4h16v2H4V9m0 4h16v2H4v-2m0 4h10v2H4v-2z"/></svg>');--icon-info:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 9h-2V7h2m0 10h-2v-6h2m-1-9A10 10 0 0 0 2 12a10 10 0 0 0 10 10 10 10 0 0 0 10-10A10 10 0 0 0 12 2z"/></svg>');--icon-flame:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17.55 11.2c-.23-.3-.5-.56-.76-.82-.65-.6-1.4-1.03-2.03-1.66C13.3 7.26 13 4.85 13.91 3c-.91.23-1.75.75-2.45 1.32-2.54 2.08-3.54 5.75-2.34 8.9.04.1.08.2.08.33 0 .22-.15.42-.35.5-.22.1-.46.04-.64-.12a.83.83 0 0 1-.15-.17c-1.1-1.43-1.28-3.48-.53-5.12C5.89 10 5 12.3 5.14 14.47c.04.5.1 1 .27 1.5.14.6.4 1.2.72 1.73 1.04 1.73 2.87 2.97 4.84 3.22 2.1.27 4.35-.12 5.96-1.6 1.8-1.66 2.45-4.32 1.5-6.6l-.13-.26c-.2-.46-.47-.87-.8-1.25l.05-.01m-3.1 6.3c-.28.24-.73.5-1.08.6-1.1.4-2.2-.16-2.87-.82 1.19-.28 1.89-1.16 2.09-2.05.17-.8-.14-1.46-.27-2.23-.12-.74-.1-1.37.18-2.06.17.38.37.76.6 1.06.76 1 1.95 1.44 2.2 2.8.04.14.06.28.06.43.03.82-.32 1.72-.92 2.27h.01z"/></svg>');--icon-question:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="m15.07 11.25-.9.92C13.45 12.89 13 13.5 13 15h-2v-.5c0-1.11.45-2.11 1.17-2.83l1.24-1.26c.37-.36.59-.86.59-1.41a2 2 0 0 0-2-2 2 2 0 0 0-2 2H8a4 4 0 0 1 4-4 4 4 0 0 1 4 4 3.2 3.2 0 0 1-.93 2.25M13 19h-2v-2h2M12 2A10 10 0 0 0 2 12a10 10 0 0 0 10 10 10 10 0 0 0 10-10c0-5.53-4.5-10-10-10z"/></svg>');--icon-warning:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 14h-2v-4h2m0 8h-2v-2h2M1 21h22L12 2 1 21z"/></svg>');--icon-failure:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 2c5.53 0 10 4.47 10 10s-4.47 10-10 10S2 17.53 2 12 6.47 2 12 2m3.59 5L12 10.59 8.41 7 7 8.41 10.59 12 7 15.59 8.41 17 12 13.41 15.59 17 17 15.59 13.41 12 17 8.41 15.59 7z"/></svg>');--icon-spark:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="m11.5 20 4.86-9.73H13V4l-5 9.73h3.5V20M12 2c2.75 0 5.1 1 7.05 2.95C21 6.9 22 9.25 22 12s-1 5.1-2.95 7.05C17.1 21 14.75 22 12 22s-5.1-1-7.05-2.95C3 17.1 2 14.75 2 12s1-5.1 2.95-7.05C6.9 3 9.25 2 12 2z"/></svg>');--color-admonition-title--caution:#ff9100;--color-admonition-title-background--caution:rgba(255,145,0,.1);--color-admonition-title--warning:#ff9100;--color-admonition-title-background--warning:rgba(255,145,0,.1);--color-admonition-title--danger:#ff5252;--color-admonition-title-background--danger:rgba(255,82,82,.1);--color-admonition-title--attention:#ff5252;--color-admonition-title-background--attention:rgba(255,82,82,.1);--color-admonition-title--error:#ff5252;--color-admonition-title-background--error:rgba(255,82,82,.1);--color-admonition-title--hint:#00c852;--color-admonition-title-background--hint:rgba(0,200,82,.1);--color-admonition-title--tip:#00c852;--color-admonition-title-background--tip:rgba(0,200,82,.1);--color-admonition-title--important:#00bfa5;--color-admonition-title-background--important:rgba(0,191,165,.1);--color-admonition-title--note:#00b0ff;--color-admonition-title-background--note:rgba(0,176,255,.1);--color-admonition-title--seealso:#448aff;--color-admonition-title-background--seealso:rgba(68,138,255,.1);--color-admonition-title--admonition-todo:grey;--color-admonition-title-background--admonition-todo:hsla(0,0%,50%,.1);--color-admonition-title:#651fff;--color-admonition-title-background:rgba(101,31,255,.1);--icon-admonition-default:var(--icon-abstract);--color-topic-title:#14b8a6;--color-topic-title-background:rgba(20,184,166,.1);--icon-topic-default:var(--icon-pencil);--color-problematic:#b30000;--color-foreground-primary:#000;--color-foreground-secondary:#5a5c63;--color-foreground-muted:#646776;--color-foreground-border:#878787;--color-background-primary:#fff;--color-background-secondary:#f8f9fb;--color-background-hover:#efeff4;--color-background-hover--transparent:#efeff400;--color-background-border:#eeebee;--color-background-item:#ccc;--color-announcement-background:#000000dd;--color-announcement-text:#eeebee;--color-brand-primary:#2962ff;--color-brand-content:#2a5adf;--color-api-background:var(--color-background-secondary);--color-api-background-hover:var(--color-background-hover);--color-api-overall:var(--color-foreground-secondary);--color-api-name:var(--color-problematic);--color-api-pre-name:var(--color-problematic);--color-api-paren:var(--color-foreground-secondary);--color-api-keyword:var(--color-foreground-primary);--color-highlight-on-target:#ffc;--color-inline-code-background:var(--color-background-secondary);--color-highlighted-background:#def;--color-highlighted-text:var(--color-foreground-primary);--color-guilabel-background:#ddeeff80;--color-guilabel-border:#bedaf580;--color-guilabel-text:var(--color-foreground-primary);--color-admonition-background:transparent;--color-table-header-background:var(--color-background-secondary);--color-table-border:var(--color-background-border);--color-card-border:var(--color-background-secondary);--color-card-background:transparent;--color-card-marginals-background:var(--color-background-secondary);--color-header-background:var(--color-background-primary);--color-header-border:var(--color-background-border);--color-header-text:var(--color-foreground-primary);--color-sidebar-background:var(--color-background-secondary);--color-sidebar-background-border:var(--color-background-border);--color-sidebar-brand-text:var(--color-foreground-primary);--color-sidebar-caption-text:var(--color-foreground-muted);--color-sidebar-link-text:var(--color-foreground-secondary);--color-sidebar-link-text--top-level:var(--color-brand-primary);--color-sidebar-item-background:var(--color-sidebar-background);--color-sidebar-item-background--current:var( --color-sidebar-item-background );--color-sidebar-item-background--hover:linear-gradient(90deg,var(--color-background-hover--transparent) 0%,var(--color-background-hover) var(--sidebar-item-spacing-horizontal),var(--color-background-hover) 100%);--color-sidebar-item-expander-background:transparent;--color-sidebar-item-expander-background--hover:var( --color-background-hover );--color-sidebar-search-text:var(--color-foreground-primary);--color-sidebar-search-background:var(--color-background-secondary);--color-sidebar-search-background--focus:var(--color-background-primary);--color-sidebar-search-border:var(--color-background-border);--color-sidebar-search-icon:var(--color-foreground-muted);--color-toc-background:var(--color-background-primary);--color-toc-title-text:var(--color-foreground-muted);--color-toc-item-text:var(--color-foreground-secondary);--color-toc-item-text--hover:var(--color-foreground-primary);--color-toc-item-text--active:var(--color-brand-primary);--color-content-foreground:var(--color-foreground-primary);--color-content-background:transparent;--color-link:var(--color-brand-content);--color-link--hover:var(--color-brand-content);--color-link-underline:var(--color-background-border);--color-link-underline--hover:var(--color-foreground-border)}.only-light{display:block!important}html body .only-dark{display:none!important}@media not print{body[data-theme=dark]{--color-problematic:#ee5151;--color-foreground-primary:#ffffffcc;--color-foreground-secondary:#9ca0a5;--color-foreground-muted:#81868d;--color-foreground-border:#666;--color-background-primary:#131416;--color-background-secondary:#1a1c1e;--color-background-hover:#1e2124;--color-background-hover--transparent:#1e212400;--color-background-border:#303335;--color-background-item:#444;--color-announcement-background:#000000dd;--color-announcement-text:#eeebee;--color-brand-primary:#2b8cee;--color-brand-content:#368ce2;--color-highlighted-background:#083563;--color-guilabel-background:#08356380;--color-guilabel-border:#13395f80;--color-api-keyword:var(--color-foreground-secondary);--color-highlight-on-target:#330;--color-admonition-background:#18181a;--color-card-border:var(--color-background-secondary);--color-card-background:#18181a;--color-card-marginals-background:var(--color-background-hover)}html body[data-theme=dark] .only-light{display:none!important}body[data-theme=dark] .only-dark{display:block!important}@media(prefers-color-scheme:dark){body:not([data-theme=light]){--color-problematic:#ee5151;--color-foreground-primary:#ffffffcc;--color-foreground-secondary:#9ca0a5;--color-foreground-muted:#81868d;--color-foreground-border:#666;--color-background-primary:#131416;--color-background-secondary:#1a1c1e;--color-background-hover:#1e2124;--color-background-hover--transparent:#1e212400;--color-background-border:#303335;--color-background-item:#444;--color-announcement-background:#000000dd;--color-announcement-text:#eeebee;--color-brand-primary:#2b8cee;--color-brand-content:#368ce2;--color-highlighted-background:#083563;--color-guilabel-background:#08356380;--color-guilabel-border:#13395f80;--color-api-keyword:var(--color-foreground-secondary);--color-highlight-on-target:#330;--color-admonition-background:#18181a;--color-card-border:var(--color-background-secondary);--color-card-background:#18181a;--color-card-marginals-background:var(--color-background-hover)}html body:not([data-theme=light]) .only-light{display:none!important}body:not([data-theme=light]) .only-dark{display:block!important}}}body[data-theme=auto] .theme-toggle svg.theme-icon-when-auto,body[data-theme=dark] .theme-toggle svg.theme-icon-when-dark,body[data-theme=light] .theme-toggle svg.theme-icon-when-light{display:block}body{font-family:var(--font-stack)}code,kbd,pre,samp{font-family:var(--font-stack--monospace)}body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}article{line-height:1.5}h1,h2,h3,h4,h5,h6{border-radius:.5rem;font-weight:700;line-height:1.25;margin:.5rem -.5rem;padding-left:.5rem;padding-right:.5rem}h1+p,h2+p,h3+p,h4+p,h5+p,h6+p{margin-top:0}h1{font-size:2.5em;margin-bottom:1rem}h1,h2{margin-top:1.75rem}h2{font-size:2em}h3{font-size:1.5em}h4{font-size:1.25em}h5{font-size:1.125em}h6{font-size:1em}small{font-size:80%;opacity:75%}p{margin-bottom:.75rem;margin-top:.5rem}hr.docutils{background-color:var(--color-background-border);border:0;height:1px;margin:2rem 0;padding:0}.centered{text-align:center}a{color:var(--color-link);text-decoration:underline;-webkit-text-decoration-color:var(--color-link-underline);text-decoration-color:var(--color-link-underline)}a:hover{color:var(--color-link--hover);-webkit-text-decoration-color:var(--color-link-underline--hover);text-decoration-color:var(--color-link-underline--hover)}a.muted-link{color:inherit}a.muted-link:hover{color:var(--color-link);-webkit-text-decoration-color:var(--color-link-underline--hover);text-decoration-color:var(--color-link-underline--hover)}html{overflow-x:hidden;overflow-y:scroll;scroll-behavior:smooth}.sidebar-scroll,.toc-scroll,article[role=main] *{scrollbar-color:var(--color-foreground-border) transparent;scrollbar-width:thin}.sidebar-scroll::-webkit-scrollbar,.toc-scroll::-webkit-scrollbar,article[role=main] ::-webkit-scrollbar{height:.25rem;width:.25rem}.sidebar-scroll::-webkit-scrollbar-thumb,.toc-scroll::-webkit-scrollbar-thumb,article[role=main] ::-webkit-scrollbar-thumb{background-color:var(--color-foreground-border);border-radius:.125rem}body,html{background:var(--color-background-primary);color:var(--color-foreground-primary);height:100%}article{background:var(--color-content-background);color:var(--color-content-foreground)}.page{display:flex;min-height:100%}.mobile-header{background-color:var(--color-header-background);border-bottom:1px solid var(--color-header-border);color:var(--color-header-text);display:none;height:var(--header-height);width:100%;z-index:10}.mobile-header.scrolled{border-bottom:none;box-shadow:0 0 .2rem rgba(0,0,0,.1),0 .2rem .4rem rgba(0,0,0,.2)}.mobile-header .header-center a{color:var(--color-header-text);text-decoration:none}.main{display:flex;flex:1}.sidebar-drawer{background:var(--color-sidebar-background);border-right:1px solid var(--color-sidebar-background-border);box-sizing:border-box;display:flex;justify-content:flex-end;min-width:15em;width:calc(50% - 26em)}.sidebar-container,.toc-drawer{box-sizing:border-box;width:15em}.toc-drawer{background:var(--color-toc-background);padding-right:1rem}.sidebar-sticky,.toc-sticky{display:flex;flex-direction:column;height:min(100%,100vh);height:100vh;position:-webkit-sticky;position:sticky;top:0}.sidebar-scroll,.toc-scroll{flex-grow:1;flex-shrink:1;overflow:auto;scroll-behavior:smooth}.content{display:flex;flex-direction:column;justify-content:space-between;padding:0 3em;width:46em}.icon{display:inline-block;height:1rem;width:1rem}.icon svg{height:100%;width:100%}.announcement{align-items:center;background-color:var(--color-announcement-background);color:var(--color-announcement-text);display:flex;height:var(--header-height);overflow-x:auto}.announcement+.page{min-height:calc(100% - var(--header-height))}.announcement-content{box-sizing:border-box;min-width:100%;padding:.5rem;text-align:center;white-space:nowrap}.announcement-content a{color:var(--color-announcement-text);-webkit-text-decoration-color:var(--color-announcement-text);text-decoration-color:var(--color-announcement-text)}.announcement-content a:hover{color:var(--color-announcement-text);-webkit-text-decoration-color:var(--color-link--hover);text-decoration-color:var(--color-link--hover)}.no-js .theme-toggle-container{display:none}.theme-toggle-container{vertical-align:middle}.theme-toggle{background:transparent;border:none;cursor:pointer;padding:0}.theme-toggle svg{color:var(--color-foreground-primary);display:none;height:1rem;vertical-align:middle;width:1rem}.theme-toggle-header{float:left;padding:1rem .5rem}.nav-overlay-icon,.toc-overlay-icon{cursor:pointer;display:none}.nav-overlay-icon .icon,.toc-overlay-icon .icon{color:var(--color-foreground-secondary);height:1rem;width:1rem}.nav-overlay-icon,.toc-header-icon{align-items:center;justify-content:center}.toc-content-icon{height:1.5rem;width:1.5rem}.content-icon-container{display:flex;float:right;gap:.5rem;margin-bottom:1rem;margin-left:1rem;margin-top:1.5rem}.content-icon-container .edit-this-page svg{color:inherit;height:1rem;width:1rem}.sidebar-toggle{display:none;position:absolute}.sidebar-toggle[name=__toc]{left:20px}.sidebar-toggle:checked{left:40px}.overlay{background-color:rgba(0,0,0,.54);height:0;opacity:0;position:fixed;top:0;transition:width 0ms,height 0ms,opacity .25s ease-out;width:0}.sidebar-overlay{z-index:20}.toc-overlay{z-index:40}.sidebar-drawer{transition:left .25s ease-in-out;z-index:30}.toc-drawer{transition:right .25s ease-in-out;z-index:50}#__navigation:checked~.sidebar-overlay{height:100%;opacity:1;width:100%}#__navigation:checked~.page .sidebar-drawer{left:0;top:0}#__toc:checked~.toc-overlay{height:100%;opacity:1;width:100%}#__toc:checked~.page .toc-drawer{right:0;top:0}.back-to-top{background:var(--color-background-primary);border-radius:1rem;box-shadow:0 .2rem .5rem rgba(0,0,0,.05),0 0 1px 0 hsla(220,9%,46%,.502);display:none;font-size:.8125rem;left:0;margin-left:50%;padding:.5rem .75rem .5rem .5rem;position:fixed;text-decoration:none;top:1rem;transform:translateX(-50%);z-index:10}.back-to-top svg{fill:currentColor;display:inline-block;height:1rem;width:1rem}.back-to-top span{margin-left:.25rem}.show-back-to-top .back-to-top{align-items:center;display:flex}@media(min-width:97em){html{font-size:110%}}@media(max-width:82em){.toc-content-icon{display:flex}.toc-drawer{border-left:1px solid var(--color-background-muted);height:100vh;position:fixed;right:-15em;top:0}.toc-tree{border-left:none;font-size:var(--toc-font-size--mobile)}.sidebar-drawer{width:calc(50% - 18.5em)}}@media(max-width:67em){.nav-overlay-icon{display:flex}.sidebar-drawer{height:100vh;left:-15em;position:fixed;top:0;width:15em}.toc-header-icon{display:flex}.theme-toggle-content,.toc-content-icon{display:none}.theme-toggle-header{display:block}.mobile-header{align-items:center;display:flex;justify-content:space-between;position:-webkit-sticky;position:sticky;top:0}.mobile-header .header-left,.mobile-header .header-right{display:flex;height:var(--header-height);padding:0 var(--header-padding)}.mobile-header .header-left label,.mobile-header .header-right label{height:100%;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:100%}:target{scroll-margin-top:var(--header-height)}.back-to-top{top:calc(var(--header-height) + .5rem)}.page{flex-direction:column;justify-content:center}.content{margin-left:auto;margin-right:auto}}@media(max-width:52em){.content{overflow-x:auto;width:100%}}@media(max-width:46em){.content{padding:0 1em}article aside.sidebar{float:none;margin:1rem 0;width:100%}}.admonition,.topic{background:var(--color-admonition-background);border-radius:.2rem;box-shadow:0 .2rem .5rem rgba(0,0,0,.05),0 0 .0625rem rgba(0,0,0,.1);font-size:var(--admonition-font-size);margin:1rem auto;overflow:hidden;padding:0 .5rem .5rem;page-break-inside:avoid}.admonition>:nth-child(2),.topic>:nth-child(2){margin-top:0}.admonition>:last-child,.topic>:last-child{margin-bottom:0}p.admonition-title,p.topic-title{font-size:var(--admonition-title-font-size);font-weight:500;line-height:1.3;margin:0 -.5rem .5rem;padding:.4rem .5rem .4rem 2rem;position:relative}p.admonition-title:before,p.topic-title:before{content:"";height:1rem;left:.5rem;position:absolute;width:1rem}p.admonition-title{background-color:var(--color-admonition-title-background)}p.admonition-title:before{background-color:var(--color-admonition-title);-webkit-mask-image:var(--icon-admonition-default);mask-image:var(--icon-admonition-default);-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat}p.topic-title{background-color:var(--color-topic-title-background)}p.topic-title:before{background-color:var(--color-topic-title);-webkit-mask-image:var(--icon-topic-default);mask-image:var(--icon-topic-default);-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat}.admonition{border-left:.2rem solid var(--color-admonition-title)}.admonition.caution{border-left-color:var(--color-admonition-title--caution)}.admonition.caution>.admonition-title{background-color:var(--color-admonition-title-background--caution)}.admonition.caution>.admonition-title:before{background-color:var(--color-admonition-title--caution);-webkit-mask-image:var(--icon-spark);mask-image:var(--icon-spark)}.admonition.warning{border-left-color:var(--color-admonition-title--warning)}.admonition.warning>.admonition-title{background-color:var(--color-admonition-title-background--warning)}.admonition.warning>.admonition-title:before{background-color:var(--color-admonition-title--warning);-webkit-mask-image:var(--icon-warning);mask-image:var(--icon-warning)}.admonition.danger{border-left-color:var(--color-admonition-title--danger)}.admonition.danger>.admonition-title{background-color:var(--color-admonition-title-background--danger)}.admonition.danger>.admonition-title:before{background-color:var(--color-admonition-title--danger);-webkit-mask-image:var(--icon-spark);mask-image:var(--icon-spark)}.admonition.attention{border-left-color:var(--color-admonition-title--attention)}.admonition.attention>.admonition-title{background-color:var(--color-admonition-title-background--attention)}.admonition.attention>.admonition-title:before{background-color:var(--color-admonition-title--attention);-webkit-mask-image:var(--icon-warning);mask-image:var(--icon-warning)}.admonition.error{border-left-color:var(--color-admonition-title--error)}.admonition.error>.admonition-title{background-color:var(--color-admonition-title-background--error)}.admonition.error>.admonition-title:before{background-color:var(--color-admonition-title--error);-webkit-mask-image:var(--icon-failure);mask-image:var(--icon-failure)}.admonition.hint{border-left-color:var(--color-admonition-title--hint)}.admonition.hint>.admonition-title{background-color:var(--color-admonition-title-background--hint)}.admonition.hint>.admonition-title:before{background-color:var(--color-admonition-title--hint);-webkit-mask-image:var(--icon-question);mask-image:var(--icon-question)}.admonition.tip{border-left-color:var(--color-admonition-title--tip)}.admonition.tip>.admonition-title{background-color:var(--color-admonition-title-background--tip)}.admonition.tip>.admonition-title:before{background-color:var(--color-admonition-title--tip);-webkit-mask-image:var(--icon-info);mask-image:var(--icon-info)}.admonition.important{border-left-color:var(--color-admonition-title--important)}.admonition.important>.admonition-title{background-color:var(--color-admonition-title-background--important)}.admonition.important>.admonition-title:before{background-color:var(--color-admonition-title--important);-webkit-mask-image:var(--icon-flame);mask-image:var(--icon-flame)}.admonition.note{border-left-color:var(--color-admonition-title--note)}.admonition.note>.admonition-title{background-color:var(--color-admonition-title-background--note)}.admonition.note>.admonition-title:before{background-color:var(--color-admonition-title--note);-webkit-mask-image:var(--icon-pencil);mask-image:var(--icon-pencil)}.admonition.seealso{border-left-color:var(--color-admonition-title--seealso)}.admonition.seealso>.admonition-title{background-color:var(--color-admonition-title-background--seealso)}.admonition.seealso>.admonition-title:before{background-color:var(--color-admonition-title--seealso);-webkit-mask-image:var(--icon-info);mask-image:var(--icon-info)}.admonition.admonition-todo{border-left-color:var(--color-admonition-title--admonition-todo)}.admonition.admonition-todo>.admonition-title{background-color:var(--color-admonition-title-background--admonition-todo)}.admonition.admonition-todo>.admonition-title:before{background-color:var(--color-admonition-title--admonition-todo);-webkit-mask-image:var(--icon-pencil);mask-image:var(--icon-pencil)}.admonition-todo>.admonition-title{text-transform:uppercase}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dd{margin-left:2rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dd>:first-child{margin-top:.125rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list,dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dd>:last-child{margin-bottom:.75rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list>dt{font-size:var(--font-size--small);text-transform:uppercase}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd:empty{margin-bottom:.5rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd>ul{margin-left:-1.2rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd>ul>li>p:nth-child(2){margin-top:0}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd>ul>li>p+p:last-child:empty{margin-bottom:0;margin-top:0}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt{color:var(--color-api-overall)}.sig:not(.sig-inline){background:var(--color-api-background);border-radius:.25rem;font-family:var(--font-stack--monospace);font-size:var(--api-font-size);font-weight:700;padding:.25rem .5rem .25rem 3em;text-indent:-2.5em}.sig:not(.sig-inline):hover{background:var(--color-api-background-hover)}.sig:not(.sig-inline) a.reference .viewcode-link{font-weight:400;width:3.5rem}.sig:not(.sig-inline) span.pre{overflow-wrap:anywhere}em.property{font-style:normal}em.property:first-child{color:var(--color-api-keyword)}.sig-name{color:var(--color-api-name)}.sig-prename{color:var(--color-api-pre-name);font-weight:400}.sig-paren{color:var(--color-api-paren)}.sig-param{font-style:normal}.versionmodified{font-style:italic}div.deprecated p,div.versionadded p,div.versionchanged p{margin-bottom:.125rem;margin-top:.125rem}.viewcode-back,.viewcode-link{float:right;text-align:right}.line-block{margin-bottom:.75rem;margin-top:.5rem}.line-block .line-block{margin-bottom:0;margin-top:0;padding-left:1rem}.code-block-caption,article p.caption,table>caption{font-size:var(--font-size--small);text-align:center}.toctree-wrapper.compound .caption,.toctree-wrapper.compound :not(.caption)>.caption-text{font-size:var(--font-size--small);margin-bottom:0;text-align:initial;text-transform:uppercase}.toctree-wrapper.compound>ul{margin-bottom:0;margin-top:0}.sig-inline,code.literal{background:var(--color-inline-code-background);border-radius:.2em;font-size:var(--font-size--small--2);padding:.1em .2em}p .sig-inline,p code.literal{border:1px solid var(--color-background-border)}.sig-inline{font-family:var(--font-stack--monospace)}div[class*=" highlight-"],div[class^=highlight-]{display:flex;margin:1em 0}div[class*=" highlight-"] .table-wrapper,div[class^=highlight-] .table-wrapper,pre{margin:0;padding:0}article[role=main] .highlight pre{line-height:1.5}.highlight pre,pre.literal-block{font-size:var(--code-font-size);overflow:auto;padding:.625rem .875rem}pre.literal-block{background-color:var(--color-code-background);border-radius:.2rem;color:var(--color-code-foreground);margin-bottom:1rem;margin-top:1rem}.highlight{border-radius:.2rem;width:100%}.highlight .gp,.highlight span.linenos{pointer-events:none;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight .hll{display:block;margin-left:-.875rem;margin-right:-.875rem;padding-left:.875rem;padding-right:.875rem}.code-block-caption{background-color:var(--color-code-background);border-bottom:1px solid;border-radius:.25rem;border-bottom-left-radius:0;border-bottom-right-radius:0;border-color:var(--color-background-border);color:var(--color-code-foreground);display:flex;font-weight:300;padding:.625rem .875rem}.code-block-caption+div[class]{margin-top:0}.code-block-caption+div[class] pre{border-top-left-radius:0;border-top-right-radius:0}.highlighttable{display:block;width:100%}.highlighttable tbody{display:block}.highlighttable tr{display:flex}.highlighttable td.linenos{background-color:var(--color-code-background);border-bottom-left-radius:.2rem;border-top-left-radius:.2rem;color:var(--color-code-foreground);padding:.625rem 0 .625rem .875rem}.highlighttable .linenodiv{box-shadow:-.0625rem 0 var(--color-foreground-border) inset;font-size:var(--code-font-size);padding-right:.875rem}.highlighttable td.code{display:block;flex:1;overflow:hidden;padding:0}.highlighttable td.code .highlight{border-bottom-left-radius:0;border-top-left-radius:0}.highlight span.linenos{box-shadow:-.0625rem 0 var(--color-foreground-border) inset;display:inline-block;margin-right:.875rem;padding-left:0;padding-right:.875rem}.footnote-reference{font-size:var(--font-size--small--4);vertical-align:super}dl.footnote.brackets{color:var(--color-foreground-secondary);display:grid;font-size:var(--font-size--small);grid-template-columns:-webkit-max-content auto;grid-template-columns:max-content auto}dl.footnote.brackets dt{margin:0}dl.footnote.brackets dt>.fn-backref{margin-left:.25rem}dl.footnote.brackets dt:after{content:":"}dl.footnote.brackets dt .brackets:before{content:"["}dl.footnote.brackets dt .brackets:after{content:"]"}dl.footnote.brackets dd{margin:0;padding:0 1rem}aside.footnote{color:var(--color-foreground-secondary);font-size:var(--font-size--small)}aside.footnote>span,div.citation>span{float:left;font-weight:500;padding-right:.25rem}aside.footnote>p,div.citation>p{margin-left:2rem}img{box-sizing:border-box;height:auto;max-width:100%}article .figure,article figure{border-radius:.2rem;margin:0}article .figure :last-child,article figure :last-child{margin-bottom:0}article .align-left{clear:left;float:left;margin:0 1rem 1rem}article .align-right{clear:right;float:right;margin:0 1rem 1rem}article .align-center,article .align-default{display:block;margin-left:auto;margin-right:auto;text-align:center}article table.align-default{display:table;text-align:initial}.domainindex-jumpbox,.genindex-jumpbox{border-bottom:1px solid var(--color-background-border);border-top:1px solid var(--color-background-border);padding:.25rem}.domainindex-section h2,.genindex-section h2{margin-bottom:.5rem;margin-top:.75rem}.domainindex-section ul,.genindex-section ul{margin-bottom:0;margin-top:0}ol,ul{margin-bottom:1rem;margin-top:1rem;padding-left:1.2rem}ol li>p:first-child,ul li>p:first-child{margin-bottom:.25rem;margin-top:.25rem}ol li>p:last-child,ul li>p:last-child{margin-top:.25rem}ol li>ol,ol li>ul,ul li>ol,ul li>ul{margin-bottom:.5rem;margin-top:.5rem}ol.arabic{list-style:decimal}ol.loweralpha{list-style:lower-alpha}ol.upperalpha{list-style:upper-alpha}ol.lowerroman{list-style:lower-roman}ol.upperroman{list-style:upper-roman}.simple li>ol,.simple li>ul,.toctree-wrapper li>ol,.toctree-wrapper li>ul{margin-bottom:0;margin-top:0}.field-list dt,.option-list dt,dl.footnote dt,dl.glossary dt,dl.simple dt,dl:not([class]) dt{font-weight:500;margin-top:.25rem}.field-list dt+dt,.option-list dt+dt,dl.footnote dt+dt,dl.glossary dt+dt,dl.simple dt+dt,dl:not([class]) dt+dt{margin-top:0}.field-list dt .classifier:before,.option-list dt .classifier:before,dl.footnote dt .classifier:before,dl.glossary dt .classifier:before,dl.simple dt .classifier:before,dl:not([class]) dt .classifier:before{content:":";margin-left:.2rem;margin-right:.2rem}.field-list dd ul,.field-list dd>p:first-child,.option-list dd ul,.option-list dd>p:first-child,dl.footnote dd ul,dl.footnote dd>p:first-child,dl.glossary dd ul,dl.glossary dd>p:first-child,dl.simple dd ul,dl.simple dd>p:first-child,dl:not([class]) dd ul,dl:not([class]) dd>p:first-child{margin-top:.125rem}.field-list dd ul,.option-list dd ul,dl.footnote dd ul,dl.glossary dd ul,dl.simple dd ul,dl:not([class]) dd ul{margin-bottom:.125rem}.math-wrapper{overflow-x:auto;width:100%}div.math{position:relative;text-align:center}div.math .headerlink,div.math:focus .headerlink{display:none}div.math:hover .headerlink{display:inline-block}div.math span.eqno{position:absolute;right:.5rem;top:50%;transform:translateY(-50%);z-index:1}abbr[title]{cursor:help}.problematic{color:var(--color-problematic)}kbd:not(.compound){background-color:var(--color-background-secondary);border:1px solid var(--color-foreground-border);border-radius:.2rem;box-shadow:0 .0625rem 0 rgba(0,0,0,.2),inset 0 0 0 .125rem var(--color-background-primary);color:var(--color-foreground-primary);display:inline-block;font-size:var(--font-size--small--3);margin:0 .2rem;padding:0 .2rem;vertical-align:text-bottom}blockquote{background:var(--color-background-secondary);border-left:4px solid var(--color-background-border);margin-left:0;margin-right:0;padding:.5rem 1rem}blockquote .attribution{font-weight:600;text-align:right}blockquote.highlights,blockquote.pull-quote{font-size:1.25em}blockquote.epigraph,blockquote.pull-quote{border-left-width:0;border-radius:.5rem}blockquote.highlights{background:transparent;border-left-width:0}p .reference img{vertical-align:middle}p.rubric{font-size:1.125em;font-weight:700;line-height:1.25}dd p.rubric{font-size:var(--font-size--small);font-weight:inherit;line-height:inherit;text-transform:uppercase}article .sidebar{background-color:var(--color-background-secondary);border:1px solid var(--color-background-border);border-radius:.2rem;clear:right;float:right;margin-left:1rem;margin-right:0;width:30%}article .sidebar>*{padding-left:1rem;padding-right:1rem}article .sidebar>ol,article .sidebar>ul{padding-left:2.2rem}article .sidebar .sidebar-title{border-bottom:1px solid var(--color-background-border);font-weight:500;margin:0;padding:.5rem 1rem}.table-wrapper{margin-bottom:.5rem;margin-top:1rem;overflow-x:auto;padding:.2rem .2rem .75rem;width:100%}table.docutils{border-collapse:collapse;border-radius:.2rem;border-spacing:0;box-shadow:0 .2rem .5rem rgba(0,0,0,.05),0 0 .0625rem rgba(0,0,0,.1)}table.docutils th{background:var(--color-table-header-background)}table.docutils td,table.docutils th{border-bottom:1px solid var(--color-table-border);border-left:1px solid var(--color-table-border);border-right:1px solid var(--color-table-border);padding:0 .25rem}table.docutils td p,table.docutils th p{margin:.25rem}table.docutils td:first-child,table.docutils th:first-child{border-left:none}table.docutils td:last-child,table.docutils th:last-child{border-right:none}table.docutils td.text-left,table.docutils th.text-left{text-align:left}table.docutils td.text-right,table.docutils th.text-right{text-align:right}table.docutils td.text-center,table.docutils th.text-center{text-align:center}:target{scroll-margin-top:.5rem}@media(max-width:67em){:target{scroll-margin-top:calc(.5rem + var(--header-height))}section>span:target{scroll-margin-top:calc(.8rem + var(--header-height))}}.headerlink{font-weight:100;-webkit-user-select:none;-moz-user-select:none;user-select:none}.code-block-caption>.headerlink,dl dt>.headerlink,figcaption p>.headerlink,h1>.headerlink,h2>.headerlink,h3>.headerlink,h4>.headerlink,h5>.headerlink,h6>.headerlink,p.caption>.headerlink,table>caption>.headerlink{margin-left:.5rem;visibility:hidden}.code-block-caption:hover>.headerlink,dl dt:hover>.headerlink,figcaption p:hover>.headerlink,h1:hover>.headerlink,h2:hover>.headerlink,h3:hover>.headerlink,h4:hover>.headerlink,h5:hover>.headerlink,h6:hover>.headerlink,p.caption:hover>.headerlink,table>caption:hover>.headerlink{visibility:visible}.code-block-caption>.toc-backref,dl dt>.toc-backref,figcaption p>.toc-backref,h1>.toc-backref,h2>.toc-backref,h3>.toc-backref,h4>.toc-backref,h5>.toc-backref,h6>.toc-backref,p.caption>.toc-backref,table>caption>.toc-backref{color:inherit;-webkit-text-decoration-line:none;text-decoration-line:none}figure:hover>figcaption>p>.headerlink,table:hover>caption>.headerlink{visibility:visible}:target>h1:first-of-type,:target>h2:first-of-type,:target>h3:first-of-type,:target>h4:first-of-type,:target>h5:first-of-type,:target>h6:first-of-type,span:target~h1:first-of-type,span:target~h2:first-of-type,span:target~h3:first-of-type,span:target~h4:first-of-type,span:target~h5:first-of-type,span:target~h6:first-of-type{background-color:var(--color-highlight-on-target)}:target>h1:first-of-type code.literal,:target>h2:first-of-type code.literal,:target>h3:first-of-type code.literal,:target>h4:first-of-type code.literal,:target>h5:first-of-type code.literal,:target>h6:first-of-type code.literal,span:target~h1:first-of-type code.literal,span:target~h2:first-of-type code.literal,span:target~h3:first-of-type code.literal,span:target~h4:first-of-type code.literal,span:target~h5:first-of-type code.literal,span:target~h6:first-of-type code.literal{background-color:transparent}.literal-block-wrapper:target .code-block-caption,.this-will-duplicate-information-and-it-is-still-useful-here li :target,figure:target,table:target>caption{background-color:var(--color-highlight-on-target)}dt:target{background-color:var(--color-highlight-on-target)!important}.footnote-reference:target,.footnote>dt:target+dd{background-color:var(--color-highlight-on-target)}.guilabel{background-color:var(--color-guilabel-background);border:1px solid var(--color-guilabel-border);border-radius:.5em;color:var(--color-guilabel-text);font-size:.9em;padding:0 .3em}footer{display:flex;flex-direction:column;font-size:var(--font-size--small);margin-top:2rem}.bottom-of-page{align-items:center;border-top:1px solid var(--color-background-border);color:var(--color-foreground-secondary);display:flex;justify-content:space-between;line-height:1.5;margin-top:1rem;padding-bottom:1rem;padding-top:1rem}@media(max-width:46em){.bottom-of-page{flex-direction:column-reverse;gap:.25rem;text-align:center}}.bottom-of-page .left-details{font-size:var(--font-size--small)}.bottom-of-page .right-details{display:flex;flex-direction:column;gap:.25rem;text-align:right}.bottom-of-page .icons{display:flex;font-size:1rem;gap:.25rem;justify-content:flex-end}.bottom-of-page .icons a{text-decoration:none}.bottom-of-page .icons img,.bottom-of-page .icons svg{font-size:1.125rem;height:1em;width:1em}.related-pages a{align-items:center;display:flex;text-decoration:none}.related-pages a:hover .page-info .title{color:var(--color-link);text-decoration:underline;-webkit-text-decoration-color:var(--color-link-underline);text-decoration-color:var(--color-link-underline)}.related-pages a svg.furo-related-icon,.related-pages a svg.furo-related-icon>use{color:var(--color-foreground-border);flex-shrink:0;height:.75rem;margin:0 .5rem;width:.75rem}.related-pages a.next-page{clear:right;float:right;max-width:50%;text-align:right}.related-pages a.prev-page{clear:left;float:left;max-width:50%}.related-pages a.prev-page svg{transform:rotate(180deg)}.page-info{display:flex;flex-direction:column;overflow-wrap:anywhere}.next-page .page-info{align-items:flex-end}.page-info .context{align-items:center;color:var(--color-foreground-muted);display:flex;font-size:var(--font-size--small);padding-bottom:.1rem;text-decoration:none}ul.search{list-style:none;padding-left:0}ul.search li{border-bottom:1px solid var(--color-background-border);padding:1rem 0}[role=main] .highlighted{background-color:var(--color-highlighted-background);color:var(--color-highlighted-text)}.sidebar-brand{display:flex;flex-direction:column;flex-shrink:0;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal);text-decoration:none}.sidebar-brand-text{color:var(--color-sidebar-brand-text);font-size:1.5rem;overflow-wrap:break-word}.sidebar-brand-text,.sidebar-logo-container{margin:var(--sidebar-item-spacing-vertical) 0}.sidebar-logo{display:block;margin:0 auto;max-width:100%}.sidebar-search-container{align-items:center;background:var(--color-sidebar-search-background);display:flex;margin-top:var(--sidebar-search-space-above);position:relative}.sidebar-search-container:focus-within,.sidebar-search-container:hover{background:var(--color-sidebar-search-background--focus)}.sidebar-search-container:before{background-color:var(--color-sidebar-search-icon);content:"";height:var(--sidebar-search-icon-size);left:var(--sidebar-item-spacing-horizontal);-webkit-mask-image:var(--icon-search);mask-image:var(--icon-search);position:absolute;width:var(--sidebar-search-icon-size)}.sidebar-search{background:transparent;border:none;border-bottom:1px solid var(--color-sidebar-search-border);border-top:1px solid var(--color-sidebar-search-border);box-sizing:border-box;color:var(--color-sidebar-search-foreground);padding:var(--sidebar-search-input-spacing-vertical) var(--sidebar-search-input-spacing-horizontal) var(--sidebar-search-input-spacing-vertical) calc(var(--sidebar-item-spacing-horizontal) + var(--sidebar-search-input-spacing-horizontal) + var(--sidebar-search-icon-size));width:100%;z-index:10}.sidebar-search:focus{outline:none}.sidebar-search::-moz-placeholder{font-size:var(--sidebar-search-input-font-size)}.sidebar-search::placeholder{font-size:var(--sidebar-search-input-font-size)}#searchbox .highlight-link{margin:0;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal) 0;text-align:center}#searchbox .highlight-link a{color:var(--color-sidebar-search-icon);font-size:var(--font-size--small--2)}.sidebar-tree{font-size:var(--sidebar-item-font-size);margin-bottom:var(--sidebar-item-spacing-vertical);margin-top:var(--sidebar-tree-space-above)}.sidebar-tree ul{display:flex;flex-direction:column;list-style:none;margin-bottom:0;margin-top:0;padding:0}.sidebar-tree li{margin:0;position:relative}.sidebar-tree li>ul{margin-left:var(--sidebar-item-spacing-horizontal)}.sidebar-tree .icon,.sidebar-tree .reference{color:var(--color-sidebar-link-text)}.sidebar-tree .reference{box-sizing:border-box;display:inline-block;height:100%;line-height:var(--sidebar-item-line-height);overflow-wrap:anywhere;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal);text-decoration:none;width:100%}.sidebar-tree .reference:hover{background:var(--color-sidebar-item-background--hover)}.sidebar-tree .reference.external:after{color:var(--color-sidebar-link-text);content:url("data:image/svg+xml;charset=utf-8,%3Csvg width='12' height='12' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M11 7H6a2 2 0 0 0-2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2-2v-5M10 14 20 4M15 4h5v5'/%3E%3C/svg%3E");margin:0 .25rem;vertical-align:middle}.sidebar-tree .current-page>.reference{font-weight:700}.sidebar-tree label{align-items:center;cursor:pointer;display:flex;height:var(--sidebar-item-height);justify-content:center;position:absolute;right:0;top:0;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:var(--sidebar-expander-width)}.sidebar-tree .caption,.sidebar-tree :not(.caption)>.caption-text{color:var(--color-sidebar-caption-text);font-size:var(--sidebar-caption-font-size);font-weight:700;margin:var(--sidebar-caption-space-above) 0 0 0;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal);text-transform:uppercase}.sidebar-tree li.has-children>.reference{padding-right:var(--sidebar-expander-width)}.sidebar-tree .toctree-l1>.reference,.sidebar-tree .toctree-l1>label .icon{color:var(--color-sidebar-link-text--top-level)}.sidebar-tree label{background:var(--color-sidebar-item-expander-background)}.sidebar-tree label:hover{background:var(--color-sidebar-item-expander-background--hover)}.sidebar-tree .current>.reference{background:var(--color-sidebar-item-background--current)}.sidebar-tree .current>.reference:hover{background:var(--color-sidebar-item-background--hover)}.toctree-checkbox{display:none;position:absolute}.toctree-checkbox~ul{display:none}.toctree-checkbox~label .icon svg{transform:rotate(90deg)}.toctree-checkbox:checked~ul{display:block}.toctree-checkbox:checked~label .icon svg{transform:rotate(-90deg)}.toc-title-container{padding:var(--toc-title-padding);padding-top:var(--toc-spacing-vertical)}.toc-title{color:var(--color-toc-title-text);font-size:var(--toc-title-font-size);padding-left:var(--toc-spacing-horizontal);text-transform:uppercase}.no-toc{display:none}.toc-tree-container{padding-bottom:var(--toc-spacing-vertical)}.toc-tree{border-left:1px solid var(--color-background-border);font-size:var(--toc-font-size);line-height:1.3;padding-left:calc(var(--toc-spacing-horizontal) - var(--toc-item-spacing-horizontal))}.toc-tree>ul>li:first-child{padding-top:0}.toc-tree>ul>li:first-child>ul{padding-left:0}.toc-tree>ul>li:first-child>a{display:none}.toc-tree ul{list-style-type:none;margin-bottom:0;margin-top:0;padding-left:var(--toc-item-spacing-horizontal)}.toc-tree li{padding-top:var(--toc-item-spacing-vertical)}.toc-tree li.scroll-current>.reference{color:var(--color-toc-item-text--active);font-weight:700}.toc-tree .reference{color:var(--color-toc-item-text);overflow-wrap:anywhere;text-decoration:none}.toc-scroll{max-height:100vh;overflow-y:scroll}.contents:not(.this-will-duplicate-information-and-it-is-still-useful-here){background:rgba(255,0,0,.25);color:var(--color-problematic)}.contents:not(.this-will-duplicate-information-and-it-is-still-useful-here):before{content:"ERROR: Adding a table of contents in Furo-based documentation is unnecessary, and does not work well with existing styling.Add a 'this-will-duplicate-information-and-it-is-still-useful-here' class, if you want an escape hatch."}.text-align\:left>p{text-align:left}.text-align\:center>p{text-align:center}.text-align\:right>p{text-align:right}
+/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */html{-webkit-text-size-adjust:100%;line-height:1.15}body{margin:0}main{display:block}h1{font-size:2em;margin:.67em 0}hr{box-sizing:content-box;height:0;overflow:visible}pre{font-family:monospace,monospace;font-size:1em}a{background-color:transparent}abbr[title]{border-bottom:none;text-decoration:underline;text-decoration:underline dotted}b,strong{font-weight:bolder}code,kbd,samp{font-family:monospace,monospace;font-size:1em}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}img{border-style:none}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;line-height:1.15;margin:0}button,input{overflow:visible}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner,button::-moz-focus-inner{border-style:none;padding:0}[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring,button:-moz-focusring{outline:1px dotted ButtonText}fieldset{padding:.35em .75em .625em}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal}progress{vertical-align:baseline}textarea{overflow:auto}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}[type=search]::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}details{display:block}summary{display:list-item}[hidden],template{display:none}@media print{.content-icon-container,.headerlink,.mobile-header,.related-pages{display:none!important}.highlight{border:.1pt solid var(--color-foreground-border)}a,blockquote,dl,ol,pre,table,ul{page-break-inside:avoid}caption,figure,h1,h2,h3,h4,h5,h6,img{page-break-after:avoid;page-break-inside:avoid}dl,ol,ul{page-break-before:avoid}}.visually-hidden{clip:rect(0,0,0,0)!important;border:0!important;height:1px!important;margin:-1px!important;overflow:hidden!important;padding:0!important;position:absolute!important;white-space:nowrap!important;width:1px!important}:-moz-focusring{outline:auto}body{--font-stack:-apple-system,BlinkMacSystemFont,Segoe UI,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji;--font-stack--monospace:"SFMono-Regular",Menlo,Consolas,Monaco,Liberation Mono,Lucida Console,monospace;--font-size--normal:100%;--font-size--small:87.5%;--font-size--small--2:81.25%;--font-size--small--3:75%;--font-size--small--4:62.5%;--sidebar-caption-font-size:var(--font-size--small--2);--sidebar-item-font-size:var(--font-size--small);--sidebar-search-input-font-size:var(--font-size--small);--toc-font-size:var(--font-size--small--3);--toc-font-size--mobile:var(--font-size--normal);--toc-title-font-size:var(--font-size--small--4);--admonition-font-size:0.8125rem;--admonition-title-font-size:0.8125rem;--code-font-size:var(--font-size--small--2);--api-font-size:var(--font-size--small);--header-height:calc(var(--sidebar-item-line-height) + var(--sidebar-item-spacing-vertical)*4);--header-padding:0.5rem;--sidebar-tree-space-above:1.5rem;--sidebar-caption-space-above:1rem;--sidebar-item-line-height:1rem;--sidebar-item-spacing-vertical:0.5rem;--sidebar-item-spacing-horizontal:1rem;--sidebar-item-height:calc(var(--sidebar-item-line-height) + var(--sidebar-item-spacing-vertical)*2);--sidebar-expander-width:var(--sidebar-item-height);--sidebar-search-space-above:0.5rem;--sidebar-search-input-spacing-vertical:0.5rem;--sidebar-search-input-spacing-horizontal:0.5rem;--sidebar-search-input-height:1rem;--sidebar-search-icon-size:var(--sidebar-search-input-height);--toc-title-padding:0.25rem 0;--toc-spacing-vertical:1.5rem;--toc-spacing-horizontal:1.5rem;--toc-item-spacing-vertical:0.4rem;--toc-item-spacing-horizontal:1rem;--icon-search:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path d="M0 0h24v24H0z" stroke="none"/><circle cx="10" cy="10" r="7"/><path d="m21 21-6-6"/></svg>');--icon-pencil:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20.71 7.04c.39-.39.39-1.04 0-1.41l-2.34-2.34c-.37-.39-1.02-.39-1.41 0l-1.84 1.83 3.75 3.75M3 17.25V21h3.75L17.81 9.93l-3.75-3.75L3 17.25z"/></svg>');--icon-abstract:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 5h16v2H4V5m0 4h16v2H4V9m0 4h16v2H4v-2m0 4h10v2H4v-2z"/></svg>');--icon-info:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 9h-2V7h2m0 10h-2v-6h2m-1-9A10 10 0 0 0 2 12a10 10 0 0 0 10 10 10 10 0 0 0 10-10A10 10 0 0 0 12 2z"/></svg>');--icon-flame:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M17.55 11.2c-.23-.3-.5-.56-.76-.82-.65-.6-1.4-1.03-2.03-1.66C13.3 7.26 13 4.85 13.91 3c-.91.23-1.75.75-2.45 1.32-2.54 2.08-3.54 5.75-2.34 8.9.04.1.08.2.08.33 0 .22-.15.42-.35.5-.22.1-.46.04-.64-.12a.83.83 0 0 1-.15-.17c-1.1-1.43-1.28-3.48-.53-5.12C5.89 10 5 12.3 5.14 14.47c.04.5.1 1 .27 1.5.14.6.4 1.2.72 1.73 1.04 1.73 2.87 2.97 4.84 3.22 2.1.27 4.35-.12 5.96-1.6 1.8-1.66 2.45-4.32 1.5-6.6l-.13-.26c-.2-.46-.47-.87-.8-1.25l.05-.01m-3.1 6.3c-.28.24-.73.5-1.08.6-1.1.4-2.2-.16-2.87-.82 1.19-.28 1.89-1.16 2.09-2.05.17-.8-.14-1.46-.27-2.23-.12-.74-.1-1.37.18-2.06.17.38.37.76.6 1.06.76 1 1.95 1.44 2.2 2.8.04.14.06.28.06.43.03.82-.32 1.72-.92 2.27h.01z"/></svg>');--icon-question:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="m15.07 11.25-.9.92C13.45 12.89 13 13.5 13 15h-2v-.5c0-1.11.45-2.11 1.17-2.83l1.24-1.26c.37-.36.59-.86.59-1.41a2 2 0 0 0-2-2 2 2 0 0 0-2 2H8a4 4 0 0 1 4-4 4 4 0 0 1 4 4 3.2 3.2 0 0 1-.93 2.25M13 19h-2v-2h2M12 2A10 10 0 0 0 2 12a10 10 0 0 0 10 10 10 10 0 0 0 10-10c0-5.53-4.5-10-10-10z"/></svg>');--icon-warning:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M13 14h-2v-4h2m0 8h-2v-2h2M1 21h22L12 2 1 21z"/></svg>');--icon-failure:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 2c5.53 0 10 4.47 10 10s-4.47 10-10 10S2 17.53 2 12 6.47 2 12 2m3.59 5L12 10.59 8.41 7 7 8.41 10.59 12 7 15.59 8.41 17 12 13.41 15.59 17 17 15.59 13.41 12 17 8.41 15.59 7z"/></svg>');--icon-spark:url('data:image/svg+xml;charset=utf-8,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="m11.5 20 4.86-9.73H13V4l-5 9.73h3.5V20M12 2c2.75 0 5.1 1 7.05 2.95C21 6.9 22 9.25 22 12s-1 5.1-2.95 7.05C17.1 21 14.75 22 12 22s-5.1-1-7.05-2.95C3 17.1 2 14.75 2 12s1-5.1 2.95-7.05C6.9 3 9.25 2 12 2z"/></svg>');--color-admonition-title--caution:#ff9100;--color-admonition-title-background--caution:rgba(255,145,0,.2);--color-admonition-title--warning:#ff9100;--color-admonition-title-background--warning:rgba(255,145,0,.2);--color-admonition-title--danger:#ff5252;--color-admonition-title-background--danger:rgba(255,82,82,.2);--color-admonition-title--attention:#ff5252;--color-admonition-title-background--attention:rgba(255,82,82,.2);--color-admonition-title--error:#ff5252;--color-admonition-title-background--error:rgba(255,82,82,.2);--color-admonition-title--hint:#00c852;--color-admonition-title-background--hint:rgba(0,200,82,.2);--color-admonition-title--tip:#00c852;--color-admonition-title-background--tip:rgba(0,200,82,.2);--color-admonition-title--important:#00bfa5;--color-admonition-title-background--important:rgba(0,191,165,.2);--color-admonition-title--note:#00b0ff;--color-admonition-title-background--note:rgba(0,176,255,.2);--color-admonition-title--seealso:#448aff;--color-admonition-title-background--seealso:rgba(68,138,255,.2);--color-admonition-title--admonition-todo:grey;--color-admonition-title-background--admonition-todo:hsla(0,0%,50%,.2);--color-admonition-title:#651fff;--color-admonition-title-background:rgba(101,31,255,.2);--icon-admonition-default:var(--icon-abstract);--color-topic-title:#14b8a6;--color-topic-title-background:rgba(20,184,166,.2);--icon-topic-default:var(--icon-pencil);--color-problematic:#b30000;--color-foreground-primary:#000;--color-foreground-secondary:#5a5c63;--color-foreground-muted:#646776;--color-foreground-border:#878787;--color-background-primary:#fff;--color-background-secondary:#f8f9fb;--color-background-hover:#efeff4;--color-background-hover--transparent:#efeff400;--color-background-border:#eeebee;--color-background-item:#ccc;--color-announcement-background:#000000dd;--color-announcement-text:#eeebee;--color-brand-primary:#2962ff;--color-brand-content:#2a5adf;--color-api-background:var(--color-background-hover--transparent);--color-api-background-hover:var(--color-background-hover);--color-api-overall:var(--color-foreground-secondary);--color-api-name:var(--color-problematic);--color-api-pre-name:var(--color-problematic);--color-api-paren:var(--color-foreground-secondary);--color-api-keyword:var(--color-foreground-primary);--color-highlight-on-target:#ffc;--color-inline-code-background:var(--color-background-secondary);--color-highlighted-background:#def;--color-highlighted-text:var(--color-foreground-primary);--color-guilabel-background:#ddeeff80;--color-guilabel-border:#bedaf580;--color-guilabel-text:var(--color-foreground-primary);--color-admonition-background:transparent;--color-table-header-background:var(--color-background-secondary);--color-table-border:var(--color-background-border);--color-card-border:var(--color-background-secondary);--color-card-background:transparent;--color-card-marginals-background:var(--color-background-secondary);--color-header-background:var(--color-background-primary);--color-header-border:var(--color-background-border);--color-header-text:var(--color-foreground-primary);--color-sidebar-background:var(--color-background-secondary);--color-sidebar-background-border:var(--color-background-border);--color-sidebar-brand-text:var(--color-foreground-primary);--color-sidebar-caption-text:var(--color-foreground-muted);--color-sidebar-link-text:var(--color-foreground-secondary);--color-sidebar-link-text--top-level:var(--color-brand-primary);--color-sidebar-item-background:var(--color-sidebar-background);--color-sidebar-item-background--current:var( --color-sidebar-item-background );--color-sidebar-item-background--hover:linear-gradient(90deg,var(--color-background-hover--transparent) 0%,var(--color-background-hover) var(--sidebar-item-spacing-horizontal),var(--color-background-hover) 100%);--color-sidebar-item-expander-background:transparent;--color-sidebar-item-expander-background--hover:var( --color-background-hover );--color-sidebar-search-text:var(--color-foreground-primary);--color-sidebar-search-background:var(--color-background-secondary);--color-sidebar-search-background--focus:var(--color-background-primary);--color-sidebar-search-border:var(--color-background-border);--color-sidebar-search-icon:var(--color-foreground-muted);--color-toc-background:var(--color-background-primary);--color-toc-title-text:var(--color-foreground-muted);--color-toc-item-text:var(--color-foreground-secondary);--color-toc-item-text--hover:var(--color-foreground-primary);--color-toc-item-text--active:var(--color-brand-primary);--color-content-foreground:var(--color-foreground-primary);--color-content-background:transparent;--color-link:var(--color-brand-content);--color-link--hover:var(--color-brand-content);--color-link-underline:var(--color-background-border);--color-link-underline--hover:var(--color-foreground-border)}.only-light{display:block!important}html body .only-dark{display:none!important}@media not print{body[data-theme=dark]{--color-problematic:#ee5151;--color-foreground-primary:#ffffffcc;--color-foreground-secondary:#9ca0a5;--color-foreground-muted:#81868d;--color-foreground-border:#666;--color-background-primary:#131416;--color-background-secondary:#1a1c1e;--color-background-hover:#1e2124;--color-background-hover--transparent:#1e212400;--color-background-border:#303335;--color-background-item:#444;--color-announcement-background:#000000dd;--color-announcement-text:#eeebee;--color-brand-primary:#2b8cee;--color-brand-content:#368ce2;--color-highlighted-background:#083563;--color-guilabel-background:#08356380;--color-guilabel-border:#13395f80;--color-api-keyword:var(--color-foreground-secondary);--color-highlight-on-target:#330;--color-admonition-background:#18181a;--color-card-border:var(--color-background-secondary);--color-card-background:#18181a;--color-card-marginals-background:var(--color-background-hover)}html body[data-theme=dark] .only-light{display:none!important}body[data-theme=dark] .only-dark{display:block!important}@media(prefers-color-scheme:dark){body:not([data-theme=light]){--color-problematic:#ee5151;--color-foreground-primary:#ffffffcc;--color-foreground-secondary:#9ca0a5;--color-foreground-muted:#81868d;--color-foreground-border:#666;--color-background-primary:#131416;--color-background-secondary:#1a1c1e;--color-background-hover:#1e2124;--color-background-hover--transparent:#1e212400;--color-background-border:#303335;--color-background-item:#444;--color-announcement-background:#000000dd;--color-announcement-text:#eeebee;--color-brand-primary:#2b8cee;--color-brand-content:#368ce2;--color-highlighted-background:#083563;--color-guilabel-background:#08356380;--color-guilabel-border:#13395f80;--color-api-keyword:var(--color-foreground-secondary);--color-highlight-on-target:#330;--color-admonition-background:#18181a;--color-card-border:var(--color-background-secondary);--color-card-background:#18181a;--color-card-marginals-background:var(--color-background-hover)}html body:not([data-theme=light]) .only-light{display:none!important}body:not([data-theme=light]) .only-dark{display:block!important}}}body[data-theme=auto] .theme-toggle svg.theme-icon-when-auto,body[data-theme=dark] .theme-toggle svg.theme-icon-when-dark,body[data-theme=light] .theme-toggle svg.theme-icon-when-light{display:block}body{font-family:var(--font-stack)}code,kbd,pre,samp{font-family:var(--font-stack--monospace)}body{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}article{line-height:1.5}h1,h2,h3,h4,h5,h6{border-radius:.5rem;font-weight:700;line-height:1.25;margin:.5rem -.5rem;padding-left:.5rem;padding-right:.5rem}h1+p,h2+p,h3+p,h4+p,h5+p,h6+p{margin-top:0}h1{font-size:2.5em;margin-bottom:1rem}h1,h2{margin-top:1.75rem}h2{font-size:2em}h3{font-size:1.5em}h4{font-size:1.25em}h5{font-size:1.125em}h6{font-size:1em}small{font-size:80%;opacity:75%}p{margin-bottom:.75rem;margin-top:.5rem}hr.docutils{background-color:var(--color-background-border);border:0;height:1px;margin:2rem 0;padding:0}.centered{text-align:center}a{color:var(--color-link);text-decoration:underline;-webkit-text-decoration-color:var(--color-link-underline);text-decoration-color:var(--color-link-underline)}a:hover{color:var(--color-link--hover);-webkit-text-decoration-color:var(--color-link-underline--hover);text-decoration-color:var(--color-link-underline--hover)}a.muted-link{color:inherit}a.muted-link:hover{color:var(--color-link);-webkit-text-decoration-color:var(--color-link-underline--hover);text-decoration-color:var(--color-link-underline--hover)}html{overflow-x:hidden;overflow-y:scroll;scroll-behavior:smooth}.sidebar-scroll,.toc-scroll,article[role=main] *{scrollbar-color:var(--color-foreground-border) transparent;scrollbar-width:thin}.sidebar-scroll::-webkit-scrollbar,.toc-scroll::-webkit-scrollbar,article[role=main] ::-webkit-scrollbar{height:.25rem;width:.25rem}.sidebar-scroll::-webkit-scrollbar-thumb,.toc-scroll::-webkit-scrollbar-thumb,article[role=main] ::-webkit-scrollbar-thumb{background-color:var(--color-foreground-border);border-radius:.125rem}body,html{background:var(--color-background-primary);color:var(--color-foreground-primary);height:100%}article{background:var(--color-content-background);color:var(--color-content-foreground)}.page{display:flex;min-height:100%}.mobile-header{background-color:var(--color-header-background);border-bottom:1px solid var(--color-header-border);color:var(--color-header-text);display:none;height:var(--header-height);width:100%;z-index:10}.mobile-header.scrolled{border-bottom:none;box-shadow:0 0 .2rem rgba(0,0,0,.1),0 .2rem .4rem rgba(0,0,0,.2)}.mobile-header .header-center a{color:var(--color-header-text);text-decoration:none}.main{display:flex;flex:1}.sidebar-drawer{background:var(--color-sidebar-background);border-right:1px solid var(--color-sidebar-background-border);box-sizing:border-box;display:flex;justify-content:flex-end;min-width:15em;width:calc(50% - 26em)}.sidebar-container,.toc-drawer{box-sizing:border-box;width:15em}.toc-drawer{background:var(--color-toc-background);padding-right:1rem}.sidebar-sticky,.toc-sticky{display:flex;flex-direction:column;height:min(100%,100vh);height:100vh;position:-webkit-sticky;position:sticky;top:0}.sidebar-scroll,.toc-scroll{flex-grow:1;flex-shrink:1;overflow:auto;scroll-behavior:smooth}.content{display:flex;flex-direction:column;justify-content:space-between;padding:0 3em;width:46em}.icon{display:inline-block;height:1rem;width:1rem}.icon svg{height:100%;width:100%}.announcement{align-items:center;background-color:var(--color-announcement-background);color:var(--color-announcement-text);display:flex;height:var(--header-height);overflow-x:auto}.announcement+.page{min-height:calc(100% - var(--header-height))}.announcement-content{box-sizing:border-box;min-width:100%;padding:.5rem;text-align:center;white-space:nowrap}.announcement-content a{color:var(--color-announcement-text);-webkit-text-decoration-color:var(--color-announcement-text);text-decoration-color:var(--color-announcement-text)}.announcement-content a:hover{color:var(--color-announcement-text);-webkit-text-decoration-color:var(--color-link--hover);text-decoration-color:var(--color-link--hover)}.no-js .theme-toggle-container{display:none}.theme-toggle-container{vertical-align:middle}.theme-toggle{background:transparent;border:none;cursor:pointer;padding:0}.theme-toggle svg{color:var(--color-foreground-primary);display:none;height:1rem;vertical-align:middle;width:1rem}.theme-toggle-header{float:left;padding:1rem .5rem}.nav-overlay-icon,.toc-overlay-icon{cursor:pointer;display:none}.nav-overlay-icon .icon,.toc-overlay-icon .icon{color:var(--color-foreground-secondary);height:1rem;width:1rem}.nav-overlay-icon,.toc-header-icon{align-items:center;justify-content:center}.toc-content-icon{height:1.5rem;width:1.5rem}.content-icon-container{display:flex;float:right;gap:.5rem;margin-bottom:1rem;margin-left:1rem;margin-top:1.5rem}.content-icon-container .edit-this-page svg{color:inherit;height:1rem;width:1rem}.sidebar-toggle{display:none;position:absolute}.sidebar-toggle[name=__toc]{left:20px}.sidebar-toggle:checked{left:40px}.overlay{background-color:rgba(0,0,0,.54);height:0;opacity:0;position:fixed;top:0;transition:width 0ms,height 0ms,opacity .25s ease-out;width:0}.sidebar-overlay{z-index:20}.toc-overlay{z-index:40}.sidebar-drawer{transition:left .25s ease-in-out;z-index:30}.toc-drawer{transition:right .25s ease-in-out;z-index:50}#__navigation:checked~.sidebar-overlay{height:100%;opacity:1;width:100%}#__navigation:checked~.page .sidebar-drawer{left:0;top:0}#__toc:checked~.toc-overlay{height:100%;opacity:1;width:100%}#__toc:checked~.page .toc-drawer{right:0;top:0}.back-to-top{background:var(--color-background-primary);border-radius:1rem;box-shadow:0 .2rem .5rem rgba(0,0,0,.05),0 0 1px 0 hsla(220,9%,46%,.502);display:none;font-size:.8125rem;left:0;margin-left:50%;padding:.5rem .75rem .5rem .5rem;position:fixed;text-decoration:none;top:1rem;transform:translateX(-50%);z-index:10}.back-to-top svg{fill:currentColor;display:inline-block;height:1rem;width:1rem}.back-to-top span{margin-left:.25rem}.show-back-to-top .back-to-top{align-items:center;display:flex}@media(min-width:97em){html{font-size:110%}}@media(max-width:82em){.toc-content-icon{display:flex}.toc-drawer{border-left:1px solid var(--color-background-muted);height:100vh;position:fixed;right:-15em;top:0}.toc-tree{border-left:none;font-size:var(--toc-font-size--mobile)}.sidebar-drawer{width:calc(50% - 18.5em)}}@media(max-width:67em){.nav-overlay-icon{display:flex}.sidebar-drawer{height:100vh;left:-15em;position:fixed;top:0;width:15em}.toc-header-icon{display:flex}.theme-toggle-content,.toc-content-icon{display:none}.theme-toggle-header{display:block}.mobile-header{align-items:center;display:flex;justify-content:space-between;position:-webkit-sticky;position:sticky;top:0}.mobile-header .header-left,.mobile-header .header-right{display:flex;height:var(--header-height);padding:0 var(--header-padding)}.mobile-header .header-left label,.mobile-header .header-right label{height:100%;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:100%}.nav-overlay-icon .icon,.theme-toggle svg{height:1.25rem;width:1.25rem}:target{scroll-margin-top:var(--header-height)}.back-to-top{top:calc(var(--header-height) + .5rem)}.page{flex-direction:column;justify-content:center}.content{margin-left:auto;margin-right:auto}}@media(max-width:52em){.content{overflow-x:auto;width:100%}}@media(max-width:46em){.content{padding:0 1em}article aside.sidebar{float:none;margin:1rem 0;width:100%}}.admonition,.topic{background:var(--color-admonition-background);border-radius:.2rem;box-shadow:0 .2rem .5rem rgba(0,0,0,.05),0 0 .0625rem rgba(0,0,0,.1);font-size:var(--admonition-font-size);margin:1rem auto;overflow:hidden;padding:0 .5rem .5rem;page-break-inside:avoid}.admonition>:nth-child(2),.topic>:nth-child(2){margin-top:0}.admonition>:last-child,.topic>:last-child{margin-bottom:0}p.admonition-title,p.topic-title{font-size:var(--admonition-title-font-size);font-weight:500;line-height:1.3;margin:0 -.5rem .5rem;padding:.4rem .5rem .4rem 2rem;position:relative}p.admonition-title:before,p.topic-title:before{content:"";height:1rem;left:.5rem;position:absolute;width:1rem}p.admonition-title{background-color:var(--color-admonition-title-background)}p.admonition-title:before{background-color:var(--color-admonition-title);-webkit-mask-image:var(--icon-admonition-default);mask-image:var(--icon-admonition-default);-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat}p.topic-title{background-color:var(--color-topic-title-background)}p.topic-title:before{background-color:var(--color-topic-title);-webkit-mask-image:var(--icon-topic-default);mask-image:var(--icon-topic-default);-webkit-mask-repeat:no-repeat;mask-repeat:no-repeat}.admonition{border-left:.2rem solid var(--color-admonition-title)}.admonition.caution{border-left-color:var(--color-admonition-title--caution)}.admonition.caution>.admonition-title{background-color:var(--color-admonition-title-background--caution)}.admonition.caution>.admonition-title:before{background-color:var(--color-admonition-title--caution);-webkit-mask-image:var(--icon-spark);mask-image:var(--icon-spark)}.admonition.warning{border-left-color:var(--color-admonition-title--warning)}.admonition.warning>.admonition-title{background-color:var(--color-admonition-title-background--warning)}.admonition.warning>.admonition-title:before{background-color:var(--color-admonition-title--warning);-webkit-mask-image:var(--icon-warning);mask-image:var(--icon-warning)}.admonition.danger{border-left-color:var(--color-admonition-title--danger)}.admonition.danger>.admonition-title{background-color:var(--color-admonition-title-background--danger)}.admonition.danger>.admonition-title:before{background-color:var(--color-admonition-title--danger);-webkit-mask-image:var(--icon-spark);mask-image:var(--icon-spark)}.admonition.attention{border-left-color:var(--color-admonition-title--attention)}.admonition.attention>.admonition-title{background-color:var(--color-admonition-title-background--attention)}.admonition.attention>.admonition-title:before{background-color:var(--color-admonition-title--attention);-webkit-mask-image:var(--icon-warning);mask-image:var(--icon-warning)}.admonition.error{border-left-color:var(--color-admonition-title--error)}.admonition.error>.admonition-title{background-color:var(--color-admonition-title-background--error)}.admonition.error>.admonition-title:before{background-color:var(--color-admonition-title--error);-webkit-mask-image:var(--icon-failure);mask-image:var(--icon-failure)}.admonition.hint{border-left-color:var(--color-admonition-title--hint)}.admonition.hint>.admonition-title{background-color:var(--color-admonition-title-background--hint)}.admonition.hint>.admonition-title:before{background-color:var(--color-admonition-title--hint);-webkit-mask-image:var(--icon-question);mask-image:var(--icon-question)}.admonition.tip{border-left-color:var(--color-admonition-title--tip)}.admonition.tip>.admonition-title{background-color:var(--color-admonition-title-background--tip)}.admonition.tip>.admonition-title:before{background-color:var(--color-admonition-title--tip);-webkit-mask-image:var(--icon-info);mask-image:var(--icon-info)}.admonition.important{border-left-color:var(--color-admonition-title--important)}.admonition.important>.admonition-title{background-color:var(--color-admonition-title-background--important)}.admonition.important>.admonition-title:before{background-color:var(--color-admonition-title--important);-webkit-mask-image:var(--icon-flame);mask-image:var(--icon-flame)}.admonition.note{border-left-color:var(--color-admonition-title--note)}.admonition.note>.admonition-title{background-color:var(--color-admonition-title-background--note)}.admonition.note>.admonition-title:before{background-color:var(--color-admonition-title--note);-webkit-mask-image:var(--icon-pencil);mask-image:var(--icon-pencil)}.admonition.seealso{border-left-color:var(--color-admonition-title--seealso)}.admonition.seealso>.admonition-title{background-color:var(--color-admonition-title-background--seealso)}.admonition.seealso>.admonition-title:before{background-color:var(--color-admonition-title--seealso);-webkit-mask-image:var(--icon-info);mask-image:var(--icon-info)}.admonition.admonition-todo{border-left-color:var(--color-admonition-title--admonition-todo)}.admonition.admonition-todo>.admonition-title{background-color:var(--color-admonition-title-background--admonition-todo)}.admonition.admonition-todo>.admonition-title:before{background-color:var(--color-admonition-title--admonition-todo);-webkit-mask-image:var(--icon-pencil);mask-image:var(--icon-pencil)}.admonition-todo>.admonition-title{text-transform:uppercase}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dd{margin-left:2rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dd>:first-child{margin-top:.125rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list,dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) dd>:last-child{margin-bottom:.75rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list>dt{font-size:var(--font-size--small);text-transform:uppercase}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd:empty{margin-bottom:.5rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd>ul{margin-left:-1.2rem}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd>ul>li>p:nth-child(2){margin-top:0}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple) .field-list dd>ul>li>p+p:last-child:empty{margin-bottom:0;margin-top:0}dl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)>dt{color:var(--color-api-overall)}.sig:not(.sig-inline){background:var(--color-api-background);border-radius:.25rem;font-family:var(--font-stack--monospace);font-size:var(--api-font-size);font-weight:700;margin-left:-.25rem;margin-right:-.25rem;padding:.25rem .5rem .25rem 3em;text-indent:-2.5em;transition:background .1s ease-out}.sig:not(.sig-inline):hover{background:var(--color-api-background-hover)}.sig:not(.sig-inline) a.reference .viewcode-link{font-weight:400;width:3.5rem}.sig:not(.sig-inline) span.pre{overflow-wrap:anywhere}em.property{font-style:normal}em.property:first-child{color:var(--color-api-keyword)}.sig-name{color:var(--color-api-name)}.sig-prename{color:var(--color-api-pre-name);font-weight:400}.sig-paren{color:var(--color-api-paren)}.sig-param{font-style:normal}.versionmodified{font-style:italic}div.deprecated p,div.versionadded p,div.versionchanged p{margin-bottom:.125rem;margin-top:.125rem}.viewcode-back,.viewcode-link{float:right;text-align:right}.line-block{margin-bottom:.75rem;margin-top:.5rem}.line-block .line-block{margin-bottom:0;margin-top:0;padding-left:1rem}.code-block-caption,article p.caption,table>caption{font-size:var(--font-size--small);text-align:center}.toctree-wrapper.compound .caption,.toctree-wrapper.compound :not(.caption)>.caption-text{font-size:var(--font-size--small);margin-bottom:0;text-align:initial;text-transform:uppercase}.toctree-wrapper.compound>ul{margin-bottom:0;margin-top:0}.sig-inline,code.literal{background:var(--color-inline-code-background);border-radius:.2em;font-size:var(--font-size--small--2);overflow-wrap:break-word;padding:.1em .2em}p .sig-inline,p code.literal{border:1px solid var(--color-background-border)}.sig-inline{font-family:var(--font-stack--monospace)}div[class*=" highlight-"],div[class^=highlight-]{display:flex;margin:1em 0}div[class*=" highlight-"] .table-wrapper,div[class^=highlight-] .table-wrapper,pre{margin:0;padding:0}pre{overflow:auto}article[role=main] .highlight pre{line-height:1.5}.highlight pre,pre.literal-block{font-size:var(--code-font-size);padding:.625rem .875rem}pre.literal-block{background-color:var(--color-code-background);border-radius:.2rem;color:var(--color-code-foreground);margin-bottom:1rem;margin-top:1rem}.highlight{border-radius:.2rem;width:100%}.highlight .gp,.highlight span.linenos{pointer-events:none;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight .hll{display:block;margin-left:-.875rem;margin-right:-.875rem;padding-left:.875rem;padding-right:.875rem}.code-block-caption{background-color:var(--color-code-background);border-bottom:1px solid;border-radius:.25rem;border-bottom-left-radius:0;border-bottom-right-radius:0;border-color:var(--color-background-border);color:var(--color-code-foreground);display:flex;font-weight:300;padding:.625rem .875rem}.code-block-caption+div[class]{margin-top:0}.code-block-caption+div[class] pre{border-top-left-radius:0;border-top-right-radius:0}.highlighttable{display:block;width:100%}.highlighttable tbody{display:block}.highlighttable tr{display:flex}.highlighttable td.linenos{background-color:var(--color-code-background);border-bottom-left-radius:.2rem;border-top-left-radius:.2rem;color:var(--color-code-foreground);padding:.625rem 0 .625rem .875rem}.highlighttable .linenodiv{box-shadow:-.0625rem 0 var(--color-foreground-border) inset;font-size:var(--code-font-size);padding-right:.875rem}.highlighttable td.code{display:block;flex:1;overflow:hidden;padding:0}.highlighttable td.code .highlight{border-bottom-left-radius:0;border-top-left-radius:0}.highlight span.linenos{box-shadow:-.0625rem 0 var(--color-foreground-border) inset;display:inline-block;margin-right:.875rem;padding-left:0;padding-right:.875rem}.footnote-reference{font-size:var(--font-size--small--4);vertical-align:super}dl.footnote.brackets{color:var(--color-foreground-secondary);display:grid;font-size:var(--font-size--small);grid-template-columns:-webkit-max-content auto;grid-template-columns:max-content auto}dl.footnote.brackets dt{margin:0}dl.footnote.brackets dt>.fn-backref{margin-left:.25rem}dl.footnote.brackets dt:after{content:":"}dl.footnote.brackets dt .brackets:before{content:"["}dl.footnote.brackets dt .brackets:after{content:"]"}dl.footnote.brackets dd{margin:0;padding:0 1rem}aside.footnote{color:var(--color-foreground-secondary);font-size:var(--font-size--small)}aside.footnote>span,div.citation>span{float:left;font-weight:500;padding-right:.25rem}aside.footnote>p,div.citation>p{margin-left:2rem}img{box-sizing:border-box;height:auto;max-width:100%}article .figure,article figure{border-radius:.2rem;margin:0}article .figure :last-child,article figure :last-child{margin-bottom:0}article .align-left{clear:left;float:left;margin:0 1rem 1rem}article .align-right{clear:right;float:right;margin:0 1rem 1rem}article .align-center,article .align-default{display:block;margin-left:auto;margin-right:auto;text-align:center}article table.align-default{display:table;text-align:initial}.domainindex-jumpbox,.genindex-jumpbox{border-bottom:1px solid var(--color-background-border);border-top:1px solid var(--color-background-border);padding:.25rem}.domainindex-section h2,.genindex-section h2{margin-bottom:.5rem;margin-top:.75rem}.domainindex-section ul,.genindex-section ul{margin-bottom:0;margin-top:0}ol,ul{margin-bottom:1rem;margin-top:1rem;padding-left:1.2rem}ol li>p:first-child,ul li>p:first-child{margin-bottom:.25rem;margin-top:.25rem}ol li>p:last-child,ul li>p:last-child{margin-top:.25rem}ol li>ol,ol li>ul,ul li>ol,ul li>ul{margin-bottom:.5rem;margin-top:.5rem}ol.arabic{list-style:decimal}ol.loweralpha{list-style:lower-alpha}ol.upperalpha{list-style:upper-alpha}ol.lowerroman{list-style:lower-roman}ol.upperroman{list-style:upper-roman}.simple li>ol,.simple li>ul,.toctree-wrapper li>ol,.toctree-wrapper li>ul{margin-bottom:0;margin-top:0}.field-list dt,.option-list dt,dl.footnote dt,dl.glossary dt,dl.simple dt,dl:not([class]) dt{font-weight:500;margin-top:.25rem}.field-list dt+dt,.option-list dt+dt,dl.footnote dt+dt,dl.glossary dt+dt,dl.simple dt+dt,dl:not([class]) dt+dt{margin-top:0}.field-list dt .classifier:before,.option-list dt .classifier:before,dl.footnote dt .classifier:before,dl.glossary dt .classifier:before,dl.simple dt .classifier:before,dl:not([class]) dt .classifier:before{content:":";margin-left:.2rem;margin-right:.2rem}.field-list dd ul,.field-list dd>p:first-child,.option-list dd ul,.option-list dd>p:first-child,dl.footnote dd ul,dl.footnote dd>p:first-child,dl.glossary dd ul,dl.glossary dd>p:first-child,dl.simple dd ul,dl.simple dd>p:first-child,dl:not([class]) dd ul,dl:not([class]) dd>p:first-child{margin-top:.125rem}.field-list dd ul,.option-list dd ul,dl.footnote dd ul,dl.glossary dd ul,dl.simple dd ul,dl:not([class]) dd ul{margin-bottom:.125rem}.math-wrapper{overflow-x:auto;width:100%}div.math{position:relative;text-align:center}div.math .headerlink,div.math:focus .headerlink{display:none}div.math:hover .headerlink{display:inline-block}div.math span.eqno{position:absolute;right:.5rem;top:50%;transform:translateY(-50%);z-index:1}abbr[title]{cursor:help}.problematic{color:var(--color-problematic)}kbd:not(.compound){background-color:var(--color-background-secondary);border:1px solid var(--color-foreground-border);border-radius:.2rem;box-shadow:0 .0625rem 0 rgba(0,0,0,.2),inset 0 0 0 .125rem var(--color-background-primary);color:var(--color-foreground-primary);display:inline-block;font-size:var(--font-size--small--3);margin:0 .2rem;padding:0 .2rem;vertical-align:text-bottom}blockquote{background:var(--color-background-secondary);border-left:4px solid var(--color-background-border);margin-left:0;margin-right:0;padding:.5rem 1rem}blockquote .attribution{font-weight:600;text-align:right}blockquote.highlights,blockquote.pull-quote{font-size:1.25em}blockquote.epigraph,blockquote.pull-quote{border-left-width:0;border-radius:.5rem}blockquote.highlights{background:transparent;border-left-width:0}p .reference img{vertical-align:middle}p.rubric{font-size:1.125em;font-weight:700;line-height:1.25}dd p.rubric{font-size:var(--font-size--small);font-weight:inherit;line-height:inherit;text-transform:uppercase}article .sidebar{background-color:var(--color-background-secondary);border:1px solid var(--color-background-border);border-radius:.2rem;clear:right;float:right;margin-left:1rem;margin-right:0;width:30%}article .sidebar>*{padding-left:1rem;padding-right:1rem}article .sidebar>ol,article .sidebar>ul{padding-left:2.2rem}article .sidebar .sidebar-title{border-bottom:1px solid var(--color-background-border);font-weight:500;margin:0;padding:.5rem 1rem}.table-wrapper{margin-bottom:.5rem;margin-top:1rem;overflow-x:auto;padding:.2rem .2rem .75rem;width:100%}table.docutils{border-collapse:collapse;border-radius:.2rem;border-spacing:0;box-shadow:0 .2rem .5rem rgba(0,0,0,.05),0 0 .0625rem rgba(0,0,0,.1)}table.docutils th{background:var(--color-table-header-background)}table.docutils td,table.docutils th{border-bottom:1px solid var(--color-table-border);border-left:1px solid var(--color-table-border);border-right:1px solid var(--color-table-border);padding:0 .25rem}table.docutils td p,table.docutils th p{margin:.25rem}table.docutils td:first-child,table.docutils th:first-child{border-left:none}table.docutils td:last-child,table.docutils th:last-child{border-right:none}table.docutils td.text-left,table.docutils th.text-left{text-align:left}table.docutils td.text-right,table.docutils th.text-right{text-align:right}table.docutils td.text-center,table.docutils th.text-center{text-align:center}:target{scroll-margin-top:.5rem}@media(max-width:67em){:target{scroll-margin-top:calc(.5rem + var(--header-height))}section>span:target{scroll-margin-top:calc(.8rem + var(--header-height))}}.headerlink{font-weight:100;-webkit-user-select:none;-moz-user-select:none;user-select:none}.code-block-caption>.headerlink,dl dt>.headerlink,figcaption p>.headerlink,h1>.headerlink,h2>.headerlink,h3>.headerlink,h4>.headerlink,h5>.headerlink,h6>.headerlink,p.caption>.headerlink,table>caption>.headerlink{margin-left:.5rem;visibility:hidden}.code-block-caption:hover>.headerlink,dl dt:hover>.headerlink,figcaption p:hover>.headerlink,h1:hover>.headerlink,h2:hover>.headerlink,h3:hover>.headerlink,h4:hover>.headerlink,h5:hover>.headerlink,h6:hover>.headerlink,p.caption:hover>.headerlink,table>caption:hover>.headerlink{visibility:visible}.code-block-caption>.toc-backref,dl dt>.toc-backref,figcaption p>.toc-backref,h1>.toc-backref,h2>.toc-backref,h3>.toc-backref,h4>.toc-backref,h5>.toc-backref,h6>.toc-backref,p.caption>.toc-backref,table>caption>.toc-backref{color:inherit;-webkit-text-decoration-line:none;text-decoration-line:none}figure:hover>figcaption>p>.headerlink,table:hover>caption>.headerlink{visibility:visible}:target>h1:first-of-type,:target>h2:first-of-type,:target>h3:first-of-type,:target>h4:first-of-type,:target>h5:first-of-type,:target>h6:first-of-type,span:target~h1:first-of-type,span:target~h2:first-of-type,span:target~h3:first-of-type,span:target~h4:first-of-type,span:target~h5:first-of-type,span:target~h6:first-of-type{background-color:var(--color-highlight-on-target)}:target>h1:first-of-type code.literal,:target>h2:first-of-type code.literal,:target>h3:first-of-type code.literal,:target>h4:first-of-type code.literal,:target>h5:first-of-type code.literal,:target>h6:first-of-type code.literal,span:target~h1:first-of-type code.literal,span:target~h2:first-of-type code.literal,span:target~h3:first-of-type code.literal,span:target~h4:first-of-type code.literal,span:target~h5:first-of-type code.literal,span:target~h6:first-of-type code.literal{background-color:transparent}.literal-block-wrapper:target .code-block-caption,.this-will-duplicate-information-and-it-is-still-useful-here li :target,figure:target,table:target>caption{background-color:var(--color-highlight-on-target)}dt:target{background-color:var(--color-highlight-on-target)!important}.footnote-reference:target,.footnote>dt:target+dd{background-color:var(--color-highlight-on-target)}.guilabel{background-color:var(--color-guilabel-background);border:1px solid var(--color-guilabel-border);border-radius:.5em;color:var(--color-guilabel-text);font-size:.9em;padding:0 .3em}footer{display:flex;flex-direction:column;font-size:var(--font-size--small);margin-top:2rem}.bottom-of-page{align-items:center;border-top:1px solid var(--color-background-border);color:var(--color-foreground-secondary);display:flex;justify-content:space-between;line-height:1.5;margin-top:1rem;padding-bottom:1rem;padding-top:1rem}@media(max-width:46em){.bottom-of-page{flex-direction:column-reverse;gap:.25rem;text-align:center}}.bottom-of-page .left-details{font-size:var(--font-size--small)}.bottom-of-page .right-details{display:flex;flex-direction:column;gap:.25rem;text-align:right}.bottom-of-page .icons{display:flex;font-size:1rem;gap:.25rem;justify-content:flex-end}.bottom-of-page .icons a{text-decoration:none}.bottom-of-page .icons img,.bottom-of-page .icons svg{font-size:1.125rem;height:1em;width:1em}.related-pages a{align-items:center;display:flex;text-decoration:none}.related-pages a:hover .page-info .title{color:var(--color-link);text-decoration:underline;-webkit-text-decoration-color:var(--color-link-underline);text-decoration-color:var(--color-link-underline)}.related-pages a svg.furo-related-icon,.related-pages a svg.furo-related-icon>use{color:var(--color-foreground-border);flex-shrink:0;height:.75rem;margin:0 .5rem;width:.75rem}.related-pages a.next-page{clear:right;float:right;max-width:50%;text-align:right}.related-pages a.prev-page{clear:left;float:left;max-width:50%}.related-pages a.prev-page svg{transform:rotate(180deg)}.page-info{display:flex;flex-direction:column;overflow-wrap:anywhere}.next-page .page-info{align-items:flex-end}.page-info .context{align-items:center;color:var(--color-foreground-muted);display:flex;font-size:var(--font-size--small);padding-bottom:.1rem;text-decoration:none}ul.search{list-style:none;padding-left:0}ul.search li{border-bottom:1px solid var(--color-background-border);padding:1rem 0}[role=main] .highlighted{background-color:var(--color-highlighted-background);color:var(--color-highlighted-text)}.sidebar-brand{display:flex;flex-direction:column;flex-shrink:0;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal);text-decoration:none}.sidebar-brand-text{color:var(--color-sidebar-brand-text);font-size:1.5rem;overflow-wrap:break-word}.sidebar-brand-text,.sidebar-logo-container{margin:var(--sidebar-item-spacing-vertical) 0}.sidebar-logo{display:block;margin:0 auto;max-width:100%}.sidebar-search-container{align-items:center;background:var(--color-sidebar-search-background);display:flex;margin-top:var(--sidebar-search-space-above);position:relative}.sidebar-search-container:focus-within,.sidebar-search-container:hover{background:var(--color-sidebar-search-background--focus)}.sidebar-search-container:before{background-color:var(--color-sidebar-search-icon);content:"";height:var(--sidebar-search-icon-size);left:var(--sidebar-item-spacing-horizontal);-webkit-mask-image:var(--icon-search);mask-image:var(--icon-search);position:absolute;width:var(--sidebar-search-icon-size)}.sidebar-search{background:transparent;border:none;border-bottom:1px solid var(--color-sidebar-search-border);border-top:1px solid var(--color-sidebar-search-border);box-sizing:border-box;color:var(--color-sidebar-search-foreground);padding:var(--sidebar-search-input-spacing-vertical) var(--sidebar-search-input-spacing-horizontal) var(--sidebar-search-input-spacing-vertical) calc(var(--sidebar-item-spacing-horizontal) + var(--sidebar-search-input-spacing-horizontal) + var(--sidebar-search-icon-size));width:100%;z-index:10}.sidebar-search:focus{outline:none}.sidebar-search::-moz-placeholder{font-size:var(--sidebar-search-input-font-size)}.sidebar-search::placeholder{font-size:var(--sidebar-search-input-font-size)}#searchbox .highlight-link{margin:0;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal) 0;text-align:center}#searchbox .highlight-link a{color:var(--color-sidebar-search-icon);font-size:var(--font-size--small--2)}.sidebar-tree{font-size:var(--sidebar-item-font-size);margin-bottom:var(--sidebar-item-spacing-vertical);margin-top:var(--sidebar-tree-space-above)}.sidebar-tree ul{display:flex;flex-direction:column;list-style:none;margin-bottom:0;margin-top:0;padding:0}.sidebar-tree li{margin:0;position:relative}.sidebar-tree li>ul{margin-left:var(--sidebar-item-spacing-horizontal)}.sidebar-tree .icon,.sidebar-tree .reference{color:var(--color-sidebar-link-text)}.sidebar-tree .reference{box-sizing:border-box;display:inline-block;height:100%;line-height:var(--sidebar-item-line-height);overflow-wrap:anywhere;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal);text-decoration:none;width:100%}.sidebar-tree .reference:hover{background:var(--color-sidebar-item-background--hover)}.sidebar-tree .reference.external:after{color:var(--color-sidebar-link-text);content:url("data:image/svg+xml;charset=utf-8,%3Csvg width='12' height='12' xmlns='http://www.w3.org/2000/svg' viewBox='0 0 24 24' stroke-width='1.5' stroke='%23607D8B' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M0 0h24v24H0z' stroke='none'/%3E%3Cpath d='M11 7H6a2 2 0 0 0-2 2v9a2 2 0 0 0 2 2h9a2 2 0 0 0 2-2v-5M10 14 20 4M15 4h5v5'/%3E%3C/svg%3E");margin:0 .25rem;vertical-align:middle}.sidebar-tree .current-page>.reference{font-weight:700}.sidebar-tree label{align-items:center;cursor:pointer;display:flex;height:var(--sidebar-item-height);justify-content:center;position:absolute;right:0;top:0;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:var(--sidebar-expander-width)}.sidebar-tree .caption,.sidebar-tree :not(.caption)>.caption-text{color:var(--color-sidebar-caption-text);font-size:var(--sidebar-caption-font-size);font-weight:700;margin:var(--sidebar-caption-space-above) 0 0 0;padding:var(--sidebar-item-spacing-vertical) var(--sidebar-item-spacing-horizontal);text-transform:uppercase}.sidebar-tree li.has-children>.reference{padding-right:var(--sidebar-expander-width)}.sidebar-tree .toctree-l1>.reference,.sidebar-tree .toctree-l1>label .icon{color:var(--color-sidebar-link-text--top-level)}.sidebar-tree label{background:var(--color-sidebar-item-expander-background)}.sidebar-tree label:hover{background:var(--color-sidebar-item-expander-background--hover)}.sidebar-tree .current>.reference{background:var(--color-sidebar-item-background--current)}.sidebar-tree .current>.reference:hover{background:var(--color-sidebar-item-background--hover)}.toctree-checkbox{display:none;position:absolute}.toctree-checkbox~ul{display:none}.toctree-checkbox~label .icon svg{transform:rotate(90deg)}.toctree-checkbox:checked~ul{display:block}.toctree-checkbox:checked~label .icon svg{transform:rotate(-90deg)}.toc-title-container{padding:var(--toc-title-padding);padding-top:var(--toc-spacing-vertical)}.toc-title{color:var(--color-toc-title-text);font-size:var(--toc-title-font-size);padding-left:var(--toc-spacing-horizontal);text-transform:uppercase}.no-toc{display:none}.toc-tree-container{padding-bottom:var(--toc-spacing-vertical)}.toc-tree{border-left:1px solid var(--color-background-border);font-size:var(--toc-font-size);line-height:1.3;padding-left:calc(var(--toc-spacing-horizontal) - var(--toc-item-spacing-horizontal))}.toc-tree>ul>li:first-child{padding-top:0}.toc-tree>ul>li:first-child>ul{padding-left:0}.toc-tree>ul>li:first-child>a{display:none}.toc-tree ul{list-style-type:none;margin-bottom:0;margin-top:0;padding-left:var(--toc-item-spacing-horizontal)}.toc-tree li{padding-top:var(--toc-item-spacing-vertical)}.toc-tree li.scroll-current>.reference{color:var(--color-toc-item-text--active);font-weight:700}.toc-tree .reference{color:var(--color-toc-item-text);overflow-wrap:anywhere;text-decoration:none}.toc-scroll{max-height:100vh;overflow-y:scroll}.contents:not(.this-will-duplicate-information-and-it-is-still-useful-here){background:rgba(255,0,0,.25);color:var(--color-problematic)}.contents:not(.this-will-duplicate-information-and-it-is-still-useful-here):before{content:"ERROR: Adding a table of contents in Furo-based documentation is unnecessary, and does not work well with existing styling.Add a 'this-will-duplicate-information-and-it-is-still-useful-here' class, if you want an escape hatch."}.text-align\:left>p{text-align:left}.text-align\:center>p{text-align:center}.text-align\:right>p{text-align:right}
 /*# sourceMappingURL=furo.css.map*/
```

### Comparing `gmpacket-0.1.2/docs/_static/styles/furo.css.map` & `gmpacket-0.1.3/docs/_static/styles/furo.css.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9097744360902256%*

 * *Differences: {"'mappings'": "'AAAA,2EAA2E,CAU3E,KAEE,6BAA8B,CAD9B,gBAEF,CASA,KACE,QACF,CAMA,KACE,aACF,CAOA,GACE,aAAc,CACd,cACF,CAUA,GACE,sBAAuB,CACvB,QAAS,CACT,gBACF,CAOA,IACE,+BAAiC,CACjC,aACF,CASA,EACE,4BACF,CAOA,YACE,kBAAmB,CACnB,yBAA0B,CAC1B,gCACF,CAMA,SAEE,kBACF,CAOA,cAGE,+BAAiC,CACjC,aACF,CAeA,QAEE,aAAc,CACd,aAAc,CACd,iBAAkB,CAClB,uBACF,CAEA,IACE,aACF,CAEA,IACE,SACF,CASA,IACE,iBACF,CAUA,sCAKE,mBAAoB,CACpB,cAAe,CACf,gBAAiB,CACjB,QACF,CAOA,aAEE,gBACF,CAOA,cAEE,mBACF,CAMA,gDAIE,yBACF,CAMA,wHAIE,iBAAkB,CAClB,SACF,CAMA […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "styles/furo.css",
-    "mappings": "AAAA,2EAA2E,CAU3E,KAEE,6BAA8B,CAD9B,gBAEF,CASA,KACE,QACF,CAMA,KACE,aACF,CAOA,GACE,aAAc,CACd,cACF,CAUA,GACE,sBAAuB,CACvB,QAAS,CACT,gBACF,CAOA,IACE,+BAAiC,CACjC,aACF,CASA,EACE,4BACF,CAOA,YACE,kBAAmB,CACnB,yBAA0B,CAC1B,gCACF,CAMA,SAEE,kBACF,CAOA,cAGE,+BAAiC,CACjC,aACF,CAeA,QAEE,aAAc,CACd,aAAc,CACd,iBAAkB,CAClB,uBACF,CAEA,IACE,aACF,CAEA,IACE,SACF,CASA,IACE,iBACF,CAUA,sCAKE,mBAAoB,CACpB,cAAe,CACf,gBAAiB,CACjB,QACF,CAOA,aAEE,gBACF,CAOA,cAEE,mBACF,CAMA,gDAIE,yBACF,CAMA,wHAIE,iBAAkB,CAClB,SACF,CAMA,4GAIE,6BACF,CAMA,SACE,0BACF,CASA,OACE,qBAAsB,CACtB,aAAc,CACd,aAAc,CACd,cAAe,CACf,SAAU,CACV,kBACF,CAMA,SACE,uBACF,CAMA,SACE,aACF,CAOA,6BAEE,qBAAsB,CACtB,SACF,CAMA,kFAEE,WACF,CAOA,cACE,4BAA6B,CAC7B,mBACF,CAMA,yCACE,uBACF,CAOA,6BACE,yBAA0B,CAC1B,YACF,CASA,QACE,aACF,CAMA,QACE,iBACF,CAiBA,kBACE,YACF,CCvVA,aAcE,kEACE,uBAOF,WACE,iDAMF,gCACE,wBAEF,qCAEE,uBADA,uBACA,CAEF,SACE,wBAtBA,CCpBJ,iBAOE,6BAEA,mBANA,qBAEA,sBACA,0BAFA,oBAHA,4BAOA,6BANA,mBAOA,CAEF,gBACE,aCPF,KCGE,mHAEA,wGAGA,wBAAyB,CACzB,wBAAyB,CACzB,4BAA6B,CAC7B,yBAA0B,CAC1B,2BAA4B,CAG5B,sDAAuD,CACvD,gDAAiD,CACjD,wDAAyD,CAGzD,0CAA2C,CAC3C,gDAAiD,CACjD,gDAAiD,CAKjD,gCAAiC,CACjC,sCAAuC,CAGvC,2CAA4C,CAG5C,uCAAwC,CChCxC,+FAGA,uBAAwB,CAGxB,iCAAkC,CAClC,kCAAmC,CAEnC,+BAAgC,CAChC,sCAAuC,CACvC,sCAAuC,CACvC,qGAIA,mDAAoD,CAEpD,mCAAoC,CACpC,8CAA+C,CAC/C,gDAAiD,CACjD,kCAAmC,CACnC,6DAA8D,CAG9D,6BAA8B,CAC9B,6BAA8B,CAC9B,+BAAgC,CAChC,kCAAmC,CACnC,kCAAmC,CCPjC,ukBCYA,srCAZF,kaCVA,mLAOA,oTAWA,2UAaA,0CACA,gEACA,0CAGA,gEAUA,yCACA,+DAIA,4CACA,kEAGA,sGAEA,mGAGA,sCACA,2DAEA,4CACA,kEACA,uCACA,6DAEA,2GACA,+CAGA,+MAOA,4BACA,2FAIA,4DACA,sEACA,kEACA,sEACA,gDAGA,kCACA,uEACA,mCACA,4DACA,yDAGA,2DACA,qDAGA,0CACA,8CACA,oDACA,oDL7GF,iCAEA,iEAME,oCKyGA,yDAIA,sCACA,kCACA,sDAGA,0CACA,kEACA,oDAEA,sDAGA,oCACA,oEAIA,CAGA,yDAGA,qDACA,oDAGA,6DAIA,iEAGA,2DAEA,2DL9IE,4DAEA,gEAIF,gEKgGA,gFAIA,oNAOA,qDAEA,gFAIA,4DAIA,oEAMA,yEAIA,6DACA,0DAGA,uDAGA,qDAEA,wDLpII,6DAEA,yDACE,2DAMN,uCAIA,yCACE,8CAGF,sDMjDA,6DAKA,oCAIA,4CACA,kBAGF,sBAMA,2BAME,qCAGA,qCAEA,iCAEA,+BAEA,mCAEA,qCAIA,CACA,gCACA,gDAKA,kCAIA,6BAEA,0CAQA,kCAIF,8BAGE,8BACA,uCAGF,sCAKE,kCAEA,sDACA,uEAGE,sDACA,gGACF,wCAGI,sBACA,yHCzEJ,2BACA,qCAGF,sEAGE,kEAGA,sHAGA,2IACE,8BACA,8BAOF,uCAEA,wEAGA,sDACA,iCAKA,CAEF,qCAEE,sDACA,gCACA,gEAKA,+CAOE,sBACA,gEAGA,GAYF,yLACA,gDAGA,mBAEA,wCACA,wCAGF,CAEE,iCAGF,wBACE,mBAIF,oBAFE,eAEF,CAJE,gBAEA,CAMA,mBACA,mBAGA,mDAIA,YACA,mBAEA,CACA,kBAGF,OAJE,kBAQA,CAJF,GACE,aAGA,IACA,mCACA,qBAEF,IACE,oBAEA,aACA,CAFA,WAEA,GAEE,oBAKJ,CAPE,gBAOF,aACE,+CAGA,UAHA,kCAGA,4BACA,GAEA,uBACA,CAHA,yBAEA,CACA,yDAGF,kDAEE,SACA,8BAEA,iEAGE,yDACA,sEAEA,iEAEE,yHAKN,kDAMA,0DAIE,CANA,oBAMA,0GAOA,aAEF,CAHE,YAGF,4HAWE,+CACE,iCAIJ,0CAGE,CALE,qCAEJ,CAHI,WAMF,SAIA,0CAIA,CANF,qCAME,mBACA,gBACA,gBAIA,+CAEE,CAIF,kDAGF,CAPI,8BAGJ,CAKE,YACF,CAbE,2BAEA,CAHA,WAYF,UAEA,yBACE,kBAIA,iEAKA,iCAGA,mDAEA,mBACF,OACE,iBAQA,0CAIA,CAPA,6DAGA,CALF,qBAEE,CAOA,qCAEE,CAGA,eAHA,sBAGA,gCAKF,qBACE,WACA,aACA,sCAEA,mBAOJ,6BASE,kCACA,CAHA,sBACA,aACA,CARA,uBAGA,gBAEA,MAIA,6BAEA,yBACA,2DAEA,sBAGA,8BACA,CANA,wBAMA,2BAEE,YACA,sBACA,WAEF,CAFE,UAEF,eAeF,kBAEE,CAhBE,qDAGA,qCAOJ,CAEI,YAEJ,CAJA,2BAEI,CAIF,eACE,qBACF,4CAIE,uBACA,sBACF,cACE,CAFA,aACF,CAEE,kBADA,kBACA,yBAGF,oCACE,6DAMF,qDAGE,CC1VY,8BDgWd,oCAEA,uDAEA,CACE,8CAIA,gCAEA,YACA,8CACA,CAEA,oCAGE,CAHF,oCAGE,mBAEA,mDADA,YADA,qBACA,WACA,sBAEE,WACA,uDAGN,cACE,CAJI,YAIJ,iDAIA,uCAIA,uBACA,oCAGA,kBAEJ,CAHI,sBAGJ,mBAEE,aACE,CACA,qCAGF,YACE,CAFJ,WACE,CAME,SE3ZJ,CF0ZI,kBACA,CAHF,gBACE,CAHA,iBEtZJ,6CAEE,yBAEA,4BAEA,aAFA,iBAGA,wEAEA,UAMA,gCAIA,CARA,SAIA,UANA,qBAEA,qDAIA,CANA,OAUA,0CACE,UAEJ,iDAEE,CAFF,UAEE,aACA,iCAEA,CAFA,UAEA,wCAIA,sBADA,UACA,6CAIA,yCAEE,qBACA,CAFA,UAEA,kCAKJ,OACE,CADF,KACE,cAGE,2CADA,kBACC,CAAD,wEAGJ,CANE,aAGE,mBAFF,OAMA,gBALE,iCAFF,cACA,CADA,qBACA,SAMA,2BADF,UACE,kBAEE,sCACA,CAFF,WACE,WACA,qEACA,mBADA,YACA,6BAKJ,cACE,uDAGE,aACE,mDAEE,CAFF,6CAEE,kEACA,yCACE,uDACA,8BANN,WAMM,oBANN,CAMM,UANN,kBACE,qDACA,kCACE,6BAEE,mBADF,0CACE,CAFF,uCACA,MACE,0DACA,wCANN,gCACE,sEACA,WACE,gEACA,CADA,UACA,+CACE,oDACA,6DANN,kCACE,kCACA,gBADA,UACA,yBACE,wDACA,cADA,UACA,qBACE,6CACA,yFALJ,sCACA,CAEE,gBACE,CAHJ,gBAGI,sBAHJ,uBACE,4DACA,4CACE,iDAJJ,2CACA,CADA,gBAEE,gBAGE,sBALJ,+BAII,iBAFF,gDACA,WACE,YADF,uCACE,6EACA,2BANN,8CACE,kDACA,0CACE,8BACA,yFACE,sBACA,sFALJ,mEACA,sBACE,kEACA,6EACE,uCACA,kEALJ,qGAEE,kEACA,6EACE,uCACA,kEALJ,8CACA,uDACE,sEACA,2EACE,sCACA,iEALJ,mGACA,qCACE,oDACA,0DACE,6GACA,gDAGR,yDCpEA,sEACE,CACA,6GACE,gEACF,iGAIF,wFACE,qDAGA,mGAEE,2CAEF,4FACE,gCACF,wGACE,8DAEE,6FAIA,iJAKN,6GACE,gDAKF,yDACA,qCAGA,6BACA,kBAGA,qDAKA,oCAEA,+DACE,2CAIA,oDAKF,sCACE,8BAGF,qBACA,wDAGA,uCAEA,kEAGA,8CAEA,uDAKA,gEAEE,6BAGJ,gEC5FE,+CAEA,0ECFF,sDAGE,+DAKA,qEACE,mCACA,wBAEA,4FAKA,gBCjBJ,yGAIE,kBACA,CAMA,2MAYA,4HAUE,iCAEF,CAHA,wBAGA,8GAQE,mBACA,2GAOJ,mBACE,CACA,4HAKE,+IAWJ,eAEE,CAFF,YAEE,4FAIA,8BAEA,uBASI,sCACA,CAFF,oBACE,CANJ,wCACA,CAFA,8BACA,CADA,gBAIA,+BAEE,mBAEE,6BAIJ,4CAGE,kDAMF,gBACE,kEACA,8BACA,yBAEA,8BACA,sCAEF,cACE,+BACA,CAFF,eAEE,YACA,2EAGF,iBACE,CACA,yDAKE,sBADF,kBAEE,+BAIJ,4BACE,aAEA,qBAFA,gBAhHsB,CAmHtB,wBACA,mGClIF,iCAKF,mBACE,0FAIA,iDACA,CADA,2CACA,8BAEE,6BACE,yBAEF,8CAIE,wDAEA,gDAGJ,+CAKF,aACE,wCACA,kDAEF,YAEE,CAFF,YAEE,CClCA,qGACA,mCAIA,gBACE,iCAGA,gCACE,aAEJ,CAHE,uBAGF,mBAKA,6CAGE,CALA,mBAEF,CAGE,kCAEF,CARE,kBACA,CAFA,eASF,YAEE,mBACA,CAHF,UAGE,wCC7BJ,oBDkCE,8CAEE,iBCpCJ,iBACE,wDACA,gEASE,6CCLF,CDIE,uBACA,CALF,oBACE,4BAEF,8BCAE,2CAEE,CALJ,kCAGE,CDHF,aAGA,eACE,CAJF,uBCKI,gCAEF,gDAGA,kDAGE,iBAIF,cADF,UACE,uBAEA,iCAEA,wCAEA,6CAEA,CASE,+BASJ,CAZE,4BAGE,CATF,kCAMA,kCAYF,4BACE,2DAEA,CAHF,+BACE,CADF,qBAGE,2GAGA,wIAEE,CAFF,8EAEE,qBACA,oCAGF,6RAIA,sGACE,oDChEJ,WAEF,yBACE,QACA,eAEA,gBAEE,uCAGA,CALF,iCAKE,uCAGA,0BACA,CACA,oBACA,iCClBJ,gBACE,KAGF,qBACE,YAGF,CAHE,cAGF,gCAEE,mBACA,iEAEA,oCACA,wCAEA,sBACA,WAEA,CAFA,YAEA,8EAEA,mCAFA,iBAEA,6BAIA,wEAKA,sDAIE,CARF,mDAIA,CAIE,cAEF,8CAIA,oBAFE,iBAEF,8CAGE,eAEF,CAFE,YAEF,OAEE,kBAGJ,CAJI,eACA,CAFF,mBAKF,yCCjDE,oBACA,CAFA,iBAEA,uCAKE,iBACA,qCAGA,mBCZJ,CDWI,gBCXJ,6BAEE,eACA,sBAGA,eAEA,sBACA,oDACA,iGAMA,gBAFE,YAEF,8FAME,iJClBF,YACA,gNAUE,6BAEF,oTAcI,kBACF,gHAIA,qBACE,eACF,qDACE,kBACF,6DACE,4BCxCJ,oBAEF,qCAEI,+CAGF,uBACE,uDAGJ,oBAkBE,mDAhBA,+CAaA,CAbA,oBAaA,0FAEE,CAFF,gGAbA,+BAaA,0BAGA,mQAIA,oNAEE,kCADA,gBACA,aAGJ,sDAHI,mBAGJ,yBAYI,+VACE,sDAGA,iBAHA,2BAGA,kWAGN,iDAEE,CALI,gGAGN,CAHM,gBAKJ,yCAGF,0EACE,2EAGF,iBACE,yDAOA,0EAGF,6EAEE,iBC/EA,wDACA,4DACA,qBAEA,oDCDA,6BACA,yBACA,sBAEA,iBAGF,sNAYE,iBAEA,kBAdF,wRA8BI,kBACA,iOAkBA,aACA,4DACE,uEAEA,uVAoBA,iDAKA,ieC1EJ,4BACA,CCFF,6JAEE,iDACA,sEAIA,mDAGA,iDAOF,4DAGE,8CAEA,CAEA,kBACA,CAHA,gCAEA,CACA,eADA,cACA,oBAEE,uBAFF,kCAEE,gCAEF,kBACE,CAIA,mDAEA,CAHA,uCACA,CALF,aACE,6BAEA,CAIA,gBAJA,mCACA,CADA,gBAIA,wBACA,6CAGF,YAHE,iBAGF,gCAGA,iEACA,6CAEA,qDACA,6EACA,2EACA,8GAEA,yCAGA,uBACA,CAFA,yBACA,CACA,yDAKA,kDACE,mFAKJ,oCACE,CANE,aAKJ,CACE,qEAIA,YAFA,WAEA,CAHA,aACA,CAEA,gBACE,4BACA,sBADA,aACA,gCAMF,oCACA,yDACA,2CAEA,qBAGE,kBAEA,CACA,mCAIF,CARE,YACA,CAOF,iCAEE,CAPA,oBACA,CAQA,oBACE,uDAEJ,sDAGA,CAHA,cAGA,0BACE,oDAIA,oCACA,4BACA,sBAGA,cAEA,oFAGA,sBAEA,yDACE,CAIA,iBAJA,wBAIA,6CAJA,6CAOA,4BAGJ,CAHI,cAGJ,yCAGA,kBACE,CAIA,iDAEA,CATA,YAEF,CACE,4CAGA,kBAIA,wEAEA,wDAIF,kCAOE,iDACA,CARF,WAIE,sCAGA,CANA,2CACA,CAMA,oEARF,iBACE,CACA,qCAMA,iBAuBE,uBAlBF,YAKA,2DALA,uDAKA,CALA,sBAiBA,4CACE,CALA,gRAIF,YACE,UAEN,uBACE,YACA,mCAOE,+CAGA,8BAGF,+CAGA,4BCjNA,SDiNA,qFCjNA,gDAGA,sCACA,qCACA,sDAIF,CAIE,kDAGA,CAPF,0CAOE,kBAEA,kDAEA,CAHA,eACA,CAFA,YACA,CADA,SAIA,mHAIE,CAGA,6CAFA,oCAeE,CAbF,yBACE,qBAEJ,CAGE,oBACA,CAEA,YAFA,2CACF,CACE,uBAEA,mFAEE,CALJ,oBACE,CAEA,UAEE,gCAGF,sDAEA,yCC7CJ,oCAGA,CD6CE,yXAQE,sCCrDJ,wCAGA,oCACE",
+    "mappings": "AAAA,2EAA2E,CAU3E,KAEE,6BAA8B,CAD9B,gBAEF,CASA,KACE,QACF,CAMA,KACE,aACF,CAOA,GACE,aAAc,CACd,cACF,CAUA,GACE,sBAAuB,CACvB,QAAS,CACT,gBACF,CAOA,IACE,+BAAiC,CACjC,aACF,CASA,EACE,4BACF,CAOA,YACE,kBAAmB,CACnB,yBAA0B,CAC1B,gCACF,CAMA,SAEE,kBACF,CAOA,cAGE,+BAAiC,CACjC,aACF,CAeA,QAEE,aAAc,CACd,aAAc,CACd,iBAAkB,CAClB,uBACF,CAEA,IACE,aACF,CAEA,IACE,SACF,CASA,IACE,iBACF,CAUA,sCAKE,mBAAoB,CACpB,cAAe,CACf,gBAAiB,CACjB,QACF,CAOA,aAEE,gBACF,CAOA,cAEE,mBACF,CAMA,gDAIE,yBACF,CAMA,wHAIE,iBAAkB,CAClB,SACF,CAMA,4GAIE,6BACF,CAMA,SACE,0BACF,CASA,OACE,qBAAsB,CACtB,aAAc,CACd,aAAc,CACd,cAAe,CACf,SAAU,CACV,kBACF,CAMA,SACE,uBACF,CAMA,SACE,aACF,CAOA,6BAEE,qBAAsB,CACtB,SACF,CAMA,kFAEE,WACF,CAOA,cACE,4BAA6B,CAC7B,mBACF,CAMA,yCACE,uBACF,CAOA,6BACE,yBAA0B,CAC1B,YACF,CASA,QACE,aACF,CAMA,QACE,iBACF,CAiBA,kBACE,YACF,CCvVA,aAcE,kEACE,uBAOF,WACE,iDAMF,gCACE,wBAEF,qCAEE,uBADA,uBACA,CAEF,SACE,wBAtBA,CCpBJ,iBAOE,6BAEA,mBANA,qBAEA,sBACA,0BAFA,oBAHA,4BAOA,6BANA,mBAOA,CAEF,gBACE,aCPF,KCGE,mHAEA,wGAGA,wBAAyB,CACzB,wBAAyB,CACzB,4BAA6B,CAC7B,yBAA0B,CAC1B,2BAA4B,CAG5B,sDAAuD,CACvD,gDAAiD,CACjD,wDAAyD,CAGzD,0CAA2C,CAC3C,gDAAiD,CACjD,gDAAiD,CAKjD,gCAAiC,CACjC,sCAAuC,CAGvC,2CAA4C,CAG5C,uCAAwC,CChCxC,+FAGA,uBAAwB,CAGxB,iCAAkC,CAClC,kCAAmC,CAEnC,+BAAgC,CAChC,sCAAuC,CACvC,sCAAuC,CACvC,qGAIA,mDAAoD,CAEpD,mCAAoC,CACpC,8CAA+C,CAC/C,gDAAiD,CACjD,kCAAmC,CACnC,6DAA8D,CAG9D,6BAA8B,CAC9B,6BAA8B,CAC9B,+BAAgC,CAChC,kCAAmC,CACnC,kCAAmC,CCPjC,ukBCYA,srCAZF,kaCVA,mLAOA,oTAWA,2UAaA,0CACA,gEACA,0CAGA,gEAUA,yCACA,+DAGA,4CACA,CACA,iEAGA,sGACA,uCACA,4DAGA,sCACA,2DAEA,4CACA,kEACA,oGACA,CAEA,0GACA,+CAGA,+MAOA,+EACA,wCAIA,4DACA,sEACA,kEACA,sEACA,gDAGA,+DACA,0CACA,gEACA,gGACA,CAGA,2DACA,qDAGA,0CACA,8CACA,oDACA,oDL7GF,iCAEA,iEAME,oCKyGA,yDAIA,sCACA,kCACA,sDAGA,0CACA,kEACA,oDAEA,sDAGA,oCACA,oEAIA,CAGA,yDAGA,qDACA,oDAGA,6DAIA,iEAGA,2DAEA,2DL9IE,4DAEA,gEAIF,gEKgGA,gFAIA,oNAOA,qDAEA,gFAIA,4DAIA,oEAMA,yEAIA,6DACA,0DAGA,uDAGA,qDAEA,wDLpII,6DAEA,yDACE,2DAMN,uCAIA,yCACE,8CAGF,sDMjDA,6DAKA,oCAIA,4CACA,kBAGF,sBAMA,2BAME,qCAGA,qCAEA,iCAEA,+BAEA,mCAEA,qCAIA,CACA,gCACA,gDAKA,kCAIA,6BAEA,0CAQA,kCAIF,8BAGE,8BACA,uCAGF,sCAKE,kCAEA,sDACA,uEAGE,sDACA,gGACF,wCAGI,sBACA,yHCzEJ,2BACA,qCAGF,sEAGE,kEAGA,sHAGA,2IACE,8BACA,8BAOF,uCAEA,wEAGA,sDACA,iCAKA,CAEF,qCAEE,sDACA,gCACA,gEAKA,+CAOE,sBACA,gEAGA,GAYF,yLACA,gDAGA,mBAEA,wCACA,wCAGF,CAEE,iCAGF,wBACE,mBAIF,oBAFE,eAEF,CAJE,gBAEA,CAMA,mBACA,mBAGA,mDAIA,YACA,mBAEA,CACA,kBAGF,OAJE,kBAQA,CAJF,GACE,aAGA,IACA,mCACA,qBAEF,IACE,oBAEA,aACA,CAFA,WAEA,GAEE,oBAKJ,CAPE,gBAOF,aACE,+CAGA,UAHA,kCAGA,4BACA,GAEA,uBACA,CAHA,yBAEA,CACA,yDAGF,kDAEE,SACA,8BAEA,iEAGE,yDACA,sEAEA,iEAEE,yHAKN,kDAMA,0DAIE,CANA,oBAMA,0GAOA,aAEF,CAHE,YAGF,4HAWE,+CACE,iCAIJ,0CAGE,CALE,qCAEJ,CAHI,WAMF,SAIA,0CAIA,CANF,qCAME,mBACA,gBACA,gBAIA,+CAEE,CAIF,kDAGF,CAPI,8BAGJ,CAKE,YACF,CAbE,2BAEA,CAHA,WAYF,UAEA,yBACE,kBAIA,iEAKA,iCAGA,mDAEA,mBACF,OACE,iBAQA,0CAIA,CAPA,6DAGA,CALF,qBAEE,CAOA,qCAEE,CAGA,eAHA,sBAGA,gCAKF,qBACE,WACA,aACA,sCAEA,mBAOJ,6BASE,kCACA,CAHA,sBACA,aACA,CARA,uBAGA,gBAEA,MAIA,6BAEA,yBACA,2DAEA,sBAGA,8BACA,CANA,wBAMA,2BAEE,YACA,sBACA,WAEF,CAFE,UAEF,eAeF,kBAEE,CAhBE,qDAGA,qCAOJ,CAEI,YAEJ,CAJA,2BAEI,CAIF,eACE,qBACF,4CAIE,uBACA,sBACF,cACE,CAFA,aACF,CAEE,kBADA,kBACA,yBAGF,oCACE,6DAMF,qDAGE,CC1VY,8BDgWd,oCAEA,uDAEA,CACE,8CAIA,gCAEA,YACA,8CACA,CAEA,oCAGE,CAHF,oCAGE,mBAEA,mDADA,YADA,qBACA,WACA,sBAEE,WACA,uDAEN,eAFM,YAEN,iDAGE,uCAIA,YAGF,+CAKE,kBACA,CALA,sBAKA,mBACF,aACE,aACA,yBAEJ,YAGI,CAHJ,YAOE,SACE,CAFJ,kBACE,CAHE,gBAEJ,CAHI,iBAKA,6CAIA,aACA,YEhaJ,4BAEE,aADA,iBACA,6BAEA,kCAEA,SACA,UAIA,gCACA,CALA,SAEA,SAEA,CAJA,0EAEA,CAFA,OAKA,CAGA,mDACE,iBAGF,gCACE,CADF,UACE,aAEJ,iCACE,CADF,UAEE,wCAEA,WACA,WAFA,UAEA,6CAIA,yCACA,WAGA,WAJA,UAIA,kCACE,OACA,CAFF,KAEE,cAQF,0CACE,CAFF,kBACA,CACE,wEACA,CARA,YACA,CAKF,mBAFF,OAII,eACA,CAJF,iCAJE,cAGJ,CANI,oBAEA,CAKF,SAIE,2BADA,UACA,kBAGF,sCACA,CAFF,WACE,WACA,qCACE,gCACA,2EACA,sDAKJ,aACE,mDAII,CAJJ,6CAII,kEACA,iBACE,iDACA,+CACE,aACA,WADA,+BACA,uEANN,YACE,mDAEE,kBACA,CADA,2CADF,uCACE,MACA,0DACE,yCACA,qGALJ,oCACA,uCACE,CAFF,UAEE,uEACA,+CACE,oDACA,6DANN,kCACE,kCACA,gBADA,UACA,yBACE,wDACA,cADA,UACA,qBACE,6CACA,yFALJ,sCACA,CAEE,gBACE,CAHJ,gBAGI,sBAHJ,uBACE,4DACA,4CACE,iDAJJ,2CACA,CADA,gBAEE,gBAGE,sBALJ,+BAII,iBAFF,gDACA,WACE,YADF,uCACE,6EACA,2BANN,8CACE,kDACA,0CACE,8BACA,yFACE,sBACA,sFALJ,mEACA,sBACE,kEACA,6EACE,uCACA,kEALJ,qGAEE,kEACA,6EACE,uCACA,kEALJ,8CACA,uDACE,sEACA,2EACE,sCACA,iEALJ,mGACA,qCACE,oDACA,0DACE,6GACA,gDAGR,yDCpEA,sEACE,CACA,6GACE,gEACF,iGAIF,wFACE,qDAGA,mGAEE,2CAEF,4FACE,gCACF,wGACE,8DAEE,6FAIA,iJAKN,6GACE,gDAKF,yDACA,qCAGA,6BACA,kBACA,qDAKA,oCAEA,+DAGA,2CAGE,oDAIA,oEAEE,qBAGJ,wDAIA,uCAEE,kEAEF,CACF,6CAEE,uDAEA,oCAIF,4BACE,6BAEA,gEAEE,+CAIF,0EC9FA,sDAGE,+DCLJ,sCAGE,8BAKA,wJAIE,gBACA,yGCZF,mBAQA,2MAIA,oBAOF,wGAKE,iCAEE,CAFF,wBAEE,8GAWF,mBAEE,2GAMA,mBAEA,6HAOF,YAGA,mIAOE,gBADA,YACA,4FAOF,8BACA,uBAYA,sCAEE,CAFF,qBARA,wCAEA,CAHA,8BACA,CAFA,eACA,CAGA,mBAEA,sBAEA,kDAEA,CAEE,kCACE,6BACA,4CAMJ,kDAGA,eAIA,6CACE,mCACA,0CACA,8BAEA,sCACA,cAEF,+BACE,CAHA,eAGA,YACA,4BACA,gEAGF,0DAME,sBAFA,kBAGE,+BACA,4BAIJ,aACE,oBACA,CAFF,gBAEE,yBAEA,eACA,CApHsB,YAmHtB,CACA,sECpIF,mDACA,2FAMA,iCAGA,0FAEE,eACA,CAFF,YAEE,0BACE,8CAEF,mBAIE,qCACE,CACF,yBADE,iBACF,8BAGJ,+CAKF,aACE,wCACA,kDAEF,YAEE,CAFF,YAEE,CClCA,mFDwCA,QCzCF,UAGE,CAFA,IACA,aACA,mCAGA,eACE,kCAGA,uDAGF,mBAKA,6CAGE,CALA,mBAEF,CAGE,kCAEF,CARE,kBACA,CAFA,eASF,YAEE,mBACA,CAHF,UAGE,wCC7BJ,oBDkCE,8CAEE,iBCpCJ,iBACE,wDACA,gEASE,6CCLF,CDIE,uBACA,CALF,oBACE,4BAEF,8BCAE,2CAEE,CALJ,kCAGE,CDHF,aAGA,eACE,CAJF,uBCKI,gCAEF,gDAGA,kDAGE,iBAIF,cADF,UACE,uBAEA,iCAEA,wCAEA,6CAEA,CASE,+BASJ,CAZE,4BAGE,CATF,kCAMA,kCAYF,4BACE,2DAEA,CAHF,+BACE,CADF,qBAGE,2GAGA,wIAEE,CAFF,8EAEE,qBACA,oCAGF,6RAIA,sGACE,oDChEJ,WAEF,yBACE,QACA,eAEA,gBAEE,uCAGA,CALF,iCAKE,uCAGA,0BACA,CACA,oBACA,iCClBJ,gBACE,KAGF,qBACE,YAGF,CAHE,cAGF,gCAEE,mBACA,iEAEA,oCACA,wCAEA,sBACA,WAEA,CAFA,YAEA,8EAEA,mCAFA,iBAEA,6BAIA,wEAKA,sDAIE,CARF,mDAIA,CAIE,cAEF,8CAIA,oBAFE,iBAEF,8CAGE,eAEF,CAFE,YAEF,OAEE,kBAGJ,CAJI,eACA,CAFF,mBAKF,yCCjDE,oBACA,CAFA,iBAEA,uCAKE,iBACA,qCAGA,mBCZJ,CDWI,gBCXJ,6BAEE,eACA,sBAGA,eAEA,sBACA,oDACA,iGAMA,gBAFE,YAEF,8FAME,iJClBF,YACA,gNAUE,6BAEF,oTAcI,kBACF,gHAIA,qBACE,eACF,qDACE,kBACF,6DACE,4BCxCJ,oBAEF,qCAEI,+CAGF,uBACE,uDAGJ,oBAkBE,mDAhBA,+CAaA,CAbA,oBAaA,0FAEE,CAFF,gGAbA,+BAaA,0BAGA,mQAIA,oNAEE,kCADA,gBACA,aAGJ,sDAHI,mBAGJ,yBAYI,+VACE,sDAGA,iBAHA,2BAGA,kWAGN,iDAEE,CALI,gGAGN,CAHM,gBAKJ,yCAGF,0EACE,2EAGF,iBACE,yDAOA,0EAGF,6EAEE,iBC/EA,wDACA,4DACA,qBAEA,oDCDA,6BACA,yBACA,sBAEA,iBAGF,sNAYE,iBAEA,kBAdF,wRA8BI,kBACA,iOAkBA,aACA,4DACE,uEAEA,uVAoBA,iDAKA,ieC1EJ,4BACA,CCFF,6JAEE,iDACA,sEAIA,mDAGA,iDAOF,4DAGE,8CAEA,CAEA,kBACA,CAHA,gCAEA,CACA,eADA,cACA,oBAEE,uBAFF,kCAEE,gCAEF,kBACE,CAIA,mDAEA,CAHA,uCACA,CALF,aACE,6BAEA,CAIA,gBAJA,mCACA,CADA,gBAIA,wBACA,6CAGF,YAHE,iBAGF,gCAGA,iEACA,6CAEA,qDACA,6EACA,2EACA,8GAEA,yCAGA,uBACA,CAFA,yBACA,CACA,yDAKA,kDACE,mFAKJ,oCACE,CANE,aAKJ,CACE,qEAIA,YAFA,WAEA,CAHA,aACA,CAEA,gBACE,4BACA,sBADA,aACA,gCAMF,oCACA,yDACA,2CAEA,qBAGE,kBAEA,CACA,mCAIF,CARE,YACA,CAOF,iCAEE,CAPA,oBACA,CAQA,oBACE,uDAEJ,sDAGA,CAHA,cAGA,0BACE,oDAIA,oCACA,4BACA,sBAGA,cAEA,oFAGA,sBAEA,yDACE,CAIA,iBAJA,wBAIA,6CAJA,6CAOA,4BAGJ,CAHI,cAGJ,yCAGA,kBACE,CAIA,iDAEA,CATA,YAEF,CACE,4CAGA,kBAIA,wEAEA,wDAIF,kCAOE,iDACA,CARF,WAIE,sCAGA,CANA,2CACA,CAMA,oEARF,iBACE,CACA,qCAMA,iBAuBE,uBAlBF,YAKA,2DALA,uDAKA,CALA,sBAiBA,4CACE,CALA,gRAIF,YACE,UAEN,uBACE,YACA,mCAOE,+CAGA,8BAGF,+CAGA,4BCjNA,SDiNA,qFCjNA,gDAGA,sCACA,qCACA,sDAIF,CAIE,kDAGA,CAPF,0CAOE,kBAEA,kDAEA,CAHA,eACA,CAFA,YACA,CADA,SAIA,mHAIE,CAGA,6CAFA,oCAeE,CAbF,yBACE,qBAEJ,CAGE,oBACA,CAEA,YAFA,2CACF,CACE,uBAEA,mFAEE,CALJ,oBACE,CAEA,UAEE,gCAGF,sDAEA,yCC7CJ,oCAGA,CD6CE,yXAQE,sCCrDJ,wCAGA,oCACE",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack:///./node_modules/normalize.css/normalize.css",
         "webpack:///./src/furo/assets/styles/base/_print.sass",
         "webpack:///./src/furo/assets/styles/base/_screen-readers.sass",
         "webpack:///./src/furo/assets/styles/base/_theme.sass",
@@ -42,24 +42,24 @@
         "/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */\n\n/* Document\n   ========================================================================== */\n\n/**\n * 1. Correct the line height in all browsers.\n * 2. Prevent adjustments of font size after orientation changes in iOS.\n */\n\nhtml {\n  line-height: 1.15; /* 1 */\n  -webkit-text-size-adjust: 100%; /* 2 */\n}\n\n/* Sections\n   ========================================================================== */\n\n/**\n * Remove the margin in all browsers.\n */\n\nbody {\n  margin: 0;\n}\n\n/**\n * Render the `main` element consistently in IE.\n */\n\nmain {\n  display: block;\n}\n\n/**\n * Correct the font size and margin on `h1` elements within `section` and\n * `article` contexts in Chrome, Firefox, and Safari.\n */\n\nh1 {\n  font-size: 2em;\n  margin: 0.67em 0;\n}\n\n/* Grouping content\n   ========================================================================== */\n\n/**\n * 1. Add the correct box sizing in Firefox.\n * 2. Show the overflow in Edge and IE.\n */\n\nhr {\n  box-sizing: content-box; /* 1 */\n  height: 0; /* 1 */\n  overflow: visible; /* 2 */\n}\n\n/**\n * 1. Correct the inheritance and scaling of font size in all browsers.\n * 2. Correct the odd `em` font sizing in all browsers.\n */\n\npre {\n  font-family: monospace, monospace; /* 1 */\n  font-size: 1em; /* 2 */\n}\n\n/* Text-level semantics\n   ========================================================================== */\n\n/**\n * Remove the gray background on active links in IE 10.\n */\n\na {\n  background-color: transparent;\n}\n\n/**\n * 1. Remove the bottom border in Chrome 57-\n * 2. Add the correct text decoration in Chrome, Edge, IE, Opera, and Safari.\n */\n\nabbr[title] {\n  border-bottom: none; /* 1 */\n  text-decoration: underline; /* 2 */\n  text-decoration: underline dotted; /* 2 */\n}\n\n/**\n * Add the correct font weight in Chrome, Edge, and Safari.\n */\n\nb,\nstrong {\n  font-weight: bolder;\n}\n\n/**\n * 1. Correct the inheritance and scaling of font size in all browsers.\n * 2. Correct the odd `em` font sizing in all browsers.\n */\n\ncode,\nkbd,\nsamp {\n  font-family: monospace, monospace; /* 1 */\n  font-size: 1em; /* 2 */\n}\n\n/**\n * Add the correct font size in all browsers.\n */\n\nsmall {\n  font-size: 80%;\n}\n\n/**\n * Prevent `sub` and `sup` elements from affecting the line height in\n * all browsers.\n */\n\nsub,\nsup {\n  font-size: 75%;\n  line-height: 0;\n  position: relative;\n  vertical-align: baseline;\n}\n\nsub {\n  bottom: -0.25em;\n}\n\nsup {\n  top: -0.5em;\n}\n\n/* Embedded content\n   ========================================================================== */\n\n/**\n * Remove the border on images inside links in IE 10.\n */\n\nimg {\n  border-style: none;\n}\n\n/* Forms\n   ========================================================================== */\n\n/**\n * 1. Change the font styles in all browsers.\n * 2. Remove the margin in Firefox and Safari.\n */\n\nbutton,\ninput,\noptgroup,\nselect,\ntextarea {\n  font-family: inherit; /* 1 */\n  font-size: 100%; /* 1 */\n  line-height: 1.15; /* 1 */\n  margin: 0; /* 2 */\n}\n\n/**\n * Show the overflow in IE.\n * 1. Show the overflow in Edge.\n */\n\nbutton,\ninput { /* 1 */\n  overflow: visible;\n}\n\n/**\n * Remove the inheritance of text transform in Edge, Firefox, and IE.\n * 1. Remove the inheritance of text transform in Firefox.\n */\n\nbutton,\nselect { /* 1 */\n  text-transform: none;\n}\n\n/**\n * Correct the inability to style clickable types in iOS and Safari.\n */\n\nbutton,\n[type=\"button\"],\n[type=\"reset\"],\n[type=\"submit\"] {\n  -webkit-appearance: button;\n}\n\n/**\n * Remove the inner border and padding in Firefox.\n */\n\nbutton::-moz-focus-inner,\n[type=\"button\"]::-moz-focus-inner,\n[type=\"reset\"]::-moz-focus-inner,\n[type=\"submit\"]::-moz-focus-inner {\n  border-style: none;\n  padding: 0;\n}\n\n/**\n * Restore the focus styles unset by the previous rule.\n */\n\nbutton:-moz-focusring,\n[type=\"button\"]:-moz-focusring,\n[type=\"reset\"]:-moz-focusring,\n[type=\"submit\"]:-moz-focusring {\n  outline: 1px dotted ButtonText;\n}\n\n/**\n * Correct the padding in Firefox.\n */\n\nfieldset {\n  padding: 0.35em 0.75em 0.625em;\n}\n\n/**\n * 1. Correct the text wrapping in Edge and IE.\n * 2. Correct the color inheritance from `fieldset` elements in IE.\n * 3. Remove the padding so developers are not caught out when they zero out\n *    `fieldset` elements in all browsers.\n */\n\nlegend {\n  box-sizing: border-box; /* 1 */\n  color: inherit; /* 2 */\n  display: table; /* 1 */\n  max-width: 100%; /* 1 */\n  padding: 0; /* 3 */\n  white-space: normal; /* 1 */\n}\n\n/**\n * Add the correct vertical alignment in Chrome, Firefox, and Opera.\n */\n\nprogress {\n  vertical-align: baseline;\n}\n\n/**\n * Remove the default vertical scrollbar in IE 10+.\n */\n\ntextarea {\n  overflow: auto;\n}\n\n/**\n * 1. Add the correct box sizing in IE 10.\n * 2. Remove the padding in IE 10.\n */\n\n[type=\"checkbox\"],\n[type=\"radio\"] {\n  box-sizing: border-box; /* 1 */\n  padding: 0; /* 2 */\n}\n\n/**\n * Correct the cursor style of increment and decrement buttons in Chrome.\n */\n\n[type=\"number\"]::-webkit-inner-spin-button,\n[type=\"number\"]::-webkit-outer-spin-button {\n  height: auto;\n}\n\n/**\n * 1. Correct the odd appearance in Chrome and Safari.\n * 2. Correct the outline style in Safari.\n */\n\n[type=\"search\"] {\n  -webkit-appearance: textfield; /* 1 */\n  outline-offset: -2px; /* 2 */\n}\n\n/**\n * Remove the inner padding in Chrome and Safari on macOS.\n */\n\n[type=\"search\"]::-webkit-search-decoration {\n  -webkit-appearance: none;\n}\n\n/**\n * 1. Correct the inability to style clickable types in iOS and Safari.\n * 2. Change font properties to `inherit` in Safari.\n */\n\n::-webkit-file-upload-button {\n  -webkit-appearance: button; /* 1 */\n  font: inherit; /* 2 */\n}\n\n/* Interactive\n   ========================================================================== */\n\n/*\n * Add the correct display in Edge, IE 10+, and Firefox.\n */\n\ndetails {\n  display: block;\n}\n\n/*\n * Add the correct display in all browsers.\n */\n\nsummary {\n  display: list-item;\n}\n\n/* Misc\n   ========================================================================== */\n\n/**\n * Add the correct display in IE 10+.\n */\n\ntemplate {\n  display: none;\n}\n\n/**\n * Add the correct display in IE 10.\n */\n\n[hidden] {\n  display: none;\n}\n",
         "// This file contains styles for managing print media.\n\n////////////////////////////////////////////////////////////////////////////////\n// Hide elements not relevant to print media.\n////////////////////////////////////////////////////////////////////////////////\n@media print\n  // Hide icon container.\n  .content-icon-container\n    display: none !important\n\n  // Hide showing header links if hovering over when printing.\n  .headerlink\n    display: none !important\n\n  // Hide mobile header.\n  .mobile-header\n    display: none !important\n\n  // Hide navigation links.\n  .related-pages\n    display: none !important\n\n////////////////////////////////////////////////////////////////////////////////\n// Tweaks related to decolorization.\n////////////////////////////////////////////////////////////////////////////////\n@media print\n  // Apply a border around code which no longer have a color background.\n  .highlight\n    border: 0.1pt solid var(--color-foreground-border)\n\n////////////////////////////////////////////////////////////////////////////////\n// Avoid page break in some relevant cases.\n////////////////////////////////////////////////////////////////////////////////\n@media print\n  ul, ol, dl, a, table, pre, blockquote\n    page-break-inside: avoid\n\n  h1, h2, h3, h4, h5, h6, img, figure, caption\n    page-break-inside: avoid\n    page-break-after: avoid\n\n  ul, ol, dl\n    page-break-before: avoid\n",
         ".visually-hidden\n  position: absolute !important\n  width: 1px !important\n  height: 1px !important\n  padding: 0 !important\n  margin: -1px !important\n  overflow: hidden !important\n  clip: rect(0,0,0,0) !important\n  white-space: nowrap !important\n  border: 0 !important\n\n:-moz-focusring\n  outline: auto\n",
         "// This file serves as the \"skeleton\" of the theming logic.\n//\n// This contains the bulk of the logic for handling dark mode, color scheme\n// toggling and the handling of color-scheme-specific hiding of elements.\n\nbody\n  @include fonts\n  @include spacing\n  @include icons\n  @include admonitions\n  @include default-admonition(#651fff, \"abstract\")\n  @include default-topic(#14B8A6, \"pencil\")\n\n  @include colors\n\n.only-light\n  display: block !important\nhtml body .only-dark\n  display: none !important\n\n// Ignore dark-mode hints if print media.\n@media not print\n  // Enable dark-mode, if requested.\n  body[data-theme=\"dark\"]\n    @include colors-dark\n\n    html & .only-light\n      display: none !important\n    .only-dark\n      display: block !important\n\n  // Enable dark mode, unless explicitly told to avoid.\n  @media (prefers-color-scheme: dark)\n    body:not([data-theme=\"light\"])\n      @include colors-dark\n\n      html & .only-light\n        display: none !important\n      .only-dark\n        display: block !important\n\n//\n// Theme toggle presentation\n//\nbody[data-theme=\"auto\"]\n  .theme-toggle svg.theme-icon-when-auto\n    display: block\n\nbody[data-theme=\"dark\"]\n  .theme-toggle svg.theme-icon-when-dark\n    display: block\n\nbody[data-theme=\"light\"]\n  .theme-toggle svg.theme-icon-when-light\n    display: block\n",
         "// Fonts used by this theme.\n//\n// There are basically two things here -- using the system font stack and\n// defining sizes for various elements in %ages. We could have also used `em`\n// but %age is easier to reason about for me.\n\n@mixin fonts {\n  // These are adapted from https://systemfontstack.com/\n  --font-stack: -apple-system, BlinkMacSystemFont, Segoe UI, Helvetica, Arial,\n    sans-serif, Apple Color Emoji, Segoe UI Emoji;\n  --font-stack--monospace: \"SFMono-Regular\", Menlo, Consolas, Monaco,\n    Liberation Mono, Lucida Console, monospace;\n\n  --font-size--normal: 100%;\n  --font-size--small: 87.5%;\n  --font-size--small--2: 81.25%;\n  --font-size--small--3: 75%;\n  --font-size--small--4: 62.5%;\n\n  // Sidebar\n  --sidebar-caption-font-size: var(--font-size--small--2);\n  --sidebar-item-font-size: var(--font-size--small);\n  --sidebar-search-input-font-size: var(--font-size--small);\n\n  // Table of Contents\n  --toc-font-size: var(--font-size--small--3);\n  --toc-font-size--mobile: var(--font-size--normal);\n  --toc-title-font-size: var(--font-size--small--4);\n\n  // Admonitions\n  //\n  // These aren't defined in terms of %ages, since nesting these is permitted.\n  --admonition-font-size: 0.8125rem;\n  --admonition-title-font-size: 0.8125rem;\n\n  // Code\n  --code-font-size: var(--font-size--small--2);\n\n  // API\n  --api-font-size: var(--font-size--small);\n}\n",
         "// Spacing for various elements on the page\n//\n// If the user wants to tweak things in a certain way, they are permitted to.\n// They also have to deal with the consequences though!\n\n@mixin spacing {\n  // Header!\n  --header-height: calc(\n    var(--sidebar-item-line-height) + 4 * #{var(--sidebar-item-spacing-vertical)}\n  );\n  --header-padding: 0.5rem;\n\n  // Sidebar\n  --sidebar-tree-space-above: 1.5rem;\n  --sidebar-caption-space-above: 1rem;\n\n  --sidebar-item-line-height: 1rem;\n  --sidebar-item-spacing-vertical: 0.5rem;\n  --sidebar-item-spacing-horizontal: 1rem;\n  --sidebar-item-height: calc(\n    var(--sidebar-item-line-height) + 2 *#{var(--sidebar-item-spacing-vertical)}\n  );\n\n  --sidebar-expander-width: var(--sidebar-item-height); // be square\n\n  --sidebar-search-space-above: 0.5rem;\n  --sidebar-search-input-spacing-vertical: 0.5rem;\n  --sidebar-search-input-spacing-horizontal: 0.5rem;\n  --sidebar-search-input-height: 1rem;\n  --sidebar-search-icon-size: var(--sidebar-search-input-height);\n\n  // Table of Contents\n  --toc-title-padding: 0.25rem 0;\n  --toc-spacing-vertical: 1.5rem;\n  --toc-spacing-horizontal: 1.5rem;\n  --toc-item-spacing-vertical: 0.4rem;\n  --toc-item-spacing-horizontal: 1rem;\n}\n",
         "// Expose theme icons as CSS variables.\n\n$icons: (\n  // Adapted from tabler-icons\n  //    url: https://tablericons.com/\n  \"search\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\" stroke-width=\"1.5\" stroke=\"currentColor\" fill=\"none\" stroke-linecap=\"round\" stroke-linejoin=\"round\"><path stroke=\"none\" d=\"M0 0h24v24H0z\"/><circle cx=\"10\" cy=\"10\" r=\"7\" /><line x1=\"21\" y1=\"21\" x2=\"15\" y2=\"15\" /></svg>'),\n  // Factored out from mkdocs-material on 24-Aug-2020.\n  //    url: https://squidfunk.github.io/mkdocs-material/reference/admonitions/\n  \"pencil\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M20.71 7.04c.39-.39.39-1.04 0-1.41l-2.34-2.34c-.37-.39-1.02-.39-1.41 0l-1.84 1.83 3.75 3.75M3 17.25V21h3.75L17.81 9.93l-3.75-3.75L3 17.25z\"/></svg>'),\n  \"abstract\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M4 5h16v2H4V5m0 4h16v2H4V9m0 4h16v2H4v-2m0 4h10v2H4v-2z\"/></svg>'),\n  \"info\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M13 9h-2V7h2m0 10h-2v-6h2m-1-9A10 10 0 002 12a10 10 0 0010 10 10 10 0 0010-10A10 10 0 0012 2z\"/></svg>'),\n  \"flame\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M17.55 11.2c-.23-.3-.5-.56-.76-.82-.65-.6-1.4-1.03-2.03-1.66C13.3 7.26 13 4.85 13.91 3c-.91.23-1.75.75-2.45 1.32-2.54 2.08-3.54 5.75-2.34 8.9.04.1.08.2.08.33 0 .22-.15.42-.35.5-.22.1-.46.04-.64-.12a.83.83 0 01-.15-.17c-1.1-1.43-1.28-3.48-.53-5.12C5.89 10 5 12.3 5.14 14.47c.04.5.1 1 .27 1.5.14.6.4 1.2.72 1.73 1.04 1.73 2.87 2.97 4.84 3.22 2.1.27 4.35-.12 5.96-1.6 1.8-1.66 2.45-4.32 1.5-6.6l-.13-.26c-.2-.46-.47-.87-.8-1.25l.05-.01m-3.1 6.3c-.28.24-.73.5-1.08.6-1.1.4-2.2-.16-2.87-.82 1.19-.28 1.89-1.16 2.09-2.05.17-.8-.14-1.46-.27-2.23-.12-.74-.1-1.37.18-2.06.17.38.37.76.6 1.06.76 1 1.95 1.44 2.2 2.8.04.14.06.28.06.43.03.82-.32 1.72-.92 2.27h.01z\"/></svg>'),\n  \"question\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M15.07 11.25l-.9.92C13.45 12.89 13 13.5 13 15h-2v-.5c0-1.11.45-2.11 1.17-2.83l1.24-1.26c.37-.36.59-.86.59-1.41a2 2 0 00-2-2 2 2 0 00-2 2H8a4 4 0 014-4 4 4 0 014 4 3.2 3.2 0 01-.93 2.25M13 19h-2v-2h2M12 2A10 10 0 002 12a10 10 0 0010 10 10 10 0 0010-10c0-5.53-4.5-10-10-10z\"/></svg>'),\n  \"warning\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M13 14h-2v-4h2m0 8h-2v-2h2M1 21h22L12 2 1 21z\"/></svg>'),\n  \"failure\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M12 2c5.53 0 10 4.47 10 10s-4.47 10-10 10S2 17.53 2 12 6.47 2 12 2m3.59 5L12 10.59 8.41 7 7 8.41 10.59 12 7 15.59 8.41 17 12 13.41 15.59 17 17 15.59 13.41 12 17 8.41 15.59 7z\"/></svg>'),\n  \"spark\":\n    url('data:image/svg+xml;charset=utf-8,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 24 24\"><path d=\"M11.5 20l4.86-9.73H13V4l-5 9.73h3.5V20M12 2c2.75 0 5.1 1 7.05 2.95C21 6.9 22 9.25 22 12s-1 5.1-2.95 7.05C17.1 21 14.75 22 12 22s-5.1-1-7.05-2.95C3 17.1 2 14.75 2 12s1-5.1 2.95-7.05C6.9 3 9.25 2 12 2z\"/></svg>')\n);\n\n@mixin icons {\n  @each $name, $glyph in $icons {\n    --icon-#{$name}: #{$glyph};\n  }\n}\n",
-        "// Admonitions\n\n// Structure of these is:\n//    admonition-class: color \"icon-name\";\n//\n// The colors are translated into CSS variables below. The icons are\n// used directly in the main declarations to set the `mask-image` in\n// the title.\n\n// prettier-ignore\n$admonitions: (\n  // Each of these has an reST directives for it.\n  \"caution\":         #ff9100 \"spark\",\n  \"warning\":         #ff9100 \"warning\",\n  \"danger\":          #ff5252 \"spark\",\n  \"attention\":       #ff5252 \"warning\",\n  \"error\":           #ff5252 \"failure\",\n  \"hint\":            #00c852 \"question\",\n  \"tip\":             #00c852 \"info\",\n  \"important\":       #00bfa5 \"flame\",\n  \"note\":            #00b0ff \"pencil\",\n  \"seealso\":         #448aff \"info\",\n  \"admonition-todo\": #808080 \"pencil\"\n);\n\n@mixin default-admonition($color, $icon-name) {\n  --color-admonition-title: #{$color};\n  --color-admonition-title-background: #{rgba($color, 0.1)};\n\n  --icon-admonition-default: var(--icon-#{$icon-name});\n}\n\n@mixin default-topic($color, $icon-name) {\n  --color-topic-title: #{$color};\n  --color-topic-title-background: #{rgba($color, 0.1)};\n\n  --icon-topic-default: var(--icon-#{$icon-name});\n}\n\n@mixin admonitions {\n  @each $name, $values in $admonitions {\n    --color-admonition-title--#{$name}: #{nth($values, 1)};\n    --color-admonition-title-background--#{$name}: #{rgba(\n        nth($values, 1),\n        0.1\n      )};\n  }\n}\n",
-        "// Colors used throughout this theme.\n//\n// The aim is to give the user more control. Thus, instead of hard-coding colors\n// in various parts of the stylesheet, the approach taken is to define all\n// colors as CSS variables and reusing them in all the places.\n//\n// `colors-dark` depends on `colors` being included at a lower specificity.\n\n@mixin colors {\n  --color-problematic: #b30000;\n\n  // Base Colors\n  --color-foreground-primary: black; // for main text and headings\n  --color-foreground-secondary: #5a5c63; // for secondary text\n  --color-foreground-muted: #646776; // for muted text\n  --color-foreground-border: #878787; // for content borders\n\n  --color-background-primary: white; // for content\n  --color-background-secondary: #f8f9fb; // for navigation + ToC\n  --color-background-hover: #efeff4ff; // for navigation-item hover\n  --color-background-hover--transparent: #efeff400;\n  --color-background-border: #eeebee; // for UI borders\n  --color-background-item: #ccc; // for \"background\" items (eg: copybutton)\n\n  // Announcements\n  --color-announcement-background: #000000dd;\n  --color-announcement-text: #eeebee;\n\n  // Brand colors\n  --color-brand-primary: #2962ff;\n  --color-brand-content: #2a5adf;\n\n  // API documentation\n  --color-api-background: var(--color-background-secondary);\n  --color-api-background-hover: var(--color-background-hover);\n  --color-api-overall: var(--color-foreground-secondary);\n  --color-api-name: var(--color-problematic);\n  --color-api-pre-name: var(--color-problematic);\n  --color-api-paren: var(--color-foreground-secondary);\n  --color-api-keyword: var(--color-foreground-primary);\n  --color-highlight-on-target: #ffffcc;\n\n  // Inline code background\n  --color-inline-code-background: var(--color-background-secondary);\n\n  // Highlighted text (search)\n  --color-highlighted-background: #ddeeff;\n  --color-highlighted-text: var(--color-foreground-primary);\n\n  // GUI Labels\n  --color-guilabel-background: #ddeeff80;\n  --color-guilabel-border: #bedaf580;\n  --color-guilabel-text: var(--color-foreground-primary);\n\n  // Admonitions!\n  --color-admonition-background: transparent;\n\n  //////////////////////////////////////////////////////////////////////////////\n  // Everything below this should be one of:\n  // - var(...)\n  // - *-gradient(...)\n  // - special literal values (eg: transparent, none)\n  //////////////////////////////////////////////////////////////////////////////\n\n  // Tables\n  --color-table-header-background: var(--color-background-secondary);\n  --color-table-border: var(--color-background-border);\n\n  // Cards\n  --color-card-border: var(--color-background-secondary);\n  --color-card-background: transparent;\n  --color-card-marginals-background: var(--color-background-secondary);\n\n  // Header\n  --color-header-background: var(--color-background-primary);\n  --color-header-border: var(--color-background-border);\n  --color-header-text: var(--color-foreground-primary);\n\n  // Sidebar (left)\n  --color-sidebar-background: var(--color-background-secondary);\n  --color-sidebar-background-border: var(--color-background-border);\n\n  --color-sidebar-brand-text: var(--color-foreground-primary);\n  --color-sidebar-caption-text: var(--color-foreground-muted);\n  --color-sidebar-link-text: var(--color-foreground-secondary);\n  --color-sidebar-link-text--top-level: var(--color-brand-primary);\n\n  --color-sidebar-item-background: var(--color-sidebar-background);\n  --color-sidebar-item-background--current: var(\n    --color-sidebar-item-background\n  );\n  --color-sidebar-item-background--hover: linear-gradient(\n    90deg,\n    var(--color-background-hover--transparent) 0%,\n    var(--color-background-hover) var(--sidebar-item-spacing-horizontal),\n    var(--color-background-hover) 100%\n  );\n\n  --color-sidebar-item-expander-background: transparent;\n  --color-sidebar-item-expander-background--hover: var(\n    --color-background-hover\n  );\n\n  --color-sidebar-search-text: var(--color-foreground-primary);\n  --color-sidebar-search-background: var(--color-background-secondary);\n  --color-sidebar-search-background--focus: var(--color-background-primary);\n  --color-sidebar-search-border: var(--color-background-border);\n  --color-sidebar-search-icon: var(--color-foreground-muted);\n\n  // Table of Contents (right)\n  --color-toc-background: var(--color-background-primary);\n  --color-toc-title-text: var(--color-foreground-muted);\n  --color-toc-item-text: var(--color-foreground-secondary);\n  --color-toc-item-text--hover: var(--color-foreground-primary);\n  --color-toc-item-text--active: var(--color-brand-primary);\n\n  // Actual page contents\n  --color-content-foreground: var(--color-foreground-primary);\n  --color-content-background: transparent;\n\n  // Links\n  --color-link: var(--color-brand-content);\n  --color-link--hover: var(--color-brand-content);\n  --color-link-underline: var(--color-background-border);\n  --color-link-underline--hover: var(--color-foreground-border);\n}\n\n@mixin colors-dark {\n  --color-problematic: #ee5151;\n\n  // Base Colors\n  --color-foreground-primary: #ffffffcc; // for main text and headings\n  --color-foreground-secondary: #9ca0a5; // for secondary text\n  --color-foreground-muted: #81868d; // for muted text\n  --color-foreground-border: #666666; // for content borders\n\n  --color-background-primary: #131416; // for content\n  --color-background-secondary: #1a1c1e; // for navigation + ToC\n  --color-background-hover: #1e2124ff; // for navigation-item hover\n  --color-background-hover--transparent: #1e212400;\n  --color-background-border: #303335; // for UI borders\n  --color-background-item: #444; // for \"background\" items (eg: copybutton)\n\n  // Announcements\n  --color-announcement-background: #000000dd;\n  --color-announcement-text: #eeebee;\n\n  // Brand colors\n  --color-brand-primary: #2b8cee;\n  --color-brand-content: #368ce2;\n\n  // Highlighted text (search)\n  --color-highlighted-background: #083563;\n\n  // GUI Labels\n  --color-guilabel-background: #08356380;\n  --color-guilabel-border: #13395f80;\n\n  // API documentation\n  --color-api-keyword: var(--color-foreground-secondary);\n  --color-highlight-on-target: #333300;\n\n  // Admonitions\n  --color-admonition-background: #18181a;\n\n  // Cards\n  --color-card-border: var(--color-background-secondary);\n  --color-card-background: #18181a;\n  --color-card-marginals-background: var(--color-background-hover);\n}\n",
+        "// Admonitions\n\n// Structure of these is:\n//    admonition-class: color \"icon-name\";\n//\n// The colors are translated into CSS variables below. The icons are\n// used directly in the main declarations to set the `mask-image` in\n// the title.\n\n// prettier-ignore\n$admonitions: (\n  // Each of these has an reST directives for it.\n  \"caution\":         #ff9100 \"spark\",\n  \"warning\":         #ff9100 \"warning\",\n  \"danger\":          #ff5252 \"spark\",\n  \"attention\":       #ff5252 \"warning\",\n  \"error\":           #ff5252 \"failure\",\n  \"hint\":            #00c852 \"question\",\n  \"tip\":             #00c852 \"info\",\n  \"important\":       #00bfa5 \"flame\",\n  \"note\":            #00b0ff \"pencil\",\n  \"seealso\":         #448aff \"info\",\n  \"admonition-todo\": #808080 \"pencil\"\n);\n\n@mixin default-admonition($color, $icon-name) {\n  --color-admonition-title: #{$color};\n  --color-admonition-title-background: #{rgba($color, 0.2)};\n\n  --icon-admonition-default: var(--icon-#{$icon-name});\n}\n\n@mixin default-topic($color, $icon-name) {\n  --color-topic-title: #{$color};\n  --color-topic-title-background: #{rgba($color, 0.2)};\n\n  --icon-topic-default: var(--icon-#{$icon-name});\n}\n\n@mixin admonitions {\n  @each $name, $values in $admonitions {\n    --color-admonition-title--#{$name}: #{nth($values, 1)};\n    --color-admonition-title-background--#{$name}: #{rgba(\n        nth($values, 1),\n        0.2\n      )};\n  }\n}\n",
+        "// Colors used throughout this theme.\n//\n// The aim is to give the user more control. Thus, instead of hard-coding colors\n// in various parts of the stylesheet, the approach taken is to define all\n// colors as CSS variables and reusing them in all the places.\n//\n// `colors-dark` depends on `colors` being included at a lower specificity.\n\n@mixin colors {\n  --color-problematic: #b30000;\n\n  // Base Colors\n  --color-foreground-primary: black; // for main text and headings\n  --color-foreground-secondary: #5a5c63; // for secondary text\n  --color-foreground-muted: #646776; // for muted text\n  --color-foreground-border: #878787; // for content borders\n\n  --color-background-primary: white; // for content\n  --color-background-secondary: #f8f9fb; // for navigation + ToC\n  --color-background-hover: #efeff4ff; // for navigation-item hover\n  --color-background-hover--transparent: #efeff400;\n  --color-background-border: #eeebee; // for UI borders\n  --color-background-item: #ccc; // for \"background\" items (eg: copybutton)\n\n  // Announcements\n  --color-announcement-background: #000000dd;\n  --color-announcement-text: #eeebee;\n\n  // Brand colors\n  --color-brand-primary: #2962ff;\n  --color-brand-content: #2a5adf;\n\n  // API documentation\n  --color-api-background: var(--color-background-hover--transparent);\n  --color-api-background-hover: var(--color-background-hover);\n  --color-api-overall: var(--color-foreground-secondary);\n  --color-api-name: var(--color-problematic);\n  --color-api-pre-name: var(--color-problematic);\n  --color-api-paren: var(--color-foreground-secondary);\n  --color-api-keyword: var(--color-foreground-primary);\n  --color-highlight-on-target: #ffffcc;\n\n  // Inline code background\n  --color-inline-code-background: var(--color-background-secondary);\n\n  // Highlighted text (search)\n  --color-highlighted-background: #ddeeff;\n  --color-highlighted-text: var(--color-foreground-primary);\n\n  // GUI Labels\n  --color-guilabel-background: #ddeeff80;\n  --color-guilabel-border: #bedaf580;\n  --color-guilabel-text: var(--color-foreground-primary);\n\n  // Admonitions!\n  --color-admonition-background: transparent;\n\n  //////////////////////////////////////////////////////////////////////////////\n  // Everything below this should be one of:\n  // - var(...)\n  // - *-gradient(...)\n  // - special literal values (eg: transparent, none)\n  //////////////////////////////////////////////////////////////////////////////\n\n  // Tables\n  --color-table-header-background: var(--color-background-secondary);\n  --color-table-border: var(--color-background-border);\n\n  // Cards\n  --color-card-border: var(--color-background-secondary);\n  --color-card-background: transparent;\n  --color-card-marginals-background: var(--color-background-secondary);\n\n  // Header\n  --color-header-background: var(--color-background-primary);\n  --color-header-border: var(--color-background-border);\n  --color-header-text: var(--color-foreground-primary);\n\n  // Sidebar (left)\n  --color-sidebar-background: var(--color-background-secondary);\n  --color-sidebar-background-border: var(--color-background-border);\n\n  --color-sidebar-brand-text: var(--color-foreground-primary);\n  --color-sidebar-caption-text: var(--color-foreground-muted);\n  --color-sidebar-link-text: var(--color-foreground-secondary);\n  --color-sidebar-link-text--top-level: var(--color-brand-primary);\n\n  --color-sidebar-item-background: var(--color-sidebar-background);\n  --color-sidebar-item-background--current: var(\n    --color-sidebar-item-background\n  );\n  --color-sidebar-item-background--hover: linear-gradient(\n    90deg,\n    var(--color-background-hover--transparent) 0%,\n    var(--color-background-hover) var(--sidebar-item-spacing-horizontal),\n    var(--color-background-hover) 100%\n  );\n\n  --color-sidebar-item-expander-background: transparent;\n  --color-sidebar-item-expander-background--hover: var(\n    --color-background-hover\n  );\n\n  --color-sidebar-search-text: var(--color-foreground-primary);\n  --color-sidebar-search-background: var(--color-background-secondary);\n  --color-sidebar-search-background--focus: var(--color-background-primary);\n  --color-sidebar-search-border: var(--color-background-border);\n  --color-sidebar-search-icon: var(--color-foreground-muted);\n\n  // Table of Contents (right)\n  --color-toc-background: var(--color-background-primary);\n  --color-toc-title-text: var(--color-foreground-muted);\n  --color-toc-item-text: var(--color-foreground-secondary);\n  --color-toc-item-text--hover: var(--color-foreground-primary);\n  --color-toc-item-text--active: var(--color-brand-primary);\n\n  // Actual page contents\n  --color-content-foreground: var(--color-foreground-primary);\n  --color-content-background: transparent;\n\n  // Links\n  --color-link: var(--color-brand-content);\n  --color-link--hover: var(--color-brand-content);\n  --color-link-underline: var(--color-background-border);\n  --color-link-underline--hover: var(--color-foreground-border);\n}\n\n@mixin colors-dark {\n  --color-problematic: #ee5151;\n\n  // Base Colors\n  --color-foreground-primary: #ffffffcc; // for main text and headings\n  --color-foreground-secondary: #9ca0a5; // for secondary text\n  --color-foreground-muted: #81868d; // for muted text\n  --color-foreground-border: #666666; // for content borders\n\n  --color-background-primary: #131416; // for content\n  --color-background-secondary: #1a1c1e; // for navigation + ToC\n  --color-background-hover: #1e2124ff; // for navigation-item hover\n  --color-background-hover--transparent: #1e212400;\n  --color-background-border: #303335; // for UI borders\n  --color-background-item: #444; // for \"background\" items (eg: copybutton)\n\n  // Announcements\n  --color-announcement-background: #000000dd;\n  --color-announcement-text: #eeebee;\n\n  // Brand colors\n  --color-brand-primary: #2b8cee;\n  --color-brand-content: #368ce2;\n\n  // Highlighted text (search)\n  --color-highlighted-background: #083563;\n\n  // GUI Labels\n  --color-guilabel-background: #08356380;\n  --color-guilabel-border: #13395f80;\n\n  // API documentation\n  --color-api-keyword: var(--color-foreground-secondary);\n  --color-highlight-on-target: #333300;\n\n  // Admonitions\n  --color-admonition-background: #18181a;\n\n  // Cards\n  --color-card-border: var(--color-background-secondary);\n  --color-card-background: #18181a;\n  --color-card-marginals-background: var(--color-background-hover);\n}\n",
         "// This file contains the styling for making the content throughout the page,\n// including fonts, paragraphs, headings and spacing among these elements.\n\nbody\n  font-family: var(--font-stack)\npre,\ncode,\nkbd,\nsamp\n  font-family: var(--font-stack--monospace)\n\n// Make fonts look slightly nicer.\nbody\n  -webkit-font-smoothing: antialiased\n  -moz-osx-font-smoothing: grayscale\n\n// Line height from Bootstrap 4.1\narticle\n  line-height: 1.5\n\n//\n// Headings\n//\nh1,\nh2,\nh3,\nh4,\nh5,\nh6\n  line-height: 1.25\n  font-weight: bold\n\n  border-radius: 0.5rem\n  margin-top: 0.5rem\n  margin-bottom: 0.5rem\n  margin-left: -0.5rem\n  margin-right: -0.5rem\n  padding-left: 0.5rem\n  padding-right: 0.5rem\n\n  + p\n    margin-top: 0\n\nh1\n  font-size: 2.5em\n  margin-top: 1.75rem\n  margin-bottom: 1rem\nh2\n  font-size: 2em\n  margin-top: 1.75rem\nh3\n  font-size: 1.5em\nh4\n  font-size: 1.25em\nh5\n  font-size: 1.125em\nh6\n  font-size: 1em\n\nsmall\n  opacity: 75%\n  font-size: 80%\n\n// Paragraph\np\n  margin-top: 0.5rem\n  margin-bottom: 0.75rem\n\n// Horizontal rules\nhr.docutils\n  height: 1px\n  padding: 0\n  margin: 2rem 0\n  background-color: var(--color-background-border)\n  border: 0\n\n.centered\n  text-align: center\n\n// Links\na\n  text-decoration: underline\n\n  color: var(--color-link)\n  text-decoration-color: var(--color-link-underline)\n\n  &:hover\n    color: var(--color-link--hover)\n    text-decoration-color: var(--color-link-underline--hover)\n  &.muted-link\n    color: inherit\n    &:hover\n      color: var(--color-link)\n      text-decoration-color: var(--color-link-underline--hover)\n",
-        "// This file contains the styles for the overall layouting of the documentation\n// skeleton, including the responsive changes as well as sidebar toggles.\n//\n// This is implemented as a mobile-last design, which isn't ideal, but it is\n// reasonably good-enough and I got pretty tired by the time I'd finished this\n// to move the rules around to fix this. Shouldn't take more than 3-4 hours,\n// if you know what you're doing tho.\n\n// HACK: Not all browsers account for the scrollbar width in media queries.\n// This results in horizontal scrollbars in the breakpoint where we go\n// from displaying everything to hiding the ToC. We accomodate for this by\n// adding a bit of padding to the TOC drawer, disabling the horizontal\n// scrollbar and allowing the scrollbars to cover the padding.\n// https://www.456bereastreet.com/archive/201301/media_query_width_and_vertical_scrollbars/\n\n// HACK: Always having the scrollbar visible, prevents certain browsers from\n// causing the content to stutter horizontally between taller-than-viewport and\n// not-taller-than-viewport pages.\n\nhtml\n  overflow-x: hidden\n  overflow-y: scroll\n  scroll-behavior: smooth\n\n.sidebar-scroll, .toc-scroll, article[role=main] *\n  // Override Firefox scrollbar style\n  scrollbar-width: thin\n  scrollbar-color: var(--color-foreground-border) transparent\n\n  // Override Chrome scrollbar styles\n  &::-webkit-scrollbar\n    width: 0.25rem\n    height: 0.25rem\n  &::-webkit-scrollbar-thumb\n    background-color: var(--color-foreground-border)\n    border-radius: 0.125rem\n\n//\n// Overalls\n//\nhtml,\nbody\n  height: 100%\n  color: var(--color-foreground-primary)\n  background: var(--color-background-primary)\n\narticle\n  color: var(--color-content-foreground)\n  background: var(--color-content-background)\n\n.page\n  display: flex\n  // fill the viewport for pages with little content.\n  min-height: 100%\n\n.mobile-header\n  width: 100%\n  height: var(--header-height)\n  background-color: var(--color-header-background)\n  color: var(--color-header-text)\n  border-bottom: 1px solid var(--color-header-border)\n\n  // Looks like sub-script/super-script have this, and we need this to\n  // be \"on top\" of those.\n  z-index: 10\n\n  // We don't show the header on large screens.\n  display: none\n\n  // Add shadow when scrolled\n  &.scrolled\n    border-bottom: none\n    box-shadow: 0 0 0.2rem rgba(0, 0, 0, 0.1), 0 0.2rem 0.4rem rgba(0, 0, 0, 0.2)\n\n  .header-center\n    a\n      color: var(--color-header-text)\n      text-decoration: none\n\n.main\n  display: flex\n  flex: 1\n\n// Sidebar (left) also covers the entire left portion of screen.\n.sidebar-drawer\n  box-sizing: border-box\n\n  border-right: 1px solid var(--color-sidebar-background-border)\n  background: var(--color-sidebar-background)\n\n  display: flex\n  justify-content: flex-end\n  // These next two lines took me two days to figure out.\n  width: calc((100% - #{$full-width}) / 2 + #{$sidebar-width})\n  min-width: $sidebar-width\n\n// Scroll-along sidebars\n.sidebar-container,\n.toc-drawer\n  box-sizing: border-box\n  width: $sidebar-width\n\n.toc-drawer\n  background: var(--color-toc-background)\n  // See HACK described on top of this document\n  padding-right: 1rem\n\n.sidebar-sticky,\n.toc-sticky\n  position: sticky\n  top: 0\n  height: min(100%, 100vh)\n  height: 100vh\n\n  display: flex\n  flex-direction: column\n\n.sidebar-scroll,\n.toc-scroll\n  flex-grow: 1\n  flex-shrink: 1\n\n  overflow: auto\n  scroll-behavior: smooth\n\n// Central items.\n.content\n  padding: 0 $content-padding\n  width: $content-width\n\n  display: flex\n  flex-direction: column\n  justify-content: space-between\n\n.icon\n  display: inline-block\n  height: 1rem\n  width: 1rem\n  svg\n    width: 100%\n    height: 100%\n\n//\n// Accommodate announcement banner\n//\n.announcement\n  background-color: var(--color-announcement-background)\n  color: var(--color-announcement-text)\n\n  height: var(--header-height)\n  display: flex\n  align-items: center\n  overflow-x: auto\n  & + .page\n    min-height: calc(100% - var(--header-height))\n\n.announcement-content\n  box-sizing: border-box\n  padding: 0.5rem\n  min-width: 100%\n  white-space: nowrap\n  text-align: center\n\n  a\n    color: var(--color-announcement-text)\n    text-decoration-color: var(--color-announcement-text)\n\n    &:hover\n      color: var(--color-announcement-text)\n      text-decoration-color: var(--color-link--hover)\n\n////////////////////////////////////////////////////////////////////////////////\n// Toggles for theme\n////////////////////////////////////////////////////////////////////////////////\n.no-js .theme-toggle-container  // don't show theme toggle if there's no JS\n  display: none\n\n.theme-toggle-container\n  vertical-align: middle\n\n.theme-toggle\n  cursor: pointer\n  border: none\n  padding: 0\n  background: transparent\n\n.theme-toggle svg\n  vertical-align: middle\n  height: 1rem\n  width: 1rem\n  color: var(--color-foreground-primary)\n  display: none\n\n.theme-toggle-header\n  float: left\n  padding: 1rem 0.5rem\n\n////////////////////////////////////////////////////////////////////////////////\n// Toggles for elements\n////////////////////////////////////////////////////////////////////////////////\n.toc-overlay-icon, .nav-overlay-icon\n  display: none\n  cursor: pointer\n\n  .icon\n    color: var(--color-foreground-secondary)\n    height: 1rem\n    width: 1rem\n\n.toc-header-icon, .nav-overlay-icon\n  // for when we set display: flex\n  justify-content: center\n  align-items: center\n\n.toc-content-icon\n  height: 1.5rem\n  width: 1.5rem\n\n.content-icon-container\n  float: right\n  display: flex\n  margin-top: 1.5rem\n  margin-left: 1rem\n  margin-bottom: 1rem\n  gap: 0.5rem\n\n  .edit-this-page svg\n    color: inherit\n    height: 1rem\n    width: 1rem\n\n.sidebar-toggle\n  position: absolute\n  display: none\n// <debugging things>\n.sidebar-toggle[name=\"__toc\"]\n  left: 20px\n.sidebar-toggle:checked\n  left: 40px\n// </debugging things>\n\n.overlay\n  position: fixed\n  top: 0\n  width: 0\n  height: 0\n\n  transition: width 0ms, height 0ms, opacity 250ms ease-out\n\n  opacity: 0\n  background-color: rgba(0, 0, 0, 0.54)\n.sidebar-overlay\n  z-index: 20\n.toc-overlay\n  z-index: 40\n\n// Keep things on top and smooth.\n.sidebar-drawer\n  z-index: 30\n  transition: left 250ms ease-in-out\n.toc-drawer\n  z-index: 50\n  transition: right 250ms ease-in-out\n\n// Show the Sidebar\n#__navigation:checked\n  & ~ .sidebar-overlay\n    width: 100%\n    height: 100%\n    opacity: 1\n  & ~ .page\n    .sidebar-drawer\n      top: 0\n      left: 0\n      // Show the toc sidebar\n#__toc:checked\n  & ~ .toc-overlay\n    width: 100%\n    height: 100%\n    opacity: 1\n  & ~ .page\n    .toc-drawer\n      top: 0\n      right: 0\n\n////////////////////////////////////////////////////////////////////////////////\n// Back to top\n////////////////////////////////////////////////////////////////////////////////\n.back-to-top\n  text-decoration: none\n\n  display: none\n  position: fixed\n  left: 0\n  top: 1rem\n  padding: 0.5rem\n  padding-right: 0.75rem\n  border-radius: 1rem\n  font-size: 0.8125rem\n\n  background: var(--color-background-primary)\n  box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), #6b728080 0px 0px 1px 0px\n\n  z-index: 10\n\n  margin-left: 50%\n  transform: translateX(-50%)\n  svg\n    height: 1rem\n    width: 1rem\n    fill: currentColor\n    display: inline-block\n\n  span\n    margin-left: 0.25rem\n\n  .show-back-to-top &\n    display: flex\n    align-items: center\n\n////////////////////////////////////////////////////////////////////////////////\n// Responsive layouting\n////////////////////////////////////////////////////////////////////////////////\n// Make things a bit bigger on bigger screens.\n@media (min-width: $full-width + $sidebar-width)\n  html\n    font-size: 110%\n\n@media (max-width: $full-width)\n  // Collapse \"toc\" into the icon.\n  .toc-content-icon\n    display: flex\n  .toc-drawer\n    position: fixed\n    height: 100vh\n    top: 0\n    right: -$sidebar-width\n    border-left: 1px solid var(--color-background-muted)\n  .toc-tree\n    border-left: none\n    font-size: var(--toc-font-size--mobile)\n\n  // Accomodate for a changed content width.\n  .sidebar-drawer\n    width: calc((100% - #{$full-width - $sidebar-width}) / 2 + #{$sidebar-width})\n\n@media (max-width: $full-width - $sidebar-width)\n  // Collapse \"navigation\".\n  .nav-overlay-icon\n    display: flex\n  .sidebar-drawer\n    position: fixed\n    height: 100vh\n    width: $sidebar-width\n\n    top: 0\n    left: -$sidebar-width\n\n  // Swap which icon is visible.\n  .toc-header-icon\n    display: flex\n  .toc-content-icon, .theme-toggle-content\n    display: none\n  .theme-toggle-header\n    display: block\n\n  // Show the header.\n  .mobile-header\n    position: sticky\n    top: 0\n    display: flex\n    justify-content: space-between\n    align-items: center\n\n    .header-left,\n    .header-right\n      display: flex\n      height: var(--header-height)\n      padding: 0 var(--header-padding)\n      label\n        height: 100%\n        width: 100%\n        user-select: none\n\n  // Add a scroll margin for the content\n  :target\n    scroll-margin-top: var(--header-height)\n\n  // Show back-to-top below the header\n  .back-to-top\n    top: calc(var(--header-height) + 0.5rem)\n\n  // Center the page, and accommodate for the header.\n  .page\n    flex-direction: column\n    justify-content: center\n  .content\n    margin-left: auto\n    margin-right: auto\n\n@media (max-width: $content-width + 2* $content-padding)\n  // Content should respect window limits.\n  .content\n    width: 100%\n    overflow-x: auto\n\n@media (max-width: $content-width)\n  .content\n    padding: 0 $content-padding--small\n    // Don't float sidebars to the right.\n  article aside.sidebar\n    float: none\n    width: 100%\n    margin: 1rem 0\n",
+        "// This file contains the styles for the overall layouting of the documentation\n// skeleton, including the responsive changes as well as sidebar toggles.\n//\n// This is implemented as a mobile-last design, which isn't ideal, but it is\n// reasonably good-enough and I got pretty tired by the time I'd finished this\n// to move the rules around to fix this. Shouldn't take more than 3-4 hours,\n// if you know what you're doing tho.\n\n// HACK: Not all browsers account for the scrollbar width in media queries.\n// This results in horizontal scrollbars in the breakpoint where we go\n// from displaying everything to hiding the ToC. We accomodate for this by\n// adding a bit of padding to the TOC drawer, disabling the horizontal\n// scrollbar and allowing the scrollbars to cover the padding.\n// https://www.456bereastreet.com/archive/201301/media_query_width_and_vertical_scrollbars/\n\n// HACK: Always having the scrollbar visible, prevents certain browsers from\n// causing the content to stutter horizontally between taller-than-viewport and\n// not-taller-than-viewport pages.\n\nhtml\n  overflow-x: hidden\n  overflow-y: scroll\n  scroll-behavior: smooth\n\n.sidebar-scroll, .toc-scroll, article[role=main] *\n  // Override Firefox scrollbar style\n  scrollbar-width: thin\n  scrollbar-color: var(--color-foreground-border) transparent\n\n  // Override Chrome scrollbar styles\n  &::-webkit-scrollbar\n    width: 0.25rem\n    height: 0.25rem\n  &::-webkit-scrollbar-thumb\n    background-color: var(--color-foreground-border)\n    border-radius: 0.125rem\n\n//\n// Overalls\n//\nhtml,\nbody\n  height: 100%\n  color: var(--color-foreground-primary)\n  background: var(--color-background-primary)\n\narticle\n  color: var(--color-content-foreground)\n  background: var(--color-content-background)\n\n.page\n  display: flex\n  // fill the viewport for pages with little content.\n  min-height: 100%\n\n.mobile-header\n  width: 100%\n  height: var(--header-height)\n  background-color: var(--color-header-background)\n  color: var(--color-header-text)\n  border-bottom: 1px solid var(--color-header-border)\n\n  // Looks like sub-script/super-script have this, and we need this to\n  // be \"on top\" of those.\n  z-index: 10\n\n  // We don't show the header on large screens.\n  display: none\n\n  // Add shadow when scrolled\n  &.scrolled\n    border-bottom: none\n    box-shadow: 0 0 0.2rem rgba(0, 0, 0, 0.1), 0 0.2rem 0.4rem rgba(0, 0, 0, 0.2)\n\n  .header-center\n    a\n      color: var(--color-header-text)\n      text-decoration: none\n\n.main\n  display: flex\n  flex: 1\n\n// Sidebar (left) also covers the entire left portion of screen.\n.sidebar-drawer\n  box-sizing: border-box\n\n  border-right: 1px solid var(--color-sidebar-background-border)\n  background: var(--color-sidebar-background)\n\n  display: flex\n  justify-content: flex-end\n  // These next two lines took me two days to figure out.\n  width: calc((100% - #{$full-width}) / 2 + #{$sidebar-width})\n  min-width: $sidebar-width\n\n// Scroll-along sidebars\n.sidebar-container,\n.toc-drawer\n  box-sizing: border-box\n  width: $sidebar-width\n\n.toc-drawer\n  background: var(--color-toc-background)\n  // See HACK described on top of this document\n  padding-right: 1rem\n\n.sidebar-sticky,\n.toc-sticky\n  position: sticky\n  top: 0\n  height: min(100%, 100vh)\n  height: 100vh\n\n  display: flex\n  flex-direction: column\n\n.sidebar-scroll,\n.toc-scroll\n  flex-grow: 1\n  flex-shrink: 1\n\n  overflow: auto\n  scroll-behavior: smooth\n\n// Central items.\n.content\n  padding: 0 $content-padding\n  width: $content-width\n\n  display: flex\n  flex-direction: column\n  justify-content: space-between\n\n.icon\n  display: inline-block\n  height: 1rem\n  width: 1rem\n  svg\n    width: 100%\n    height: 100%\n\n//\n// Accommodate announcement banner\n//\n.announcement\n  background-color: var(--color-announcement-background)\n  color: var(--color-announcement-text)\n\n  height: var(--header-height)\n  display: flex\n  align-items: center\n  overflow-x: auto\n  & + .page\n    min-height: calc(100% - var(--header-height))\n\n.announcement-content\n  box-sizing: border-box\n  padding: 0.5rem\n  min-width: 100%\n  white-space: nowrap\n  text-align: center\n\n  a\n    color: var(--color-announcement-text)\n    text-decoration-color: var(--color-announcement-text)\n\n    &:hover\n      color: var(--color-announcement-text)\n      text-decoration-color: var(--color-link--hover)\n\n////////////////////////////////////////////////////////////////////////////////\n// Toggles for theme\n////////////////////////////////////////////////////////////////////////////////\n.no-js .theme-toggle-container  // don't show theme toggle if there's no JS\n  display: none\n\n.theme-toggle-container\n  vertical-align: middle\n\n.theme-toggle\n  cursor: pointer\n  border: none\n  padding: 0\n  background: transparent\n\n.theme-toggle svg\n  vertical-align: middle\n  height: 1rem\n  width: 1rem\n  color: var(--color-foreground-primary)\n  display: none\n\n.theme-toggle-header\n  float: left\n  padding: 1rem 0.5rem\n\n////////////////////////////////////////////////////////////////////////////////\n// Toggles for elements\n////////////////////////////////////////////////////////////////////////////////\n.toc-overlay-icon, .nav-overlay-icon\n  display: none\n  cursor: pointer\n\n  .icon\n    color: var(--color-foreground-secondary)\n    height: 1rem\n    width: 1rem\n\n.toc-header-icon, .nav-overlay-icon\n  // for when we set display: flex\n  justify-content: center\n  align-items: center\n\n.toc-content-icon\n  height: 1.5rem\n  width: 1.5rem\n\n.content-icon-container\n  float: right\n  display: flex\n  margin-top: 1.5rem\n  margin-left: 1rem\n  margin-bottom: 1rem\n  gap: 0.5rem\n\n  .edit-this-page svg\n    color: inherit\n    height: 1rem\n    width: 1rem\n\n.sidebar-toggle\n  position: absolute\n  display: none\n// <debugging things>\n.sidebar-toggle[name=\"__toc\"]\n  left: 20px\n.sidebar-toggle:checked\n  left: 40px\n// </debugging things>\n\n.overlay\n  position: fixed\n  top: 0\n  width: 0\n  height: 0\n\n  transition: width 0ms, height 0ms, opacity 250ms ease-out\n\n  opacity: 0\n  background-color: rgba(0, 0, 0, 0.54)\n.sidebar-overlay\n  z-index: 20\n.toc-overlay\n  z-index: 40\n\n// Keep things on top and smooth.\n.sidebar-drawer\n  z-index: 30\n  transition: left 250ms ease-in-out\n.toc-drawer\n  z-index: 50\n  transition: right 250ms ease-in-out\n\n// Show the Sidebar\n#__navigation:checked\n  & ~ .sidebar-overlay\n    width: 100%\n    height: 100%\n    opacity: 1\n  & ~ .page\n    .sidebar-drawer\n      top: 0\n      left: 0\n      // Show the toc sidebar\n#__toc:checked\n  & ~ .toc-overlay\n    width: 100%\n    height: 100%\n    opacity: 1\n  & ~ .page\n    .toc-drawer\n      top: 0\n      right: 0\n\n////////////////////////////////////////////////////////////////////////////////\n// Back to top\n////////////////////////////////////////////////////////////////////////////////\n.back-to-top\n  text-decoration: none\n\n  display: none\n  position: fixed\n  left: 0\n  top: 1rem\n  padding: 0.5rem\n  padding-right: 0.75rem\n  border-radius: 1rem\n  font-size: 0.8125rem\n\n  background: var(--color-background-primary)\n  box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), #6b728080 0px 0px 1px 0px\n\n  z-index: 10\n\n  margin-left: 50%\n  transform: translateX(-50%)\n  svg\n    height: 1rem\n    width: 1rem\n    fill: currentColor\n    display: inline-block\n\n  span\n    margin-left: 0.25rem\n\n  .show-back-to-top &\n    display: flex\n    align-items: center\n\n////////////////////////////////////////////////////////////////////////////////\n// Responsive layouting\n////////////////////////////////////////////////////////////////////////////////\n// Make things a bit bigger on bigger screens.\n@media (min-width: $full-width + $sidebar-width)\n  html\n    font-size: 110%\n\n@media (max-width: $full-width)\n  // Collapse \"toc\" into the icon.\n  .toc-content-icon\n    display: flex\n  .toc-drawer\n    position: fixed\n    height: 100vh\n    top: 0\n    right: -$sidebar-width\n    border-left: 1px solid var(--color-background-muted)\n  .toc-tree\n    border-left: none\n    font-size: var(--toc-font-size--mobile)\n\n  // Accomodate for a changed content width.\n  .sidebar-drawer\n    width: calc((100% - #{$full-width - $sidebar-width}) / 2 + #{$sidebar-width})\n\n@media (max-width: $full-width - $sidebar-width)\n  // Collapse \"navigation\".\n  .nav-overlay-icon\n    display: flex\n  .sidebar-drawer\n    position: fixed\n    height: 100vh\n    width: $sidebar-width\n\n    top: 0\n    left: -$sidebar-width\n\n  // Swap which icon is visible.\n  .toc-header-icon\n    display: flex\n  .toc-content-icon, .theme-toggle-content\n    display: none\n  .theme-toggle-header\n    display: block\n\n  // Show the header.\n  .mobile-header\n    position: sticky\n    top: 0\n    display: flex\n    justify-content: space-between\n    align-items: center\n\n    .header-left,\n    .header-right\n      display: flex\n      height: var(--header-height)\n      padding: 0 var(--header-padding)\n      label\n        height: 100%\n        width: 100%\n        user-select: none\n\n  .nav-overlay-icon .icon,\n  .theme-toggle svg\n    height: 1.25rem\n    width: 1.25rem\n\n  // Add a scroll margin for the content\n  :target\n    scroll-margin-top: var(--header-height)\n\n  // Show back-to-top below the header\n  .back-to-top\n    top: calc(var(--header-height) + 0.5rem)\n\n  // Center the page, and accommodate for the header.\n  .page\n    flex-direction: column\n    justify-content: center\n  .content\n    margin-left: auto\n    margin-right: auto\n\n@media (max-width: $content-width + 2* $content-padding)\n  // Content should respect window limits.\n  .content\n    width: 100%\n    overflow-x: auto\n\n@media (max-width: $content-width)\n  .content\n    padding: 0 $content-padding--small\n    // Don't float sidebars to the right.\n  article aside.sidebar\n    float: none\n    width: 100%\n    margin: 1rem 0\n",
         "// Overall Layout Variables\n//\n// Because CSS variables can't be used in media queries. The fact that this\n// makes the layout non-user-configurable is a good thing.\n$content-padding: 3em;\n$content-padding--small: 1em;\n$content-width: 46em;\n$sidebar-width: 15em;\n$full-width: $content-width + 2 * ($content-padding + $sidebar-width);\n",
         "//\n// The design here is strongly inspired by mkdocs-material.\n.admonition, .topic\n  margin: 1rem auto\n  padding: 0 0.5rem 0.5rem 0.5rem\n\n  background: var(--color-admonition-background)\n\n  border-radius: 0.2rem\n  box-shadow: 0 0.2rem 0.5rem rgba(0, 0, 0, 0.05), 0 0 0.0625rem rgba(0, 0, 0, 0.1)\n\n  font-size: var(--admonition-font-size)\n\n  overflow: hidden\n  page-break-inside: avoid\n\n  // First element should have no margin, since the title has it.\n  > :nth-child(2)\n    margin-top: 0\n\n  // Last item should have no margin, since we'll control that w/ padding\n  > :last-child\n    margin-bottom: 0\n\np.admonition-title, p.topic-title\n  position: relative\n  margin: 0 -0.5rem 0.5rem\n  padding-left: 2rem\n  padding-right: .5rem\n  padding-top: .4rem\n  padding-bottom: .4rem\n\n  font-weight: 500\n  font-size: var(--admonition-title-font-size)\n  line-height: 1.3\n\n    // Our fancy icon\n  &::before\n    content: \"\"\n    position: absolute\n    left: 0.5rem\n    width: 1rem\n    height: 1rem\n\n// Default styles\np.admonition-title\n  background-color: var(--color-admonition-title-background)\n  &::before\n    background-color: var(--color-admonition-title)\n    mask-image: var(--icon-admonition-default)\n    mask-repeat: no-repeat\n\np.topic-title\n  background-color: var(--color-topic-title-background)\n  &::before\n    background-color: var(--color-topic-title)\n    mask-image: var(--icon-topic-default)\n    mask-repeat: no-repeat\n\n//\n// Variants\n//\n.admonition\n  border-left: 0.2rem solid var(--color-admonition-title)\n\n  @each $type, $value in $admonitions\n    &.#{$type}\n      border-left-color: var(--color-admonition-title--#{$type})\n      > .admonition-title\n        background-color: var(--color-admonition-title-background--#{$type})\n        &::before\n          background-color: var(--color-admonition-title--#{$type})\n          mask-image: var(--icon-#{nth($value, 2)})\n\n.admonition-todo > .admonition-title\n  text-transform: uppercase\n",
-        "// This file stylizes the API documentation (stuff generated by autodoc). It's\n// deeply nested due to how autodoc structures the HTML without enough classes\n// to select the relevant items.\n\n// API docs!\ndl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)\n  // Tweak the spacing of all the things!\n  dd\n    margin-left: 2rem\n    > :first-child\n      margin-top: 0.125rem\n    > :last-child\n      margin-bottom: 0.75rem\n\n  // This is used for the arguments\n  .field-list\n    margin-bottom: 0.75rem\n\n    // \"Headings\" (like \"Parameters\" and \"Return\")\n    > dt\n      text-transform: uppercase\n      font-size: var(--font-size--small)\n\n    dd:empty\n      margin-bottom: 0.5rem\n    dd > ul\n      margin-left: -1.2rem\n      > li\n        > p:nth-child(2)\n          margin-top: 0\n        // When the last-empty-paragraph follows a paragraph, it doesn't need\n        // to augument the existing spacing.\n        > p + p:last-child:empty\n          margin-top: 0\n          margin-bottom: 0\n\n  // Colorize the elements\n  > dt\n    color: var(--color-api-overall)\n\n.sig:not(.sig-inline)\n  font-weight: bold\n\n  font-size: var(--api-font-size)\n  font-family: var(--font-stack--monospace)\n\n  padding-top: 0.25rem\n  padding-bottom: 0.25rem\n  padding-right: 0.5rem\n\n  // These are intentionally em, to properly match the font size.\n  padding-left: 3em\n  text-indent: -2.5em\n\n  border-radius: 0.25rem\n\n  background: var(--color-api-background)\n\n  &:hover\n    background: var(--color-api-background-hover)\n\n  // adjust the size of the [source] link on the right.\n  a.reference\n    .viewcode-link\n      font-weight: normal\n      width: 3.5rem\n\n  // Break words when they're too long\n  span.pre\n    overflow-wrap: anywhere\n\nem.property\n  font-style: normal\n  &:first-child\n    color: var(--color-api-keyword)\n.sig-name\n  color: var(--color-api-name)\n.sig-prename\n  font-weight: normal\n  color: var(--color-api-pre-name)\n.sig-paren\n  color: var(--color-api-paren)\n.sig-param\n  font-style: normal\n\n.versionmodified\n  font-style: italic\ndiv.versionadded, div.versionchanged, div.deprecated\n  p\n    margin-top: 0.125rem\n    margin-bottom: 0.125rem\n\n// Align the [docs] and [source] to the right.\n.viewcode-link, .viewcode-back\n  float: right\n  text-align: right\n",
+        "// This file stylizes the API documentation (stuff generated by autodoc). It's\n// deeply nested due to how autodoc structures the HTML without enough classes\n// to select the relevant items.\n\n// API docs!\ndl[class]:not(.option-list):not(.field-list):not(.footnote):not(.glossary):not(.simple)\n  // Tweak the spacing of all the things!\n  dd\n    margin-left: 2rem\n    > :first-child\n      margin-top: 0.125rem\n    > :last-child\n      margin-bottom: 0.75rem\n\n  // This is used for the arguments\n  .field-list\n    margin-bottom: 0.75rem\n\n    // \"Headings\" (like \"Parameters\" and \"Return\")\n    > dt\n      text-transform: uppercase\n      font-size: var(--font-size--small)\n\n    dd:empty\n      margin-bottom: 0.5rem\n    dd > ul\n      margin-left: -1.2rem\n      > li\n        > p:nth-child(2)\n          margin-top: 0\n        // When the last-empty-paragraph follows a paragraph, it doesn't need\n        // to augument the existing spacing.\n        > p + p:last-child:empty\n          margin-top: 0\n          margin-bottom: 0\n\n  // Colorize the elements\n  > dt\n    color: var(--color-api-overall)\n\n.sig:not(.sig-inline)\n  font-weight: bold\n\n  font-size: var(--api-font-size)\n  font-family: var(--font-stack--monospace)\n\n  margin-left: -0.25rem\n  margin-right: -0.25rem\n  padding-top: 0.25rem\n  padding-bottom: 0.25rem\n  padding-right: 0.5rem\n\n  // These are intentionally em, to properly match the font size.\n  padding-left: 3em\n  text-indent: -2.5em\n\n  border-radius: 0.25rem\n\n  background: var(--color-api-background)\n  transition: background 100ms ease-out\n\n  &:hover\n    background: var(--color-api-background-hover)\n\n  // adjust the size of the [source] link on the right.\n  a.reference\n    .viewcode-link\n      font-weight: normal\n      width: 3.5rem\n\n  // Break words when they're too long\n  span.pre\n    overflow-wrap: anywhere\n\nem.property\n  font-style: normal\n  &:first-child\n    color: var(--color-api-keyword)\n.sig-name\n  color: var(--color-api-name)\n.sig-prename\n  font-weight: normal\n  color: var(--color-api-pre-name)\n.sig-paren\n  color: var(--color-api-paren)\n.sig-param\n  font-style: normal\n\n.versionmodified\n  font-style: italic\ndiv.versionadded, div.versionchanged, div.deprecated\n  p\n    margin-top: 0.125rem\n    margin-bottom: 0.125rem\n\n// Align the [docs] and [source] to the right.\n.viewcode-link, .viewcode-back\n  float: right\n  text-align: right\n",
         ".line-block\n  margin-top: 0.5rem\n  margin-bottom: 0.75rem\n  .line-block\n    margin-top: 0rem\n    margin-bottom: 0rem\n    padding-left: 1rem\n",
         "// Captions\narticle p.caption,\ntable > caption,\n.code-block-caption\n  font-size: var(--font-size--small)\n  text-align: center\n\n// Caption above a TOCTree\n.toctree-wrapper.compound\n  .caption, :not(.caption) > .caption-text\n    font-size: var(--font-size--small)\n    text-transform: uppercase\n\n    text-align: initial\n    margin-bottom: 0\n\n  > ul\n    margin-top: 0\n    margin-bottom: 0\n",
-        "// Inline code\ncode.literal, .sig-inline\n  background: var(--color-inline-code-background)\n  border-radius: 0.2em\n  // Make the font smaller, and use padding to recover.\n  font-size: var(--font-size--small--2)\n  padding: 0.1em 0.2em\n\n  p &\n    border: 1px solid var(--color-background-border)\n\n.sig-inline\n  font-family: var(--font-stack--monospace)\n\n// Code and Literal Blocks\n$code-spacing-vertical: 0.625rem\n$code-spacing-horizontal: 0.875rem\n\n// Wraps every literal block + line numbers.\ndiv[class*=\" highlight-\"],\ndiv[class^=\"highlight-\"]\n  margin: 1em 0\n  display: flex\n\n  .table-wrapper\n    margin: 0\n    padding: 0\n\npre\n  margin: 0\n  padding: 0\n\n  // Needed to have more specificity than pygments' \"pre\" selector. :(\n  article[role=\"main\"] .highlight &\n    line-height: 1.5\n\n  &.literal-block,\n  .highlight &\n    font-size: var(--code-font-size)\n    padding: $code-spacing-vertical $code-spacing-horizontal\n    overflow: auto\n\n  // Make it look like all the other blocks.\n  &.literal-block\n    margin-top: 1rem\n    margin-bottom: 1rem\n\n    border-radius: 0.2rem\n    background-color: var(--color-code-background)\n    color: var(--color-code-foreground)\n\n// All code is always contained in this.\n.highlight\n  width: 100%\n  border-radius: 0.2rem\n\n  // Make line numbers and prompts un-selectable.\n  .gp, span.linenos\n    user-select: none\n    pointer-events: none\n\n  // Expand the line-highlighting.\n  .hll\n    display: block\n    margin-left: -$code-spacing-horizontal\n    margin-right: -$code-spacing-horizontal\n    padding-left: $code-spacing-horizontal\n    padding-right: $code-spacing-horizontal\n\n/* Make code block captions be nicely integrated */\n.code-block-caption\n  display: flex\n  padding: $code-spacing-vertical $code-spacing-horizontal\n\n  border-radius: 0.25rem\n  border-bottom-left-radius: 0\n  border-bottom-right-radius: 0\n  font-weight: 300\n  border-bottom: 1px solid\n\n  background-color: var(--color-code-background)\n  color: var(--color-code-foreground)\n  border-color: var(--color-background-border)\n\n  + div[class]\n    margin-top: 0\n    pre\n      border-top-left-radius: 0\n      border-top-right-radius: 0\n\n// When `html_codeblock_linenos_style` is table.\n.highlighttable\n  width: 100%\n  display: block\n  tbody\n    display: block\n\n  tr\n    display: flex\n\n  // Line numbers\n  td.linenos\n    background-color: var(--color-code-background)\n    color: var(--color-code-foreground)\n    padding: $code-spacing-vertical $code-spacing-horizontal\n    padding-right: 0\n    border-top-left-radius: 0.2rem\n    border-bottom-left-radius: 0.2rem\n\n  .linenodiv\n    padding-right: $code-spacing-horizontal\n    font-size: var(--code-font-size)\n    box-shadow: -0.0625rem 0 var(--color-foreground-border) inset\n\n  // Actual code\n  td.code\n    padding: 0\n    display: block\n    flex: 1\n    overflow: hidden\n\n    .highlight\n      border-top-left-radius: 0\n      border-bottom-left-radius: 0\n\n// When `html_codeblock_linenos_style` is inline.\n.highlight\n  span.linenos\n    display: inline-block\n    padding-left: 0\n    padding-right: $code-spacing-horizontal\n    margin-right: $code-spacing-horizontal\n    box-shadow: -0.0625rem 0 var(--color-foreground-border) inset\n",
+        "// Inline code\ncode.literal, .sig-inline\n  background: var(--color-inline-code-background)\n  border-radius: 0.2em\n  // Make the font smaller, and use padding to recover.\n  font-size: var(--font-size--small--2)\n  padding: 0.1em 0.2em\n\n  overflow-wrap: break-word\n\n  p &\n    border: 1px solid var(--color-background-border)\n\n.sig-inline\n  font-family: var(--font-stack--monospace)\n\n// Code and Literal Blocks\n$code-spacing-vertical: 0.625rem\n$code-spacing-horizontal: 0.875rem\n\n// Wraps every literal block + line numbers.\ndiv[class*=\" highlight-\"],\ndiv[class^=\"highlight-\"]\n  margin: 1em 0\n  display: flex\n\n  .table-wrapper\n    margin: 0\n    padding: 0\n\npre\n  margin: 0\n  padding: 0\n  overflow: auto\n\n  // Needed to have more specificity than pygments' \"pre\" selector. :(\n  article[role=\"main\"] .highlight &\n    line-height: 1.5\n\n  &.literal-block,\n  .highlight &\n    font-size: var(--code-font-size)\n    padding: $code-spacing-vertical $code-spacing-horizontal\n\n  // Make it look like all the other blocks.\n  &.literal-block\n    margin-top: 1rem\n    margin-bottom: 1rem\n\n    border-radius: 0.2rem\n    background-color: var(--color-code-background)\n    color: var(--color-code-foreground)\n\n// All code is always contained in this.\n.highlight\n  width: 100%\n  border-radius: 0.2rem\n\n  // Make line numbers and prompts un-selectable.\n  .gp, span.linenos\n    user-select: none\n    pointer-events: none\n\n  // Expand the line-highlighting.\n  .hll\n    display: block\n    margin-left: -$code-spacing-horizontal\n    margin-right: -$code-spacing-horizontal\n    padding-left: $code-spacing-horizontal\n    padding-right: $code-spacing-horizontal\n\n/* Make code block captions be nicely integrated */\n.code-block-caption\n  display: flex\n  padding: $code-spacing-vertical $code-spacing-horizontal\n\n  border-radius: 0.25rem\n  border-bottom-left-radius: 0\n  border-bottom-right-radius: 0\n  font-weight: 300\n  border-bottom: 1px solid\n\n  background-color: var(--color-code-background)\n  color: var(--color-code-foreground)\n  border-color: var(--color-background-border)\n\n  + div[class]\n    margin-top: 0\n    pre\n      border-top-left-radius: 0\n      border-top-right-radius: 0\n\n// When `html_codeblock_linenos_style` is table.\n.highlighttable\n  width: 100%\n  display: block\n  tbody\n    display: block\n\n  tr\n    display: flex\n\n  // Line numbers\n  td.linenos\n    background-color: var(--color-code-background)\n    color: var(--color-code-foreground)\n    padding: $code-spacing-vertical $code-spacing-horizontal\n    padding-right: 0\n    border-top-left-radius: 0.2rem\n    border-bottom-left-radius: 0.2rem\n\n  .linenodiv\n    padding-right: $code-spacing-horizontal\n    font-size: var(--code-font-size)\n    box-shadow: -0.0625rem 0 var(--color-foreground-border) inset\n\n  // Actual code\n  td.code\n    padding: 0\n    display: block\n    flex: 1\n    overflow: hidden\n\n    .highlight\n      border-top-left-radius: 0\n      border-bottom-left-radius: 0\n\n// When `html_codeblock_linenos_style` is inline.\n.highlight\n  span.linenos\n    display: inline-block\n    padding-left: 0\n    padding-right: $code-spacing-horizontal\n    margin-right: $code-spacing-horizontal\n    box-shadow: -0.0625rem 0 var(--color-foreground-border) inset\n",
         "// Inline Footnote Reference\n.footnote-reference\n  font-size: var(--font-size--small--4)\n  vertical-align: super\n\n// Definition list, listing the content of each note.\n// docutils <= 0.17\ndl.footnote.brackets\n  font-size: var(--font-size--small)\n  color: var(--color-foreground-secondary)\n\n  display: grid\n  grid-template-columns: max-content auto\n  dt\n    margin: 0\n    > .fn-backref\n      margin-left: 0.25rem\n\n    &:after\n      content: \":\"\n\n    .brackets\n      &:before\n        content: \"[\"\n      &:after\n        content: \"]\"\n\n  dd\n    margin: 0\n    padding: 0 1rem\n\n// docutils >= 0.18\naside.footnote\n  font-size: var(--font-size--small)\n  color: var(--color-foreground-secondary)\n\naside.footnote > span,\ndiv.citation > span\n  float: left\n  font-weight: 500\n  padding-right: 0.25rem\n\naside.footnote > p,\ndiv.citation > p\n  margin-left: 2rem\n",
         "//\n// Figures\n//\nimg\n  box-sizing: border-box\n  max-width: 100%\n  height: auto\n\narticle\n  figure, .figure\n    border-radius: 0.2rem\n\n    margin: 0\n    :last-child\n      margin-bottom: 0\n\n  .align-left\n    float: left\n    clear: left\n    margin: 0 1rem 1rem\n\n  .align-right\n    float: right\n    clear: right\n    margin: 0 1rem 1rem\n\n  .align-default,\n  .align-center\n    display: block\n    text-align: center\n    margin-left: auto\n    margin-right: auto\n\n  // WELL, table needs to be stylised like a table.\n  table.align-default\n    display: table\n    text-align: initial\n",
         ".genindex-jumpbox, .domainindex-jumpbox\n  border-top: 1px solid var(--color-background-border)\n  border-bottom: 1px solid var(--color-background-border)\n  padding: 0.25rem\n\n.genindex-section, .domainindex-section\n  h2\n    margin-top: 0.75rem\n    margin-bottom: 0.5rem\n  ul\n    margin-top: 0\n    margin-bottom: 0\n",
         "ul,\nol\n  padding-left: 1.2rem\n\n  // Space lists out like paragraphs\n  margin-top: 1rem\n  margin-bottom: 1rem\n  // reduce margins within li.\n  li\n    > p:first-child\n      margin-top: 0.25rem\n      margin-bottom: 0.25rem\n\n    > p:last-child\n      margin-top: 0.25rem\n\n    > ul,\n    > ol\n      margin-top: 0.5rem\n      margin-bottom: 0.5rem\n\nol\n  &.arabic\n    list-style: decimal\n  &.loweralpha\n    list-style: lower-alpha\n  &.upperalpha\n    list-style: upper-alpha\n  &.lowerroman\n    list-style: lower-roman\n  &.upperroman\n    list-style: upper-roman\n\n// Don't space lists out when they're \"simple\" or in a `.. toctree::`\n.simple,\n.toctree-wrapper\n  li\n    > ul,\n    > ol\n      margin-top: 0\n      margin-bottom: 0\n\n// Definition Lists\n.field-list,\n.option-list,\ndl:not([class]),\ndl.simple,\ndl.footnote,\ndl.glossary\n  dt\n    font-weight: 500\n    margin-top: 0.25rem\n    + dt\n      margin-top: 0\n\n    .classifier::before\n      content: \":\"\n      margin-left: 0.2rem\n      margin-right: 0.2rem\n\n  dd\n    > p:first-child,\n    ul\n      margin-top: 0.125rem\n\n    ul\n      margin-bottom: 0.125rem\n",
         ".math-wrapper\n  width: 100%\n  overflow-x: auto\n\ndiv.math\n  position: relative\n  text-align: center\n\n  .headerlink,\n  &:focus .headerlink\n    display: none\n\n  &:hover .headerlink\n    display: inline-block\n\n  span.eqno\n    position: absolute\n    right: 0.5rem\n    top: 50%\n    transform: translate(0, -50%)\n    z-index: 1\n",
         "// Abbreviations\nabbr[title]\n  cursor: help\n\n// \"Problematic\" content, as identified by Sphinx\n.problematic\n  color: var(--color-problematic)\n\n// Keyboard / Mouse \"instructions\"\nkbd:not(.compound)\n  margin: 0 0.2rem\n  padding: 0 0.2rem\n  border-radius: 0.2rem\n  border: 1px solid var(--color-foreground-border)\n  color: var(--color-foreground-primary)\n  vertical-align: text-bottom\n\n  font-size: var(--font-size--small--3)\n  display: inline-block\n\n  box-shadow: 0 0.0625rem 0 rgba(0, 0, 0, 0.2), inset 0 0 0 0.125rem var(--color-background-primary)\n\n  background-color: var(--color-background-secondary)\n\n// Blockquote\nblockquote\n  border-left: 4px solid var(--color-background-border)\n  background: var(--color-background-secondary)\n\n  margin-left: 0\n  margin-right: 0\n  padding: 0.5rem 1rem\n\n  .attribution\n    font-weight: 600\n    text-align: right\n\n  &.pull-quote,\n  &.highlights\n    font-size: 1.25em\n\n  &.epigraph,\n  &.pull-quote\n    border-left-width: 0\n    border-radius: 0.5rem\n\n  &.highlights\n    border-left-width: 0\n    background: transparent\n\n// Center align embedded-in-text images\np .reference img\n  vertical-align: middle\n",
         "p.rubric\n  line-height: 1.25\n  font-weight: bold\n  font-size: 1.125em\n\n  // For Numpy-style documentation that's got rubrics within it.\n  // https://github.com/pradyunsg/furo/discussions/505\n  dd &\n    line-height: inherit\n    font-weight: inherit\n\n    font-size: var(--font-size--small)\n    text-transform: uppercase\n",
```

### Comparing `gmpacket-0.1.2/docs/_static/tabs.css` & `gmpacket-0.1.3/docs/_static/tabs.css`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/tabs.js` & `gmpacket-0.1.3/docs/_static/tabs.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/underscore-1.13.1.js` & `gmpacket-0.1.3/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/_static/underscore.js` & `gmpacket-0.1.3/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/docs/cli.html` & `gmpacket-0.1.3/docs/dev.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Demo" href="demo.html" /><link rel="prev" title="Examples" href="examples.html" />
+<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="Pydantic Demo" href="pydantic_demo.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Command Line Tools - Ground Motion Packet Documentation</title>
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>Developer Notes - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
@@ -156,33 +156,32 @@
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
 <li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
+<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
       </div>
       
@@ -209,86 +208,57 @@
           </div>
           <label class="toc-overlay-icon toc-content-icon" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="command-line-tools">
-<h1>Command Line Tools<a class="headerlink" href="#command-line-tools" title="Permalink to this heading">#</a></h1>
-<p>This respository contains some command line tools that are meant to assist in reading,
-parsing, and validating the ground motion data packet format. This is a python package
-that can be imported and the functions can be called directly in new scripts, jupyter
-notebooks, or interactive python sessions. An example session is given in the
-<a class="reference internal" href="demo.html"><span class="doc std std-doc">Demo</span></a> section.</p>
-<section id="installation">
-<h2>Installation<a class="headerlink" href="#installation" title="Permalink to this heading">#</a></h2>
-<p>The basic dependencies are <code class="docutils literal notranslate"><span class="pre">pip</span></code> and <code class="docutils literal notranslate"><span class="pre">git</span></code>.</p>
-<p>The main python dependency is the
-<a class="reference external" href="http://seismicdata.github.io/SEIS-PROV/validation.html#official-validator">SEIS-PROV validator</a>.
-To install:</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>git<span class="w"> </span>clone<span class="w"> </span>https://github.com/SeismicData/SEIS-PROV.git
-<span class="nb">cd</span><span class="w"> </span>SEIS-PROV/validator
-pip<span class="w"> </span>install<span class="w"> </span>-e<span class="w"> </span>.
+          <section id="developer-notes">
+<h1>Developer Notes<a class="headerlink" href="#developer-notes" title="Permalink to this heading">#</a></h1>
+<p>We welcome comments and contributions through github issues.</p>
+<section id="documentation">
+<h2>Documentation<a class="headerlink" href="#documentation" title="Permalink to this heading">#</a></h2>
+<p>Never edit the contents of the <code class="docutils literal notranslate"><span class="pre">docs</span></code> directory, only edit files in the <code class="docutils literal notranslate"><span class="pre">doc_source</span></code>
+directory.</p>
+<p>To build this documentation, it is convenient to create a conda virtual environment
+with <a class="reference external" href="https://github.com/mamba-org/mamba">mamba</a> (note that mamba can be installed
+with <a class="reference external" href="https://docs.conda.io/en/latest/">conda</a>).</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">cd</span> <span class="n">doc_source</span>
+<span class="n">mamba</span> <span class="n">create</span> <span class="o">-</span><span class="n">n</span> <span class="n">gmpdocs</span> <span class="n">python</span><span class="o">=</span><span class="mf">3.9</span> <span class="o">--</span><span class="n">file</span> <span class="n">requirements</span><span class="o">.</span><span class="n">txt</span>
+<span class="n">conda</span> <span class="n">activate</span> <span class="n">gmpdocs</span>
 </pre></div>
 </div>
-<p>We also need the “schema” package:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="n">schema</span>
+<p>Then install the python packages as described  in the
+<a class="reference internal" href="getting_started.html"><span class="doc std std-doc">Getting Started</span></a> section. For the demo, we’ll also need</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="n">ipyleaflet</span>
+<span class="n">jupyter</span> <span class="n">nbextension</span> <span class="n">enable</span> <span class="o">--</span><span class="n">py</span> <span class="n">widgetsnbextension</span>
 </pre></div>
 </div>
-<p>Then, to install this package:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">git</span> <span class="n">clone</span> <span class="n">https</span><span class="p">:</span><span class="o">//</span><span class="n">github</span><span class="o">.</span><span class="n">com</span><span class="o">/</span><span class="n">SCEDC</span><span class="o">/</span><span class="n">ground</span><span class="o">-</span><span class="n">motion</span><span class="o">-</span><span class="n">packet</span><span class="o">.</span><span class="n">git</span>
-<span class="n">cd</span> <span class="n">ground</span><span class="o">-</span><span class="n">motion</span><span class="o">-</span><span class="n">packet</span>
-<span class="n">pip</span> <span class="n">install</span> <span class="o">-</span><span class="n">e</span> <span class="o">.</span>
-</pre></div>
-</div>
-</section>
-<section id="usage">
-<h2>Usage<a class="headerlink" href="#usage" title="Permalink to this heading">#</a></h2>
-<p>The installed program is called <code class="docutils literal notranslate"><span class="pre">gmpformat</span></code>:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span>$ gmpformat -h
-usage: gmpformat [-h] {print,csv,validate} ...
-
-This is a program for describing, validating, and converting Ground Motion Packet (GMP) formatted data.
-
-optional arguments:
-  -h, --help            show this help message and exit
-
-subcommands:
-  {print,csv,validate}
-    print               Print GMP file contents.
-    csv                 Convert GMP file contents to a CSV flatfile.
-    validate            Validate a GMP file; will print encountered error messages.
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">./</span><span class="n">makedocs</span><span class="o">.</span><span class="n">sh</span>
 </pre></div>
 </div>
+<p>The above script builds the docs html in the <code class="docutils literal notranslate"><span class="pre">docs</span></code> subdirectory. It can be previewed
+locally by opening <code class="docutils literal notranslate"><span class="pre">docs/index.html</span></code> in a browser.</p>
 </section>
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="demo.html">
-              <div class="page-info">
-                <div class="context">
-                  <span>Next</span>
-                </div>
-                <div class="title">Demo</div>
-              </div>
-              <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
-            </a>
-          <a class="prev-page" href="examples.html">
+          
+          <a class="prev-page" href="pydantic_demo.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Examples</div>
+                <div class="title">Pydantic Demo</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
@@ -321,17 +291,16 @@
           <span class="toc-title">
             On this page
           </span>
         </div>
         <div class="toc-tree-container">
           <div class="toc-tree">
             <ul>
-<li><a class="reference internal" href="#">Command Line Tools</a><ul>
-<li><a class="reference internal" href="#installation">Installation</a></li>
-<li><a class="reference internal" href="#usage">Usage</a></li>
+<li><a class="reference internal" href="#">Developer Notes</a><ul>
+<li><a class="reference internal" href="#documentation">Documentation</a></li>
 </ul>
 </li>
 </ul>
 
           </div>
         </div>
       </div>
```

#### html2text {}

```diff
@@ -25,79 +25,55 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Command Line Tools# ******
-This respository contains some command line tools that are meant to assist in
-reading, parsing, and validating the ground motion data packet format. This is
-a python package that can be imported and the functions can be called directly
-in new scripts, jupyter notebooks, or interactive python sessions. An example
-session is given in the Demo section.
-***** Installation# *****
-The basic dependencies are pip and git.
-The main python dependency is the SEIS-PROV_validator. To install:
-git clone https://github.com/SeismicData/SEIS-PROV.git
-cd SEIS-PROV/validator
-pip install -e .
-We also need the âschemaâ package:
-pip install schema
-Then, to install this package:
-git clone https://github.com/SCEDC/ground-motion-packet.git
-cd ground-motion-packet
-pip install -e .
-
-***** Usage# *****
-The installed program is called gmpformat:
-$ gmpformat -h
-usage: gmpformat [-h] {print,csv,validate} ...
-
-This is a program for describing, validating, and converting Ground Motion
-Packet (GMP) formatted data.
-
-optional arguments:
-  -h, --help            show this help message and exit
-
-subcommands:
-  {print,csv,validate}
-    print               Print GMP file contents.
-    csv                 Convert GMP file contents to a CSV flatfile.
-    validate            Validate a GMP file; will print encountered error
-messages.
-
-Next
-Demo
+****** Developer Notes# ******
+We welcome comments and contributions through github issues.
+***** Documentation# *****
+Never edit the contents of the docs directory, only edit files in the
+doc_source directory.
+To build this documentation, it is convenient to create a conda virtual
+environment with mamba (note that mamba can be installed with conda).
+cd doc_source
+mamba create -n gmpdocs python=3.9 --file requirements.txt
+conda activate gmpdocs
+Then install the python packages as described in the Getting_Started section.
+For the demo, weâll also need
+pip install ipyleaflet
+jupyter nbextension enable --py widgetsnbextension
+./makedocs.sh
+The above script builds the docs html in the docs subdirectory. It can be
+previewed locally by opening docs/index.html in a browser.
 
 Previous
-Examples
+Pydantic_Demo
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
  On this page
-    * Command_Line_Tools
-          o Installation
-          o Usage
+    * Developer_Notes
+          o Documentation
```

### Comparing `gmpacket-0.1.2/docs/demo.html` & `gmpacket-0.1.3/docs/specification/features/metrics_dict.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Pydantic Demo" href="pydantic_demo.html" /><link rel="prev" title="Command Line Tools" href="cli.html" />
+<link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" /><link rel="next" title="GMP Examples" href="../../examples.html" /><link rel="prev" title="Streams and Traces" href="streams_traces.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Demo - Ground Motion Packet Documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
-    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
-    <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
-    <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
-    <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
-    <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>Metrics Dictionary - Ground Motion Packet Documentation</title>
+      <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
+    <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/tabs.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/css/custom.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
+    <link rel="stylesheet" type="text/css" href="../../_static/pied-piper-admonition.css" />
     
     
 
 
 <style>
   body {
     --color-code-background: #f8f8f8;
@@ -124,15 +124,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
+      <a href="../../index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -144,45 +144,44 @@
         <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
       </label>
     </div>
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
-      <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
+      <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
   <span class="sidebar-brand-text">Ground Motion Packet Documentation</span>
   
-</a><form class="sidebar-search-container" method="get" action="search.html" role="search">
+</a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
-<li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
-<li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
-<li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
-<li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
-<li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
-<li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
-<li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
-<li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../getting_started.html">Getting Started</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../geojson.html">GeoJSON Overview</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../terms.html">Terminology</a></li>
+<li class="toctree-l1 current has-children"><a class="reference internal" href="../index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
+<li class="toctree-l2"><a class="reference internal" href="../base.html">Base Dictionary</a></li>
+<li class="toctree-l2"><a class="reference internal" href="../event.html">Event</a></li>
+<li class="toctree-l2"><a class="reference internal" href="../provenance.html">Provenance</a></li>
+<li class="toctree-l2 current has-children"><a class="reference internal" href="index.html">Features</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
+<li class="toctree-l3"><a class="reference internal" href="station.html">Stations</a></li>
+<li class="toctree-l3"><a class="reference internal" href="streams_traces.html">Streams and Traces</a></li>
+<li class="toctree-l3 current current-page"><a class="current reference internal" href="#">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../examples.html">GMP Examples</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../pydantic_demo.html">Pydantic Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
       </div>
       
@@ -209,116 +208,139 @@
           </div>
           <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="demo">
-<h1>Demo<a class="headerlink" href="#demo" title="Permalink to this heading">#</a></h1>
-<p>Be sure to install the python packages as described
-in the <a class="reference internal" href="cli.html"><span class="doc std std-doc">Command Line Tools</span></a> section.</p>
-<p>Also, for this demo specifically, also install ipyleaflet with</p>
-<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>pip<span class="w"> </span>install<span class="w"> </span>ipyleaflet
-jupyter<span class="w"> </span>nbextension<span class="w"> </span><span class="nb">enable</span><span class="w"> </span>--py<span class="w"> </span>widgetsnbextension
+          <section id="metrics-dictionary">
+<h1>Metrics Dictionary<a class="headerlink" href="#metrics-dictionary" title="Permalink to this heading">#</a></h1>
+<p>The “metrics” dictionary contains the values and metadata relevant for the
+metrics associated with the parent trace. One challenge with ground motion
+metric data is that different metrics exhibit very different structure. For
+example, some metrics are simply scalars (e.g., PGA) while others are arrays
+(e.g., response spectra, which are a function of both oscillator period and
+the assumed percent of critical damping).</p>
+<p>While it is possible to list each metric as a separate element in a list, there
+are two main drawbacks to doing so:</p>
+<ol class="arabic simple">
+<li><p>It is inefficient from a file size perspective, and</p></li>
+<li><p>It is difficult to parse because the properties will be different for each
+metric.</p></li>
+</ol>
+<p>Thus, we have designed a general metrics data structure with the goals of
+being easy to extend to a wide range of metric data structures, consistency in
+how the metrics are stored to make parsing the data more straight-forward, and minimizing the file size.</p>
+<p>The dictionary has the following required keys:</p>
+<dl class="simple myst">
+<dt><strong>properties</strong></dt><dd><p>A dictionary with the following keys <em>(dictionary; required)</em>:</p>
+<dl class="simple myst">
+<dt><strong>description</strong></dt><dd><p>Metric description <em>(string; required)</em>.</p>
+</dd>
+<dt><strong>name</strong></dt><dd><p>Metric name <em>(string; required)</em>.</p>
+</dd>
+<dt><strong>units</strong></dt><dd><p>Metric units <em>(string; required)</em>.</p>
+</dd>
+<dt><strong>provenance_ids</strong></dt><dd><p>A list of strings giving provenance IDs relevant to this trace
+<em>(list; optional)</em>.</p>
+</dd>
+<dt><strong>time_of_peak</strong></dt><dd><p>Time of metric peak for the PGA metric in UTC in ISO 8601 <em>extended</em> format
+<em>(str; optional)</em>.</p>
+</dd>
+</dl>
+</dd>
+<dt><strong>dimensions</strong></dt><dd><p>A dictionary with the following keys <em>(dictionary; required when metric is an array)</em>:</p>
+<dl class="simple myst">
+<dt><strong>number</strong></dt><dd><p>The number of dimentions for this metric (<code class="docutils literal notranslate"><span class="pre">n</span></code>)
+<em>(integer; required)</em>.</p>
+</dd>
+<dt><strong>names</strong></dt><dd><p>A list of strings describing the metric dimension names; length must
+be equal to the number of metric dimentions <code class="docutils literal notranslate"><span class="pre">n</span></code>
+<em>(list; required)</em>.</p>
+</dd>
+<dt><strong>units</strong></dt><dd><p>A string or list of strings describing the units of the metric dimensions;
+length must be equal to the number of metric dimentions
+<code class="docutils literal notranslate"><span class="pre">n</span></code> <em>(list; required)</em>.</p>
+</dd>
+<dt><strong>axis_values</strong></dt><dd><p>An array giving the values of the dimensions; the first dimension of
+the array must equal the number of metric dimentions <code class="docutils literal notranslate"><span class="pre">n</span></code>;
+the lengths of each constituent array are are
+<code class="docutils literal notranslate"><span class="pre">[p,</span> <span class="pre">q,</span> <span class="pre">...]</span></code> <em>(array; required)</em>.</p>
+</dd>
+</dl>
+</dd>
+<dt><strong>values</strong></dt><dd><p>An array giving the metric values; the dimensions of the array must be
+equal to the length of each of the dimention value arrays
+<code class="docutils literal notranslate"><span class="pre">p</span> <span class="pre">x</span> <span class="pre">q</span> <span class="pre">x</span> <span class="pre">...</span></code> <em>(float or array; required)</em>.</p>
+</dd>
+</dl>
+<p>An example metrics dictionary:</p>
+<div class="highlight-json notranslate"><div class="highlight"><pre><span></span><span class="w">  </span><span class="err">...</span>
+<span class="w">  </span><span class="nt">&quot;traces&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">      </span><span class="p">{</span>
+<span class="w">          </span><span class="err">...</span>
+<span class="w">          </span><span class="nt">&quot;metrics&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">              </span><span class="p">{</span>
+<span class="w">                  </span><span class="nt">&quot;properties&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
+<span class="w">                      </span><span class="nt">&quot;description&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Spectral acceleration&quot;</span><span class="p">,</span>
+<span class="w">                      </span><span class="nt">&quot;name&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;SA&quot;</span><span class="p">,</span>
+<span class="w">                      </span><span class="nt">&quot;units&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;g&quot;</span><span class="p">,</span>
+<span class="w">                      </span><span class="nt">&quot;provenance_ids&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">                          </span><span class="s2">&quot;seis_prov:sp000_sa_0000000&quot;</span><span class="p">,</span>
+<span class="w">                          </span><span class="s2">&quot;seis_prov:sp000_pp_0000000&quot;</span><span class="p">,</span>
+<span class="w">                          </span><span class="s2">&quot;seis_prov:sp000_og_0000000&quot;</span>
+<span class="w">                      </span><span class="p">]</span>
+<span class="w">                  </span><span class="p">},</span>
+<span class="w">                  </span><span class="nt">&quot;dimensions&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
+<span class="w">                      </span><span class="nt">&quot;number&quot;</span><span class="p">:</span><span class="w"> </span><span class="mi">2</span><span class="p">,</span>
+<span class="w">                      </span><span class="nt">&quot;names&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">                          </span><span class="s2">&quot;critical damping&quot;</span><span class="p">,</span>
+<span class="w">                          </span><span class="s2">&quot;period&quot;</span>
+<span class="w">                      </span><span class="p">],</span>
+<span class="w">                      </span><span class="nt">&quot;units&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span><span class="s2">&quot;%&quot;</span><span class="p">,</span><span class="w"> </span><span class="s2">&quot;s&quot;</span><span class="p">],</span>
+<span class="w">                      </span><span class="nt">&quot;values&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">                          </span><span class="p">[</span><span class="mf">5.0</span><span class="p">,</span><span class="w"> </span><span class="mf">10.0</span><span class="p">,</span><span class="w"> </span><span class="mf">20.0</span><span class="p">],</span>
+<span class="w">                          </span><span class="p">[</span><span class="mf">0.5</span><span class="p">,</span><span class="w"> </span><span class="mf">1.0</span><span class="p">]</span>
+<span class="w">                      </span><span class="p">]</span>
+<span class="w">                  </span><span class="p">},</span>
+<span class="w">                  </span><span class="nt">&quot;values&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">                      </span><span class="p">[</span><span class="mf">2.3</span><span class="p">,</span><span class="w"> </span><span class="mf">2.0</span><span class="p">],</span>
+<span class="w">                      </span><span class="p">[</span><span class="mf">1.6</span><span class="p">,</span><span class="w"> </span><span class="mf">1.4</span><span class="p">],</span>
+<span class="w">                      </span><span class="p">[</span><span class="mf">2.0</span><span class="p">,</span><span class="w"> </span><span class="mf">1.8</span><span class="p">]</span>
+<span class="w">                  </span><span class="p">]</span>
+<span class="w">              </span><span class="p">}</span>
+<span class="w">          </span><span class="p">]</span>
+<span class="w">      </span><span class="p">}</span>
+<span class="w">  </span><span class="p">]</span>
 </pre></div>
 </div>
-<p>The following tutorial can be run in an ipython notebook or in
-an ipython shell.</p>
-<p>We will start with the necessary imports</p>
-<div class="cell docutils container">
-<div class="cell_input docutils container">
-<div class="highlight-ipython3 notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">os</span>
-<span class="kn">import</span> <span class="nn">json</span>
-<span class="kn">import</span> <span class="nn">requests</span>
-<span class="kn">import</span> <span class="nn">pkg_resources</span>
-
-<span class="kn">from</span> <span class="nn">ipyleaflet</span> <span class="kn">import</span> <span class="n">Map</span><span class="p">,</span> <span class="n">GeoJSON</span>
-<span class="kn">from</span> <span class="nn">gmpacket.scan</span> <span class="kn">import</span> <span class="n">scan_gmp</span>
-</pre></div>
-</div>
-</div>
-<div class="cell_output docutils container">
-<div class="output traceback highlight-ipythontb notranslate"><div class="highlight"><pre><span></span><span class="gt">---------------------------------------------------------------------------</span>
-<span class="ne">ModuleNotFoundError</span><span class="g g-Whitespace">                       </span>Traceback (most recent call last)
-<span class="n">Cell</span> <span class="n">In</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="n">line</span> <span class="mi">6</span>
-<span class="g g-Whitespace">      </span><span class="mi">3</span> <span class="kn">import</span> <span class="nn">requests</span>
-<span class="g g-Whitespace">      </span><span class="mi">4</span> <span class="kn">import</span> <span class="nn">pkg_resources</span>
-<span class="ne">----&gt; </span><span class="mi">6</span> <span class="kn">from</span> <span class="nn">ipyleaflet</span> <span class="kn">import</span> <span class="n">Map</span><span class="p">,</span> <span class="n">GeoJSON</span>
-<span class="g g-Whitespace">      </span><span class="mi">7</span> <span class="kn">from</span> <span class="nn">gmpacket.scan</span> <span class="kn">import</span> <span class="n">scan_gmp</span>
-
-<span class="ne">ModuleNotFoundError</span>: No module named &#39;ipyleaflet&#39;
-</pre></div>
-</div>
-</div>
-</div>
-<p>Now we will read in the example data that is in the data directory
-of the gmpacket package</p>
-<div class="cell docutils container">
-<div class="cell_input docutils container">
-<div class="highlight-ipython3 notranslate"><div class="highlight"><pre><span></span><span class="n">datapath</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s1">&#39;data&#39;</span><span class="p">,</span> <span class="s1">&#39;examples&#39;</span><span class="p">,</span> <span class="s1">&#39;sps-100-200-example.json&#39;</span><span class="p">)</span> <span class="c1"># </span>
-<span class="n">data_file</span> <span class="o">=</span> <span class="n">pkg_resources</span><span class="o">.</span><span class="n">resource_filename</span><span class="p">(</span><span class="s1">&#39;gmpacket&#39;</span><span class="p">,</span> <span class="n">datapath</span><span class="p">)</span>
-<span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="n">data_file</span><span class="p">,</span> <span class="s1">&#39;r&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">f</span><span class="p">:</span>
-    <span class="n">data</span> <span class="o">=</span> <span class="n">json</span><span class="o">.</span><span class="n">load</span><span class="p">(</span><span class="n">f</span><span class="p">)</span>
-<span class="n">geo_json</span> <span class="o">=</span> <span class="n">GeoJSON</span><span class="p">(</span><span class="n">data</span><span class="o">=</span><span class="n">data</span><span class="p">)</span>
-</pre></div>
-</div>
-</div>
-</div>
-<p>There is only one feature, so we will grab it to set the center of the map</p>
-<div class="cell docutils container">
-<div class="cell_input docutils container">
-<div class="highlight-ipython3 notranslate"><div class="highlight"><pre><span></span><span class="n">lon</span><span class="p">,</span> <span class="n">lat</span><span class="p">,</span> <span class="n">depth</span> <span class="o">=</span> <span class="n">geo_json</span><span class="o">.</span><span class="n">data</span><span class="p">[</span><span class="s1">&#39;features&#39;</span><span class="p">][</span><span class="mi">0</span><span class="p">][</span><span class="s1">&#39;geometry&#39;</span><span class="p">][</span><span class="s1">&#39;coordinates&#39;</span><span class="p">]</span>
-<span class="n">m</span> <span class="o">=</span> <span class="n">Map</span><span class="p">(</span><span class="n">center</span><span class="o">=</span><span class="p">(</span><span class="n">lat</span><span class="p">,</span> <span class="n">lon</span><span class="p">),</span> <span class="n">zoom</span><span class="o">=</span><span class="mi">7</span><span class="p">)</span>
-<span class="n">m</span><span class="o">.</span><span class="n">add_layer</span><span class="p">(</span><span class="n">geo_json</span><span class="p">)</span>
-<span class="n">m</span>
-</pre></div>
-</div>
-</div>
-</div>
-<p>Now we can use the <code class="docutils literal notranslate"><span class="pre">scan_gmp</span></code> function to print a summary of the example data</p>
-<div class="cell docutils container">
-<div class="cell_input docutils container">
-<div class="highlight-ipython3 notranslate"><div class="highlight"><pre><span></span><span class="n">scan_gmp</span><span class="p">(</span><span class="n">data_file</span><span class="p">,</span> <span class="n">print_what</span><span class="o">=</span><span class="s1">&#39;summary&#39;</span><span class="p">)</span>
-</pre></div>
-</div>
-</div>
-</div>
-<p>We can also change the <code class="docutils literal notranslate"><span class="pre">print_what</span></code> argument to also include the metrics</p>
-<div class="cell docutils container">
-<div class="cell_input docutils container">
-<div class="highlight-ipython3 notranslate"><div class="highlight"><pre><span></span><span class="n">scan_gmp</span><span class="p">(</span><span class="n">data_file</span><span class="p">,</span> <span class="n">print_what</span><span class="o">=</span><span class="s1">&#39;all&#39;</span><span class="p">)</span>
-</pre></div>
-</div>
-</div>
-</div>
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="pydantic_demo.html">
+          <a class="next-page" href="../../examples.html">
               <div class="page-info">
                 <div class="context">
                   <span>Next</span>
                 </div>
-                <div class="title">Pydantic Demo</div>
+                <div class="title">GMP Examples</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
-          <a class="prev-page" href="cli.html">
+          <a class="prev-page" href="streams_traces.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Command Line Tools</div>
+                <div class="title">Streams and Traces</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
@@ -345,19 +367,19 @@
     </div>
     <aside class="toc-drawer no-toc">
       
       
       
     </aside>
   </div>
-</div><script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
-    <script src="_static/scripts/furo.js"></script>
-    <script src="_static/clipboard.min.js"></script>
-    <script src="_static/copybutton.js"></script>
-    <script src="_static/tabs.js"></script>
+</div><script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
+    <script src="../../_static/jquery.js"></script>
+    <script src="../../_static/underscore.js"></script>
+    <script src="../../_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="../../_static/doctools.js"></script>
+    <script src="../../_static/sphinx_highlight.js"></script>
+    <script src="../../_static/scripts/furo.js"></script>
+    <script src="../../_static/clipboard.min.js"></script>
+    <script src="../../_static/copybutton.js"></script>
+    <script src="../../_static/tabs.js"></script>
     </body>
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -25,81 +25,130 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
-    * Specification⁰
+    * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
-          o Features⁰
+          o Features*
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Demo# ******
-Be sure to install the python packages as described in the Command_Line_Tools
-section.
-Also, for this demo specifically, also install ipyleaflet with
-pip install ipyleaflet
-jupyter nbextension enable --py widgetsnbextension
-The following tutorial can be run in an ipython notebook or in an ipython
-shell.
-We will start with the necessary imports
-import os
-import json
-import requests
-import pkg_resources
-
-from ipyleaflet import Map, GeoJSON
-from gmpacket.scan import scan_gmp
----------------------------------------------------------------------------
-ModuleNotFoundError                       Traceback (most recent call last)
-Cell In[1], line 6
-      3 import requests
-      4 import pkg_resources
-----> 6 from ipyleaflet import Map, GeoJSON
-      7 from gmpacket.scan import scan_gmp
-
-ModuleNotFoundError: No module named 'ipyleaflet'
-Now we will read in the example data that is in the data directory of the
-gmpacket package
-datapath = os.path.join('data', 'examples', 'sps-100-200-example.json') #
-data_file = pkg_resources.resource_filename('gmpacket', datapath)
-with open(data_file, 'r') as f:
-    data = json.load(f)
-geo_json = GeoJSON(data=data)
-There is only one feature, so we will grab it to set the center of the map
-lon, lat, depth = geo_json.data['features'][0]['geometry']['coordinates']
-m = Map(center=(lat, lon), zoom=7)
-m.add_layer(geo_json)
-m
-Now we can use the scan_gmp function to print a summary of the example data
-scan_gmp(data_file, print_what='summary')
-We can also change the print_what argument to also include the metrics
-scan_gmp(data_file, print_what='all')
+****** Metrics Dictionary# ******
+The âmetricsâ dictionary contains the values and metadata relevant for the
+metrics associated with the parent trace. One challenge with ground motion
+metric data is that different metrics exhibit very different structure. For
+example, some metrics are simply scalars (e.g., PGA) while others are arrays
+(e.g., response spectra, which are a function of both oscillator period and the
+assumed percent of critical damping).
+While it is possible to list each metric as a separate element in a list, there
+are two main drawbacks to doing so:
+   1. It is inefficient from a file size perspective, and
+   2. It is difficult to parse because the properties will be different for
+      each metric.
+Thus, we have designed a general metrics data structure with the goals of being
+easy to extend to a wide range of metric data structures, consistency in how
+the metrics are stored to make parsing the data more straight-forward, and
+minimizing the file size.
+The dictionary has the following required keys:
+  properties
+      A dictionary with the following keys (dictionary; required):
+        description
+            Metric description (string; required).
+        name
+            Metric name (string; required).
+        units
+            Metric units (string; required).
+        provenance_ids
+            A list of strings giving provenance IDs relevant to this trace
+            (list; optional).
+        time_of_peak
+            Time of metric peak for the PGA metric in UTC in ISO 8601 extended
+            format (str; optional).
+  dimensions
+      A dictionary with the following keys (dictionary; required when metric is
+      an array):
+        number
+            The number of dimentions for this metric (n) (integer; required).
+        names
+            A list of strings describing the metric dimension names; length
+            must be equal to the number of metric dimentions n (list;
+            required).
+        units
+            A string or list of strings describing the units of the metric
+            dimensions; length must be equal to the number of metric dimentions
+            n (list; required).
+        axis_values
+            An array giving the values of the dimensions; the first dimension
+            of the array must equal the number of metric dimentions n; the
+            lengths of each constituent array are are [p, q, ...] (array;
+            required).
+  values
+      An array giving the metric values; the dimensions of the array must be
+      equal to the length of each of the dimention value arrays p x q x ...
+      (float or array; required).
+An example metrics dictionary:
+  ...
+  "traces": [
+      {
+          ...
+          "metrics": [
+              {
+                  "properties": {
+                      "description": "Spectral acceleration",
+                      "name": "SA",
+                      "units": "g",
+                      "provenance_ids": [
+                          "seis_prov:sp000_sa_0000000",
+                          "seis_prov:sp000_pp_0000000",
+                          "seis_prov:sp000_og_0000000"
+                      ]
+                  },
+                  "dimensions": {
+                      "number": 2,
+                      "names": [
+                          "critical damping",
+                          "period"
+                      ],
+                      "units": ["%", "s"],
+                      "values": [
+                          [5.0, 10.0, 20.0],
+                          [0.5, 1.0]
+                      ]
+                  },
+                  "values": [
+                      [2.3, 2.0],
+                      [1.6, 1.4],
+                      [2.0, 1.8]
+                  ]
+              }
+          ]
+      }
+  ]
 
 Next
-Pydantic_Demo
+GMP_Examples
 
 Previous
-Command_Line_Tools
+Streams_and_Traces
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
```

### Comparing `gmpacket-0.1.2/docs/dev.html` & `gmpacket-0.1.3/docs/specification/features/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="Pydantic Demo" href="pydantic_demo.html" />
+<link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" /><link rel="next" title="Stations" href="station.html" /><link rel="prev" title="Provenance" href="../provenance.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Developer Notes - Ground Motion Packet Documentation</title>
-      <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
-    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
-    <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
-    <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
-    <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
-    <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>Features - Ground Motion Packet Documentation</title>
+      <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
+    <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/tabs.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/css/custom.css" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
+    <link rel="stylesheet" type="text/css" href="../../_static/pied-piper-admonition.css" />
     
     
 
 
 <style>
   body {
     --color-code-background: #f8f8f8;
@@ -124,65 +124,64 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
+      <a href="../../index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
           <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
         </button>
       </div>
-      <label class="toc-overlay-icon toc-header-icon" for="__toc">
+      <label class="toc-overlay-icon toc-header-icon no-toc" for="__toc">
         <div class="visually-hidden">Toggle table of contents sidebar</div>
         <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
       </label>
     </div>
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
-      <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
+      <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
   <span class="sidebar-brand-text">Ground Motion Packet Documentation</span>
   
-</a><form class="sidebar-search-container" method="get" action="search.html" role="search">
+</a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
-<li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
-<li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
-<li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
-<li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
-<li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
-<li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
-<li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
-<li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../getting_started.html">Getting Started</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../geojson.html">GeoJSON Overview</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../terms.html">Terminology</a></li>
+<li class="toctree-l1 current has-children"><a class="reference internal" href="../index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
+<li class="toctree-l2"><a class="reference internal" href="../base.html">Base Dictionary</a></li>
+<li class="toctree-l2"><a class="reference internal" href="../event.html">Event</a></li>
+<li class="toctree-l2"><a class="reference internal" href="../provenance.html">Provenance</a></li>
+<li class="toctree-l2 current has-children current-page"><a class="current reference internal" href="#">Features</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
+<li class="toctree-l3"><a class="reference internal" href="station.html">Stations</a></li>
+<li class="toctree-l3"><a class="reference internal" href="streams_traces.html">Streams and Traces</a></li>
+<li class="toctree-l3"><a class="reference internal" href="metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
-<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Developer Notes</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../examples.html">GMP Examples</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../pydantic_demo.html">Pydantic Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
       </div>
       
@@ -203,63 +202,54 @@
             <button class="theme-toggle">
               <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
               <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
               <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
               <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
             </button>
           </div>
-          <label class="toc-overlay-icon toc-content-icon" for="__toc">
+          <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="developer-notes">
-<h1>Developer Notes<a class="headerlink" href="#developer-notes" title="Permalink to this heading">#</a></h1>
-<p>We welcome comments and contributions through github issues.</p>
-<section id="documentation">
-<h2>Documentation<a class="headerlink" href="#documentation" title="Permalink to this heading">#</a></h2>
-<p>Never edit the contents of the <code class="docutils literal notranslate"><span class="pre">docs</span></code> directory, only edit files in the <code class="docutils literal notranslate"><span class="pre">doc_source</span></code>
-directory.</p>
-<p>To build this documentation, it is convenient to create a conda virtual environment
-with <a class="reference external" href="https://github.com/mamba-org/mamba">mamba</a> (note that mamba can be installed
-with <a class="reference external" href="https://docs.conda.io/en/latest/">conda</a>).</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">cd</span> <span class="n">doc_source</span>
-<span class="n">mamba</span> <span class="n">create</span> <span class="o">-</span><span class="n">n</span> <span class="n">gmpdocs</span> <span class="n">python</span><span class="o">=</span><span class="mf">3.9</span> <span class="o">--</span><span class="n">file</span> <span class="n">requirements</span><span class="o">.</span><span class="n">txt</span>
-<span class="n">conda</span> <span class="n">activate</span> <span class="n">gmpdocs</span>
-</pre></div>
-</div>
-<p>Then install the python packages as described  in the
-<a class="reference internal" href="cli.html"><span class="doc std std-doc">Command Line Tools</span></a> section. For the demo, we’ll also need</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="n">ipyleaflet</span>
-<span class="n">jupyter</span> <span class="n">nbextension</span> <span class="n">enable</span> <span class="o">--</span><span class="n">py</span> <span class="n">widgetsnbextension</span>
-</pre></div>
-</div>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">./</span><span class="n">makedocs</span><span class="o">.</span><span class="n">sh</span>
-</pre></div>
+          <section id="features">
+<h1>Features<a class="headerlink" href="#features" title="Permalink to this heading">#</a></h1>
+<p>Here we give more details about the features.</p>
+<div class="toctree-wrapper compound">
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="station.html">Stations</a></li>
+<li class="toctree-l1"><a class="reference internal" href="streams_traces.html">Streams and Traces</a></li>
+<li class="toctree-l1"><a class="reference internal" href="metrics_dict.html">Metrics Dictionary</a></li>
+</ul>
 </div>
-<p>The above script builds the docs html in the <code class="docutils literal notranslate"><span class="pre">docs</span></code> subdirectory. It can be previewed
-locally by opening <code class="docutils literal notranslate"><span class="pre">docs/index.html</span></code> in a browser.</p>
-</section>
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          
-          <a class="prev-page" href="pydantic_demo.html">
+          <a class="next-page" href="station.html">
+              <div class="page-info">
+                <div class="context">
+                  <span>Next</span>
+                </div>
+                <div class="title">Stations</div>
+              </div>
+              <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
+            </a>
+          <a class="prev-page" href="../provenance.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Pydantic Demo</div>
+                <div class="title">Provenance</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
@@ -280,44 +270,25 @@
               
             </div>
           </div>
         </div>
         
       </footer>
     </div>
-    <aside class="toc-drawer">
-      
+    <aside class="toc-drawer no-toc">
       
-      <div class="toc-sticky toc-scroll">
-        <div class="toc-title-container">
-          <span class="toc-title">
-            On this page
-          </span>
-        </div>
-        <div class="toc-tree-container">
-          <div class="toc-tree">
-            <ul>
-<li><a class="reference internal" href="#">Developer Notes</a><ul>
-<li><a class="reference internal" href="#documentation">Documentation</a></li>
-</ul>
-</li>
-</ul>
-
-          </div>
-        </div>
-      </div>
       
       
     </aside>
   </div>
-</div><script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="_static/doctools.js"></script>
-    <script src="_static/sphinx_highlight.js"></script>
-    <script src="_static/scripts/furo.js"></script>
-    <script src="_static/clipboard.min.js"></script>
-    <script src="_static/copybutton.js"></script>
-    <script src="_static/tabs.js"></script>
+</div><script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
+    <script src="../../_static/jquery.js"></script>
+    <script src="../../_static/underscore.js"></script>
+    <script src="../../_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="../../_static/doctools.js"></script>
+    <script src="../../_static/sphinx_highlight.js"></script>
+    <script src="../../_static/scripts/furo.js"></script>
+    <script src="../../_static/clipboard.min.js"></script>
+    <script src="../../_static/copybutton.js"></script>
+    <script src="../../_static/tabs.js"></script>
     </body>
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -25,56 +25,44 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
-    * Specification⁰
+    * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
-          o Features⁰
+          o Features*
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Developer Notes# ******
-We welcome comments and contributions through github issues.
-***** Documentation# *****
-Never edit the contents of the docs directory, only edit files in the
-doc_source directory.
-To build this documentation, it is convenient to create a conda virtual
-environment with mamba (note that mamba can be installed with conda).
-cd doc_source
-mamba create -n gmpdocs python=3.9 --file requirements.txt
-conda activate gmpdocs
-Then install the python packages as described in the Command_Line_Tools
-section. For the demo, weâll also need
-pip install ipyleaflet
-jupyter nbextension enable --py widgetsnbextension
-./makedocs.sh
-The above script builds the docs html in the docs subdirectory. It can be
-previewed locally by opening docs/index.html in a browser.
+****** Features# ******
+Here we give more details about the features.
+    * Stations
+    * Streams_and_Traces
+    * Metrics_Dictionary
+
+Next
+Stations
 
 Previous
-Pydantic_Demo
+Provenance
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
- On this page
-    * Developer_Notes
-          o Documentation
+
```

### Comparing `gmpacket-0.1.2/docs/examples.html` & `gmpacket-0.1.3/docs/examples.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Command Line Tools" href="cli.html" /><link rel="prev" title="Metrics Dictionary" href="specification/features/metrics_dict.html" />
+<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Pydantic Demo" href="pydantic_demo.html" /><link rel="prev" title="Metrics Dictionary" href="specification/features/metrics_dict.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Examples - Ground Motion Packet Documentation</title>
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>GMP Examples - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
 <li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
+<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
@@ -209,16 +208,16 @@
           </div>
           <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="examples">
-<h1>Examples<a class="headerlink" href="#examples" title="Permalink to this heading">#</a></h1>
+          <section id="gmp-examples">
+<h1>GMP Examples<a class="headerlink" href="#gmp-examples" title="Permalink to this heading">#</a></h1>
 <p>Examples <strong>with fake data</strong> can be found in this repository
 <a class="reference external" href="https://github.com/SCEDC/ground-motion-packet/tree/main/gmpacket/data/examples">here</a>.
 These examples are selected to illustrate a number of different possible
 instrument configurations and to highlight the value of sensible grouping
 of traces into streams.</p>
 <dl class="simple myst">
 <dt><a class="reference external" href="https://raw.githubusercontent.com/SCEDC/ground-motion-packet/main/gmpacket/data/examples/example1.json">Example 1</a></dt><dd><p>This is a very simple example for station CI.CCC. It contains a single stream
@@ -249,20 +248,20 @@
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="cli.html">
+          <a class="next-page" href="pydantic_demo.html">
               <div class="page-info">
                 <div class="context">
                   <span>Next</span>
                 </div>
-                <div class="title">Command Line Tools</div>
+                <div class="title">Pydantic Demo</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
           <a class="prev-page" href="specification/features/metrics_dict.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
```

#### html2text {}

```diff
@@ -25,38 +25,37 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Examples# ******
+****** GMP Examples# ******
 Examples with fake data can be found in this repository here. These examples
 are selected to illustrate a number of different possible instrument
 configurations and to highlight the value of sensible grouping of traces into
 streams.
   Example_1
       This is a very simple example for station CI.CCC. It contains a single
       stream for the HN instrument with. It contains two traces: the HNE
@@ -81,15 +80,15 @@
   Multisamplerate
       This is example is for a single free field station (CI.CCC). This station
       has a 3 component strong motion sensor that is being recorded at 100 sps
       and 200 sps. Each sample rate is grouped as a stream and as 3 traces for
       each sensor component as well as ROTD50 trace in the 100 sps stream.
 
 Next
-Command_Line_Tools
+Pydantic_Demo
 
 Previous
 Metrics_Dictionary
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
```

### Comparing `gmpacket-0.1.2/docs/genindex.html` & `gmpacket-0.1.3/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 --><title>Index - Ground Motion Packet Documentation</title>
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 --><title>Index - Ground Motion Packet Documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
@@ -154,31 +154,30 @@
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul>
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
 <li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
```

#### html2text {}

```diff
@@ -23,29 +23,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
```

### Comparing `gmpacket-0.1.2/docs/geojson.html` & `gmpacket-0.1.3/docs/geojson.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Terminology" href="terms.html" /><link rel="prev" title="Earthquake Ground Motion Data Packet" href="index.html" />
+<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Terminology" href="terms.html" /><link rel="prev" title="Getting Started" href="getting_started.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
         <title>GeoJSON Overview - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
 <li class="toctree-l1 current current-page"><a class="current reference internal" href="#">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
 <li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
@@ -271,22 +270,22 @@
                 <div class="context">
                   <span>Next</span>
                 </div>
                 <div class="title">Terminology</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
-          <a class="prev-page" href="index.html">
+          <a class="prev-page" href="getting_started.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Home</div>
+                <div class="title">Getting Started</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
```

#### html2text {}

```diff
@@ -25,29 +25,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
@@ -94,12 +93,12 @@
       âfeaturesâ key in the base dictionary is itself a list of
       dictionaries, each of which corresponds to one point.
 
 Next
 Terminology
 
 Previous
-Home
+Getting_Started
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
```

### Comparing `gmpacket-0.1.2/docs/index.html` & `gmpacket-0.1.3/docs/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="GeoJSON Overview" href="geojson.html" />
+<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Getting Started" href="getting_started.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
         <title>Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul>
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
 <li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
@@ -248,20 +247,20 @@
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="geojson.html">
+          <a class="next-page" href="getting_started.html">
               <div class="page-info">
                 <div class="context">
                   <span>Next</span>
                 </div>
-                <div class="title">GeoJSON Overview</div>
+                <div class="title">Getting Started</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
           
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
```

#### html2text {}

```diff
@@ -25,29 +25,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
@@ -74,12 +73,12 @@
 Attention
 Although the use of the terms âtraceâ and âstreamâ is convenient for
 use in organizing waveform metrics, there is the potential for confusion since
 we are referring to the trace or streams from which the metrics are derived,
 and the waveforms themselves are not stored in the format presented here.
 
 Next
-GeoJSON_Overview
+Getting_Started
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
```

### Comparing `gmpacket-0.1.2/docs/pydantic_demo.html` & `gmpacket-0.1.3/docs/pydantic_demo.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Developer Notes" href="dev.html" /><link rel="prev" title="Demo" href="demo.html" />
+<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Developer Notes" href="dev.html" /><link rel="prev" title="GMP Examples" href="examples.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
         <title>Pydantic Demo - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
 <li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
 <li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
@@ -211,14 +210,15 @@
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
           <section id="pydantic-demo">
 <h1>Pydantic Demo<a class="headerlink" href="#pydantic-demo" title="Permalink to this heading">#</a></h1>
+<p>Before starting, ensure you have installed the python packages as described in the <a class="reference internal" href="getting_started.html"><span class="doc std std-doc">Getting Started</span></a> section.</p>
 <p>We will start with the necessary imports</p>
 <div class="cell docutils container">
 <div class="cell_input docutils container">
 <div class="highlight-ipython3 notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">datetime</span> <span class="kn">import</span> <span class="n">datetime</span><span class="p">,</span> <span class="n">timedelta</span>
 <span class="kn">from</span> <span class="nn">gmpacket.provenance</span> <span class="kn">import</span> <span class="n">SoftwareAgent</span><span class="p">,</span> <span class="n">PersonAgent</span><span class="p">,</span> <span class="n">OrganizationAgent</span><span class="p">,</span> <span class="n">Website</span><span class="p">,</span> <span class="n">Provenance</span>
 <span class="kn">from</span> <span class="nn">gmpacket.feature</span> <span class="kn">import</span> <span class="p">(</span>
     <span class="n">Feature</span><span class="p">,</span>
@@ -345,16 +345,16 @@
 <span class="n">metrics</span> <span class="o">=</span> <span class="p">[</span><span class="n">pga_metric</span><span class="p">,</span> <span class="n">sa_metric</span><span class="p">]</span>
 <span class="n">hne_trace</span> <span class="o">=</span> <span class="n">Trace</span><span class="p">(</span><span class="n">properties</span><span class="o">=</span><span class="n">sa_trace_props</span><span class="p">,</span> <span class="n">metrics</span><span class="o">=</span><span class="n">metrics</span><span class="p">)</span>
 <span class="nb">print</span><span class="p">(</span><span class="n">hne_trace</span><span class="p">)</span>
 </pre></div>
 </div>
 </div>
 <div class="cell_output docutils container">
-<div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>channel_code=&#39;HNE&#39; location_code=&#39;10&#39; as_recorded=True azimuth=90.0 dip=0.0 start_time=datetime.datetime(2023, 2, 1, 17, 2, 19, 290235) end_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 290235)
-properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2, 1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 290235)) metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])]
+<div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>channel_code=&#39;HNE&#39; location_code=&#39;10&#39; as_recorded=True azimuth=90.0 dip=0.0 start_time=datetime.datetime(2023, 4, 11, 20, 38, 10, 450774) end_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 450774)
+properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4, 11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 450774)) metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])]
 </pre></div>
 </div>
 </div>
 </div>
 </section>
 <section id="creating-a-stream">
 <h2>Creating a Stream<a class="headerlink" href="#creating-a-stream" title="Permalink to this heading">#</a></h2>
@@ -373,15 +373,15 @@
 <span class="nb">print</span><span class="p">(</span><span class="n">stream</span><span class="p">)</span>
 </pre></div>
 </div>
 </div>
 <div class="cell_output docutils container">
 <div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>cosmos_code=10 description=&#39;A building&#39; stream_depth=0.0 stream_location=None
 band_code=&#39;H&#39; instrument_code=&#39;N&#39; samples_per_second=100.0 stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)
-properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)) traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2, 1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 290235)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])]
+properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)) traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4, 11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 450774)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])]
 </pre></div>
 </div>
 </div>
 </div>
 </section>
 <section id="creating-a-feature-station">
 <h2>Creating a Feature (station)<a class="headerlink" href="#creating-a-feature-station" title="Permalink to this heading">#</a></h2>
@@ -399,16 +399,16 @@
 <span class="n">feature</span> <span class="o">=</span> <span class="n">Feature</span><span class="p">(</span><span class="n">geometry</span><span class="o">=</span><span class="n">feature_geom</span><span class="p">,</span> <span class="n">properties</span><span class="o">=</span><span class="n">feature_props</span><span class="p">)</span>
 <span class="nb">print</span><span class="p">(</span><span class="n">feature</span><span class="p">)</span>
 </pre></div>
 </div>
 </div>
 <div class="cell_output docutils container">
 <div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>coordinates=[-124.1, 32.0, 1.1] type=&#39;Point&#39;
-network_code=&#39;NC&#39; station_code=&#39;ABCD&#39; name=&#39;A nice place for picnics&#39; streams=[Stream(properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)), traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2, 1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 290235)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])])] structure_reference_orientation=None
-geometry=FeatureGeometry(coordinates=[-124.1, 32.0, 1.1], type=&#39;Point&#39;) properties=FeatureProperties(network_code=&#39;NC&#39;, station_code=&#39;ABCD&#39;, name=&#39;A nice place for picnics&#39;, streams=[Stream(properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)), traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2, 1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 290235)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])])], structure_reference_orientation=None) type=&#39;Feature&#39;
+network_code=&#39;NC&#39; station_code=&#39;ABCD&#39; name=&#39;A nice place for picnics&#39; streams=[Stream(properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)), traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4, 11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 450774)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])])] structure_reference_orientation=None
+geometry=FeatureGeometry(coordinates=[-124.1, 32.0, 1.1], type=&#39;Point&#39;) properties=FeatureProperties(network_code=&#39;NC&#39;, station_code=&#39;ABCD&#39;, name=&#39;A nice place for picnics&#39;, streams=[Stream(properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)), traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4, 11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 450774)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])])], structure_reference_orientation=None) type=&#39;Feature&#39;
 </pre></div>
 </div>
 </div>
 </div>
 </section>
 <section id="creating-a-ground-motion-packet">
 <h2>Creating a Ground Motion Packet<a class="headerlink" href="#creating-a-ground-motion-packet" title="Permalink to this heading">#</a></h2>
@@ -423,16 +423,16 @@
                                <span class="n">features</span><span class="o">=</span><span class="p">[</span><span class="n">feature</span><span class="p">]</span>
                               <span class="p">)</span>
 <span class="nb">print</span><span class="p">(</span><span class="n">gm_packet</span><span class="p">)</span>
 </pre></div>
 </div>
 </div>
 <div class="cell_output docutils container">
-<div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>type=&#39;Feature&#39; properties={&#39;id&#39;: &#39;us2023abcd&#39;, &#39;time&#39;: datetime.datetime(2023, 2, 1, 17, 2, 49, 309312), &#39;magnitude&#39;: 7.3} geometry={&#39;type&#39;: &#39;Point&#39;, &#39;coordinates&#39;: [-120.0, 32.1, 35300.0]}
-version=&#39;0.1dev&#39; creation_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 258873) event=Event(type=&#39;Feature&#39;, properties={&#39;id&#39;: &#39;us2023abcd&#39;, &#39;time&#39;: datetime.datetime(2023, 2, 1, 17, 2, 49, 309312), &#39;magnitude&#39;: 7.3}, geometry={&#39;type&#39;: &#39;Point&#39;, &#39;coordinates&#39;: [-120.0, 32.1, 35300.0]}) provenance=Provenance(agent={&#39;person&#39;: PersonAgent(label=&#39;Alex Processor&#39;, name=&#39;Alex Processor&#39;, email=&#39;aprocessor@datagenerator.org&#39;, role=&#39;Data Processor&#39;, prov:type={&#39;$&#39;: &#39;prov:Person&#39;, &#39;type&#39;: &#39;prov:QUALIFIED_NAME&#39;}), &#39;software&#39;: SoftwareAgent(label=&#39;gmprocess&#39;, name=&#39;gmprocess&#39;, version=&#39;1.2.0&#39;, website=Website(url=&#39;https://code.usgs.gov/ghsc/esi/groundmotion-processing/#introduction&#39;, site_type=&#39;xsd:anyURI&#39;), prov:type={&#39;$&#39;: &#39;prov:SoftwareAgent&#39;, &#39;type&#39;: &#39;prov:QUALIFIED_NAME&#39;}), &#39;organization&#39;: OrganizationAgent(label=&#39;Data Generator&#39;, name=&#39;Data Generator&#39;, role=&#39;Data Provider&#39;, website=Website(url=&#39;https://www.datagenerator.org&#39;, site_type=&#39;xsd:anyURI&#39;), prov:type={&#39;$&#39;: &#39;prov:Organization&#39;, &#39;type&#39;: &#39;prov:QUALIFIED_NAME&#39;})}, prefix={&#39;seis_prov&#39;: &#39;http://seisprov.org/seis_prov/0.1/#&#39;}) features=[Feature(geometry=FeatureGeometry(coordinates=[-124.1, 32.0, 1.1], type=&#39;Point&#39;), properties=FeatureProperties(network_code=&#39;NC&#39;, station_code=&#39;ABCD&#39;, name=&#39;A nice place for picnics&#39;, streams=[Stream(properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)), traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2, 1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 290235)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])])], structure_reference_orientation=None), type=&#39;Feature&#39;)] type=&#39;FeatureCollection&#39;
+<div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>type=&#39;Feature&#39; properties={&#39;id&#39;: &#39;us2023abcd&#39;, &#39;time&#39;: datetime.datetime(2023, 4, 11, 20, 38, 40, 463823), &#39;magnitude&#39;: 7.3} geometry={&#39;type&#39;: &#39;Point&#39;, &#39;coordinates&#39;: [-120.0, 32.1, 35300.0]}
+version=&#39;0.1dev&#39; creation_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 426764) event=Event(type=&#39;Feature&#39;, properties={&#39;id&#39;: &#39;us2023abcd&#39;, &#39;time&#39;: datetime.datetime(2023, 4, 11, 20, 38, 40, 463823), &#39;magnitude&#39;: 7.3}, geometry={&#39;type&#39;: &#39;Point&#39;, &#39;coordinates&#39;: [-120.0, 32.1, 35300.0]}) provenance=Provenance(agent={&#39;person&#39;: PersonAgent(label=&#39;Alex Processor&#39;, name=&#39;Alex Processor&#39;, email=&#39;aprocessor@datagenerator.org&#39;, role=&#39;Data Processor&#39;, prov:type={&#39;$&#39;: &#39;prov:Person&#39;, &#39;type&#39;: &#39;prov:QUALIFIED_NAME&#39;}), &#39;software&#39;: SoftwareAgent(label=&#39;gmprocess&#39;, name=&#39;gmprocess&#39;, version=&#39;1.2.0&#39;, website=Website(url=&#39;https://code.usgs.gov/ghsc/esi/groundmotion-processing/#introduction&#39;, site_type=&#39;xsd:anyURI&#39;), prov:type={&#39;$&#39;: &#39;prov:SoftwareAgent&#39;, &#39;type&#39;: &#39;prov:QUALIFIED_NAME&#39;}), &#39;organization&#39;: OrganizationAgent(label=&#39;Data Generator&#39;, name=&#39;Data Generator&#39;, role=&#39;Data Provider&#39;, website=Website(url=&#39;https://www.datagenerator.org&#39;, site_type=&#39;xsd:anyURI&#39;), prov:type={&#39;$&#39;: &#39;prov:Organization&#39;, &#39;type&#39;: &#39;prov:QUALIFIED_NAME&#39;})}, prefix={&#39;seis_prov&#39;: &#39;http://seisprov.org/seis_prov/0.1/#&#39;}) features=[Feature(geometry=FeatureGeometry(coordinates=[-124.1, 32.0, 1.1], type=&#39;Point&#39;), properties=FeatureProperties(network_code=&#39;NC&#39;, station_code=&#39;ABCD&#39;, name=&#39;A nice place for picnics&#39;, streams=[Stream(properties=StreamProperties(band_code=&#39;H&#39;, instrument_code=&#39;N&#39;, samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10, description=&#39;A building&#39;, stream_depth=0.0, stream_location=None)), traces=[Trace(properties=TraceProperties(channel_code=&#39;HNE&#39;, location_code=&#39;10&#39;, as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4, 11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 450774)), metrics=[Metric(properties=MetricProperties(description=&#39;Peak Ground Accleration&#39;, name=&#39;PGA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=None, values=1.5), Metric(properties=MetricProperties(description=&#39;Spectral Accleration&#39;, name=&#39;SA&#39;, units=&#39;g&#39;, provenance_ids=[&#39;person&#39;, &#39;software&#39;, &#39;organization&#39;], time_of_peak=None), dimensions=MetricDimensions(number=2, names=[&#39;critical damping&#39;, &#39;period&#39;], units=[&#39;%&#39;, &#39;s&#39;], axis_values=[[5.0], [0.3, 1.0, 3.0]]), values=[[1.2, 1.4, 1.6]])])])], structure_reference_orientation=None), type=&#39;Feature&#39;)] type=&#39;FeatureCollection&#39;
 </pre></div>
 </div>
 </div>
 </div>
 </section>
 <section id="exporting-groundmotion-packets">
 <h2>Exporting GroundMotion Packets<a class="headerlink" href="#exporting-groundmotion-packets" title="Permalink to this heading">#</a></h2>
@@ -442,15 +442,15 @@
 
 <span class="n">df</span> <span class="o">=</span> <span class="n">gm_packet</span><span class="o">.</span><span class="n">to_dataframe</span><span class="p">()</span>
 <span class="n">df</span>
 </pre></div>
 </div>
 </div>
 <div class="cell_output docutils container">
-<div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>{&quot;version&quot;:&quot;0.1dev&quot;,&quot;creation_time&quot;:&quot;2023-02-01T17:02:49Z&quot;,&quot;event&quot;:{&quot;type&quot;:&quot;Feature&quot;,&quot;properties&quot;:{&quot;id&quot;:&quot;us2023abcd&quot;,&quot;time&quot;:&quot;2023-02-01T17:02:49Z&quot;,&quot;magnitude&quot;:7.3},&quot;geometry&quot;:{&quot;type&quot;:&quot;Point&quot;,&quot;coordinates&quot;:[-120,32.1,35300]}},&quot;provenance&quot;:{&quot;agent&quot;:{&quot;person&quot;:{&quot;prov:label&quot;:&quot;Alex Processor&quot;,&quot;seis_prov:name&quot;:&quot;Alex Processor&quot;,&quot;seis_prov:email&quot;:&quot;aprocessor@datagenerator.org&quot;,&quot;seis_prov:role&quot;:&quot;Data Processor&quot;,&quot;prov:type&quot;:{&quot;$&quot;:&quot;prov:Person&quot;,&quot;type&quot;:&quot;prov:QUALIFIED_NAME&quot;}},&quot;software&quot;:{&quot;prov:label&quot;:&quot;gmprocess&quot;,&quot;seis_prov:software_name&quot;:&quot;gmprocess&quot;,&quot;seis_prov:software_version&quot;:&quot;1.2.0&quot;,&quot;seis_prov:website&quot;:{&quot;$&quot;:&quot;https://code.usgs.gov/ghsc/esi/groundmotion-processing/#introduction&quot;,&quot;type&quot;:&quot;xsd:anyURI&quot;},&quot;prov:type&quot;:{&quot;$&quot;:&quot;prov:SoftwareAgent&quot;,&quot;type&quot;:&quot;prov:QUALIFIED_NAME&quot;}},&quot;organization&quot;:{&quot;prov:label&quot;:&quot;Data Generator&quot;,&quot;seis_prov:name&quot;:&quot;Data Generator&quot;,&quot;seis_prov:role&quot;:&quot;Data Provider&quot;,&quot;seis_prov:website&quot;:{&quot;$&quot;:&quot;https://www.datagenerator.org&quot;,&quot;type&quot;:&quot;xsd:anyURI&quot;},&quot;prov:type&quot;:{&quot;$&quot;:&quot;prov:Organization&quot;,&quot;type&quot;:&quot;prov:QUALIFIED_NAME&quot;}}},&quot;prefix&quot;:{&quot;seis_prov&quot;:&quot;http://seisprov.org/seis_prov/0.1/#&quot;}},&quot;features&quot;:[{&quot;geometry&quot;:{&quot;coordinates&quot;:[-124.1,32,1.1],&quot;type&quot;:&quot;Point&quot;},&quot;properties&quot;:{&quot;network_code&quot;:&quot;NC&quot;,&quot;station_code&quot;:&quot;ABCD&quot;,&quot;name&quot;:&quot;A nice place for picnics&quot;,&quot;streams&quot;:[{&quot;properties&quot;:{&quot;band_code&quot;:&quot;H&quot;,&quot;instrument_code&quot;:&quot;N&quot;,&quot;samples_per_second&quot;:100,&quot;stream_housing&quot;:{&quot;cosmos_code&quot;:10,&quot;description&quot;:&quot;A building&quot;,&quot;stream_depth&quot;:0,&quot;stream_location&quot;:null}},&quot;traces&quot;:[{&quot;properties&quot;:{&quot;channel_code&quot;:&quot;HNE&quot;,&quot;location_code&quot;:&quot;10&quot;,&quot;as_recorded&quot;:true,&quot;azimuth&quot;:90,&quot;dip&quot;:0,&quot;start_time&quot;:&quot;2023-02-01T17:02:19Z&quot;,&quot;end_time&quot;:&quot;2023-02-01T17:02:49Z&quot;},&quot;metrics&quot;:[{&quot;properties&quot;:{&quot;description&quot;:&quot;Peak Ground Accleration&quot;,&quot;name&quot;:&quot;PGA&quot;,&quot;units&quot;:&quot;g&quot;,&quot;provenance_ids&quot;:[&quot;person&quot;,&quot;software&quot;,&quot;organization&quot;],&quot;time_of_peak&quot;:null},&quot;dimensions&quot;:null,&quot;values&quot;:1.5},{&quot;properties&quot;:{&quot;description&quot;:&quot;Spectral Accleration&quot;,&quot;name&quot;:&quot;SA&quot;,&quot;units&quot;:&quot;g&quot;,&quot;provenance_ids&quot;:[&quot;person&quot;,&quot;software&quot;,&quot;organization&quot;],&quot;time_of_peak&quot;:null},&quot;dimensions&quot;:{&quot;number&quot;:2,&quot;names&quot;:[&quot;critical damping&quot;,&quot;period&quot;],&quot;units&quot;:[&quot;%&quot;,&quot;s&quot;],&quot;axis_values&quot;:[[5],[0.3,1,3]]},&quot;values&quot;:[[1.2,1.4,1.6]]}]}]}],&quot;structure_reference_orientation&quot;:null},&quot;type&quot;:&quot;Feature&quot;}],&quot;type&quot;:&quot;FeatureCollection&quot;}
+<div class="output stream highlight-myst-ansi notranslate"><div class="highlight"><pre><span></span>{&quot;version&quot;:&quot;0.1dev&quot;,&quot;creation_time&quot;:&quot;2023-04-11T20:38:40Z&quot;,&quot;event&quot;:{&quot;type&quot;:&quot;Feature&quot;,&quot;properties&quot;:{&quot;id&quot;:&quot;us2023abcd&quot;,&quot;time&quot;:&quot;2023-04-11T20:38:40Z&quot;,&quot;magnitude&quot;:7.3},&quot;geometry&quot;:{&quot;type&quot;:&quot;Point&quot;,&quot;coordinates&quot;:[-120,32.1,35300]}},&quot;provenance&quot;:{&quot;agent&quot;:{&quot;person&quot;:{&quot;prov:label&quot;:&quot;Alex Processor&quot;,&quot;seis_prov:name&quot;:&quot;Alex Processor&quot;,&quot;seis_prov:email&quot;:&quot;aprocessor@datagenerator.org&quot;,&quot;seis_prov:role&quot;:&quot;Data Processor&quot;,&quot;prov:type&quot;:{&quot;$&quot;:&quot;prov:Person&quot;,&quot;type&quot;:&quot;prov:QUALIFIED_NAME&quot;}},&quot;software&quot;:{&quot;prov:label&quot;:&quot;gmprocess&quot;,&quot;seis_prov:software_name&quot;:&quot;gmprocess&quot;,&quot;seis_prov:software_version&quot;:&quot;1.2.0&quot;,&quot;seis_prov:website&quot;:{&quot;$&quot;:&quot;https://code.usgs.gov/ghsc/esi/groundmotion-processing/#introduction&quot;,&quot;type&quot;:&quot;xsd:anyURI&quot;},&quot;prov:type&quot;:{&quot;$&quot;:&quot;prov:SoftwareAgent&quot;,&quot;type&quot;:&quot;prov:QUALIFIED_NAME&quot;}},&quot;organization&quot;:{&quot;prov:label&quot;:&quot;Data Generator&quot;,&quot;seis_prov:name&quot;:&quot;Data Generator&quot;,&quot;seis_prov:role&quot;:&quot;Data Provider&quot;,&quot;seis_prov:website&quot;:{&quot;$&quot;:&quot;https://www.datagenerator.org&quot;,&quot;type&quot;:&quot;xsd:anyURI&quot;},&quot;prov:type&quot;:{&quot;$&quot;:&quot;prov:Organization&quot;,&quot;type&quot;:&quot;prov:QUALIFIED_NAME&quot;}}},&quot;prefix&quot;:{&quot;seis_prov&quot;:&quot;http://seisprov.org/seis_prov/0.1/#&quot;}},&quot;features&quot;:[{&quot;geometry&quot;:{&quot;coordinates&quot;:[-124.1,32,1.1],&quot;type&quot;:&quot;Point&quot;},&quot;properties&quot;:{&quot;network_code&quot;:&quot;NC&quot;,&quot;station_code&quot;:&quot;ABCD&quot;,&quot;name&quot;:&quot;A nice place for picnics&quot;,&quot;streams&quot;:[{&quot;properties&quot;:{&quot;band_code&quot;:&quot;H&quot;,&quot;instrument_code&quot;:&quot;N&quot;,&quot;samples_per_second&quot;:100,&quot;stream_housing&quot;:{&quot;cosmos_code&quot;:10,&quot;description&quot;:&quot;A building&quot;,&quot;stream_depth&quot;:0,&quot;stream_location&quot;:null}},&quot;traces&quot;:[{&quot;properties&quot;:{&quot;channel_code&quot;:&quot;HNE&quot;,&quot;location_code&quot;:&quot;10&quot;,&quot;as_recorded&quot;:true,&quot;azimuth&quot;:90,&quot;dip&quot;:0,&quot;start_time&quot;:&quot;2023-04-11T20:38:10Z&quot;,&quot;end_time&quot;:&quot;2023-04-11T20:38:40Z&quot;},&quot;metrics&quot;:[{&quot;properties&quot;:{&quot;description&quot;:&quot;Peak Ground Accleration&quot;,&quot;name&quot;:&quot;PGA&quot;,&quot;units&quot;:&quot;g&quot;,&quot;provenance_ids&quot;:[&quot;person&quot;,&quot;software&quot;,&quot;organization&quot;],&quot;time_of_peak&quot;:null},&quot;dimensions&quot;:null,&quot;values&quot;:1.5},{&quot;properties&quot;:{&quot;description&quot;:&quot;Spectral Accleration&quot;,&quot;name&quot;:&quot;SA&quot;,&quot;units&quot;:&quot;g&quot;,&quot;provenance_ids&quot;:[&quot;person&quot;,&quot;software&quot;,&quot;organization&quot;],&quot;time_of_peak&quot;:null},&quot;dimensions&quot;:{&quot;number&quot;:2,&quot;names&quot;:[&quot;critical damping&quot;,&quot;period&quot;],&quot;units&quot;:[&quot;%&quot;,&quot;s&quot;],&quot;axis_values&quot;:[[5],[0.3,1,3]]},&quot;values&quot;:[[1.2,1.4,1.6]]}]}]}],&quot;structure_reference_orientation&quot;:null},&quot;type&quot;:&quot;Feature&quot;}],&quot;type&quot;:&quot;FeatureCollection&quot;}
 </pre></div>
 </div>
 <div class="output text_html"><div>
 <style scoped>
     .dataframe tbody tr th:only-of-type {
         vertical-align: middle;
     }
@@ -475,58 +475,39 @@
       <th>event_depth</th>
       <th>network</th>
       <th>station</th>
       <th>station_name</th>
       <th>station_longitude</th>
       <th>station_latitude</th>
       <th>station_elevation</th>
-      <th>channel</th>
+      <th>epicentral_distance_km</th>
+      <th>component</th>
       <th>location</th>
       <th>PGA(g)</th>
       <th>SA(g)_critical_damping_5.0%_period_0.3s</th>
       <th>SA(g)_critical_damping_5.0%_period_1.0s</th>
       <th>SA(g)_critical_damping_5.0%_period_3.0s</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <th>0</th>
       <td>us2023abcd</td>
-      <td>2023-02-01 17:02:49.309312</td>
-      <td>7.3</td>
-      <td>-120.0</td>
-      <td>32.1</td>
-      <td>35300.0</td>
-      <td>NC</td>
-      <td>ABCD</td>
-      <td>A nice place for picnics</td>
-      <td>-124.1</td>
-      <td>32.0</td>
-      <td>1.1</td>
-      <td>HNE</td>
-      <td>10</td>
-      <td>1.5</td>
-      <td>1.2</td>
-      <td>1.4</td>
-      <td>1.6</td>
-    </tr>
-    <tr>
-      <th>1</th>
-      <td>us2023abcd</td>
-      <td>2023-02-01 17:02:49.309312</td>
+      <td>2023-04-11 20:38:40.463823</td>
       <td>7.3</td>
       <td>-120.0</td>
       <td>32.1</td>
       <td>35300.0</td>
       <td>NC</td>
       <td>ABCD</td>
       <td>A nice place for picnics</td>
       <td>-124.1</td>
       <td>32.0</td>
       <td>1.1</td>
+      <td>387.346866</td>
       <td>HNE</td>
       <td>10</td>
       <td>1.5</td>
       <td>1.2</td>
       <td>1.4</td>
       <td>1.6</td>
     </tr>
@@ -547,22 +528,22 @@
                 <div class="context">
                   <span>Next</span>
                 </div>
                 <div class="title">Developer Notes</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
-          <a class="prev-page" href="demo.html">
+          <a class="prev-page" href="examples.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Demo</div>
+                <div class="title">GMP Examples</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
```

#### html2text {}

```diff
@@ -25,38 +25,39 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 ****** Pydantic Demo# ******
+Before starting, ensure you have installed the python packages as described in
+the Getting_Started section.
 We will start with the necessary imports
 from datetime import datetime, timedelta
 from gmpacket.provenance import SoftwareAgent, PersonAgent, OrganizationAgent,
 Website, Provenance
 from gmpacket.feature import (
     Feature,
     FeatureGeometry,
@@ -168,20 +169,20 @@
                                  end_time=end_time)
 print(sa_trace_props)
 
 metrics = [pga_metric, sa_metric]
 hne_trace = Trace(properties=sa_trace_props, metrics=metrics)
 print(hne_trace)
 channel_code='HNE' location_code='10' as_recorded=True azimuth=90.0 dip=0.0
-start_time=datetime.datetime(2023, 2, 1, 17, 2, 19, 290235)
-end_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 290235)
+start_time=datetime.datetime(2023, 4, 11, 20, 38, 10, 450774)
+end_time=datetime.datetime(2023, 4, 11, 20, 38, 40, 450774)
 properties=TraceProperties(channel_code='HNE', location_code='10',
-as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2,
-1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49,
-290235)) metrics=[Metric(properties=MetricProperties(description='Peak Ground
+as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4,
+11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40,
+450774)) metrics=[Metric(properties=MetricProperties(description='Peak Ground
 Accleration', name='PGA', units='g', provenance_ids=['person', 'software',
 'organization'], time_of_peak=None), dimensions=None, values=1.5), Metric
 (properties=MetricProperties(description='Spectral Accleration', name='SA',
 units='g', provenance_ids=['person', 'software', 'organization'],
 time_of_peak=None), dimensions=MetricDimensions(number=2, names=['critical
 damping', 'period'], units=['%', 's'], axis_values=[[5.0], [0.3, 1.0, 3.0]]),
 values=[[1.2, 1.4, 1.6]])]
@@ -203,17 +204,17 @@
 band_code='H' instrument_code='N' samples_per_second=100.0
 stream_housing=StreamHousing(cosmos_code=10, description='A building',
 stream_depth=0.0, stream_location=None)
 properties=StreamProperties(band_code='H', instrument_code='N',
 samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10,
 description='A building', stream_depth=0.0, stream_location=None)) traces=
 [Trace(properties=TraceProperties(channel_code='HNE', location_code='10',
-as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2,
-1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49,
-290235)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
+as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4,
+11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40,
+450774)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
 Accleration', name='PGA', units='g', provenance_ids=['person', 'software',
 'organization'], time_of_peak=None), dimensions=None, values=1.5), Metric
 (properties=MetricProperties(description='Spectral Accleration', name='SA',
 units='g', provenance_ids=['person', 'software', 'organization'],
 time_of_peak=None), dimensions=MetricDimensions(number=2, names=['critical
 damping', 'period'], units=['%', 's'], axis_values=[[5.0], [0.3, 1.0, 3.0]]),
 values=[[1.2, 1.4, 1.6]])])]
@@ -232,34 +233,34 @@
 print(feature)
 coordinates=[-124.1, 32.0, 1.1] type='Point'
 network_code='NC' station_code='ABCD' name='A nice place for picnics' streams=
 [Stream(properties=StreamProperties(band_code='H', instrument_code='N',
 samples_per_second=100.0, stream_housing=StreamHousing(cosmos_code=10,
 description='A building', stream_depth=0.0, stream_location=None)), traces=
 [Trace(properties=TraceProperties(channel_code='HNE', location_code='10',
-as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2,
-1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49,
-290235)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
+as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4,
+11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40,
+450774)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
 Accleration', name='PGA', units='g', provenance_ids=['person', 'software',
 'organization'], time_of_peak=None), dimensions=None, values=1.5), Metric
 (properties=MetricProperties(description='Spectral Accleration', name='SA',
 units='g', provenance_ids=['person', 'software', 'organization'],
 time_of_peak=None), dimensions=MetricDimensions(number=2, names=['critical
 damping', 'period'], units=['%', 's'], axis_values=[[5.0], [0.3, 1.0, 3.0]]),
 values=[[1.2, 1.4, 1.6]])])])] structure_reference_orientation=None
 geometry=FeatureGeometry(coordinates=[-124.1, 32.0, 1.1], type='Point')
 properties=FeatureProperties(network_code='NC', station_code='ABCD', name='A
 nice place for picnics', streams=[Stream(properties=StreamProperties
 (band_code='H', instrument_code='N', samples_per_second=100.0,
 stream_housing=StreamHousing(cosmos_code=10, description='A building',
 stream_depth=0.0, stream_location=None)), traces=[Trace
 (properties=TraceProperties(channel_code='HNE', location_code='10',
-as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2,
-1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49,
-290235)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
+as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4,
+11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40,
+450774)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
 Accleration', name='PGA', units='g', provenance_ids=['person', 'software',
 'organization'], time_of_peak=None), dimensions=None, values=1.5), Metric
 (properties=MetricProperties(description='Spectral Accleration', name='SA',
 units='g', provenance_ids=['person', 'software', 'organization'],
 time_of_peak=None), dimensions=MetricDimensions(number=2, names=['critical
 damping', 'period'], units=['%', 's'], axis_values=[[5.0], [0.3, 1.0, 3.0]]),
 values=[[1.2, 1.4, 1.6]])])])], structure_reference_orientation=None)
@@ -273,20 +274,20 @@
 gm_packet = GroundMotionPacket(version="0.1dev",
                                event=event,
                                provenance=provenance,
                                features=[feature]
                               )
 print(gm_packet)
 type='Feature' properties={'id': 'us2023abcd', 'time': datetime.datetime(2023,
-2, 1, 17, 2, 49, 309312), 'magnitude': 7.3} geometry={'type': 'Point',
+4, 11, 20, 38, 40, 463823), 'magnitude': 7.3} geometry={'type': 'Point',
 'coordinates': [-120.0, 32.1, 35300.0]}
-version='0.1dev' creation_time=datetime.datetime(2023, 2, 1, 17, 2, 49, 258873)
-event=Event(type='Feature', properties={'id': 'us2023abcd', 'time':
-datetime.datetime(2023, 2, 1, 17, 2, 49, 309312), 'magnitude': 7.3}, geometry=
-{'type': 'Point', 'coordinates': [-120.0, 32.1, 35300.0]})
+version='0.1dev' creation_time=datetime.datetime(2023, 4, 11, 20, 38, 40,
+426764) event=Event(type='Feature', properties={'id': 'us2023abcd', 'time':
+datetime.datetime(2023, 4, 11, 20, 38, 40, 463823), 'magnitude': 7.3},
+geometry={'type': 'Point', 'coordinates': [-120.0, 32.1, 35300.0]})
 provenance=Provenance(agent={'person': PersonAgent(label='Alex Processor',
 name='Alex Processor', email='aprocessor@datagenerator.org', role='Data
 Processor', prov:type={'$': 'prov:Person', 'type': 'prov:QUALIFIED_NAME'}),
 'software': SoftwareAgent(label='gmprocess', name='gmprocess', version='1.2.0',
 website=Website(url='https://code.usgs.gov/ghsc/esi/groundmotion-processing/
 #introduction', site_type='xsd:anyURI'), prov:type={'$': 'prov:SoftwareAgent',
 'type': 'prov:QUALIFIED_NAME'}), 'organization': OrganizationAgent(label='Data
@@ -297,34 +298,34 @@
 (geometry=FeatureGeometry(coordinates=[-124.1, 32.0, 1.1], type='Point'),
 properties=FeatureProperties(network_code='NC', station_code='ABCD', name='A
 nice place for picnics', streams=[Stream(properties=StreamProperties
 (band_code='H', instrument_code='N', samples_per_second=100.0,
 stream_housing=StreamHousing(cosmos_code=10, description='A building',
 stream_depth=0.0, stream_location=None)), traces=[Trace
 (properties=TraceProperties(channel_code='HNE', location_code='10',
-as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 2,
-1, 17, 2, 19, 290235), end_time=datetime.datetime(2023, 2, 1, 17, 2, 49,
-290235)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
+as_recorded=True, azimuth=90.0, dip=0.0, start_time=datetime.datetime(2023, 4,
+11, 20, 38, 10, 450774), end_time=datetime.datetime(2023, 4, 11, 20, 38, 40,
+450774)), metrics=[Metric(properties=MetricProperties(description='Peak Ground
 Accleration', name='PGA', units='g', provenance_ids=['person', 'software',
 'organization'], time_of_peak=None), dimensions=None, values=1.5), Metric
 (properties=MetricProperties(description='Spectral Accleration', name='SA',
 units='g', provenance_ids=['person', 'software', 'organization'],
 time_of_peak=None), dimensions=MetricDimensions(number=2, names=['critical
 damping', 'period'], units=['%', 's'], axis_values=[[5.0], [0.3, 1.0, 3.0]]),
 values=[[1.2, 1.4, 1.6]])])])], structure_reference_orientation=None),
 type='Feature')] type='FeatureCollection'
 
 ***** Exporting GroundMotion Packets# *****
 print(gm_packet.as_json())
 
 df = gm_packet.to_dataframe()
 df
-{"version":"0.1dev","creation_time":"2023-02-01T17:02:49Z","event":{"type":
-"Feature","properties":{"id":"us2023abcd","time":"2023-02-01T17:02:
-49Z","magnitude":7.3},"geometry":{"type":"Point","coordinates":[-
+{"version":"0.1dev","creation_time":"2023-04-11T20:38:40Z","event":{"type":
+"Feature","properties":{"id":"us2023abcd","time":"2023-04-11T20:38:
+40Z","magnitude":7.3},"geometry":{"type":"Point","coordinates":[-
 120,32.1,35300]}},"provenance":{"agent":{"person":{"prov:label":"Alex
 Processor","seis_prov:name":"Alex Processor","seis_prov:email":
 "aprocessor@datagenerator.org","seis_prov:role":"Data Processor","prov:type":
 {"$":"prov:Person","type":"prov:QUALIFIED_NAME"}},"software":{"prov:label":
 "gmprocess","seis_prov:software_name":"gmprocess","seis_prov:software_version":
 "1.2.0","seis_prov:website":{"$":"https://code.usgs.gov/ghsc/esi/groundmotion-
 processing/#introduction","type":"xsd:anyURI"},"prov:type":{"$":"prov:
@@ -335,40 +336,37 @@
 QUALIFIED_NAME"}}},"prefix":{"seis_prov":"http://seisprov.org/seis_prov/0.1/
 #"}},"features":[{"geometry":{"coordinates":[-124.1,32,1.1],"type":
 "Point"},"properties":{"network_code":"NC","station_code":"ABCD","name":"A nice
 place for picnics","streams":[{"properties":{"band_code":"H","instrument_code":
 "N","samples_per_second":100,"stream_housing":{"cosmos_code":10,"description":
 "A building","stream_depth":0,"stream_location":null}},"traces":[{"properties":
 {"channel_code":"HNE","location_code":"10","as_recorded":true,"azimuth":
-90,"dip":0,"start_time":"2023-02-01T17:02:19Z","end_time":"2023-02-01T17:02:
-49Z"},"metrics":[{"properties":{"description":"Peak Ground Accleration","name":
+90,"dip":0,"start_time":"2023-04-11T20:38:10Z","end_time":"2023-04-11T20:38:
+40Z"},"metrics":[{"properties":{"description":"Peak Ground Accleration","name":
 "PGA","units":"g","provenance_ids":
 ["person","software","organization"],"time_of_peak":null},"dimensions":
 null,"values":1.5},{"properties":{"description":"Spectral Accleration","name":
 "SA","units":"g","provenance_ids":
 ["person","software","organization"],"time_of_peak":null},"dimensions":
 {"number":2,"names":["critical damping","period"],"units":
 ["%","s"],"axis_values":[[5],[0.3,1,3]]},"values":[
 [1.2,1.4,1.6]]}]}]}],"structure_reference_orientation":null},"type":
 "Feature"}],"type":"FeatureCollection"}
- ____________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
-| |id        |time     |magnitude|event_longitude|event_latitude|event_depth|network|station|station_name|station_longitude|station_latitude|station_elevation|channel|location|PGA|SA                                   |SA                                   |SA                                   |
-|_|__________|_________|_________|_______________|______________|___________|_______|_______|____________|_________________|________________|_________________|_______|________|(g)|(g)_critical_damping_5.0%_period_0.3s|(g)_critical_damping_5.0%_period_1.0s|(g)_critical_damping_5.0%_period_3.0s|
-| |          |2023-02- |         |               |              |           |       |       |A nice place|                 |                |                 |       |        |   |                                     |                                     |                                     |
-|0|us2023abcd|01 17:02:|7.3      |-120.0         |32.1          |35300.0    |NC     |ABCD   |for picnics |-124.1           |32.0            |1.1              |HNE    |10      |1.5|1.2                                  |1.4                                  |1.6                                  |
-|_|__________|49.309312|_________|_______________|______________|___________|_______|_______|____________|_________________|________________|_________________|_______|________|___|_____________________________________|_____________________________________|_____________________________________|
-| |          |2023-02- |         |               |              |           |       |       |A nice place|                 |                |                 |       |        |   |                                     |                                     |                                     |
-|1|us2023abcd|01 17:02:|7.3      |-120.0         |32.1          |35300.0    |NC     |ABCD   |for picnics |-124.1           |32.0            |1.1              |HNE    |10      |1.5|1.2                                  |1.4                                  |1.6                                  |
-|_|__________|49.309312|_________|_______________|______________|___________|_______|_______|____________|_________________|________________|_________________|_______|________|___|_____________________________________|_____________________________________|_____________________________________|
+ _____________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
+| |id        |time     |magnitude|event_longitude|event_latitude|event_depth|network|station|station_name|station_longitude|station_latitude|station_elevation|epicentral_distance_km|component|location|PGA|SA                                   |SA                                   |SA                                   |
+|_|__________|_________|_________|_______________|______________|___________|_______|_______|____________|_________________|________________|_________________|______________________|_________|________|(g)|(g)_critical_damping_5.0%_period_0.3s|(g)_critical_damping_5.0%_period_1.0s|(g)_critical_damping_5.0%_period_3.0s|
+| |          |2023-04- |         |               |              |           |       |       |A nice place|                 |                |                 |                      |         |        |   |                                     |                                     |                                     |
+|0|us2023abcd|11 20:38:|7.3      |-120.0         |32.1          |35300.0    |NC     |ABCD   |for picnics |-124.1           |32.0            |1.1              |387.346866            |HNE      |10      |1.5|1.2                                  |1.4                                  |1.6                                  |
+|_|__________|40.463823|_________|_______________|______________|___________|_______|_______|____________|_________________|________________|_________________|______________________|_________|________|___|_____________________________________|_____________________________________|_____________________________________|
 
 Next
 Developer_Notes
 
 Previous
-Demo
+GMP_Examples
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
  On this page
     * Pydantic_Demo
           o Dealing_with_Provenance
           o Creating_Simple_Metrics
```

### Comparing `gmpacket-0.1.2/docs/search.html` & `gmpacket-0.1.3/docs/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 --><title>Search - Ground Motion Packet Documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 --><title>Search - Ground Motion Packet Documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
@@ -153,31 +153,30 @@
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul>
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
 <li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
```

#### html2text {}

```diff
@@ -23,29 +23,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
```

### Comparing `gmpacket-0.1.2/docs/specification/base.html` & `gmpacket-0.1.3/docs/specification/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" /><link rel="next" title="Event" href="event.html" /><link rel="prev" title="Specification" href="index.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
         <title>Base Dictionary - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="../_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="../_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="../getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../terms.html">Terminology</a></li>
 <li class="toctree-l1 current has-children"><a class="reference internal" href="index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
 <li class="toctree-l2 current current-page"><a class="current reference internal" href="#">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
```

#### html2text {}

```diff
@@ -25,29 +25,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
```

### Comparing `gmpacket-0.1.2/docs/specification/event.html` & `gmpacket-0.1.3/docs/specification/event.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" /><link rel="next" title="Provenance" href="provenance.html" /><link rel="prev" title="Base Dictionary" href="base.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
         <title>Event - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="../_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="../_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="../getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../terms.html">Terminology</a></li>
 <li class="toctree-l1 current has-children"><a class="reference internal" href="index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
 <li class="toctree-l2"><a class="reference internal" href="base.html">Base Dictionary</a></li>
 <li class="toctree-l2 current current-page"><a class="current reference internal" href="#">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="provenance.html">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
```

#### html2text {}

```diff
@@ -25,29 +25,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
```

### Comparing `gmpacket-0.1.2/docs/specification/features/index.html` & `gmpacket-0.1.3/docs/specification/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" /><link rel="next" title="Stations" href="station.html" /><link rel="prev" title="Provenance" href="../provenance.html" />
+<link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" /><link rel="next" title="Base Dictionary" href="base.html" /><link rel="prev" title="Terminology" href="../terms.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Features - Ground Motion Packet Documentation</title>
-      <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
-    <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/tabs.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/css/custom.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
-    <link rel="stylesheet" type="text/css" href="../../_static/pied-piper-admonition.css" />
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>Specification - Ground Motion Packet Documentation</title>
+      <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
+    <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="../_static/tabs.css" />
+    <link rel="stylesheet" type="text/css" href="../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
+    <link rel="stylesheet" type="text/css" href="../_static/css/custom.css" />
+    <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
+    <link rel="stylesheet" type="text/css" href="../_static/pied-piper-admonition.css" />
     
     
 
 
 <style>
   body {
     --color-code-background: #f8f8f8;
@@ -124,15 +124,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
+      <a href="../index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -144,45 +144,44 @@
         <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
       </label>
     </div>
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
-      <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
+      <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
   <span class="sidebar-brand-text">Ground Motion Packet Documentation</span>
   
-</a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
+</a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="../../geojson.html">GeoJSON Overview</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../terms.html">Terminology</a></li>
-<li class="toctree-l1 current has-children"><a class="reference internal" href="../index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
-<li class="toctree-l2"><a class="reference internal" href="../base.html">Base Dictionary</a></li>
-<li class="toctree-l2"><a class="reference internal" href="../event.html">Event</a></li>
-<li class="toctree-l2"><a class="reference internal" href="../provenance.html">Provenance</a></li>
-<li class="toctree-l2 current has-children current-page"><a class="current reference internal" href="#">Features</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
-<li class="toctree-l3"><a class="reference internal" href="station.html">Stations</a></li>
-<li class="toctree-l3"><a class="reference internal" href="streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l3"><a class="reference internal" href="metrics_dict.html">Metrics Dictionary</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../getting_started.html">Getting Started</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../geojson.html">GeoJSON Overview</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../terms.html">Terminology</a></li>
+<li class="toctree-l1 current has-children current-page"><a class="current reference internal" href="#">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
+<li class="toctree-l2"><a class="reference internal" href="base.html">Base Dictionary</a></li>
+<li class="toctree-l2"><a class="reference internal" href="event.html">Event</a></li>
+<li class="toctree-l2"><a class="reference internal" href="provenance.html">Provenance</a></li>
+<li class="toctree-l2 has-children"><a class="reference internal" href="features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
+<li class="toctree-l3"><a class="reference internal" href="features/station.html">Stations</a></li>
+<li class="toctree-l3"><a class="reference internal" href="features/streams_traces.html">Streams and Traces</a></li>
+<li class="toctree-l3"><a class="reference internal" href="features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../demo.html">Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../pydantic_demo.html">Pydantic Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../dev.html">Developer Notes</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../examples.html">GMP Examples</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../pydantic_demo.html">Pydantic Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
       </div>
       
@@ -209,48 +208,54 @@
           </div>
           <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="features">
-<h1>Features<a class="headerlink" href="#features" title="Permalink to this heading">#</a></h1>
-<p>Here we give more details about the features.</p>
+          <section id="specification">
+<h1>Specification<a class="headerlink" href="#specification" title="Permalink to this heading">#</a></h1>
+<p>Here we give more details about the GMP format specification.</p>
 <div class="toctree-wrapper compound">
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="station.html">Stations</a></li>
-<li class="toctree-l1"><a class="reference internal" href="streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l1"><a class="reference internal" href="metrics_dict.html">Metrics Dictionary</a></li>
+<li class="toctree-l1"><a class="reference internal" href="base.html">Base Dictionary</a></li>
+<li class="toctree-l1"><a class="reference internal" href="event.html">Event</a></li>
+<li class="toctree-l1"><a class="reference internal" href="provenance.html">Provenance</a></li>
+<li class="toctree-l1"><a class="reference internal" href="features/index.html">Features</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="features/station.html">Stations</a></li>
+<li class="toctree-l2"><a class="reference internal" href="features/streams_traces.html">Streams and Traces</a></li>
+<li class="toctree-l2"><a class="reference internal" href="features/metrics_dict.html">Metrics Dictionary</a></li>
+</ul>
+</li>
 </ul>
 </div>
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="station.html">
+          <a class="next-page" href="base.html">
               <div class="page-info">
                 <div class="context">
                   <span>Next</span>
                 </div>
-                <div class="title">Stations</div>
+                <div class="title">Base Dictionary</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
-          <a class="prev-page" href="../provenance.html">
+          <a class="prev-page" href="../terms.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Provenance</div>
+                <div class="title">Terminology</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
@@ -277,19 +282,19 @@
     </div>
     <aside class="toc-drawer no-toc">
       
       
       
     </aside>
   </div>
-</div><script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
-    <script src="../../_static/jquery.js"></script>
-    <script src="../../_static/underscore.js"></script>
-    <script src="../../_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="../../_static/doctools.js"></script>
-    <script src="../../_static/sphinx_highlight.js"></script>
-    <script src="../../_static/scripts/furo.js"></script>
-    <script src="../../_static/clipboard.min.js"></script>
-    <script src="../../_static/copybutton.js"></script>
-    <script src="../../_static/tabs.js"></script>
+</div><script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
+    <script src="../_static/jquery.js"></script>
+    <script src="../_static/underscore.js"></script>
+    <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="../_static/doctools.js"></script>
+    <script src="../_static/sphinx_highlight.js"></script>
+    <script src="../_static/scripts/furo.js"></script>
+    <script src="../_static/clipboard.min.js"></script>
+    <script src="../_static/copybutton.js"></script>
+    <script src="../_static/tabs.js"></script>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -25,45 +25,48 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
-          o Features*
+          o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Features# ******
-Here we give more details about the features.
-    * Stations
-    * Streams_and_Traces
-    * Metrics_Dictionary
+****** Specification# ******
+Here we give more details about the GMP format specification.
+    * Base_Dictionary
+    * Event
+    * Provenance
+    * Features
+          o Stations
+          o Streams_and_Traces
+          o Metrics_Dictionary
 
 Next
-Stations
+Base_Dictionary
 
 Previous
-Provenance
+Terminology
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
```

### Comparing `gmpacket-0.1.2/docs/specification/features/metrics_dict.html` & `gmpacket-0.1.3/docs/specification/features/station.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" /><link rel="next" title="Examples" href="../../examples.html" /><link rel="prev" title="Streams and Traces" href="streams_traces.html" />
+<link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" /><link rel="next" title="Streams and Traces" href="streams_traces.html" /><link rel="prev" title="Features" href="index.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Metrics Dictionary - Ground Motion Packet Documentation</title>
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>Stations - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="../../_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="../../getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../terms.html">Terminology</a></li>
 <li class="toctree-l1 current has-children"><a class="reference internal" href="../index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
 <li class="toctree-l2"><a class="reference internal" href="../base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="../event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="../provenance.html">Provenance</a></li>
 <li class="toctree-l2 current has-children"><a class="reference internal" href="index.html">Features</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
-<li class="toctree-l3"><a class="reference internal" href="station.html">Stations</a></li>
+<li class="toctree-l3 current current-page"><a class="current reference internal" href="#">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l3 current current-page"><a class="current reference internal" href="#">Metrics Dictionary</a></li>
+<li class="toctree-l3"><a class="reference internal" href="metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
@@ -209,140 +208,108 @@
           </div>
           <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="metrics-dictionary">
-<h1>Metrics Dictionary<a class="headerlink" href="#metrics-dictionary" title="Permalink to this heading">#</a></h1>
-<p>The “metrics” dictionary contains the values and metadata relevant for the
-metrics associated with the parent trace. One challenge with ground motion
-metric data is that different metrics exhibit very different structure. For
-example, some metrics are simply scalars (e.g., PGA) while others are arrays
-(e.g., response spectra, which are a function of both oscillator period and
-the assumed percent of critical damping).</p>
-<p>While it is possible to list each metric as a separate element in a list, there
-are two main drawbacks to doing so:</p>
-<ol class="arabic simple">
-<li><p>It is inefficient from a file size perspective, and</p></li>
-<li><p>It is difficult to parse because the properties will be different for each
-metric.</p></li>
-</ol>
-<p>Thus, we have designed a general metrics data structure with the goals of
-being easy to extend to a wide range of metric data structures, consistency in
-how the metrics are stored to make parsing the data more straight-forward, and
-minimizing the file size.</p>
-<p>The dictionary has the following required keys:</p>
+          <section id="stations">
+<h1>Stations<a class="headerlink" href="#stations" title="Permalink to this heading">#</a></h1>
+<p>The GeoJSON features represent seismic stations in the GMP specification.
+Station metadata is included in the GeoJSON feature “properties” dictionary.
+Requited properties include:</p>
 <dl class="simple myst">
-<dt><strong>properties</strong></dt><dd><p>A dictionary with the following keys <em>(dictionary; required)</em>:</p>
-<dl class="simple myst">
-<dt><strong>description</strong></dt><dd><p>Metric description <em>(string; required)</em>.</p>
-</dd>
-<dt><strong>name</strong></dt><dd><p>Metric name <em>(string; required)</em>.</p>
-</dd>
-<dt><strong>units</strong></dt><dd><p>Metric units <em>(string; required)</em>.</p>
+<dt><strong>type</strong></dt><dd><p>Must be “Feature” <em>(string; required)</em>.</p>
 </dd>
-<dt><strong>provenance_ids</strong></dt><dd><p>A list of strings giving provenance IDs relevant to this trace
-<em>(list; optional)</em>.</p>
+<dt><strong>geometry</strong></dt><dd><p>A dictionary with the following keys <em>(dictionary; required)</em>.</p>
+<dl class="simple myst">
+<dt><strong>type</strong></dt><dd><p>Must be “Point” <em>(string; required)</em>.</p>
 </dd>
-<dt><strong>time_of_peak</strong></dt><dd><p>Time of metric peak for the PGA metric in UTC in ISO 8601 <em>extended</em> format
-<em>(str; optional)</em>.</p>
+<dt><strong>coordinates</strong></dt><dd><p>List of coordinates as floats <em>(list; required)</em>.</p>
 </dd>
 </dl>
 </dd>
-<dt><strong>dimensions</strong></dt><dd><p>A dictionary with the following keys <em>(dictionary; required when metric is an array)</em>:</p>
+<dt><strong>properties</strong></dt><dd><p>A dictionary to store station-level metadata that contains the following
+keys <em>(dictionary; required)</em>:</p>
 <dl class="simple myst">
-<dt><strong>number</strong></dt><dd><p>The number of dimentions for this metric (<code class="docutils literal notranslate"><span class="pre">n</span></code>)
-<em>(integer; required)</em>.</p>
+<dt><strong>network_code</strong></dt><dd><p>The <a class="reference external" href="https://www.fdsn.org/networks/">FSDN</a> network code <em>(string; required)</em>.</p>
 </dd>
-<dt><strong>names</strong></dt><dd><p>A list of strings describing the metric dimension names; length must
-be equal to the number of metric dimentions <code class="docutils literal notranslate"><span class="pre">n</span></code>
-<em>(list; required)</em>.</p>
+<dt><strong>station_code</strong></dt><dd><p>FDSN station code <em>(string; required)</em>.</p>
 </dd>
-<dt><strong>units</strong></dt><dd><p>A string or list of strings describing the units of the metric dimensions;
-length must be equal to the number of metric dimentions
-<code class="docutils literal notranslate"><span class="pre">n</span></code> <em>(list; required)</em>.</p>
+<dt><strong>name</strong></dt><dd><p>Station name <em>(string; optional)</em>.</p>
 </dd>
-<dt><strong>axis_values</strong></dt><dd><p>An array giving the values of the dimensions; the first dimension of
-the array must equal the number of metric dimentions <code class="docutils literal notranslate"><span class="pre">n</span></code>;
-the lengths of each constituent array are are
-<code class="docutils literal notranslate"><span class="pre">[p,</span> <span class="pre">q,</span> <span class="pre">...]</span></code> <em>(array; required)</em>.</p>
+<dt><strong>streams</strong></dt><dd><p>A list of dictionaries, one for each stream at this station.
+<em>(list; required)</em>.</p>
 </dd>
-</dl>
+<dt><strong>structure_reference_orientation</strong></dt><dd><p>Reference for the structural coordinate system with respect to geographic north.
+Equivalent to COSMOS integer 21 <em>(int; optional)</em></p>
 </dd>
-<dt><strong>values</strong></dt><dd><p>An array giving the metric values; the dimensions of the array must be
-equal to the length of each of the dimention value arrays
-<code class="docutils literal notranslate"><span class="pre">p</span> <span class="pre">x</span> <span class="pre">q</span> <span class="pre">x</span> <span class="pre">...</span></code> <em>(float or array; required)</em>.</p>
+</dl>
 </dd>
 </dl>
-<p>An example metrics dictionary:</p>
-<div class="highlight-json notranslate"><div class="highlight"><pre><span></span><span class="w">  </span><span class="err">...</span>
-<span class="w">  </span><span class="nt">&quot;traces&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">      </span><span class="p">{</span>
-<span class="w">          </span><span class="err">...</span>
-<span class="w">          </span><span class="nt">&quot;metrics&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">              </span><span class="p">{</span>
-<span class="w">                  </span><span class="nt">&quot;properties&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
-<span class="w">                      </span><span class="nt">&quot;description&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Spectral acceleration&quot;</span><span class="p">,</span>
-<span class="w">                      </span><span class="nt">&quot;name&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;SA&quot;</span><span class="p">,</span>
-<span class="w">                      </span><span class="nt">&quot;units&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;g&quot;</span><span class="p">,</span>
-<span class="w">                      </span><span class="nt">&quot;provenance_ids&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">                          </span><span class="s2">&quot;seis_prov:sp000_sa_0000000&quot;</span><span class="p">,</span>
-<span class="w">                          </span><span class="s2">&quot;seis_prov:sp000_pp_0000000&quot;</span><span class="p">,</span>
-<span class="w">                          </span><span class="s2">&quot;seis_prov:sp000_og_0000000&quot;</span>
-<span class="w">                      </span><span class="p">]</span>
-<span class="w">                  </span><span class="p">},</span>
-<span class="w">                  </span><span class="nt">&quot;dimensions&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
-<span class="w">                      </span><span class="nt">&quot;number&quot;</span><span class="p">:</span><span class="w"> </span><span class="mi">2</span><span class="p">,</span>
-<span class="w">                      </span><span class="nt">&quot;names&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">                          </span><span class="s2">&quot;critical damping&quot;</span><span class="p">,</span>
-<span class="w">                          </span><span class="s2">&quot;period&quot;</span>
-<span class="w">                      </span><span class="p">],</span>
-<span class="w">                      </span><span class="nt">&quot;units&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span><span class="s2">&quot;%&quot;</span><span class="p">,</span><span class="w"> </span><span class="s2">&quot;s&quot;</span><span class="p">],</span>
-<span class="w">                      </span><span class="nt">&quot;values&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">                          </span><span class="p">[</span><span class="mf">5.0</span><span class="p">,</span><span class="w"> </span><span class="mf">10.0</span><span class="p">,</span><span class="w"> </span><span class="mf">20.0</span><span class="p">],</span>
-<span class="w">                          </span><span class="p">[</span><span class="mf">0.5</span><span class="p">,</span><span class="w"> </span><span class="mf">1.0</span><span class="p">]</span>
-<span class="w">                      </span><span class="p">]</span>
-<span class="w">                  </span><span class="p">},</span>
-<span class="w">                  </span><span class="nt">&quot;values&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">                      </span><span class="p">[</span><span class="mf">2.3</span><span class="p">,</span><span class="w"> </span><span class="mf">2.0</span><span class="p">],</span>
-<span class="w">                      </span><span class="p">[</span><span class="mf">1.6</span><span class="p">,</span><span class="w"> </span><span class="mf">1.4</span><span class="p">],</span>
-<span class="w">                      </span><span class="p">[</span><span class="mf">2.0</span><span class="p">,</span><span class="w"> </span><span class="mf">1.8</span><span class="p">]</span>
-<span class="w">                  </span><span class="p">]</span>
-<span class="w">              </span><span class="p">}</span>
-<span class="w">          </span><span class="p">]</span>
-<span class="w">      </span><span class="p">}</span>
-<span class="w">  </span><span class="p">]</span>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>“depth” in the station geometry coordinates array is defined as
+meters positive from the WGS84 datum. This conforms with GEOJSON
+standard, but defiates from metadata convention.</p>
+</div>
+<p>Example:</p>
+<div class="highlight-json notranslate"><div class="highlight"><pre><span></span><span class="p">{</span>
+<span class="w">    </span><span class="err">...</span>
+<span class="w">    </span><span class="nt">&quot;features&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">        </span><span class="p">{</span>
+<span class="w">            </span><span class="nt">&quot;type&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Feature&quot;</span><span class="p">,</span>
+<span class="w">            </span><span class="nt">&quot;properties&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
+<span class="w">                </span><span class="nt">&quot;network_code&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;CI&quot;</span><span class="p">,</span>
+<span class="w">                </span><span class="nt">&quot;station_code&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;CCC&quot;</span><span class="p">,</span>
+<span class="w">                </span><span class="nt">&quot;name&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Christmas Canyon China Lake&quot;</span><span class="p">,</span>
+<span class="w">                </span><span class="nt">&quot;streams&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">                    </span><span class="p">{</span>
+<span class="w">                        </span><span class="err">...</span>
+<span class="w">                    </span><span class="p">},</span>
+<span class="w">                    </span><span class="err">...</span>
+<span class="w">                </span><span class="p">]</span>
+<span class="w">            </span><span class="p">},</span>
+<span class="w">            </span><span class="nt">&quot;geometry&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
+<span class="w">                </span><span class="nt">&quot;type&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Point&quot;</span><span class="p">,</span>
+<span class="w">                </span><span class="nt">&quot;coordinates&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
+<span class="w">                    </span><span class="mf">-117.3645</span><span class="p">,</span>
+<span class="w">                    </span><span class="mf">35.5249</span><span class="p">,</span>
+<span class="w">                    </span><span class="mf">670.0</span>
+<span class="w">                </span><span class="p">]</span>
+<span class="w">            </span><span class="p">}</span>
+<span class="w">        </span><span class="p">}</span>
+<span class="w">    </span><span class="p">]</span>
+<span class="p">}</span>
 </pre></div>
 </div>
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="../../examples.html">
+          <a class="next-page" href="streams_traces.html">
               <div class="page-info">
                 <div class="context">
                   <span>Next</span>
                 </div>
-                <div class="title">Examples</div>
+                <div class="title">Streams and Traces</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
-          <a class="prev-page" href="streams_traces.html">
+          <a class="prev-page" href="index.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Streams and Traces</div>
+                <div class="title">Features</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
```

#### html2text {}

```diff
@@ -25,131 +25,98 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features*
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Metrics Dictionary# ******
-The âmetricsâ dictionary contains the values and metadata relevant for the
-metrics associated with the parent trace. One challenge with ground motion
-metric data is that different metrics exhibit very different structure. For
-example, some metrics are simply scalars (e.g., PGA) while others are arrays
-(e.g., response spectra, which are a function of both oscillator period and the
-assumed percent of critical damping).
-While it is possible to list each metric as a separate element in a list, there
-are two main drawbacks to doing so:
-   1. It is inefficient from a file size perspective, and
-   2. It is difficult to parse because the properties will be different for
-      each metric.
-Thus, we have designed a general metrics data structure with the goals of being
-easy to extend to a wide range of metric data structures, consistency in how
-the metrics are stored to make parsing the data more straight-forward, and
-minimizing the file size.
-The dictionary has the following required keys:
+****** Stations# ******
+The GeoJSON features represent seismic stations in the GMP specification.
+Station metadata is included in the GeoJSON feature âpropertiesâ
+dictionary. Requited properties include:
+  type
+      Must be âFeatureâ (string; required).
+  geometry
+      A dictionary with the following keys (dictionary; required).
+        type
+            Must be âPointâ (string; required).
+        coordinates
+            List of coordinates as floats (list; required).
   properties
-      A dictionary with the following keys (dictionary; required):
-        description
-            Metric description (string; required).
+      A dictionary to store station-level metadata that contains the following
+      keys (dictionary; required):
+        network_code
+            The FSDN network code (string; required).
+        station_code
+            FDSN station code (string; required).
         name
-            Metric name (string; required).
-        units
-            Metric units (string; required).
-        provenance_ids
-            A list of strings giving provenance IDs relevant to this trace
-            (list; optional).
-        time_of_peak
-            Time of metric peak for the PGA metric in UTC in ISO 8601 extended
-            format (str; optional).
-  dimensions
-      A dictionary with the following keys (dictionary; required when metric is
-      an array):
-        number
-            The number of dimentions for this metric (n) (integer; required).
-        names
-            A list of strings describing the metric dimension names; length
-            must be equal to the number of metric dimentions n (list;
+            Station name (string; optional).
+        streams
+            A list of dictionaries, one for each stream at this station. (list;
             required).
-        units
-            A string or list of strings describing the units of the metric
-            dimensions; length must be equal to the number of metric dimentions
-            n (list; required).
-        axis_values
-            An array giving the values of the dimensions; the first dimension
-            of the array must equal the number of metric dimentions n; the
-            lengths of each constituent array are are [p, q, ...] (array;
-            required).
-  values
-      An array giving the metric values; the dimensions of the array must be
-      equal to the length of each of the dimention value arrays p x q x ...
-      (float or array; required).
-An example metrics dictionary:
-  ...
-  "traces": [
-      {
-          ...
-          "metrics": [
-              {
-                  "properties": {
-                      "description": "Spectral acceleration",
-                      "name": "SA",
-                      "units": "g",
-                      "provenance_ids": [
-                          "seis_prov:sp000_sa_0000000",
-                          "seis_prov:sp000_pp_0000000",
-                          "seis_prov:sp000_og_0000000"
-                      ]
-                  },
-                  "dimensions": {
-                      "number": 2,
-                      "names": [
-                          "critical damping",
-                          "period"
-                      ],
-                      "units": ["%", "s"],
-                      "values": [
-                          [5.0, 10.0, 20.0],
-                          [0.5, 1.0]
-                      ]
-                  },
-                  "values": [
-                      [2.3, 2.0],
-                      [1.6, 1.4],
-                      [2.0, 1.8]
-                  ]
-              }
-          ]
-      }
-  ]
+        structure_reference_orientation
+            Reference for the structural coordinate system with respect to
+            geographic north. Equivalent to COSMOS integer 21 (int; optional)
+Note
+âdepthâ in the station geometry coordinates array is defined as meters
+positive from the WGS84 datum. This conforms with GEOJSON standard, but
+defiates from metadata convention.
+Example:
+{
+    ...
+    "features": [
+        {
+            "type": "Feature",
+            "properties": {
+                "network_code": "CI",
+                "station_code": "CCC",
+                "name": "Christmas Canyon China Lake",
+                "streams": [
+                    {
+                        ...
+                    },
+                    ...
+                ]
+            },
+            "geometry": {
+                "type": "Point",
+                "coordinates": [
+                    -117.3645,
+                    35.5249,
+                    670.0
+                ]
+            }
+        }
+    ]
+}
 
 Next
-Examples
+Streams_and_Traces
 
 Previous
-Streams_and_Traces
+Features
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
```

### Comparing `gmpacket-0.1.2/docs/specification/features/station.html` & `gmpacket-0.1.3/docs/getting_started.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" /><link rel="next" title="Streams and Traces" href="streams_traces.html" /><link rel="prev" title="Features" href="index.html" />
+<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="GeoJSON Overview" href="geojson.html" /><link rel="prev" title="Earthquake Ground Motion Data Packet" href="index.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Stations - Ground Motion Packet Documentation</title>
-      <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
-    <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/tabs.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/css/custom.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
-    <link rel="stylesheet" type="text/css" href="../../_static/pied-piper-admonition.css" />
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>Getting Started - Ground Motion Packet Documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
+    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
+    <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
+    <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
+    <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
     
 
 
 <style>
   body {
     --color-code-background: #f8f8f8;
@@ -124,65 +124,64 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
+      <a href="index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
           <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
         </button>
       </div>
-      <label class="toc-overlay-icon toc-header-icon no-toc" for="__toc">
+      <label class="toc-overlay-icon toc-header-icon" for="__toc">
         <div class="visually-hidden">Toggle table of contents sidebar</div>
         <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
       </label>
     </div>
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
-      <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
+      <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
   <span class="sidebar-brand-text">Ground Motion Packet Documentation</span>
   
-</a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
+</a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="../../geojson.html">GeoJSON Overview</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../terms.html">Terminology</a></li>
-<li class="toctree-l1 current has-children"><a class="reference internal" href="../index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
-<li class="toctree-l2"><a class="reference internal" href="../base.html">Base Dictionary</a></li>
-<li class="toctree-l2"><a class="reference internal" href="../event.html">Event</a></li>
-<li class="toctree-l2"><a class="reference internal" href="../provenance.html">Provenance</a></li>
-<li class="toctree-l2 current has-children"><a class="reference internal" href="index.html">Features</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
-<li class="toctree-l3 current current-page"><a class="current reference internal" href="#">Stations</a></li>
-<li class="toctree-l3"><a class="reference internal" href="streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l3"><a class="reference internal" href="metrics_dict.html">Metrics Dictionary</a></li>
+<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Getting Started</a></li>
+<li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
+<li class="toctree-l1"><a class="reference internal" href="terms.html">Terminology</a></li>
+<li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
+<li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
+<li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
+<li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
+<li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
+<li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
+<li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
+<li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../demo.html">Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../pydantic_demo.html">Pydantic Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../dev.html">Developer Notes</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
+<li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
       </div>
       
@@ -203,114 +202,79 @@
             <button class="theme-toggle">
               <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
               <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
               <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
               <svg class="theme-icon-when-light"><use href="#svg-sun"></use></svg>
             </button>
           </div>
-          <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
+          <label class="toc-overlay-icon toc-content-icon" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="stations">
-<h1>Stations<a class="headerlink" href="#stations" title="Permalink to this heading">#</a></h1>
-<p>The GeoJSON features represent seismic stations in the GMP specification.
-Station metadata is included in the GeoJSON feature “properties” dictionary.
-Requited properties include:</p>
-<dl class="simple myst">
-<dt><strong>type</strong></dt><dd><p>Must be “Feature” <em>(string; required)</em>.</p>
-</dd>
-<dt><strong>geometry</strong></dt><dd><p>A dictionary with the following keys <em>(dictionary; required)</em>.</p>
-<dl class="simple myst">
-<dt><strong>type</strong></dt><dd><p>Must be “Point” <em>(string; required)</em>.</p>
-</dd>
-<dt><strong>coordinates</strong></dt><dd><p>List of coordinates as floats <em>(list; required)</em>.</p>
-</dd>
-</dl>
-</dd>
-<dt><strong>properties</strong></dt><dd><p>A dictionary to store station-level metadata that contains the following
-keys <em>(dictionary; required)</em>:</p>
-<dl class="simple myst">
-<dt><strong>network_code</strong></dt><dd><p>The <a class="reference external" href="https://www.fdsn.org/networks/">FSDN</a> network code <em>(string; required)</em>.</p>
-</dd>
-<dt><strong>station_code</strong></dt><dd><p>FDSN station code <em>(string; required)</em>.</p>
-</dd>
-<dt><strong>name</strong></dt><dd><p>Station name <em>(string; optional)</em>.</p>
-</dd>
-<dt><strong>streams</strong></dt><dd><p>A list of dictionaries, one for each stream at this station.
-<em>(list; required)</em>.</p>
-</dd>
-<dt><strong>structure_reference_orientation</strong></dt><dd><p>Reference for the structural coordinate system with respect to geographic north.
-Equivalent to COSMOS integer 21 <em>(int; optional)</em></p>
-</dd>
-</dl>
-</dd>
-</dl>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>“depth” in the station geometry coordinates array is defined as
-meters positive from the WGS84 datum. This conforms with GEOJSON
-standard, but defiates from metadata convention.</p>
+          <section id="getting-started">
+<h1>Getting Started<a class="headerlink" href="#getting-started" title="Permalink to this heading">#</a></h1>
+<p>This is a python package that can be imported and the functions can be called directly in new scripts, jupyter
+notebooks, or interactive python sessions. Examples using different aspects of the GMP format can be foun in the
+<a class="reference internal" href="pydantic_demo.html"><span class="doc std std-doc">Pydantic Demo</span></a> section.</p>
+<section id="installation">
+<h2>Installation<a class="headerlink" href="#installation" title="Permalink to this heading">#</a></h2>
+<p>The basic dependencies are <code class="docutils literal notranslate"><span class="pre">pip</span></code> and <code class="docutils literal notranslate"><span class="pre">git</span></code>.</p>
+<p>The main python dependency  for the <code class="docutils literal notranslate"><span class="pre">validate</span></code> and <code class="docutils literal notranslate"><span class="pre">scan</span></code> modules is the
+<a class="reference external" href="http://seismicdata.github.io/SEIS-PROV/validation.html#official-validator">SEIS-PROV validator</a>.
+To install:</p>
+<div class="highlight-shell notranslate"><div class="highlight"><pre><span></span>git<span class="w"> </span>clone<span class="w"> </span>https://github.com/SeismicData/SEIS-PROV.git
+<span class="nb">cd</span><span class="w"> </span>SEIS-PROV/validator
+pip<span class="w"> </span>install<span class="w"> </span>-e<span class="w"> </span>.
+</pre></div>
+</div>
+<p>We also need the “schema” package:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="n">schema</span>
+</pre></div>
+</div>
+<p>Then, to install this package:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">git</span> <span class="n">clone</span> <span class="n">https</span><span class="p">:</span><span class="o">//</span><span class="n">github</span><span class="o">.</span><span class="n">com</span><span class="o">/</span><span class="n">SCEDC</span><span class="o">/</span><span class="n">ground</span><span class="o">-</span><span class="n">motion</span><span class="o">-</span><span class="n">packet</span><span class="o">.</span><span class="n">git</span>
+<span class="n">cd</span> <span class="n">ground</span><span class="o">-</span><span class="n">motion</span><span class="o">-</span><span class="n">packet</span>
+<span class="n">pip</span> <span class="n">install</span> <span class="o">-</span><span class="n">e</span> <span class="o">.</span>
+</pre></div>
 </div>
-<p>Example:</p>
-<div class="highlight-json notranslate"><div class="highlight"><pre><span></span><span class="p">{</span>
-<span class="w">    </span><span class="err">...</span>
-<span class="w">    </span><span class="nt">&quot;features&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">        </span><span class="p">{</span>
-<span class="w">            </span><span class="nt">&quot;type&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Feature&quot;</span><span class="p">,</span>
-<span class="w">            </span><span class="nt">&quot;properties&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
-<span class="w">                </span><span class="nt">&quot;network_code&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;CI&quot;</span><span class="p">,</span>
-<span class="w">                </span><span class="nt">&quot;station_code&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;CCC&quot;</span><span class="p">,</span>
-<span class="w">                </span><span class="nt">&quot;name&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Christmas Canyon China Lake&quot;</span><span class="p">,</span>
-<span class="w">                </span><span class="nt">&quot;streams&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">                    </span><span class="p">{</span>
-<span class="w">                        </span><span class="err">...</span>
-<span class="w">                    </span><span class="p">},</span>
-<span class="w">                    </span><span class="err">...</span>
-<span class="w">                </span><span class="p">]</span>
-<span class="w">            </span><span class="p">},</span>
-<span class="w">            </span><span class="nt">&quot;geometry&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">{</span>
-<span class="w">                </span><span class="nt">&quot;type&quot;</span><span class="p">:</span><span class="w"> </span><span class="s2">&quot;Point&quot;</span><span class="p">,</span>
-<span class="w">                </span><span class="nt">&quot;coordinates&quot;</span><span class="p">:</span><span class="w"> </span><span class="p">[</span>
-<span class="w">                    </span><span class="mf">-117.3645</span><span class="p">,</span>
-<span class="w">                    </span><span class="mf">35.5249</span><span class="p">,</span>
-<span class="w">                    </span><span class="mf">670.0</span>
-<span class="w">                </span><span class="p">]</span>
-<span class="w">            </span><span class="p">}</span>
-<span class="w">        </span><span class="p">}</span>
-<span class="w">    </span><span class="p">]</span>
-<span class="p">}</span>
+<p>For developers or other interested users, there are optional dependencies for development (<code class="docutils literal notranslate"><span class="pre">dev</span></code>), running tests (<code class="docutils literal notranslate"><span class="pre">test</span></code>), making documentation (<code class="docutils literal notranslate"><span class="pre">doc</span></code>), and building distributions (<code class="docutils literal notranslate"><span class="pre">build</span></code>), that can instead be installed using:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="o">-</span><span class="n">e</span> <span class="o">.</span><span class="p">[</span><span class="n">dev</span><span class="p">,</span><span class="n">test</span><span class="p">,</span><span class="n">doc</span><span class="p">,</span><span class="n">build</span><span class="p">]</span>
+</pre></div>
+</div>
+<p>Alternatively, you can install a pre-built wheel distribution directly from PyPi:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">pip</span> <span class="n">install</span> <span class="n">gmpacket</span>
 </pre></div>
 </div>
 </section>
+</section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="streams_traces.html">
+          <a class="next-page" href="geojson.html">
               <div class="page-info">
                 <div class="context">
                   <span>Next</span>
                 </div>
-                <div class="title">Streams and Traces</div>
+                <div class="title">GeoJSON Overview</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
           <a class="prev-page" href="index.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Features</div>
+                <div class="title">Home</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
@@ -331,25 +295,44 @@
               
             </div>
           </div>
         </div>
         
       </footer>
     </div>
-    <aside class="toc-drawer no-toc">
+    <aside class="toc-drawer">
+      
       
+      <div class="toc-sticky toc-scroll">
+        <div class="toc-title-container">
+          <span class="toc-title">
+            On this page
+          </span>
+        </div>
+        <div class="toc-tree-container">
+          <div class="toc-tree">
+            <ul>
+<li><a class="reference internal" href="#">Getting Started</a><ul>
+<li><a class="reference internal" href="#installation">Installation</a></li>
+</ul>
+</li>
+</ul>
+
+          </div>
+        </div>
+      </div>
       
       
     </aside>
   </div>
-</div><script data-url_root="../../" id="documentation_options" src="../../_static/documentation_options.js"></script>
-    <script src="../../_static/jquery.js"></script>
-    <script src="../../_static/underscore.js"></script>
-    <script src="../../_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="../../_static/doctools.js"></script>
-    <script src="../../_static/sphinx_highlight.js"></script>
-    <script src="../../_static/scripts/furo.js"></script>
-    <script src="../../_static/clipboard.min.js"></script>
-    <script src="../../_static/copybutton.js"></script>
-    <script src="../../_static/tabs.js"></script>
+</div><script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+    <script src="_static/jquery.js"></script>
+    <script src="_static/underscore.js"></script>
+    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/scripts/furo.js"></script>
+    <script src="_static/clipboard.min.js"></script>
+    <script src="_static/copybutton.js"></script>
+    <script src="_static/tabs.js"></script>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -25,99 +25,66 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
-    * Specification*
+    * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
-          o Features*
+          o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Stations# ******
-The GeoJSON features represent seismic stations in the GMP specification.
-Station metadata is included in the GeoJSON feature âpropertiesâ
-dictionary. Requited properties include:
-  type
-      Must be âFeatureâ (string; required).
-  geometry
-      A dictionary with the following keys (dictionary; required).
-        type
-            Must be âPointâ (string; required).
-        coordinates
-            List of coordinates as floats (list; required).
-  properties
-      A dictionary to store station-level metadata that contains the following
-      keys (dictionary; required):
-        network_code
-            The FSDN network code (string; required).
-        station_code
-            FDSN station code (string; required).
-        name
-            Station name (string; optional).
-        streams
-            A list of dictionaries, one for each stream at this station. (list;
-            required).
-        structure_reference_orientation
-            Reference for the structural coordinate system with respect to
-            geographic north. Equivalent to COSMOS integer 21 (int; optional)
-Note
-âdepthâ in the station geometry coordinates array is defined as meters
-positive from the WGS84 datum. This conforms with GEOJSON standard, but
-defiates from metadata convention.
-Example:
-{
-    ...
-    "features": [
-        {
-            "type": "Feature",
-            "properties": {
-                "network_code": "CI",
-                "station_code": "CCC",
-                "name": "Christmas Canyon China Lake",
-                "streams": [
-                    {
-                        ...
-                    },
-                    ...
-                ]
-            },
-            "geometry": {
-                "type": "Point",
-                "coordinates": [
-                    -117.3645,
-                    35.5249,
-                    670.0
-                ]
-            }
-        }
-    ]
-}
+****** Getting Started# ******
+This is a python package that can be imported and the functions can be called
+directly in new scripts, jupyter notebooks, or interactive python sessions.
+Examples using different aspects of the GMP format can be foun in the Pydantic
+Demo section.
+***** Installation# *****
+The basic dependencies are pip and git.
+The main python dependency for the validate and scan modules is the SEIS-PROV
+validator. To install:
+git clone https://github.com/SeismicData/SEIS-PROV.git
+cd SEIS-PROV/validator
+pip install -e .
+We also need the âschemaâ package:
+pip install schema
+Then, to install this package:
+git clone https://github.com/SCEDC/ground-motion-packet.git
+cd ground-motion-packet
+pip install -e .
+For developers or other interested users, there are optional dependencies for
+development (dev), running tests (test), making documentation (doc), and
+building distributions (build), that can instead be installed using:
+pip install -e .[dev,test,doc,build]
+Alternatively, you can install a pre-built wheel distribution directly from
+PyPi:
+pip install gmpacket
 
 Next
-Streams_and_Traces
+GeoJSON_Overview
 
 Previous
-Features
+Home
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
-
+ On this page
+    * Getting_Started
+          o Installation
```

### Comparing `gmpacket-0.1.2/docs/specification/features/streams_traces.html` & `gmpacket-0.1.3/docs/specification/features/streams_traces.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" /><link rel="next" title="Metrics Dictionary" href="metrics_dict.html" /><link rel="prev" title="Stations" href="station.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
         <title>Streams and Traces - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="../../_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="../../getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../terms.html">Terminology</a></li>
 <li class="toctree-l1 current has-children"><a class="reference internal" href="../index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
 <li class="toctree-l2"><a class="reference internal" href="../base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="../event.html">Event</a></li>
 <li class="toctree-l2"><a class="reference internal" href="../provenance.html">Provenance</a></li>
 <li class="toctree-l2 current has-children"><a class="reference internal" href="index.html">Features</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
 <li class="toctree-l3"><a class="reference internal" href="station.html">Stations</a></li>
 <li class="toctree-l3 current current-page"><a class="current reference internal" href="#">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../../demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../../examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
```

#### html2text {}

```diff
@@ -25,29 +25,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features*
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
```

### Comparing `gmpacket-0.1.2/docs/specification/index.html` & `gmpacket-0.1.3/docs/terms.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
-<link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" /><link rel="next" title="Base Dictionary" href="base.html" /><link rel="prev" title="Terminology" href="../terms.html" />
+<link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="Specification" href="specification/index.html" /><link rel="prev" title="GeoJSON Overview" href="geojson.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
-        <title>Specification - Ground Motion Packet Documentation</title>
-      <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
-    <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/tabs.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/css/custom.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
-    <link rel="stylesheet" type="text/css" href="../_static/pied-piper-admonition.css" />
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
+        <title>Terminology - Ground Motion Packet Documentation</title>
+      <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
+    <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
+    <link rel="stylesheet" type="text/css" href="_static/tabs.css" />
+    <link rel="stylesheet" type="text/css" href="_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
+    <link rel="stylesheet" type="text/css" href="_static/css/custom.css" />
+    <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
+    <link rel="stylesheet" type="text/css" href="_static/pied-piper-admonition.css" />
     
     
 
 
 <style>
   body {
     --color-code-background: #f8f8f8;
@@ -124,15 +124,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
+      <a href="index.html"><div class="brand">Ground Motion Packet Documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -144,45 +144,44 @@
         <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
       </label>
     </div>
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
-      <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
+      <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
   <span class="sidebar-brand-text">Ground Motion Packet Documentation</span>
   
-</a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
+</a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
-<li class="toctree-l1"><a class="reference internal" href="../geojson.html">GeoJSON Overview</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../terms.html">Terminology</a></li>
-<li class="toctree-l1 current has-children current-page"><a class="current reference internal" href="#">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
-<li class="toctree-l2"><a class="reference internal" href="base.html">Base Dictionary</a></li>
-<li class="toctree-l2"><a class="reference internal" href="event.html">Event</a></li>
-<li class="toctree-l2"><a class="reference internal" href="provenance.html">Provenance</a></li>
-<li class="toctree-l2 has-children"><a class="reference internal" href="features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
-<li class="toctree-l3"><a class="reference internal" href="features/station.html">Stations</a></li>
-<li class="toctree-l3"><a class="reference internal" href="features/streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l3"><a class="reference internal" href="features/metrics_dict.html">Metrics Dictionary</a></li>
+<li class="toctree-l1"><a class="reference internal" href="getting_started.html">Getting Started</a></li>
+<li class="toctree-l1"><a class="reference internal" href="geojson.html">GeoJSON Overview</a></li>
+<li class="toctree-l1 current current-page"><a class="current reference internal" href="#">Terminology</a></li>
+<li class="toctree-l1 has-children"><a class="reference internal" href="specification/index.html">Specification</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
+<li class="toctree-l2"><a class="reference internal" href="specification/base.html">Base Dictionary</a></li>
+<li class="toctree-l2"><a class="reference internal" href="specification/event.html">Event</a></li>
+<li class="toctree-l2"><a class="reference internal" href="specification/provenance.html">Provenance</a></li>
+<li class="toctree-l2 has-children"><a class="reference internal" href="specification/features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
+<li class="toctree-l3"><a class="reference internal" href="specification/features/station.html">Stations</a></li>
+<li class="toctree-l3"><a class="reference internal" href="specification/features/streams_traces.html">Streams and Traces</a></li>
+<li class="toctree-l3"><a class="reference internal" href="specification/features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../demo.html">Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../pydantic_demo.html">Pydantic Demo</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../dev.html">Developer Notes</a></li>
+<li class="toctree-l1"><a class="reference internal" href="examples.html">GMP Examples</a></li>
+<li class="toctree-l1"><a class="reference internal" href="pydantic_demo.html">Pydantic Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
 
       </div>
       
@@ -209,54 +208,78 @@
           </div>
           <label class="toc-overlay-icon toc-content-icon no-toc" for="__toc">
             <div class="visually-hidden">Toggle table of contents sidebar</div>
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
-          <section id="specification">
-<h1>Specification<a class="headerlink" href="#specification" title="Permalink to this heading">#</a></h1>
-<p>Here we give more details about the GMP format specification.</p>
-<div class="toctree-wrapper compound">
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="base.html">Base Dictionary</a></li>
-<li class="toctree-l1"><a class="reference internal" href="event.html">Event</a></li>
-<li class="toctree-l1"><a class="reference internal" href="provenance.html">Provenance</a></li>
-<li class="toctree-l1"><a class="reference internal" href="features/index.html">Features</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="features/station.html">Stations</a></li>
-<li class="toctree-l2"><a class="reference internal" href="features/streams_traces.html">Streams and Traces</a></li>
-<li class="toctree-l2"><a class="reference internal" href="features/metrics_dict.html">Metrics Dictionary</a></li>
-</ul>
-</li>
-</ul>
-</div>
+          <section id="terminology">
+<h1>Terminology<a class="headerlink" href="#terminology" title="Permalink to this heading">#</a></h1>
+<dl class="simple myst">
+<dt><a class="reference external" href="https://www.json.org/json-en.html">JSON</a></dt><dd><p>A standard file format, which stands for JavaScript Object Notation.
+This standard is appealing because it is human readable, allows for
+flexible data structures, and is supported by many programming languages.</p>
+</dd>
+<dt><a class="reference external" href="https://geojson.org/">GeoJSON</a></dt><dd><p>A JSON specification that is designed for spatial data. This is a
+format that can be read by most GIS software and is supported in many
+programming languages.</p>
+</dd>
+<dt><strong>Feature</strong></dt><dd><p>GeoJSON term for specifying a spatial object (point, line, or polygon).
+Here all of our features will be points (denoting
+latitude/longitude/elevation of a station and/or an event).</p>
+</dd>
+<dt><strong>Intensity Measure/Metric</strong></dt><dd><p>A parametric representation of a ground motion record. Examples include
+PGA or PGV, spectral acceleration, Arias Intensity, significant duration,
+cumulative absolute velocity, and inelastic response spectra.</p>
+</dd>
+<dt><strong>Trace</strong></dt><dd><p>A reference to the time series used to compute the <b>Intensity
+Measure/Metric</b>. This might be from a single seismic data channel
+(e.g., HNE, HNN) or a derived combination of seismic channels such as the
+rotd50 or transverse time series. This is often referred to as
+“component” in other contexts, especially when the station has only one
+sensor sampled at one sample rate. We use the term “trace” to avoid
+confusion with the use of the term “component” in the instrumentation
+context and therefore avoid assumptions about sample rate and
+orientation. Note that these terms are important for defining the
+hierarchy of the data structure, but this format does not report the time
+series array itself.</p>
+</dd>
+<dt><strong>Stream</strong></dt><dd><p>A collection of traces. The terms
+“<a class="reference external" href="https://docs.obspy.org/packages/autogen/obspy.core.trace.Trace.html">trace</a>” and
+“<a class="reference external" href="https://docs.obspy.org/packages/autogen/obspy.core.stream.Stream.html">stream</a>”
+follow the terminology adopted by <a class="reference external" href="https://docs.obspy.org/">ObsPy</a>.</p>
+</dd>
+<dt><strong>Provenance</strong></dt><dd><p>A <a class="reference external" href="http://seismicdata.github.io/SEIS-PROV/">SEIS-PROV</a>-compliant
+provenance document.</p>
+</dd>
+</dl>
 </section>
 
         </article>
       </div>
       <footer>
         
         <div class="related-pages">
-          <a class="next-page" href="base.html">
+          <a class="next-page" href="specification/index.html">
               <div class="page-info">
                 <div class="context">
                   <span>Next</span>
                 </div>
-                <div class="title">Base Dictionary</div>
+                <div class="title">Specification</div>
               </div>
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
             </a>
-          <a class="prev-page" href="../terms.html">
+          <a class="prev-page" href="geojson.html">
               <svg class="furo-related-icon"><use href="#svg-arrow-right"></use></svg>
               <div class="page-info">
                 <div class="context">
                   <span>Previous</span>
                 </div>
                 
-                <div class="title">Terminology</div>
+                <div class="title">GeoJSON Overview</div>
                 
               </div>
             </a>
         </div>
         <div class="bottom-of-page">
           <div class="left-details">
             <div class="copyright">
@@ -283,19 +306,19 @@
     </div>
     <aside class="toc-drawer no-toc">
       
       
       
     </aside>
   </div>
-</div><script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
-    <script src="../_static/jquery.js"></script>
-    <script src="../_static/underscore.js"></script>
-    <script src="../_static/_sphinx_javascript_frameworks_compat.js"></script>
-    <script src="../_static/doctools.js"></script>
-    <script src="../_static/sphinx_highlight.js"></script>
-    <script src="../_static/scripts/furo.js"></script>
-    <script src="../_static/clipboard.min.js"></script>
-    <script src="../_static/copybutton.js"></script>
-    <script src="../_static/tabs.js"></script>
+</div><script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
+    <script src="_static/jquery.js"></script>
+    <script src="_static/underscore.js"></script>
+    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
+    <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
+    <script src="_static/scripts/furo.js"></script>
+    <script src="_static/clipboard.min.js"></script>
+    <script src="_static/copybutton.js"></script>
+    <script src="_static/tabs.js"></script>
     </body>
 </html>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -25,49 +25,72 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
-    * Specification*
+    * Specification⁰
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-****** Specification# ******
-Here we give more details about the GMP format specification.
-    * Base_Dictionary
-    * Event
-    * Provenance
-    * Features
-          o Stations
-          o Streams_and_Traces
-          o Metrics_Dictionary
+****** Terminology# ******
+  JSON
+      A standard file format, which stands for JavaScript Object Notation. This
+      standard is appealing because it is human readable, allows for flexible
+      data structures, and is supported by many programming languages.
+  GeoJSON
+      A JSON specification that is designed for spatial data. This is a format
+      that can be read by most GIS software and is supported in many
+      programming languages.
+  Feature
+      GeoJSON term for specifying a spatial object (point, line, or polygon).
+      Here all of our features will be points (denoting latitude/longitude/
+      elevation of a station and/or an event).
+  Intensity Measure/Metric
+      A parametric representation of a ground motion record. Examples include
+      PGA or PGV, spectral acceleration, Arias Intensity, significant duration,
+      cumulative absolute velocity, and inelastic response spectra.
+  Trace
+      A reference to the time series used to compute the Intensity Measure/
+      Metric. This might be from a single seismic data channel (e.g., HNE, HNN)
+      or a derived combination of seismic channels such as the rotd50 or
+      transverse time series. This is often referred to as âcomponentâ in
+      other contexts, especially when the station has only one sensor sampled
+      at one sample rate. We use the term âtraceâ to avoid confusion with
+      the use of the term âcomponentâ in the instrumentation context and
+      therefore avoid assumptions about sample rate and orientation. Note that
+      these terms are important for defining the hierarchy of the data
+      structure, but this format does not report the time series array itself.
+  Stream
+      A collection of traces. The terms âtraceâ and âstreamâ follow the
+      terminology adopted by ObsPy.
+  Provenance
+      A SEIS-PROV-compliant provenance document.
 
 Next
-Base_Dictionary
+Specification
 
 Previous
-Terminology
+GeoJSON_Overview
 Copyright © Unlicense
 Made with Sphinx and @pradyunsg's Furo
 __
```

### Comparing `gmpacket-0.1.2/docs/specification/provenance.html` & `gmpacket-0.1.3/docs/specification/provenance.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" /><link rel="next" title="Features" href="features/index.html" /><link rel="prev" title="Event" href="event.html" />
 
-    <!-- Generated with Sphinx 5.3.0 and Furo 2022.12.07 -->
+    <!-- Generated with Sphinx 5.3.0 and Furo 2023.03.27 -->
         <title>Provenance - Ground Motion Packet Documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
-    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=91d0f0d1c444bdcb17a68e833c7a53903343c195" />
+    <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=fad236701ea90a88636c2a8c73b44ae642ed2a53" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/tabs.css" />
     <link rel="stylesheet" type="text/css" href="../_static/mystnb.4510f1fc1dee50b3e5859aac5469c37c29e427902b24a333a5f9fcb2f0b3ac41.css" />
     <link rel="stylesheet" type="text/css" href="../_static/css/custom.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     <link rel="stylesheet" type="text/css" href="../_static/pied-piper-admonition.css" />
     
@@ -156,31 +156,30 @@
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder="Search" name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
   <ul class="current">
+<li class="toctree-l1"><a class="reference internal" href="../getting_started.html">Getting Started</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../geojson.html">GeoJSON Overview</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../terms.html">Terminology</a></li>
 <li class="toctree-l1 current has-children"><a class="reference internal" href="index.html">Specification</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" role="switch" type="checkbox"/><label for="toctree-checkbox-1"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul class="current">
 <li class="toctree-l2"><a class="reference internal" href="base.html">Base Dictionary</a></li>
 <li class="toctree-l2"><a class="reference internal" href="event.html">Event</a></li>
 <li class="toctree-l2 current current-page"><a class="current reference internal" href="#">Provenance</a></li>
 <li class="toctree-l2 has-children"><a class="reference internal" href="features/index.html">Features</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" role="switch" type="checkbox"/><label for="toctree-checkbox-2"><div class="visually-hidden">Toggle child pages in navigation</div><i class="icon"><svg><use href="#svg-arrow-right"></use></svg></i></label><ul>
 <li class="toctree-l3"><a class="reference internal" href="features/station.html">Stations</a></li>
 <li class="toctree-l3"><a class="reference internal" href="features/streams_traces.html">Streams and Traces</a></li>
 <li class="toctree-l3"><a class="reference internal" href="features/metrics_dict.html">Metrics Dictionary</a></li>
 </ul>
 </li>
 </ul>
 </li>
-<li class="toctree-l1"><a class="reference internal" href="../examples.html">Examples</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../cli.html">Command Line Tools</a></li>
-<li class="toctree-l1"><a class="reference internal" href="../demo.html">Demo</a></li>
+<li class="toctree-l1"><a class="reference internal" href="../examples.html">GMP Examples</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../pydantic_demo.html">Pydantic Demo</a></li>
 <li class="toctree-l1"><a class="reference internal" href="../dev.html">Developer Notes</a></li>
 </ul>
 
 </div>
 </div>
```

#### html2text {}

```diff
@@ -25,29 +25,28 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
 Ground_Motion_Packet_Documentation
 [q                   ]
+    * Getting_Started
     * GeoJSON_Overview
     * Terminology
     * Specification*
       Toggle child pages in navigation
           o Base_Dictionary
           o Event
           o Provenance
           o Features⁰
             Toggle child pages in navigation
                 # Stations
                 # Streams_and_Traces
                 # Metrics_Dictionary
-    * Examples
-    * Command_Line_Tools
-    * Demo
+    * GMP_Examples
     * Pydantic_Demo
     * Developer_Notes
 ___Back_to_top
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
```

### Comparing `gmpacket-0.1.2/gmpacket/data/examples/borehole_example.json` & `gmpacket-0.1.3/gmpacket/data/examples/borehole_example.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/data/examples/example1.json` & `gmpacket-0.1.3/gmpacket/data/examples/example1.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/data/examples/multichannel_example.json` & `gmpacket-0.1.3/gmpacket/data/examples/multichannel_example.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/data/examples/sps-100-200-example.json` & `gmpacket-0.1.3/gmpacket/data/examples/sps-100-200-example.json`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/feature.py` & `gmpacket-0.1.3/gmpacket/feature.py`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/packet.py` & `gmpacket-0.1.3/gmpacket/packet.py`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/provenance.py` & `gmpacket-0.1.3/gmpacket/provenance.py`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/scan.py` & `gmpacket-0.1.3/gmpacket/scan.py`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket/validate.py` & `gmpacket-0.1.3/gmpacket/validate.py`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/gmpacket.egg-info/PKG-INFO` & `gmpacket-0.1.3/gmpacket.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmpacket
-Version: 0.1.2
+Version: 0.1.3
 Summary: ANSS Ground Motion Packet
 Home-page: https://github.com/SCEDC/ground-motion-packet
 Author: Ellen Yu, Lijam Hagos, Jamie Steidl, Eric Thompson, Bruce Worden
 Author-email: Mike Hearne <mhearne@usgs.gov>, Eric Thompson <ethompson@usgs.gov>, Ellen Yu <eyu@caltech.edu>
 License: License
         =======
         
@@ -13,14 +13,16 @@
         http://unlicense.org/
         
 Keywords: ground motion,earthquake
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: build
 License-File: LICENSE.md
 
 # Description of GMP —A GeoJSON Specification for Ground Motion Metrics
 
 Here we present a specification for a GeoJSON (https://geojson.org/) format for 
 unassociated and event-associated ground motion metrics—that is, quantities 
 derived from ground motion records (e.g., accelerograms, velocity recordings).
```

### Comparing `gmpacket-0.1.2/install.sh` & `gmpacket-0.1.3/install.sh`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/notebooks/pydantic_demo.ipynb` & `gmpacket-0.1.3/notebooks/pydantic_demo.ipynb`

 * *Files identical despite different names*

### Comparing `gmpacket-0.1.2/pyproject.toml` & `gmpacket-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gmpacket"
-version = "0.1.2"
+dynamic = ["version"]
 description = "ANSS Ground Motion Packet"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Eric Thompson", email="ethompson@usgs.gov"},
     {name = "Ellen Yu", email="eyu@caltech.edu"},
 ]
 
@@ -17,56 +17,57 @@
 
 dependencies = [
     "geopy>=2.1.0",
     "pandas>=1.4.0",
     "pydantic[email]>=1.10.0",
 ]
 
-dynamic = ["entry-points"]
-
-[project.scripts]
-gmpformat = "gmpacket.bin.gmpformat:main"
-
 [tool.setuptools]
-packages = ["gmpacket", "gmpacket.bin"]
+packages = ["gmpacket"]
 
 
 
 [project.optional-dependencies]
 dev = [
-    "altair",
-    "build>=0.7.0",
     "black>=21",
     "flake8>=3.9",
-    "furo",
     "ipython>=7.26",
+    "setuptools_scm",
+    "notebook>=6.4.1",
+]
+test = [
+    "deepdiff>=5.7.0",
+    "openpyxl>=3.0.9",
+    "pytest>=6.2",
+    "pytest-cov>=2.12.0",
+
+]
+doc = [
+    "sphinx>3.0.0",
+    "requests>=2",
+    "furo",
     "myst-nb",
     "myst-parser",
+    "altair",
     "nbsphinx",
-    "notebook>=6.4.1",
-    "twine>=3.8.0",
     "recommonmark",
-    "requests>=2",
-    "setuptools_scm",
-    "sphinx>3.0.0",
     "sphinx-autoapi",
     "sphinx-copybutton",
     "sphinx-inline-tabs",
     "sphinxcontrib-programoutput"
 ]
-test = [
-    "deepdiff>=5.7.0",
-    "openpyxl>=3.0.9",
-    "pytest>=6.2",
-    "pytest-cov>=2.12.0",
-
+build = [
+    "build",
+    "twine",
 ]
 
 [build-system]
 requires = [
   "setuptools>=42",
   "wheel",
   "setuptools_scm[toml]>=3.4",
   "Cython>=0.29.23",
   "numpy",
 ]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
```

