# Comparing `tmp/streamlink-5.3.1.tar.gz` & `tmp/streamlink-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlink-5.3.1.tar", last modified: Sat Feb 25 01:14:54 2023, max compression
+gzip compressed data, was "streamlink-5.4.0.tar", last modified: Wed Apr 12 18:44:03 2023, max compression
```

## Comparing `streamlink-5.3.1.tar` & `streamlink-5.4.0.tar`

### file list

```diff
@@ -1,569 +1,571 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.090853 streamlink-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-25 01:14:08.000000 streamlink-5.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    70836 2023-02-25 01:14:08.000000 streamlink-5.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-25 01:14:08.000000 streamlink-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-25 01:14:08.000000 streamlink-5.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-02-25 01:14:54.090853 streamlink-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-02-25 01:14:08.000000 streamlink-5.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.014851 streamlink-5.3.1/completions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.018852 streamlink-5.3.1/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-02-25 01:14:41.000000 streamlink-5.3.1/completions/bash/streamlink
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.018852 streamlink-5.3.1/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)    32411 2023-02-25 01:14:42.000000 streamlink-5.3.1/completions/zsh/_streamlink
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-25 01:14:08.000000 streamlink-5.3.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.022852 streamlink-5.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_applications.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.014851 streamlink-5.3.1/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.022852 streamlink-5.3.1/docs/_build/man/
--rw-r--r--   0 runner    (1001) docker     (123)    37068 2023-02-25 01:14:46.000000 streamlink-5.3.1/docs/_build/man/streamlink.1
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_man.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.026852 streamlink-5.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/icon-ffmpeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/icon-python.svg
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/opengraph-image.png
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/site.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.026852 streamlink-5.3.1/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_static/styles/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.026852 streamlink-5.3.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_templates/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.026852 streamlink-5.3.1/docs/_templates/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_templates/sidebar/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/_templates/sidebar/github-buttons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/api_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/applications.rst
--rw-r--r--   0 runner    (1001) docker     (123)    70836 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.026852 streamlink-5.3.1/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/plugin-sideloading.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.026852 streamlink-5.3.1/docs/cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/plugins/crunchyroll.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/plugins/twitch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/protocols.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/proxy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/deprecations.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/donate.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/ext_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/ext_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/ext_html_template_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/ext_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/ext_releaseref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24180 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/issues.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/players.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs/thirdparty.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-25 01:14:08.000000 streamlink-5.3.1/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-02-25 01:14:08.000000 streamlink-5.3.1/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-02-25 01:14:08.000000 streamlink-5.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-02-25 01:14:54.090853 streamlink-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-02-25 01:14:08.000000 streamlink-5.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.018852 streamlink-5.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.094853 streamlink-5.3.1/src/streamlink/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-25 01:14:54.094853 streamlink-5.3.1/src/streamlink/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.030852 streamlink-5.3.1/src/streamlink/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/packages/requests_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.030852 streamlink-5.3.1/src/streamlink/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.030852 streamlink-5.3.1/src/streamlink/plugin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/useragents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.030852 streamlink-5.3.1/src/streamlink/plugin/api/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/validate/_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/validate/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/validate/_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/validate/_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/api/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)    25703 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.046852 streamlink-5.3.1/src/streamlink/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/app17.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/btv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/htv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/huya.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/nbcnews.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/nos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/qq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/streann.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/stv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    26269 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/useetv.py
--rw-r--r--   0 runner    (1001) docker     (123)    19111 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/vk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/welt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)    15130 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/plugins/zhanqi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24850 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.050852 streamlink-5.3.1/src/streamlink/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    28436 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/dash_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    30590 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/hls.py
--rw-r--r--   0 runner    (1001) docker     (123)    20619 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/segmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/stream/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/user_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.050852 streamlink-5.3.1/src/streamlink/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/args.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink/utils/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.030852 streamlink-5.3.1/src/streamlink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-02-25 01:14:53.000000 streamlink-5.3.1/src/streamlink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-02-25 01:14:54.000000 streamlink-5.3.1/src/streamlink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 01:14:53.000000 streamlink-5.3.1/src/streamlink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-25 01:14:53.000000 streamlink-5.3.1/src/streamlink.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-25 01:14:53.000000 streamlink-5.3.1/src/streamlink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-25 01:14:53.000000 streamlink-5.3.1/src/streamlink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.050852 streamlink-5.3.1/src/streamlink_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31699 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.054852 streamlink-5.3.1/src/streamlink_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/utils/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/utils/player.py
--rw-r--r--   0 runner    (1001) docker     (123)    10384 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-02-25 01:14:08.000000 streamlink-5.3.1/src/streamlink_cli/utils/versioncheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.054852 streamlink-5.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.054852 streamlink-5.3.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.058852 streamlink-5.3.1/tests/cli/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/output/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/output/test_playeroutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_cmdline_player_fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_cmdline_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    35849 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_main_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_main_setup_config_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    23635 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/test_streamrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.058852 streamlink-5.3.1/tests/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/utils/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/cli/utils/test_versioncheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.058852 streamlink-5.3.1/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/mixins/stream_hls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.058852 streamlink-5.3.1/tests/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.058852 streamlink-5.3.1/tests/plugin/override/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugin/override/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugin/testplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugin/testplugin_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugin/testplugin_missing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.074852 streamlink-5.3.1/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_abematv.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_adultswim.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_afreeca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_albavision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_aloula.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_app17.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ard_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ard_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_artetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_atpchallenger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_atresplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_bbciplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_bfmtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_bigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_bilibili.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_blazetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_bloomberg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_booyah.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_brightcove.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_btv.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_cbsnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_cdnbg.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ceskatelevize.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_cinergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_clubbingtv.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_cmmedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_cnews.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_crunchyroll.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_dailymotion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_delfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_deutschewelle.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_dlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_dogan.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_dogus.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_drdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_earthcam.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_euronews.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_facebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_filmon.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_foxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_galatasaraytv.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_goltelevision.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_goodgame.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_googledrive.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_gulli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_hiplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_htv.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_huajiao.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_huya.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_idf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_invintus.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_kugou.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_linelive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_livestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ltv_lsm_lv.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mdstrm.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mediaklikk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mediavitrina.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mildom.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mitele.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mixcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mjunoon.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_mrtmk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_n13tv.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_nbcnews.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_nhkworld.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_nicolive.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_nimotv.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_nos.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_nownews.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_nrk.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ntv.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_okru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_olympicchannel.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_oneplusone.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_onetv.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_openrectv.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_pandalive.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_picarto.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_piczel.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_pixiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_pluto.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_pluzz.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_qq.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_radiko.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_radionet.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_raiplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_reuters.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_rtbf.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_rtpa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_rtpplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_rtve.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_rtvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ruv.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_sbscokr.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_showroom.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_sportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_sportschau.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ssh101.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_stadium.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_steam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_streamable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_streann.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_stv.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_svtplay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_swisstxt.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_telefe.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tf1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_trovo.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_turkuvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tv360.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tv3cat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tv4play.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tv5monde.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tv8.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tv999.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tvibo.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tviplayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tvrby.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tvrplus.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_tvtoya.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_twitcasting.py
--rw-r--r--   0 runner    (1001) docker     (123)    31521 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_twitch.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_useetv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ustreamtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_ustvnow.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_vidio.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_vimeo.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_vinhlongtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_vk.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_vkplay.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_vlive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_vtvgo.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_wasd.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_webtv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_welt.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_wwenetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_youtube.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_yupptv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_zattoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_zdf_mediathek.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_zeenews.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_zengatv.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/plugins/test_zhanqi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.074852 streamlink-5.3.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.018852 streamlink-5.3.1/tests/resources/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.078853 streamlink-5.3.1/tests/resources/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/cli/config/custom
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/cli/config/primary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/cli/config/primary.testplugin
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/cli/config/secondary
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/cli/config/secondary.testplugin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.078853 streamlink-5.3.1/tests/resources/dash/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_10.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_11_static.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_3.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_4.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_5.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_6_p1.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_6_p2.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_7.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_8.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_9.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_nested_baseurls.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/dash/test_segments_byterange.mpd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.078853 streamlink-5.3.1/tests/resources/hls/
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/hls/test_1.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/hls/test_2.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/hls/test_date.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/hls/test_master.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/resources/hls/test_master_twitch_vod.m3u8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.086853 streamlink-5.3.1/tests/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)    14631 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_dash_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_ffmpegmux.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    29444 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_hls_filtered.py
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_hls_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_stream_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_stream_to_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/stream/test_stream_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_api_http_session.py
--rw-r--r--   0 runner    (1001) docker     (123)    48697 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_api_websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    10015 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    15313 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_plugin_userinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    22837 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/test_streamlink_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.086853 streamlink-5.3.1/tests/testutils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/testutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/testutils/handshake.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/testutils/test_handshake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:54.090853 streamlink-5.3.1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_l10n.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_named_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_processoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-02-25 01:14:08.000000 streamlink-5.3.1/tests/utils/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-12 18:43:13.000000 streamlink-5.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    74305 2023-04-12 18:43:13.000000 streamlink-5.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-12 18:43:13.000000 streamlink-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-12 18:43:13.000000 streamlink-5.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-12 18:44:03.087135 streamlink-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-12 18:43:13.000000 streamlink-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/completions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.987133 streamlink-5.4.0/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-04-12 18:43:49.000000 streamlink-5.4.0/completions/bash/streamlink
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.987133 streamlink-5.4.0/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-04-12 18:43:49.000000 streamlink-5.4.0/completions/zsh/_streamlink
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-12 18:43:13.000000 streamlink-5.4.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.991133 streamlink-5.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_applications.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.991133 streamlink-5.4.0/docs/_build/man/
+-rw-r--r--   0 runner    (1001) docker     (123)    37413 2023-04-12 18:43:54.000000 streamlink-5.4.0/docs/_build/man/streamlink.1
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_man.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/icon-ffmpeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/icon-python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/opengraph-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/site.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_static/styles/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/_templates/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/sidebar/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/_templates/sidebar/github-buttons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/api_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/applications.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    74305 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugin-sideloading.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.995133 streamlink-5.4.0/docs/cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugins/crunchyroll.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugins/twitch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/protocols.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/proxy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/deprecations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/donate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_html_template_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/ext_releaseref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/issues.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/players.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs/thirdparty.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 18:43:13.000000 streamlink-5.4.0/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-04-12 18:43:13.000000 streamlink-5.4.0/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-12 18:43:13.000000 streamlink-5.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-12 18:44:03.091135 streamlink-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-12 18:43:13.000000 streamlink-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.091135 streamlink-5.4.0/src/streamlink/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-12 18:44:03.091135 streamlink-5.4.0/src/streamlink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.999133 streamlink-5.4.0/src/streamlink/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/packages/requests_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.003133 streamlink-5.4.0/src/streamlink/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.003133 streamlink-5.4.0/src/streamlink/plugin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/useragents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.003133 streamlink-5.4.0/src/streamlink/plugin/api/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/validate/_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/api/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25759 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.035134 streamlink-5.4.0/src/streamlink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9680 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26292 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/plugins/zhanqi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25641 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.035134 streamlink-5.4.0/src/streamlink/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13506 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34203 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/dash_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20608 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/segmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/stream/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/user_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.039134 streamlink-5.4.0/src/streamlink/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink/utils/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.999133 streamlink-5.4.0/src/streamlink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16363 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 18:44:02.000000 streamlink-5.4.0/src/streamlink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.039134 streamlink-5.4.0/src/streamlink_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43909 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32194 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.043134 streamlink-5.4.0/src/streamlink_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-12 18:43:13.000000 streamlink-5.4.0/src/streamlink_cli/utils/versioncheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/cli/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/output/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/output/test_playeroutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_cmdline_player_fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_cmdline_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38201 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_main_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_main_setup_config_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23237 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/test_streamrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.047134 streamlink-5.4.0/tests/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/cli/utils/test_versioncheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.051134 streamlink-5.4.0/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/mixins/stream_hls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.051134 streamlink-5.4.0/tests/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.051134 streamlink-5.4.0/tests/plugin/override/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/override/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/testplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/testplugin_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugin/testplugin_missing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.079135 streamlink-5.4.0/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_abematv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_adultswim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_afreeca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_albavision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_aloula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_app17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ard_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ard_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_artetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_atpchallenger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_atresplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bbciplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bfmtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bilibili.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_blazetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_bloomberg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_booyah.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_brightcove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_btv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cbsnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cdnbg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ceskatelevize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cinergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_clubbingtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cmmedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_cnews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_crunchyroll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dailymotion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_delfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_deutschewelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dogan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_dogus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_drdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_earthcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_euronews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_facebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_filmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_foxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_galatasaraytv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_goltelevision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_goodgame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_googledrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_gulli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_hiplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_htv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_huajiao.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_huya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_idf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_indihometv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_invintus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_kugou.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_linelive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_livestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ltv_lsm_lv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mdstrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mediaklikk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mediavitrina.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mildom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mitele.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mixcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mjunoon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_mrtmk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_n13tv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nhkworld.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nicolive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nimotv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nownews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_nrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ntv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_okru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_olympicchannel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_oneplusone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_onetv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_openrectv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pandalive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_picarto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_piczel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pixiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pluto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_pluzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_qq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_radiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_radionet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_raiplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_reuters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtpa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtpplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_rtvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ruv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_sbscokr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_showroom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_sportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ssh101.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_stadium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_steam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_streamable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_streann.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_stv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_svtplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_swisstxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_telefe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_telemadrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_trovo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_turkuvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv360.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv3cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv4play.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv5monde.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tv999.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvibo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tviplayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvrby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvrplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_tvtoya.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_twitcasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ustreamtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_ustvnow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vidio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vimeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vinhlongtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vkplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vlive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_vtvgo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_wasd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_webtv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_welt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_wwenetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_youtube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_yupptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zattoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zdf_mediathek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zeenews.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zengatv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/plugins/test_zhanqi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.079135 streamlink-5.4.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:02.983133 streamlink-5.4.0/tests/resources/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.079135 streamlink-5.4.0/tests/resources/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/custom
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/primary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/primary.testplugin
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/secondary
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/cli/config/secondary.testplugin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.083135 streamlink-5.4.0/tests/resources/dash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_10.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_11_static.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_3.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_8.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_9.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_nested_baseurls.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_no_segment_list_or_template.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_segment_list.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_segments_byterange.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_segments_dynamic_number.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_static_no_publish_time.mpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/dash/test_timeline_ids.mpd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.083135 streamlink-5.4.0/tests/resources/hls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_1.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_2.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_date.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_master.m3u8
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/resources/hls/test_master_twitch_vod.m3u8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/tests/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19665 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_dash_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_ffmpegmux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29307 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_hls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_hls_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_hls_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_stream_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_stream_to_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/stream/test_stream_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_api_http_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48733 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_api_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10625 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15329 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_plugin_userinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/test_streamlink_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/tests/testutils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/testutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/testutils/handshake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/testutils/test_handshake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 18:44:03.087135 streamlink-5.4.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_l10n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_named_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_processoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-12 18:43:13.000000 streamlink-5.4.0/tests/utils/test_url.py
```

### Comparing `streamlink-5.3.1/CHANGELOG.md` & `streamlink-5.4.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,39 @@
 # Changelog
 
+## streamlink 5.4.0 (2023-04-12)
+
+Release highlights:
+
+- Added: `--progress` CLI argument and [deprecated `--force-progress`](https://streamlink.github.io/deprecations.html#deprecation-of-force-progress) ([#5268](https://github.com/streamlink/streamlink/pull/5268))
+- Added: `--dash-manifest-reload-attempts` and respective session option ([#5208](https://github.com/streamlink/streamlink/pull/5208))
+- Improved: DASH segment availability/download logging ([#5214](https://github.com/streamlink/streamlink/pull/5214), [#5235](https://github.com/streamlink/streamlink/pull/5235))
+- Refactored: DASH parser + stream implementation ([#5221](https://github.com/streamlink/streamlink/pull/5221), [#5224](https://github.com/streamlink/streamlink/pull/5224), [#5225](https://github.com/streamlink/streamlink/pull/5225), [#5244](https://github.com/streamlink/streamlink/pull/5244), [#5248](https://github.com/streamlink/streamlink/pull/5248))
+- Fixed: DASH segment template numbers and availability times ([#5213](https://github.com/streamlink/streamlink/pull/5213), [#5217](https://github.com/streamlink/streamlink/pull/5217), [#5233](https://github.com/streamlink/streamlink/pull/5233))
+- Fixed: DASH manifest mediaPresentationDuration and period duration ([#5226](https://github.com/streamlink/streamlink/pull/5226))
+- Fixed: DASH manifest suggestedPresentationDelay ([#5215](https://github.com/streamlink/streamlink/pull/5215))
+- Fixed: various DASH manifest parsing bugs ([#5247](https://github.com/streamlink/streamlink/pull/5247))
+- Fixed: DASH timeline IDs not being unique ([#5199](https://github.com/streamlink/streamlink/pull/5199))
+- Fixed: DASH substreams not having synced timelines ([#5262](https://github.com/streamlink/streamlink/pull/5262))
+- Fixed: queued DASH segments being downloaded after closing the stream ([#5236](https://github.com/streamlink/streamlink/pull/5236), [#5237](https://github.com/streamlink/streamlink/pull/5237))
+- Fixed: incorrect min/max values of certain numeric CLI arguments ([#5239](https://github.com/streamlink/streamlink/pull/5239))
+- Fixed: all naive datetime objects and made them timezone-aware ([#5210](https://github.com/streamlink/streamlink/pull/5210))
+- Fixed: TV5monde plugin with new implementation ([#5206](https://github.com/streamlink/streamlink/pull/5206))
+- Fixed: Steam plugin missing CDN auth data in stream URLs ([#5222](https://github.com/streamlink/streamlink/pull/5222))
+- Fixed: Vimeo plugin's playerConfig regex ([#5227](https://github.com/streamlink/streamlink/pull/5227))
+- Fixed: VKplay plugin's validation schema ([#5251](https://github.com/streamlink/streamlink/pull/5251))
+- Fixed: Twitcasting plugin with new implementation ([#5255](https://github.com/streamlink/streamlink/pull/5255))
+- Tests: fixed setuptools/pkg\_resources DeprecationWarnings ([#5167](https://github.com/streamlink/streamlink/pull/5167), [#5230](https://github.com/streamlink/streamlink/pull/5230))
+- Tests: fixed ResourceWarnings due to stale file handles ([#5242](https://github.com/streamlink/streamlink/pull/5242))
+- Added plugins: indihometv ([#5266](https://github.com/streamlink/streamlink/pull/5266)), telemadrid ([#5212](https://github.com/streamlink/streamlink/pull/5212))
+- Removed plugins: nbcnews ([#5279](https://github.com/streamlink/streamlink/pull/5279)), useetv ([#5266](https://github.com/streamlink/streamlink/pull/5266))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.3.1...5.4.0)
+
+
 ## streamlink 5.3.1 (2023-02-25)
 
 Patch release:
 
 - Fixed: `http-trust-env` session option name (`--http-ignore-env` CLI parameter) ([#5193](https://github.com/streamlink/streamlink/pull/5193))
 - Fixed: missing byterange attribute of initialization segments in DASH streams ([#5189](https://github.com/streamlink/streamlink/pull/5189))
 - Fixed: broken BaseURL context in DASH streams ([#5194](https://github.com/streamlink/streamlink/pull/5194))
```

### Comparing `streamlink-5.3.1/LICENSE` & `streamlink-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/PKG-INFO` & `streamlink-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.3.1
+Version: 5.4.0
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.3.1 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 5.4.0 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Home-page: https://github.com/streamlink/
 streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
 Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
 URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
 https://streamlink.github.io/latest/donate.html Classifier: Development Status
```

### Comparing `streamlink-5.3.1/README.md` & `streamlink-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/completions/bash/streamlink` & `streamlink-5.4.0/completions/bash/streamlink`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # AUTOMATICALLY GENERATED by `shtab`
 
 
 
-_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-f' '--force' '--force-progress' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-disable-reruns' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
+_shtab_streamlink_cli_option_strings=('-h' '--help' '-V' '--version' '--plugins' '--plugin-dirs' '--can-handle-url' '--can-handle-url-no-redirect' '--config' '-l' '--loglevel' '--logfile' '-Q' '--quiet' '-j' '--json' '--auto-version-check' '--version-check' '--locale' '--interface' '-4' '--ipv4' '-6' '--ipv6' '-p' '--player' '-a' '--player-args' '-v' '--verbose-player' '-n' '--player-fifo' '--fifo' '--player-http' '--player-continuous-http' '--player-external-http' '--player-external-http-continuous' '--player-external-http-port' '--player-passthrough' '--player-no-close' '-t' '--title' '-o' '--output' '-O' '--stdout' '-r' '--record' '-R' '--record-and-pipe' '--fs-safe-rules' '-f' '--force' '--progress' '--force-progress' '--url' '--default-stream' '--stream-url' '--retry-streams' '--retry-max' '--retry-open' '--stream-types' '--stream-priority' '--stream-sorting-excludes' '--ringbuffer-size' '--stream-segment-attempts' '--stream-segment-threads' '--stream-segment-timeout' '--stream-timeout' '--mux-subtitles' '--hls-live-edge' '--hls-segment-stream-data' '--hls-playlist-reload-attempts' '--hls-playlist-reload-time' '--hls-segment-ignore-names' '--hls-segment-key-uri' '--hls-audio-select' '--hls-start-offset' '--hls-duration' '--hls-live-restart' '--dash-manifest-reload-attempts' '--ffmpeg-ffmpeg' '--ffmpeg-no-validation' '--ffmpeg-verbose' '--ffmpeg-verbose-path' '--ffmpeg-fout' '--ffmpeg-video-transcode' '--ffmpeg-audio-transcode' '--ffmpeg-copyts' '--ffmpeg-start-at-zero' '--http-proxy' '--http-cookie' '--http-header' '--http-query-param' '--http-ignore-env' '--http-no-ssl-verify' '--http-disable-dh' '--http-ssl-cert' '--http-ssl-cert-crt-key' '--http-timeout' '--afreeca-username' '--afreeca-password' '--afreeca-purge-credentials' '--bbciplayer-username' '--bbciplayer-password' '--bbciplayer-hd' '--clubbingtv-username' '--clubbingtv-password' '--crunchyroll-username' '--crunchyroll-password' '--crunchyroll-purge-credentials' '--crunchyroll-session-id' '--niconico-email' '--niconico-password' '--niconico-user-session' '--niconico-purge-credentials' '--niconico-timeshift-offset' '--openrectv-email' '--openrectv-password' '--pixiv-sessionid' '--pixiv-devicetoken' '--pixiv-purge-credentials' '--pixiv-performer' '--steam-email' '--steam-password' '--streann-url' '--twitcasting-password' '--twitch-disable-ads' '--twitch-disable-reruns' '--twitch-low-latency' '--twitch-api-header' '--twitch-access-token-param' '--ustream-password' '--ustvnow-username' '--ustvnow-password' '--wwenetwork-email' '--wwenetwork-password' '--yupptv-boxid' '--yupptv-yuppflixtoken' '--yupptv-purge-credentials' '--zattoo-email' '--zattoo-password' '--zattoo-purge-credentials' '--zattoo-stream-types')
 
 
 
 _shtab_streamlink_cli__l_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___loglevel_choices=('none' 'critical' 'error' 'warning' 'info' 'debug' 'trace' 'all')
 _shtab_streamlink_cli___fs_safe_rules_choices=('POSIX' 'Windows')
+_shtab_streamlink_cli___progress_choices=('yes' 'force' 'no')
 
 _shtab_streamlink_cli__h_nargs=0
 _shtab_streamlink_cli___help_nargs=0
 _shtab_streamlink_cli__V_nargs=0
 _shtab_streamlink_cli___version_nargs=0
 _shtab_streamlink_cli___plugins_nargs=0
 _shtab_streamlink_cli__Q_nargs=0
@@ -29,19 +30,19 @@
 _shtab_streamlink_cli__n_nargs=0
 _shtab_streamlink_cli___player_fifo_nargs=0
 _shtab_streamlink_cli___fifo_nargs=0
 _shtab_streamlink_cli___player_http_nargs=0
 _shtab_streamlink_cli___player_continuous_http_nargs=0
 _shtab_streamlink_cli___player_external_http_nargs=0
 _shtab_streamlink_cli___player_no_close_nargs=0
+_shtab_streamlink_cli__O_nargs=0
+_shtab_streamlink_cli___stdout_nargs=0
 _shtab_streamlink_cli__f_nargs=0
 _shtab_streamlink_cli___force_nargs=0
 _shtab_streamlink_cli___force_progress_nargs=0
-_shtab_streamlink_cli__O_nargs=0
-_shtab_streamlink_cli___stdout_nargs=0
 _shtab_streamlink_cli___stream_url_nargs=0
 _shtab_streamlink_cli___mux_subtitles_nargs=0
 _shtab_streamlink_cli___hls_segment_stream_data_nargs=0
 _shtab_streamlink_cli___hls_live_restart_nargs=0
 _shtab_streamlink_cli___ffmpeg_no_validation_nargs=0
 _shtab_streamlink_cli___ffmpeg_verbose_nargs=0
 _shtab_streamlink_cli___ffmpeg_copyts_nargs=0
```

### Comparing `streamlink-5.3.1/completions/zsh/_streamlink` & `streamlink-5.4.0/completions/zsh/_streamlink`

 * *Files 2% similar despite different names*

```diff
@@ -264,21 +264,14 @@
 
         Unsupported characters in substituted variables will be replaced with an underscore.
 
         Example\:
 
             \%(prog)s --output \"\~\/recordings\/\{author\}\/\{category\}\/\{id\}-\{time\:\%\%Y\%\%m\%\%d\%\%H\%\%M\%\%S\}.ts\" \<URL\> \[STREAM\]
         ]:output:"
-  {-f,--force}"[
-        When using --output or --record, always write to file even if it already exists (overwrite).
-        ]"
-  "--force-progress[
-        When using --output or --record,
-        show the download progress bar even if there is no terminal.
-        ]"
   {-O,--stdout}"[
         Write stream data to stdout instead of playing it.
         ]"
   {-r,--record}"[
         Open the stream in the player, while at the same time writing it to \`FILENAME\`. If \`FILENAME\` is set to \`-\` (dash),
         then the stream data will be written to stdout, similar to the --stdout argument, while still opening the player.
 
@@ -319,14 +312,25 @@
         shares that are enforcing Windows filename limitations, etc.
 
         These characters are replaced with an underscore for the rules in use\:
 
         - POSIX\: \`\\x00-\\x1F \/\`
         - Windows\: \`\\x00-\\x1F \\x7F \" \* \/ \: \< \> \? \\ \|\`
         ]:fs_safe_rules:(POSIX Windows)"
+  {-f,--force}"[
+        When using --output or --record, always write to file even if it already exists (overwrite).
+        ]"
+  "--progress[
+        When using --output or --record, show or hide the download progress bar, or force it if there\'s no terminal.
+
+        Default is yes.
+        ]:progress:(yes force no)"
+  "--force-progress[
+        Deprecated in favor of --progress\=force.
+        ]"
   "--url[
         A URL to attempt to extract streams from.
 
         Usually, the protocol of http(s) URLs can be omitted (\`https\:\/\/\`),
         depending on the implementation of the plugin being used.
 
         This is an alternative to setting the URL using a positional argument
@@ -469,15 +473,15 @@
         this, please refer to the player\'s own documentation for the required configuration. Player parameters can be set via
         --player-args.
         ]:hls_live_edge:"
   "--hls-segment-stream-data[
         Immediately write segment data into output buffer while downloading.
         ]"
   "--hls-playlist-reload-attempts[
-        How many attempts should be done to reload the HLS playlist before giving up.
+        Max number of attempts when reloading the HLS playlist before giving up.
 
         Default is 3.
         ]:hls_playlist_reload_attempts:"
   "--hls-playlist-reload-time[
         Set a custom HLS playlist reload time value, either in seconds
         or by using one of the following keywords\:
 
@@ -539,14 +543,19 @@
         nearest HLS segment.
 
         Default is unlimited.
         ]:hls_duration:"
   "--hls-live-restart[
         Skip to the beginning of a live stream, or as far back as possible.
         ]"
+  "--dash-manifest-reload-attempts[
+        Max number of attempts when reloading the DASH manifest before giving up.
+
+        Default is 3.
+        ]:dash_manifest_reload_attempts:"
   "--ffmpeg-ffmpeg[
         FFMPEG is used to access or mux separate video and audio streams. You
         can specify the location of the ffmpeg executable if it is not in your
         \`PATH\`.
 
         Example\: --ffmpeg-ffmpeg \"\/usr\/local\/bin\/ffmpeg\"
         ]:ffmpeg_ffmpeg:"
```

### Comparing `streamlink-5.3.1/docs/Makefile` & `streamlink-5.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_build/man/streamlink.1` & `streamlink-5.4.0/docs/_build/man/streamlink.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "STREAMLINK" "1" "Feb 25, 2023" "5.3.1" "Streamlink"
+.TH "STREAMLINK" "1" "Apr 12, 2023" "5.4.0" "Streamlink"
 .SH NAME
 streamlink \- extracts streams from various services and pipes them into a video player of choice
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -532,27 +532,14 @@
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B \-f
-.TP
-.B \-\-force
-When using \fI\%\-\-output\fP or \fI\%\-\-record\fP, always write to file even if it already exists (overwrite).
-.UNINDENT
-.INDENT 0.0
-.TP
-.B \-\-force\-progress
-When using \fI\%\-\-output\fP or \fI\%\-\-record\fP,
-show the download progress bar even if there is no terminal.
-.UNINDENT
-.INDENT 0.0
-.TP
 .B \-O
 .TP
 .B \-\-stdout
 Write stream data to stdout instead of playing it.
 .UNINDENT
 .INDENT 0.0
 .TP
@@ -624,14 +611,33 @@
 .INDENT 7.0
 .IP \(bu 2
 POSIX: \fB\ex00\-\ex1F /\fP
 .IP \(bu 2
 Windows: \fB\ex00\-\ex1F \ex7F \(dq * / : < > ? \e |\fP
 .UNINDENT
 .UNINDENT
+.INDENT 0.0
+.TP
+.B \-f
+.TP
+.B \-\-force
+When using \fI\%\-\-output\fP or \fI\%\-\-record\fP, always write to file even if it already exists (overwrite).
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-progress {yes,force,no}
+When using \fI\%\-\-output\fP or \fI\%\-\-record\fP, show or hide the download progress bar, or force it if there\(aqs no terminal.
+.sp
+Default is: \fByes\fP\&.
+.UNINDENT
+.INDENT 0.0
+.TP
+.B \-\-force\-progress
+Deprecated in favor of \fI\%\-\-progress=force\fP\&.
+.UNINDENT
 .SS Stream options
 .INDENT 0.0
 .TP
 .B \-\-url URL
 A URL to attempt to extract streams from.
 .sp
 Usually, the protocol of http(s) URLs can be omitted (\fBhttps://\fP),
@@ -854,15 +860,15 @@
 .TP
 .B \-\-hls\-segment\-stream\-data
 Immediately write segment data into output buffer while downloading.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-hls\-playlist\-reload\-attempts ATTEMPTS
-How many attempts should be done to reload the HLS playlist before giving up.
+Max number of attempts when reloading the HLS playlist before giving up.
 .sp
 Default is: \fB3\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-hls\-playlist\-reload\-time TIME
 Set a custom HLS playlist reload time value, either in seconds
@@ -971,14 +977,22 @@
 Default is: \fBunlimited\fP\&.
 .UNINDENT
 .INDENT 0.0
 .TP
 .B \-\-hls\-live\-restart
 Skip to the beginning of a live stream, or as far back as possible.
 .UNINDENT
+.SS DASH options
+.INDENT 0.0
+.TP
+.B \-\-dash\-manifest\-reload\-attempts ATTEMPTS
+Max number of attempts when reloading the DASH manifest before giving up.
+.sp
+Default is: \fB3\fP\&.
+.UNINDENT
 .SS FFmpeg options
 .INDENT 0.0
 .TP
 .B \-\-ffmpeg\-ffmpeg FILENAME
 FFMPEG is used to access or mux separate video and audio streams. You
 can specify the location of the ffmpeg executable if it is not in your
 \fBPATH\fP\&.
```

### Comparing `streamlink-5.3.1/docs/_man.rst` & `streamlink-5.4.0/docs/_man.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/apple-touch-icon.png` & `streamlink-5.4.0/docs/_static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/favicon-16x16.png` & `streamlink-5.4.0/docs/_static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/favicon-32x32.png` & `streamlink-5.4.0/docs/_static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/favicon.ico` & `streamlink-5.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/icon-ffmpeg.svg` & `streamlink-5.4.0/docs/_static/icon-ffmpeg.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/icon-python.svg` & `streamlink-5.4.0/docs/_static/icon-python.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/icon.svg` & `streamlink-5.4.0/docs/_static/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/opengraph-image.png` & `streamlink-5.4.0/docs/_static/opengraph-image.png`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_static/styles/custom.css` & `streamlink-5.4.0/docs/_static/styles/custom.css`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_templates/base.html` & `streamlink-5.4.0/docs/_templates/base.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_templates/sidebar/brand.html` & `streamlink-5.4.0/docs/_templates/sidebar/brand.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/_templates/sidebar/github-buttons.html` & `streamlink-5.4.0/docs/_templates/sidebar/github-buttons.html`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/api.rst` & `streamlink-5.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/api_guide.rst` & `streamlink-5.4.0/docs/api_guide.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/applications.rst` & `streamlink-5.4.0/docs/applications.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/changelog.md` & `streamlink-5.4.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,39 @@
 # Changelog
 
+## streamlink 5.4.0 (2023-04-12)
+
+Release highlights:
+
+- Added: `--progress` CLI argument and [deprecated `--force-progress`](https://streamlink.github.io/deprecations.html#deprecation-of-force-progress) ([#5268](https://github.com/streamlink/streamlink/pull/5268))
+- Added: `--dash-manifest-reload-attempts` and respective session option ([#5208](https://github.com/streamlink/streamlink/pull/5208))
+- Improved: DASH segment availability/download logging ([#5214](https://github.com/streamlink/streamlink/pull/5214), [#5235](https://github.com/streamlink/streamlink/pull/5235))
+- Refactored: DASH parser + stream implementation ([#5221](https://github.com/streamlink/streamlink/pull/5221), [#5224](https://github.com/streamlink/streamlink/pull/5224), [#5225](https://github.com/streamlink/streamlink/pull/5225), [#5244](https://github.com/streamlink/streamlink/pull/5244), [#5248](https://github.com/streamlink/streamlink/pull/5248))
+- Fixed: DASH segment template numbers and availability times ([#5213](https://github.com/streamlink/streamlink/pull/5213), [#5217](https://github.com/streamlink/streamlink/pull/5217), [#5233](https://github.com/streamlink/streamlink/pull/5233))
+- Fixed: DASH manifest mediaPresentationDuration and period duration ([#5226](https://github.com/streamlink/streamlink/pull/5226))
+- Fixed: DASH manifest suggestedPresentationDelay ([#5215](https://github.com/streamlink/streamlink/pull/5215))
+- Fixed: various DASH manifest parsing bugs ([#5247](https://github.com/streamlink/streamlink/pull/5247))
+- Fixed: DASH timeline IDs not being unique ([#5199](https://github.com/streamlink/streamlink/pull/5199))
+- Fixed: DASH substreams not having synced timelines ([#5262](https://github.com/streamlink/streamlink/pull/5262))
+- Fixed: queued DASH segments being downloaded after closing the stream ([#5236](https://github.com/streamlink/streamlink/pull/5236), [#5237](https://github.com/streamlink/streamlink/pull/5237))
+- Fixed: incorrect min/max values of certain numeric CLI arguments ([#5239](https://github.com/streamlink/streamlink/pull/5239))
+- Fixed: all naive datetime objects and made them timezone-aware ([#5210](https://github.com/streamlink/streamlink/pull/5210))
+- Fixed: TV5monde plugin with new implementation ([#5206](https://github.com/streamlink/streamlink/pull/5206))
+- Fixed: Steam plugin missing CDN auth data in stream URLs ([#5222](https://github.com/streamlink/streamlink/pull/5222))
+- Fixed: Vimeo plugin's playerConfig regex ([#5227](https://github.com/streamlink/streamlink/pull/5227))
+- Fixed: VKplay plugin's validation schema ([#5251](https://github.com/streamlink/streamlink/pull/5251))
+- Fixed: Twitcasting plugin with new implementation ([#5255](https://github.com/streamlink/streamlink/pull/5255))
+- Tests: fixed setuptools/pkg\_resources DeprecationWarnings ([#5167](https://github.com/streamlink/streamlink/pull/5167), [#5230](https://github.com/streamlink/streamlink/pull/5230))
+- Tests: fixed ResourceWarnings due to stale file handles ([#5242](https://github.com/streamlink/streamlink/pull/5242))
+- Added plugins: indihometv ([#5266](https://github.com/streamlink/streamlink/pull/5266)), telemadrid ([#5212](https://github.com/streamlink/streamlink/pull/5212))
+- Removed plugins: nbcnews ([#5279](https://github.com/streamlink/streamlink/pull/5279)), useetv ([#5266](https://github.com/streamlink/streamlink/pull/5266))
+
+[Full changelog](https://github.com/streamlink/streamlink/compare/5.3.1...5.4.0)
+
+
 ## streamlink 5.3.1 (2023-02-25)
 
 Patch release:
 
 - Fixed: `http-trust-env` session option name (`--http-ignore-env` CLI parameter) ([#5193](https://github.com/streamlink/streamlink/pull/5193))
 - Fixed: missing byterange attribute of initialization segments in DASH streams ([#5189](https://github.com/streamlink/streamlink/pull/5189))
 - Fixed: broken BaseURL context in DASH streams ([#5194](https://github.com/streamlink/streamlink/pull/5194))
```

### Comparing `streamlink-5.3.1/docs/cli/config.rst` & `streamlink-5.4.0/docs/cli/config.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli/metadata.rst` & `streamlink-5.4.0/docs/cli/metadata.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli/plugin-sideloading.rst` & `streamlink-5.4.0/docs/cli/plugin-sideloading.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli/plugins/crunchyroll.rst` & `streamlink-5.4.0/docs/cli/plugins/crunchyroll.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli/plugins/twitch.rst` & `streamlink-5.4.0/docs/cli/plugins/twitch.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli/protocols.rst` & `streamlink-5.4.0/docs/cli/protocols.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli/proxy.rst` & `streamlink-5.4.0/docs/cli/proxy.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli/tutorial.rst` & `streamlink-5.4.0/docs/cli/tutorial.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/cli.rst` & `streamlink-5.4.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/conf.py` & `streamlink-5.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/deprecations.rst` & `streamlink-5.4.0/docs/deprecations.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Deprecations
 ============
 
+streamlink 5.4.0
+----------------
+
+Deprecation of --force-progress
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+The ``--force-progress`` CLI argument has been deprecated in favor of :option:`--progress=force`.
+
+
 streamlink 5.3.0
 ----------------
 
 Deprecation of global plugin arguments
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The ``is_global=True`` :py:class:`plugin argument <streamlink.options.Argument>` parameter has been deprecated.
```

### Comparing `streamlink-5.3.1/docs/developing.rst` & `streamlink-5.4.0/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/donate.rst` & `streamlink-5.4.0/docs/donate.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/ext_argparse.py` & `streamlink-5.4.0/docs/ext_argparse.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from sphinx.util.nodes import nested_parse_with_titles
 
 
 _block_re = re.compile(r":\n{2}\s{2}")
 _default_re = re.compile(r"Default is (.+)\.\n")
 _note_re = re.compile(r"Note: (.*)(?:\n\n|\n*$)", re.DOTALL)
 _option_line_re = re.compile(r"^(?!\s{2,}%\(prog\)s|\s{2,}--\w[\w-]*\w\b|Example: )(.+)$", re.MULTILINE)
-_option_re = re.compile(r"(?:^|(?<=\s))(--\w[\w-]*\w)\b")
+_option_re = re.compile(r"(?:^|(?<=\s))(?P<arg>--\w[\w-]*\w)(?P<val>=\w+)?\b")
 _prog_re = re.compile(r"%\(prog\)s")
 _percent_re = re.compile(r"%%")
 _cli_metadata_variables_section_cross_link_re = re.compile(r"the \"Metadata variables\" section")
 _inline_code_block_re = re.compile(r"(?<!`)`([^`]+?)`")
 _example_inline_code_block_re = re.compile(r"(?<=^Example: )(.+)$", re.MULTILINE)
 
 
@@ -63,23 +63,17 @@
         )
 
         helptext = _example_inline_code_block_re.sub(r":code:`\1`", helptext)
 
         # Replace option references with links.
         # Do this before indenting blocks and notes.
         helptext = _option_line_re.sub(
-            lambda m: (
-                _option_re.sub(
-                    lambda m2: (
-                        ":option:`{0}`".format(m2.group(1))
-                        if m2.group(1) in self._available_options
-                        else m2.group(0)
-                    ),
-                    m.group(1),
-                )
+            lambda m: _option_re.sub(
+                lambda m2: f":option:`{m2['arg']}{m2['val'] or ''}`" if m2["arg"] in self._available_options else m2[0],
+                m[1],
             ),
             helptext,
         )
 
         # Create simple blocks.
         helptext = _block_re.sub("::\n\n  ", helptext)
```

### Comparing `streamlink-5.3.1/docs/ext_github.py` & `streamlink-5.4.0/docs/ext_github.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/ext_plugins.py` & `streamlink-5.4.0/docs/ext_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,15 +213,15 @@
                 for item in self._re_metadata_item.finditer(metadata):
                     key, value = item.groups()
                     pluginmetadata.set(key, value)
 
                 return pluginmetadata
 
             except Exception as err:
-                raise ExtensionError(f"Error while parsing plugin file {pluginfile.name}", err)
+                raise ExtensionError(f"Error while parsing plugin file {pluginfile.name}", err) from err
 
 
 class PluginsDirective(Directive):
     def run(self):
         pluginfinder = PluginFinder()
 
         node = nodes.section()
```

### Comparing `streamlink-5.3.1/docs/ext_releaseref.py` & `streamlink-5.4.0/docs/ext_releaseref.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 import os.path
 
 from docutils import nodes
 from sphinx.util.nodes import split_explicit_title
 
 
-def releaseref_role(name, rawtext, text, lineno, inliner, options={}, content=[]):
+def releaseref_role(name, rawtext, text, lineno, inliner, options=None, content=None):
     config = inliner.document.settings.env.config
     text = text.replace("|version|", config.version)
     text = text.replace("|release|", config.release)
 
     has_explicit_title, title, target = split_explicit_title(text)
     if not has_explicit_title:
         title = os.path.basename(target)
 
-    node = nodes.reference(rawtext, title, refuri=target, **options)
+    node = nodes.reference(rawtext, title, refuri=target, **(options or {}))
 
     return [node], []
 
 
 def setup(app):
     app.add_role("releaseref", releaseref_role)
```

### Comparing `streamlink-5.3.1/docs/index.rst` & `streamlink-5.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/install.rst` & `streamlink-5.4.0/docs/install.rst`

 * *Files 2% similar despite different names*

```diff
@@ -179,33 +179,28 @@
 
                                      `NixOS channel`_
 
 `openSUSE`_                          .. code-block:: bash
 
                                         sudo zypper install streamlink
 
-`Solus`_                             .. code-block:: bash
-
-                                        sudo eopkg install streamlink
-
 `Void`_                              .. code-block:: bash
 
                                         sudo xbps-install streamlink
 ==================================== ===========================================
 
 .. _Arch Linux: https://www.archlinux.org/packages/community/any/streamlink/
 .. _Arch Linux (aur, git): https://aur.archlinux.org/packages/streamlink-git/
 .. _Debian (sid, testing): https://packages.debian.org/unstable/streamlink
 .. _Debian (stable): https://packages.debian.org/unstable/streamlink
 .. _Fedora: https://src.fedoraproject.org/rpms/python-streamlink
 .. _Gentoo Linux: https://packages.gentoo.org/package/net-misc/streamlink
 .. _NetBSD (pkgsrc): https://pkgsrc.se/multimedia/streamlink
 .. _NixOS: https://github.com/NixOS/nixpkgs/tree/master/pkgs/applications/video/streamlink
 .. _openSUSE: https://build.opensuse.org/package/show/multimedia:apps/streamlink
-.. _Solus: https://dev.getsol.us/source/streamlink/
 .. _Void: https://github.com/void-linux/void-packages/tree/master/srcpkgs/streamlink
 
 .. _Installing AUR packages: https://wiki.archlinux.org/index.php/Arch_User_Repository#Installing_packages
 .. _Installing Debian backported packages: https://wiki.debian.org/Backports#Using_the_command_line
 .. _NixOS channel: https://search.nixos.org/packages?show=streamlink&query=streamlink
 
 
@@ -222,15 +217,14 @@
 Chocolatey                           Scott Walters <me at scowalt.com>
 Debian                               Alexis Murzeau <amubtdx at gmail.com>
 Fedora                               Mohamed El Morabity <melmorabity at fedoraproject.org>
 Gentoo                               soredake <fdsfgs at krutt.org>
 NetBSD                               Maya Rashish <maya at netbsd.org>
 NixOS                                Tuomas Tynkkynen <tuomas.tynkkynen at iki.fi>
 openSUSE                             Simon Puchert <simonpuchert at alice.de>
-Solus                                Joey Riches <josephriches at gmail.com>
 Void                                 Michal Vasilek <michal at vasilek.cz>
 Windows binaries                     Sebastian Meyer <mail at bastimeyer.de>
 Linux AppImages                      Sebastian Meyer <mail at bastimeyer.de>
 ==================================== ===========================================
 
 
 Package availability
```

### Comparing `streamlink-5.3.1/docs/issues.rst` & `streamlink-5.4.0/docs/issues.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/players.rst` & `streamlink-5.4.0/docs/players.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/docs/thirdparty.rst` & `streamlink-5.4.0/docs/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/icon.svg` & `streamlink-5.4.0/icon.svg`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/pyproject.toml` & `streamlink-5.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 # https://docs.pytest.org/en/latest/reference/customize.html#configuration
 # https://docs.pytest.org/en/latest/reference/reference.html#ini-options-ref
 [tool.pytest.ini_options]
 filterwarnings = [
   "always",
-  "ignore:.*pkg_resources\\.declare_namespace.*:DeprecationWarning",
+  "ignore:::pkg_resources",
 ]
 
 
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 source = [
@@ -77,18 +77,22 @@
   "PLC",
   "PLE",
   "PLW",
   # isort
   "I",
   # flake8-builtins
   "A",
+  # flake8-bugbear
+  "B",
   # flake8-commas
   "COM",
   # flake8-comprehensions
   "C4",
+  # flake8-datetimez
+  "DTZ",
   # flake8-implicit-str-concat
   "ISC",
   # flake8-pie
   "PIE",
   # flake8-pytest-style
   "PT",
   # flake8-quotes
@@ -96,27 +100,29 @@
   # flake8-tidy-imports
   "TID",
 ]
 extend-ignore = [
   "A003",  # builtin-attribute-shadowing
   "C408",  # unnecessary-collection-call
   "ISC003",  # explicit-string-concatenation
+  "PLC1901",  # compare-to-empty-string
   "PLW2901",  # redefined-loop-name
 ]
 extend-exclude = [
   "docs/conf.py",
   "src/streamlink/packages/",
   "src/streamlink_cli/packages/",
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "src/streamlink/__init__.py" = ["I"]
 "src/streamlink/_version.py" = ["I"]
 "src/streamlink/plugin/api/useragents.py" = ["E501"]
+"src/streamlink_cli/main.py" = ["PLW0603"]
 
 [tool.ruff.isort]
 known-first-party = ["streamlink", "streamlink_cli"]
 lines-after-imports = 2
 combine-as-imports = true
 
 [tool.ruff.flake8-tidy-imports]
```

### Comparing `streamlink-5.3.1/setup.cfg` & `streamlink-5.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/setup.py` & `streamlink-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/__init__.py` & `streamlink-5.4.0/src/streamlink/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/_version.py` & `streamlink-5.4.0/src/streamlink/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
     return get_version(
         project_dir=Path(streamlink.__file__).parents[2],
     )
 
 
 # The following _get_version() call will get replaced by versioningit with a static version string when building streamlink
 # `pip install .` / `pip wheel .` / `python setup.py build` / `python setup.py bdist_wheel` / etc.
-__version__ = "5.3.1"
+__version__ = "5.4.0"
```

### Comparing `streamlink-5.3.1/src/streamlink/api.py` & `streamlink-5.4.0/src/streamlink/api.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/buffers.py` & `streamlink-5.4.0/src/streamlink/buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/cache.py` & `streamlink-5.4.0/src/streamlink/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/exceptions.py` & `streamlink-5.4.0/src/streamlink/exceptions.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/logger.py` & `streamlink-5.4.0/src/streamlink/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import sys
 import warnings
-from datetime import datetime
 from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING
 from pathlib import Path
 from sys import version_info
 from threading import Lock
 from typing import IO, TYPE_CHECKING, Iterator, List, Optional, Union
 
 # noinspection PyProtectedMember
 from warnings import WarningMessage
 
 from streamlink.exceptions import StreamlinkWarning
+from streamlink.utils.times import fromlocaltimestamp
 
 
 if TYPE_CHECKING:  # pragma: no cover
     _BaseLoggerClass = logging.Logger
 else:
     _BaseLoggerClass = logging.getLoggerClass()
 
@@ -103,15 +103,15 @@
         self.remove_base = remove_base or []
         self._usesTime = (style == "%" and "%(asctime)" in fmt) or (style == "{" and "{asctime}" in fmt)
 
     def usesTime(self):
         return self._usesTime
 
     def formatTime(self, record, datefmt=None):
-        tdt = datetime.fromtimestamp(record.created)
+        tdt = fromlocaltimestamp(record.created)
 
         return tdt.strftime(datefmt or self.default_time_format)
 
     def formatMessage(self, record):
         if self.style == "{":
             return self.fmt.format(**record.__dict__)
         else:
@@ -162,19 +162,19 @@
 
     warning = WarningMessage(message, category, filename, lineno, None, line)
     kwargs = {"stacklevel": 2} if sys.version_info >= (3, 8) else {}
     root.log(WARNING, warning, **kwargs)
 
 
 def capturewarnings(capture=False):
-    global _showwarning_default
+    global _showwarning_default  # noqa: PLW0603
 
     if capture:
         if _showwarning_default is None:
-            _showwarning_default = warnings.showwarning
+            _showwarning_default = warnings.showwarning  # noqa: PLW0603
             warnings.showwarning = _showwarning
     else:
         if _showwarning_default is not None:
             warnings.showwarning = _showwarning_default
             _showwarning_default = None
```

### Comparing `streamlink-5.3.1/src/streamlink/options.py` & `streamlink-5.4.0/src/streamlink/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,17 @@
         self.sensitive = sensitive
         self._default = options.get("default")
         self.is_global = is_global
         if is_global:
             warnings.warn(
                 "Defining global plugin arguments is deprecated. Use the session options instead.",
                 StreamlinkDeprecationWarning,
+                # set stacklevel to 3 because of the @pluginargument decorator
+                # which is the public interface for defining plugin arguments
+                stacklevel=3,
             )
 
     @staticmethod
     def _normalize_name(name: str) -> str:
         return name.replace("_", "-").strip("-")
 
     @staticmethod
```

### Comparing `streamlink-5.3.1/src/streamlink/packages/requests_file.py` & `streamlink-5.4.0/src/streamlink/packages/requests_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugin/__init__.py` & `streamlink-5.4.0/src/streamlink/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/http_session.py` & `streamlink-5.4.0/src/streamlink/plugin/api/http_session.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -148,19 +148,19 @@
             params.update(session.params)
 
         while True:
             try:
                 res = super().request(
                     method,
                     url,
+                    *args,
                     headers=headers,
                     params=params,
                     timeout=timeout,
                     proxies=proxies,
-                    *args,
                     **kwargs,
                 )
                 if raise_for_status and res.status_code not in acceptable_status:
                     res.raise_for_status()
                 break
             except KeyboardInterrupt:
                 raise
```

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/useragents.py` & `streamlink-5.4.0/src/streamlink/plugin/api/useragents.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-ANDROID = "Mozilla/5.0 (Linux; Android 13) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.5414.117 Mobile Safari/537.36"
-CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"
+ANDROID = "Mozilla/5.0 (Linux; Android 13) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.5563.116 Mobile Safari/537.36"
+CHROME = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"
 CHROME_OS = "Mozilla/5.0 (X11; CrOS x86_64 15236.80.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.5414.125 Safari/537.36"
-FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/109.0"
+FIREFOX = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:111.0) Gecko/20100101 Firefox/111.0"
 IE_11 = "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko"
-IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 16_3 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.3 Mobile/15E148 Safari/604.1"
-OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36 OPR/94.0.4606.65"
-SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_2) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.3 Safari/605.1.15"
+IPHONE = "Mozilla/5.0 (iPhone; CPU iPhone OS 16_4 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Mobile/15E148 Safari/604.1"
+OPERA = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 OPR/97.0.4719.17"
+SAFARI = "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_3) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.4 Safari/605.1.15"
 
 # Backwards compatibility
 EDGE = CHROME
 FIREFOX_MAC = FIREFOX
 IE_6 = IE_7 = IE_8 = IE_9 = IE_11
 IPHONE_6 = IPAD = IPHONE
 SAFARI_7 = SAFARI_8 = SAFARI
```

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/validate/__init__.py` & `streamlink-5.4.0/src/streamlink/plugin/api/validate/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,22 +60,22 @@
     def __getattr__(_attr: str):
         if _attr in deprecations:
             import warnings
 
             from streamlink.exceptions import StreamlinkDeprecationWarning
 
             val, msg = deprecations[_attr]
-            warnings.warn(msg, StreamlinkDeprecationWarning)
+            warnings.warn(msg, StreamlinkDeprecationWarning, stacklevel=2)
 
             return val
 
         raise AttributeError
 
     __all__ = [k for k in globals().keys() if not k.startswith("_")]
     __all__.extend(deprecations.keys())
 
-    setattr(sys.modules[__name__], "__getattr__", __getattr__)
-    setattr(sys.modules[__name__], "__all__", __all__)
+    sys.modules[__name__].__getattr__ = __getattr__
+    sys.modules[__name__].__all__ = __all__
 
 
 _deprecations()
 del _deprecations
```

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/validate/_exception.py` & `streamlink-5.4.0/src/streamlink/plugin/api/validate/_exception.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/validate/_schemas.py` & `streamlink-5.4.0/src/streamlink/plugin/api/validate/_schemas.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/validate/_validate.py` & `streamlink-5.4.0/src/streamlink/plugin/api/validate/_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,16 +147,16 @@
         raise ValidationError(err, schema=Pattern) from None
 
     return result
 
 
 @validate.register
 def _validate_allschema(schema: AllSchema, value):
-    for schema in schema.schema:
-        value = validate(schema, value)
+    for subschema in schema.schema:
+        value = validate(subschema, value)
 
     return value
 
 
 @validate.register
 def _validate_anyschema(schema: AnySchema, value):
     errors = []
@@ -169,16 +169,16 @@
     raise ValidationError(*errors, schema=AnySchema)
 
 
 @validate.register
 def _validate_noneorallschema(schema: NoneOrAllSchema, value):
     if value is not None:
         try:
-            for schema in schema.schema:
-                value = validate(schema, value)
+            for subschema in schema.schema:
+                value = validate(subschema, value)
         except ValidationError as err:
             raise ValidationError(err, schema=NoneOrAllSchema) from None
 
     return value
 
 
 @validate.register
@@ -372,21 +372,21 @@
         type=type(schema).__name__,
     )
 
 
 @validate_union.register(dict)
 def _validate_union_dict(schema, value):
     new = type(schema)()
-    for key, schema in schema.items():
+    for key, subschema in schema.items():
         is_optional = isinstance(key, OptionalSchema)
         if is_optional:
             key = key.key
 
         try:
-            new[key] = validate(schema, value)
+            new[key] = validate(subschema, value)
         except ValidationError as err:
             if is_optional:
                 continue
 
             raise ValidationError(
                 "Unable to validate union {key}",
                 key=repr(key),
```

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/validate/_validators.py` & `streamlink-5.4.0/src/streamlink/plugin/api/validate/_validators.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugin/api/websocket.py` & `streamlink-5.4.0/src/streamlink/plugin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugin/plugin.py` & `streamlink-5.4.0/src/streamlink/plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,17 +119,17 @@
     return 0, "none"
 
 
 def iterate_streams(streams):
     for name, stream in streams:
         if isinstance(stream, list):
             for sub_stream in stream:
-                yield (name, sub_stream)
+                yield name, sub_stream
         else:
-            yield (name, stream)
+            yield name, stream
 
 
 def stream_type_priority(stream_types, stream):
     stream_type = type(stream[1]).shortname()
 
     try:
         prio = stream_types.index(stream_type)
@@ -302,14 +302,15 @@
             def __init__(self, session, url):
                 # Take any arguments, but only pass the URL to the custom constructor of the deprecated plugin
                 # noinspection PyArgumentList
                 super().__init__(url)
                 warnings.warn(
                     f"Initialized {self.module} plugin with deprecated constructor",
                     FutureWarning,
+                    stacklevel=2,
                 )
 
         # Wrapper class which comes after the deprecated plugin in the MRO
         # noinspection PyAbstractClass
         class PluginWrapperBack(PluginWrapperFront, metaclass=PluginWrapperMeta):
             def __init__(self, *_, **__):
                 # Take any arguments from the super() call of the constructor of the deprecated plugin,
@@ -370,15 +371,15 @@
     def stream_weight(cls, stream):
         return stream_weight(stream)
 
     @classmethod
     def default_stream_types(cls, streams):
         stream_types = ["hls", "http"]
 
-        for name, stream in iterate_streams(streams):
+        for _name, stream in iterate_streams(streams):
             stream_type = type(stream).shortname()
 
             if stream_type not in stream_types:
                 stream_types.append(stream_type)
 
         return stream_types
 
@@ -424,15 +425,15 @@
 
             # Flatten the iterator to a list so we can reuse it.
             if ostreams:
                 ostreams = list(ostreams)
         except NoStreamsError:
             return {}
         except (OSError, ValueError) as err:
-            raise PluginError(err)
+            raise PluginError(err) from err
 
         if not ostreams:
             return {}
 
         if stream_types is None:
             stream_types = self.default_stream_types(ostreams)
 
@@ -478,15 +479,15 @@
                 continue
 
             # Force lowercase name and replace space with underscore.
             streams[name.lower()] = stream
 
         # Create the best/worst synonyms
         def stream_weight_only(s):
-            return (self.stream_weight(s)[0] or (len(streams) == 1 and 1))
+            return self.stream_weight(s)[0] or (len(streams) == 1 and 1)
 
         stream_names = filter(stream_weight_only, streams.keys())
         sorted_streams = sorted(stream_names, key=stream_weight_only)
         unfiltered_sorted_streams = sorted_streams
 
         if isinstance(sorting_excludes, list):
             for expr in sorting_excludes:
@@ -629,24 +630,24 @@
 
     def input_ask(self, prompt: str) -> str:
         user_input_requester: Optional[UserInputRequester] = self.session.get_option("user-input-requester")
         if user_input_requester:
             try:
                 return user_input_requester.ask(prompt)
             except OSError as err:
-                raise FatalPluginError(f"User input error: {err}")
+                raise FatalPluginError(f"User input error: {err}") from err
         raise FatalPluginError("This plugin requires user input, however it is not supported on this platform")
 
     def input_ask_password(self, prompt: str) -> str:
         user_input_requester: Optional[UserInputRequester] = self.session.get_option("user-input-requester")
         if user_input_requester:
             try:
                 return user_input_requester.ask_password(prompt)
             except OSError as err:
-                raise FatalPluginError(f"User input error: {err}")
+                raise FatalPluginError(f"User input error: {err}") from err
         raise FatalPluginError("This plugin requires user input, however it is not supported on this platform")
 
 
 def pluginmatcher(
     pattern: Pattern,
     priority: int = NORMAL_PRIORITY,
     name: Optional[str] = None,
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/abematv.py` & `streamlink-5.4.0/src/streamlink/plugins/abematv.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,31 +175,31 @@
         ts_1hour = (int(time.time()) + 60 * 60) // 3600 * 3600
         time_struct = time.gmtime(ts_1hour)
         ts_1hour_str = str(ts_1hour).encode("utf-8")
 
         h = hmac.new(self.SECRETKEY, digestmod=hashlib.sha256)
         h.update(self.SECRETKEY)
         tmp = h.digest()
-        for i in range(time_struct.tm_mon):
+        for _ in range(time_struct.tm_mon):
             h = hmac.new(self.SECRETKEY, digestmod=hashlib.sha256)
             h.update(tmp)
             tmp = h.digest()
         h = hmac.new(self.SECRETKEY, digestmod=hashlib.sha256)
         h.update(urlsafe_b64encode(tmp).rstrip(b"=") + deviceid)
         tmp = h.digest()
-        for i in range(time_struct.tm_mday % 5):
+        for _ in range(time_struct.tm_mday % 5):
             h = hmac.new(self.SECRETKEY, digestmod=hashlib.sha256)
             h.update(tmp)
             tmp = h.digest()
 
         h = hmac.new(self.SECRETKEY, digestmod=hashlib.sha256)
         h.update(urlsafe_b64encode(tmp).rstrip(b"=") + ts_1hour_str)
         tmp = h.digest()
 
-        for i in range(time_struct.tm_hour % 5):  # utc hour
+        for _ in range(time_struct.tm_hour % 5):  # utc hour
             h = hmac.new(self.SECRETKEY, digestmod=hashlib.sha256)
             h.update(tmp)
             tmp = h.digest()
 
         return urlsafe_b64encode(tmp).rstrip(b"=").decode("utf-8")
 
     def _is_playable(self, vtype, vid):
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/adultswim.py` & `streamlink-5.4.0/src/streamlink/plugins/adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/afreeca.py` & `streamlink-5.4.0/src/streamlink/plugins/afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/albavision.py` & `streamlink-5.4.0/src/streamlink/plugins/albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/aloula.py` & `streamlink-5.4.0/src/streamlink/plugins/aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/app17.py` & `streamlink-5.4.0/src/streamlink/plugins/app17.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ard_live.py` & `streamlink-5.4.0/src/streamlink/plugins/ard_live.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ard_mediathek.py` & `streamlink-5.4.0/src/streamlink/plugins/ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/artetv.py` & `streamlink-5.4.0/src/streamlink/plugins/artetv.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,12 +63,12 @@
         ))
 
         if not streams:
             return
 
         self.title = f"{metadata['title']} - {metadata['subtitle']}" if metadata["subtitle"] else metadata["title"]
 
-        for slot, protocol, url in sorted(streams, key=itemgetter(0)):
+        for _slot, _protocol, url in sorted(streams, key=itemgetter(0)):
             return HLSStream.parse_variant_playlist(self.session, url)
 
 
 __plugin__ = ArteTV
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/atpchallenger.py` & `streamlink-5.4.0/src/streamlink/plugins/atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/atresplayer.py` & `streamlink-5.4.0/src/streamlink/plugins/atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/bbciplayer.py` & `streamlink-5.4.0/src/streamlink/plugins/bbciplayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,17 @@
                                       platform=platform)
             log.debug(f"Info API request: {url}")
             medias = self.session.http.get(url, schema=self.mediaselector_schema)
             for media in medias:
                 for connection in media["connection"]:
                     urls[connection.get("transferFormat")].add(connection["href"])
 
-        for stream_type, urls in urls.items():
-            log.debug(f"{len(urls)} {stream_type} streams")
-            for url in list(urls):
+        for stream_type, urlitems in urls.items():
+            log.debug(f"{len(urlitems)} {stream_type} streams")
+            for url in list(urlitems):
                 try:
                     if stream_type == "hls":
                         yield from HLSStream.parse_variant_playlist(self.session, url).items()
                     if stream_type == "dash":
                         yield from DASHStream.parse_manifest(self.session, url).items()
                     log.debug(f"  OK:   {url}")
                 except Exception:
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/bfmtv.py` & `streamlink-5.4.0/src/streamlink/plugins/bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/bigo.py` & `streamlink-5.4.0/src/streamlink/plugins/bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/bilibili.py` & `streamlink-5.4.0/src/streamlink/plugins/bilibili.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/blazetv.py` & `streamlink-5.4.0/src/streamlink/plugins/blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/bloomberg.py` & `streamlink-5.4.0/src/streamlink/plugins/bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/booyah.py` & `streamlink-5.4.0/src/streamlink/plugins/booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/brightcove.py` & `streamlink-5.4.0/src/streamlink/plugins/brightcove.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/btv.py` & `streamlink-5.4.0/src/streamlink/plugins/btv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/cbsnews.py` & `streamlink-5.4.0/src/streamlink/plugins/cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/cdnbg.py` & `streamlink-5.4.0/src/streamlink/plugins/cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ceskatelevize.py` & `streamlink-5.4.0/src/streamlink/plugins/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/cinergroup.py` & `streamlink-5.4.0/src/streamlink/plugins/cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/clubbingtv.py` & `streamlink-5.4.0/src/streamlink/plugins/clubbingtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/cmmedia.py` & `streamlink-5.4.0/src/streamlink/plugins/cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/cnews.py` & `streamlink-5.4.0/src/streamlink/plugins/cnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/crunchyroll.py` & `streamlink-5.4.0/src/streamlink/plugins/crunchyroll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 $description Video streaming service focused on anime, manga, and dorama.
 $url crunchyroll.com
 $type vod
 """
 
-import datetime
 import logging
 import re
 from uuid import uuid4
 
 from streamlink.plugin import Plugin, PluginError, pluginargument, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.times import parse_datetime
 
 
 log = logging.getLogger(__name__)
 
 STREAM_WEIGHTS = {
     "low": 240,
     "mid": 420,
@@ -25,23 +25,14 @@
 STREAM_NAMES = {
     "120k": "low",
     "328k": "mid",
     "864k": "high",
 }
 
 
-def parse_timestamp(ts):
-    """Takes ISO 8601 format(string) and converts into a utc datetime(naive)"""
-    return (
-        datetime.datetime.strptime(ts[:-7], "%Y-%m-%dT%H:%M:%S")
-        + datetime.timedelta(hours=int(ts[-5:-3]), minutes=int(ts[-2:]))
-        * int(f"{ts[-6:-5]}1")
-    )
-
-
 _api_schema = validate.Schema({
     "error": bool,
     validate.optional("code"): str,
     validate.optional("message"): str,
     validate.optional("data"): object,
 })
 _media_schema = validate.Schema(
@@ -66,15 +57,15 @@
         ),
     },
 )
 _login_schema = validate.Schema({
     "auth": validate.any(str, None),
     "expires": validate.all(
         str,
-        validate.transform(parse_timestamp),
+        validate.transform(parse_datetime),
     ),
     "user": {
         "username": validate.any(str, None),
         "email": str,
     },
 })
 _session_schema = validate.Schema(
@@ -320,15 +311,15 @@
 
         api = self._create_api()
         try:
             # the media.stream_data field is required, no stream data is returned otherwise
             info = api.get_info(media_id, fields=["media.name", "media.series_name",
                                 "media.media_type", "media.stream_data"], schema=_media_schema)
         except CrunchyrollAPIError as err:
-            raise PluginError(f"Media lookup error: {err.msg}")
+            raise PluginError(f"Media lookup error: {err.msg}") from err
 
         if not info:
             return
 
         streams = {}
 
         self.id = media_id
@@ -395,15 +386,15 @@
                     api.login(self.options.get("username"),
                               self.options.get("password"))
                     login = api.authenticate()
                     login_name = login["user"]["username"] or login["user"]["email"]
                     log.info(f"Logged in as '{login_name}'")
 
                 except CrunchyrollAPIError as err:
-                    raise PluginError(f"Authentication error: {err.msg}")
+                    raise PluginError(f"Authentication error: {err.msg}") from err
             if not api.auth:
                 log.warning("No authentication provided, you won't be able to access premium restricted content")
 
         return api
 
 
 __plugin__ = Crunchyroll
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/dailymotion.py` & `streamlink-5.4.0/src/streamlink/plugins/dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/dash.py` & `streamlink-5.4.0/src/streamlink/plugins/dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/delfi.py` & `streamlink-5.4.0/src/streamlink/plugins/delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/deutschewelle.py` & `streamlink-5.4.0/src/streamlink/plugins/deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/dlive.py` & `streamlink-5.4.0/src/streamlink/plugins/dlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/dogan.py` & `streamlink-5.4.0/src/streamlink/plugins/dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/dogus.py` & `streamlink-5.4.0/src/streamlink/plugins/dogus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/drdk.py` & `streamlink-5.4.0/src/streamlink/plugins/drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/earthcam.py` & `streamlink-5.4.0/src/streamlink/plugins/earthcam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/euronews.py` & `streamlink-5.4.0/src/streamlink/plugins/euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/facebook.py` & `streamlink-5.4.0/src/streamlink/plugins/facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/filmon.py` & `streamlink-5.4.0/src/streamlink/plugins/filmon.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
         vod_id = self.match.group("vod_id")
         is_group = self.match.group("is_group")
 
         # get cookies
         self.session.http.get(self.url)
 
         if vod_id:
-            for quality, url, timeout in self.api.vod(vod_id):
+            for quality, url, _timeout in self.api.vod(vod_id):
                 if url.endswith(".m3u8"):
                     streams = HLSStream.parse_variant_playlist(self.session, url)
                     if streams:
                         yield from streams.items()
                         return
                     yield quality, HLSStream(self.session, url)
                 elif url.endswith(".mp4"):
@@ -230,15 +230,15 @@
                     if _id and not is_group:
                         self.cache.set(channel, _id, expires=self.TIME_CHANNEL)
 
             if _id is None:
                 raise PluginError(f"Unable to find channel ID: {channel}")
 
             try:
-                for quality, url, timeout in self.api.channel(_id):
+                for quality, url, _timeout in self.api.channel(_id):
                     yield quality, FilmOnHLS(self.session, url, self.api, channel=_id, quality=quality)
             except Exception:
                 if channel and not channel.isdigit():
                     self.cache.set(channel, None, expires=0)
                     log.debug(f"Reset cached channel: {channel}")
                 raise
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/foxtr.py` & `streamlink-5.4.0/src/streamlink/plugins/foxtr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/galatasaraytv.py` & `streamlink-5.4.0/src/streamlink/plugins/galatasaraytv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/goltelevision.py` & `streamlink-5.4.0/src/streamlink/plugins/goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/goodgame.py` & `streamlink-5.4.0/src/streamlink/plugins/goodgame.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/googledrive.py` & `streamlink-5.4.0/src/streamlink/plugins/googledrive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/gulli.py` & `streamlink-5.4.0/src/streamlink/plugins/gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/hiplayer.py` & `streamlink-5.4.0/src/streamlink/plugins/hiplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/hls.py` & `streamlink-5.4.0/src/streamlink/plugins/hls.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/http.py` & `streamlink-5.4.0/src/streamlink/plugins/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/htv.py` & `streamlink-5.4.0/src/streamlink/plugins/htv.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 $url htv.com.vn
 $type live
 $region Vietnam
 """
 
 import logging
 import re
-from datetime import date
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.times import localnow
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
     r"https?://(?:www\.)?htv\.com\.vn/truc-tuyen(?:\?channel=(?P<channel>\w+)&?|$)",
@@ -55,15 +55,15 @@
         json = self.session.http.post(
             "https://www.htv.com.vn/HTVModule/Services/htvService.aspx",
             data={
                 "method": "GetScheduleList",
                 "channelid": channel_id,
                 "template": "AjaxSchedules.xslt",
                 "channelcode": channel_code,
-                "date": date.today().strftime("%d-%m-%Y"),
+                "date": localnow().strftime("%d-%m-%Y"),
             },
             schema=validate.Schema(
                 validate.parse_json(),
                 {
                     "success": bool,
                     "chanelUrl": validate.url(),
                 },
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/huajiao.py` & `streamlink-5.4.0/src/streamlink/plugins/huajiao.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/huya.py` & `streamlink-5.4.0/src/streamlink/plugins/huya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/idf1.py` & `streamlink-5.4.0/src/streamlink/plugins/idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/invintus.py` & `streamlink-5.4.0/src/streamlink/plugins/invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/kugou.py` & `streamlink-5.4.0/src/streamlink/plugins/kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/linelive.py` & `streamlink-5.4.0/src/streamlink/plugins/linelive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/livestream.py` & `streamlink-5.4.0/src/streamlink/plugins/livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/lnk.py` & `streamlink-5.4.0/src/streamlink/plugins/lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/lrt.py` & `streamlink-5.4.0/src/streamlink/plugins/lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ltv_lsm_lv.py` & `streamlink-5.4.0/src/streamlink/plugins/ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mdstrm.py` & `streamlink-5.4.0/src/streamlink/plugins/mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mediaklikk.py` & `streamlink-5.4.0/src/streamlink/plugins/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mediavitrina.py` & `streamlink-5.4.0/src/streamlink/plugins/mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mildom.py` & `streamlink-5.4.0/src/streamlink/plugins/mildom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mitele.py` & `streamlink-5.4.0/src/streamlink/plugins/mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mixcloud.py` & `streamlink-5.4.0/src/streamlink/plugins/mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mjunoon.py` & `streamlink-5.4.0/src/streamlink/plugins/mjunoon.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/mrtmk.py` & `streamlink-5.4.0/src/streamlink/plugins/mrtmk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/n13tv.py` & `streamlink-5.4.0/src/streamlink/plugins/n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/nbcnews.py` & `streamlink-5.4.0/src/streamlink/plugins/tv3cat.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,70 @@
 """
-$description 24-hour world, US and local news channel, based in the United States of America.
-$url nbcnews.com
-$type live
+$description Live TV channels and video on-demand service from CCMA, a Catalan public, state-owned broadcaster.
+$url ccma.cat
+$type live, vod
+$region Spain
 """
 
 import logging
 import re
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"https?://(?:www\.)?nbcnews\.com/now",
+    r"https?://(?:www\.)?ccma\.cat/tv3/directe/(?P<ident>.+?)/",
 ))
-class NBCNews(Plugin):
-    URL_API = "https://api-leap.nbcsports.com/feeds/assets/{}?application=NBCNews&format=nbc-player&platform=desktop"
-    URL_TOKEN = "https://tokens.playmakerservices.com/"
+class TV3Cat(Plugin):
+    _URL_STREAM_INFO = "https://dinamics.ccma.cat/pvideo/media.jsp"
 
-    title = "NBC News Now"
+    _MAP_CHANNELS = {
+        "tv3": "tvi",
+    }
 
     def _get_streams(self):
-        self.id = self.session.http.get(
-            self.url,
-            schema=validate.Schema(
-                validate.parse_html(),
-                validate.xml_xpath_string(".//script[@type='application/ld+json'][1]/text()"),
-                validate.none_or_all(
-                    validate.parse_json(),
-                    {"embedUrl": validate.url()},
-                    validate.get("embedUrl"),
-                    validate.transform(lambda embed_url: embed_url.split("/")[-1]),
-                ),
-            ),
-        )
-        if self.id is None:
-            return
-        log.debug(f"API ID: {self.id}")
+        ident = self.match.group("ident")
 
-        stream = self.session.http.get(
-            self.URL_API.format(self.id),
-            schema=validate.Schema(
-                validate.parse_json(),
-                {
-                    "videoSources": [{
-                        "cdnSources": {
-                            "primary": [{
-                                "sourceUrl": validate.url(path=validate.endswith(".m3u8")),
-                            }],
-                        },
-                    }],
-                },
-                validate.get(("videoSources", 0, "cdnSources", "primary", 0, "sourceUrl")),
-            ),
-        )
-
-        url = self.session.http.post(
-            self.URL_TOKEN,
-            json={
-                "requestorId": "nbcnews",
-                "pid": self.id,
-                "application": "NBCSports",
-                "version": "v1",
-                "platform": "desktop",
-                "token": "",
-                "resourceId": "",
-                "inPath": "false",
-                "authenticationType": "unauth",
-                "cdn": "akamai",
-                "url": stream,
+        schema_media = {
+            "geo": str,
+            "url": validate.url(path=validate.endswith(".m3u8")),
+        }
+
+        stream_infos = self.session.http.get(
+            self._URL_STREAM_INFO,
+            params={
+                "media": "video",
+                "versio": "vast",
+                "idint": self._MAP_CHANNELS.get(ident, ident),
+                "profile": "pc",
+                "desplacament": "0",
+                "broadcast": "false",
             },
             schema=validate.Schema(
                 validate.parse_json(),
                 {
-                    "akamai": [{
-                        "tokenizedUrl": validate.url(),
-                    }],
+                    "media": validate.any(
+                        [schema_media],
+                        validate.all(
+                            schema_media,
+                            validate.transform(lambda item: [item]),
+                        ),
+                    ),
                 },
-                validate.get(("akamai", 0, "tokenizedUrl")),
+                validate.get("media"),
             ),
         )
-        return HLSStream.parse_variant_playlist(self.session, url)
+
+        for stream in stream_infos:
+            log.info(f"Accessing stream from region {stream['geo']}")
+            try:
+                return HLSStream.parse_variant_playlist(self.session, stream["url"], name_fmt="{pixels}_{bitrate}")
+            except OSError:
+                pass
 
 
-__plugin__ = NBCNews
+__plugin__ = TV3Cat
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/nhkworld.py` & `streamlink-5.4.0/src/streamlink/plugins/nhkworld.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/nicolive.py` & `streamlink-5.4.0/src/streamlink/plugins/nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/nimotv.py` & `streamlink-5.4.0/src/streamlink/plugins/nimotv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/nos.py` & `streamlink-5.4.0/src/streamlink/plugins/nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/nownews.py` & `streamlink-5.4.0/src/streamlink/plugins/nownews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/nrk.py` & `streamlink-5.4.0/src/streamlink/plugins/nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ntv.py` & `streamlink-5.4.0/src/streamlink/plugins/ntv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/okru.py` & `streamlink-5.4.0/src/streamlink/plugins/okru.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/olympicchannel.py` & `streamlink-5.4.0/src/streamlink/plugins/olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/oneplusone.py` & `streamlink-5.4.0/src/streamlink/plugins/oneplusone.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 $url 1plus1.video
 $type live
 """
 
 import logging
 import re
 from base64 import b64decode
-from datetime import datetime
 from time import time
 from urllib.parse import urljoin, urlparse
 
 from streamlink.exceptions import NoStreamsError, PluginError
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.times import fromlocaltimestamp
 
 
 log = logging.getLogger(__name__)
 
 
 class OnePlusOneHLS(HLSStream):
     __shortname__ = "hls-oneplusone"
@@ -30,15 +30,15 @@
         first_parsed = urlparse(self._url)
         self._first_netloc = first_parsed.netloc
         self._first_path_chunklist = first_parsed.path.split("/")[-1]
         self.watch_timeout = int(first_parsed.path.split("/")[2]) - 15
         self.api = OnePlusOneAPI(session_, self_url)
 
     def _next_watch_timeout(self):
-        _next = datetime.fromtimestamp(self.watch_timeout).isoformat(" ")
+        _next = fromlocaltimestamp(self.watch_timeout).isoformat(" ")
         log.debug(f"next watch_timeout at {_next}")
 
     def open(self):
         self._next_watch_timeout()
         return super().open()
 
     @property
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/onetv.py` & `streamlink-5.4.0/src/streamlink/plugins/onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/openrectv.py` & `streamlink-5.4.0/src/streamlink/plugins/openrectv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/pandalive.py` & `streamlink-5.4.0/src/streamlink/plugins/pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/picarto.py` & `streamlink-5.4.0/src/streamlink/plugins/picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/piczel.py` & `streamlink-5.4.0/src/streamlink/plugins/piczel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/pixiv.py` & `streamlink-5.4.0/src/streamlink/plugins/pixiv.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 $url sketch.pixiv.net
 $type live
 """
 
 import logging
 import re
 
-from streamlink.exceptions import FatalPluginError, NoStreamsError, PluginError
+from streamlink.exceptions import FatalPluginError, NoStreamsError
 from streamlink.plugin import Plugin, pluginargument, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
 
 
 log = logging.getLogger(__name__)
 
@@ -154,17 +154,19 @@
                     if number == 0:
                         # default stream
                         self.set_option("performer", None)
                     else:
                         # other co-hosts
                         self.set_option("performer", co_hosts[number - 1][0])
                 except FatalPluginError:
-                    raise PluginError("Selected performer is invalid.")
+                    log.error("Selected performer is invalid.")
+                    return
                 except (IndexError, ValueError, TypeError):
-                    raise PluginError("Input is invalid")
+                    log.error("Input is invalid")
+                    return
 
         # ignore the owner stream, if a performer is selected
         # or use it when there are no other performers
         if not self.get_option("performer") or not performers:
             return self.hls_stream(streamer_data["owner"]["hls_movie"]["url"])
 
         # play a co-host stream
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/pluto.py` & `streamlink-5.4.0/src/streamlink/plugins/pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/pluzz.py` & `streamlink-5.4.0/src/streamlink/plugins/pluzz.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 $url francetvinfo.fr
 $type live, vod
 $region France, Andorra, Monaco
 """
 
 import logging
 import re
-from datetime import datetime
 from urllib.parse import urlparse
 
-from isodate import LOCAL as LOCALTIMEZONE  # type: ignore[import]
-
 from streamlink.plugin import Plugin, PluginError, pluginmatcher
 from streamlink.plugin.api import useragents, validate
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.times import localnow
 from streamlink.utils.url import update_qsd
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(r"""
@@ -99,15 +97,15 @@
             "h": 1080,
             "player_version": self.PLAYER_VERSION,
             "domain": urlparse(self.url).netloc,
             "device_type": "mobile",
             "browser": "chrome",
             "browser_version": CHROME_VERSION,
             "os": "ios",
-            "gmt": datetime.now(tz=LOCALTIMEZONE).strftime("%z"),
+            "gmt": localnow().strftime("%z"),
         })
         video_format, token_url, url, self.title = self.session.http.get(api_url, schema=validate.Schema(
             validate.parse_json(),
             {
                 "video": {
                     "workflow": validate.any("token-akamai", "dai"),
                     "format": validate.any("dash", "hls"),
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/qq.py` & `streamlink-5.4.0/src/streamlink/plugins/qq.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/radiko.py` & `streamlink-5.4.0/src/streamlink/plugins/radiko.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/radionet.py` & `streamlink-5.4.0/src/streamlink/plugins/radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/raiplay.py` & `streamlink-5.4.0/src/streamlink/plugins/raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/reuters.py` & `streamlink-5.4.0/src/streamlink/plugins/reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/rtbf.py` & `streamlink-5.4.0/src/streamlink/plugins/rtbf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from html import unescape as html_unescape
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
+from streamlink.utils.times import parse_datetime
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(r"""
     https?://(?:www\.)?
@@ -105,20 +106,14 @@
         return data["country"] == geoloc_flag or data["zone"] == geoloc_flag
 
     def tokenize_stream(self, url):
         res = self.session.http.post(self.TOKEN_URL, data={"streams[url]": url})
         data = self.session.http.json(res)
         return data["streams"]["url"]
 
-    @staticmethod
-    def iso8601_to_epoch(date):
-        # Convert an ISO 8601-formatted string date to datetime
-        return datetime.datetime.strptime(date[:-6], "%Y-%m-%dT%H:%M:%S") + \
-            datetime.timedelta(hours=int(date[-6:-3]), minutes=int(date[-2:]))
-
     def _get_radio_streams(self):
         res = self.session.http.get(self.url)
         match = self._radio_id_re.search(res.text)
         if match is None:
             return
         radio_id = match.group("radio_id")
         res = self.session.http.get(self.RADIO_STREAM_URL.format(radio_id))
@@ -148,15 +143,15 @@
             return
 
         # Check whether streams are DRM-protected
         if stream_data.get("drm", False):
             log.error("Stream is DRM-protected")
             return
 
-        now = datetime.datetime.now()
+        now = datetime.datetime.now(datetime.timezone.utc)
         try:
             if isinstance(stream_data["sources"], dict):
                 urls = []
                 for profile, url in stream_data["sources"].items():
                     if not url or url in urls:
                         continue
                     match = self._stream_size_re.match(url)
@@ -181,18 +176,18 @@
                     dash_url = self.tokenize_stream(dash_url)
                 yield from DASHStream.parse_manifest(self.session, dash_url).items()
 
         except OSError as err:
             if "403 Client Error" in str(err):
                 # Check whether video is expired
                 if "startDate" in stream_data:
-                    if now < self.iso8601_to_epoch(stream_data["startDate"]):
+                    if now < parse_datetime(stream_data["startDate"]):
                         log.error("Stream is not yet available")
                 elif "endDate" in stream_data:
-                    if now > self.iso8601_to_epoch(stream_data["endDate"]):
+                    if now > parse_datetime(stream_data["endDate"]):
                         log.error("Stream has expired")
 
     def _get_streams(self):
         if self.match.group("video_id"):
             return self._get_video_streams()
         return self._get_radio_streams()
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/rtpa.py` & `streamlink-5.4.0/src/streamlink/plugins/rtpa.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/rtpplay.py` & `streamlink-5.4.0/src/streamlink/plugins/rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/rtve.py` & `streamlink-5.4.0/src/streamlink/plugins/rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/rtvs.py` & `streamlink-5.4.0/src/streamlink/plugins/rtvs.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ruv.py` & `streamlink-5.4.0/src/streamlink/plugins/ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/sbscokr.py` & `streamlink-5.4.0/src/streamlink/plugins/sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/showroom.py` & `streamlink-5.4.0/src/streamlink/plugins/showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/sportal.py` & `streamlink-5.4.0/src/streamlink/plugins/sportal.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/sportschau.py` & `streamlink-5.4.0/src/streamlink/plugins/sportschau.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ssh101.py` & `streamlink-5.4.0/src/streamlink/plugins/ssh101.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/stadium.py` & `streamlink-5.4.0/src/streamlink/plugins/stadium.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/steam.py` & `streamlink-5.4.0/src/streamlink/plugins/steam.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,26 +133,26 @@
                 try:
                     captcha_text = self.input_ask("Captcha text")
                 except FatalPluginError:
                     captcha_text = None
                 if not captcha_text:
                     return False
             else:
-                # If the user must enter the code that was emailed to them
+                # Whether the user must enter the code that was emailed to them
                 if resp.get("emailauth_needed"):
                     if emailauth:
                         raise SteamLoginFailed("Email auth key error")
                     try:
                         emailauth = self.input_ask("Email auth code required")
                     except FatalPluginError:
                         emailauth = None
                     if not emailauth:
                         return False
 
-                # If the user must enter a two factor auth code
+                # Whether the user must enter a two-factor auth code
                 if resp.get("requires_twofactor"):
                     try:
                         twofactorcode = self.input_ask("Two factor auth code required")
                     except FatalPluginError:
                         twofactorcode = None
                     if not twofactorcode:
                         return False
@@ -182,20 +182,19 @@
                 steamid=steamid,
                 viewertoken=viewertoken,
                 sessionid=sessionid,
             ),
             schema=validate.Schema(
                 validate.parse_json(),
                 {
-                    "success": validate.any("ready", "unavailable", "waiting", "waiting_to_start", "waiting_for_start"),
-                    "retry": int,
-                    "broadcastid": validate.any(str, int),
+                    "success": str,
                     validate.optional("url"): validate.url(),
-                    validate.optional("viewertoken"): str,
+                    validate.optional("cdn_auth_url_parameters"): validate.any(str, None),
                 },
+                validate.union_get("success", "url", "cdn_auth_url_parameters"),
             ),
         )
 
     def _find_steamid(self, url):
         return self.session.http.get(url, schema=validate.Schema(
             validate.parse_html(),
             validate.xml_xpath_string(".//div[@id='webui_config']/@data-broadcast"),
@@ -228,24 +227,21 @@
             if not steamid:
                 return
             self.url = self._watch_broadcast_url.format(steamid=steamid)
 
         res = self.session.http.get(self.url)  # get the page to set some cookies
         sessionid = res.cookies.get("sessionid")
 
-        streamdata = None
-        while streamdata is None or streamdata["success"] in ("waiting", "waiting_for_start"):
-            streamdata = self._get_broadcast_stream(steamid, sessionid=sessionid)
+        success, url, cdn_auth = self._get_broadcast_stream(steamid, sessionid=sessionid)
+        if success != "ready" or not url:
+            log.error("This stream is currently unavailable")
+            return
+
+        # CDN auth data is only required at certain times of the day, and it makes
+        # segment requests fail if missing (the DASH manifest still works regardless).
+        # Remove leading ampersand and pass the params as a string, to avoid URL quoting.
+        params = re.sub(r"^&", "", cdn_auth) if cdn_auth else None
 
-            if streamdata["success"] == "ready":
-                return DASHStream.parse_manifest(self.session, streamdata["url"])
-
-            if streamdata["success"] == "unavailable":
-                log.error("This stream is currently unavailable")
-                return
-
-            r = streamdata["retry"] / 1000.0
-            log.info(f"Waiting for stream, will retry again in {r:.1f} seconds...")
-            time.sleep(r)
+        return DASHStream.parse_manifest(self.session, url, params=params)
 
 
 __plugin__ = SteamBroadcastPlugin
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/streamable.py` & `streamlink-5.4.0/src/streamlink/plugins/streamable.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/streann.py` & `streamlink-5.4.0/src/streamlink/plugins/streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/stv.py` & `streamlink-5.4.0/src/streamlink/plugins/stv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/svtplay.py` & `streamlink-5.4.0/src/streamlink/plugins/svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/swisstxt.py` & `streamlink-5.4.0/src/streamlink/plugins/swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/telefe.py` & `streamlink-5.4.0/src/streamlink/plugins/telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tf1.py` & `streamlink-5.4.0/src/streamlink/plugins/tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/trovo.py` & `streamlink-5.4.0/src/streamlink/plugins/trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/turkuvaz.py` & `streamlink-5.4.0/src/streamlink/plugins/turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tv360.py` & `streamlink-5.4.0/src/streamlink/plugins/tv360.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tv3cat.py` & `streamlink-5.4.0/src/streamlink/plugins/tviplayer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,79 @@
 """
-$description Live TV channels and video on-demand service from CCMA, a Catalan public, state-owned broadcaster.
-$url ccma.cat
+$description Live TV channels and video on-demand service from TVI, a Portuguese free-to-air broadcaster.
+$url tviplayer.iol.pt
 $type live, vod
-$region Spain
 """
 
 import logging
 import re
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
+from streamlink.utils.url import update_qsd
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"https?://(?:www\.)?ccma\.cat/tv3/directe/(?P<ident>.+?)/",
+    r"https://tviplayer\.iol\.pt/(?:direto|programa)/",
 ))
-class TV3Cat(Plugin):
-    _URL_STREAM_INFO = "https://dinamics.ccma.cat/pvideo/media.jsp"
-
-    _MAP_CHANNELS = {
-        "tv3": "tvi",
-    }
-
+class TVIPlayer(Plugin):
     def _get_streams(self):
-        ident = self.match.group("ident")
-
-        schema_media = {
-            "geo": str,
-            "url": validate.url(path=validate.endswith(".m3u8")),
-        }
-
-        stream_infos = self.session.http.get(
-            self._URL_STREAM_INFO,
-            params={
-                "media": "video",
-                "versio": "vast",
-                "idint": self._MAP_CHANNELS.get(ident, ident),
-                "profile": "pc",
-                "desplacament": "0",
-                "broadcast": "false",
-            },
+        self.session.http.headers.update({"Referer": "https://tviplayer.iol.pt/"})
+        data = self.session.http.get(
+            self.url,
+            schema=validate.Schema(
+                validate.parse_html(),
+                validate.xml_xpath_string(".//script[contains(text(),'.m3u8')]/text()"),
+                validate.none_or_all(
+                    re.compile(r"jsonData\s*=\s*(?P<json>{.+?})\s*;", re.DOTALL),
+                    validate.none_or_all(
+                        validate.get("json"),
+                        validate.parse_json(),
+                        {
+                            "id": str,
+                            "liveType": str,
+                            "videoType": str,
+                            "videoUrl": validate.url(path=validate.endswith(".m3u8")),
+                            validate.optional("channel"): str,
+                        },
+                    ),
+                ),
+            ),
+        )
+        if not data:
+            return
+        log.debug(f"{data!r}")
+
+        if data["liveType"].upper() == "DIRETO" and data["videoType"].upper() == "LIVE":
+            geo_path = "live"
+        else:
+            geo_path = "vod"
+        data_geo = self.session.http.get(
+            f"https://services.iol.pt/direitos/rights/{geo_path}?id={data['id']}",
+            acceptable_status=(200, 403),
             schema=validate.Schema(
                 validate.parse_json(),
                 {
-                    "media": validate.any(
-                        [schema_media],
-                        validate.all(
-                            schema_media,
-                            validate.transform(lambda item: [item]),
-                        ),
-                    ),
+                    "code": str,
+                    "error": validate.any(None, str),
+                    "detail": str,
                 },
-                validate.get("media"),
             ),
         )
-
-        for stream in stream_infos:
-            log.info(f"Accessing stream from region {stream['geo']}")
-            try:
-                return HLSStream.parse_variant_playlist(self.session, stream["url"], name_fmt="{pixels}_{bitrate}")
-            except OSError:
-                pass
+        log.debug(f"{data_geo!r}")
+        if data_geo["detail"] != "ok":
+            log.error(f"{data_geo['detail']}")
+            return
+
+        wmsAuthSign = self.session.http.get(
+            "https://services.iol.pt/matrix?userId=",
+            schema=validate.Schema(str),
+        )
+        hls_url = update_qsd(data["videoUrl"], {"wmsAuthSign": wmsAuthSign})
+        return HLSStream.parse_variant_playlist(self.session, hls_url)
 
 
-__plugin__ = TV3Cat
+__plugin__ = TVIPlayer
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tv4play.py` & `streamlink-5.4.0/src/streamlink/plugins/tv4play.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 $notes Only non-premium streams are supported
 """
 
 import logging
 import re
 from urllib.parse import urljoin
 
-from streamlink.plugin import Plugin, PluginError, pluginmatcher
+from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
 
 
 log = logging.getLogger(__name__)
 
 
@@ -59,15 +59,16 @@
         try:
             res = self.session.http.get(
                 self.api_assets.format(self.get_video_id),
                 params=params,
             )
         except Exception as e:
             if "404 Client Error" in str(e):
-                raise PluginError("This Video is not available")
+                log.error("This Video is not available")
+                return
             raise e
         log.debug("Found metadata")
         metadata = self.session.http.json(res, schema=self._meta_schema)
         self.title = metadata["metadata"]["title"]
         return metadata
 
     def get_title(self):
@@ -78,15 +79,16 @@
     def _get_streams(self):
         metadata = self.get_metadata()
 
         try:
             res = self.session.http.get(urljoin(self.api_url, metadata["mediaUri"]))
         except Exception as e:
             if "401 Client Error" in str(e):
-                raise PluginError("This Video is not available in your country")
+                log.error("This Video is not available in your country")
+                return
             raise e
 
         log.debug("Found stream data")
         data = self.session.http.json(res)
         hls_url = data["playbackItem"]["manifestUrl"]
         log.debug("URL={0}".format(hls_url))
         yield from HLSStream.parse_variant_playlist(self.session, hls_url).items()
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tv5monde.py` & `streamlink-5.4.0/src/streamlink/plugins/vkplay.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,93 @@
 """
-$description Live TV channel and video on-demand service from TV5Monde, a French free-to-air broadcaster.
-$url tv5monde.com
-$url tivi5mondeplus.com
-$type live, vod
-$region France, Belgium, Switzerland
+$description Russian live-streaming platform for gaming and esports, owned by VKontakte.
+$url vkplay.live
+$type live
 """
 
+import logging
 import re
-from urllib.parse import urlparse
 
-from streamlink.plugin import Plugin, PluginError, pluginmatcher
+from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.hls import HLSStream
-from streamlink.stream.http import HTTPStream
-from streamlink.utils.url import update_scheme
 
 
-@pluginmatcher(re.compile(r"""
-    https?://(?:[\w-]+\.)*(?:tv5monde|tivi5mondeplus)\.com/
-""", re.VERBOSE))
-class TV5Monde(Plugin):
-    def _get_hls(self, root):
-        schema_live = validate.Schema(
-            validate.xml_xpath_string(".//*[contains(@data-broadcast,'m3u8')]/@data-broadcast"),
-            str,
-            validate.parse_json(),
-            validate.any(
-                validate.all({"files": list}, validate.get("files")),
-                list,
-            ),
-            [{
-                "url": validate.url(path=validate.endswith(".m3u8")),
-            }],
-            validate.get((0, "url")),
-            validate.transform(lambda content_url: update_scheme("https://", content_url)),
-        )
-        try:
-            live = schema_live.validate(root)
-        except PluginError:
-            return
+log = logging.getLogger(__name__)
 
-        return HLSStream.parse_variant_playlist(self.session, live)
 
-    def _get_vod(self, root):
-        schema_vod = validate.Schema(
-            validate.xml_xpath_string(".//script[@type='application/ld+json'][contains(text(),'VideoObject')][1]/text()"),
-            str,
-            validate.transform(lambda jsonlike: re.sub(r"[\r\n]+", "", jsonlike)),
-            validate.parse_json(),
-            validate.any(
-                validate.all(
-                    {"@graph": [dict]},
-                    validate.get("@graph"),
-                    validate.filter(lambda obj: obj["@type"] == "VideoObject"),
-                    validate.get(0),
+@pluginmatcher(re.compile(
+    r"https?://vkplay\.live/(?P<channel_name>\w+)/?$",
+))
+class VKplay(Plugin):
+    API_URL = "https://api.vkplay.live/v1"
+
+    def _get_streams(self):
+        self.author = self.match.group("channel_name")
+        log.debug(f"Channel name: {self.author}")
+
+        data = self.session.http.get(
+            f"{self.API_URL}/blog/{self.author}/public_video_stream",
+            headers={"Referer": self.url},
+            acceptable_status=(200, 404),
+            schema=validate.Schema(
+                validate.parse_json(),
+                validate.any(
+                    validate.all(
+                        {"error": str, "error_description": str},
+                        validate.get("error_description"),
+                    ),
+                    validate.all(
+                        {
+                            validate.optional("category"): validate.all(
+                                {
+                                    "title": str,
+                                },
+                                validate.get("title"),
+                            ),
+                            "title": str,
+                            "data": validate.any(
+                                [
+                                    validate.all(
+                                        {
+                                            "vid": str,
+                                            "playerUrls": [
+                                                validate.all(
+                                                    {
+                                                        "type": str,
+                                                        "url": validate.any("", validate.url()),
+                                                    },
+                                                    validate.union_get("type", "url"),
+                                                ),
+                                            ],
+                                        },
+                                        validate.union_get("vid", "playerUrls"),
+                                    ),
+                                ],
+                                [],
+                            ),
+                        },
+                        validate.union_get(
+                            "category",
+                            "title",
+                            ("data", 0),
+                        ),
+                    ),
                 ),
-                dict,
             ),
-            {"contentUrl": validate.url()},
-            validate.get("contentUrl"),
-            validate.transform(lambda content_url: update_scheme("https://", content_url)),
         )
-        try:
-            vod = schema_vod.validate(root)
-        except PluginError:
+        if type(data) is str:
+            log.error(data)
             return
 
-        if urlparse(vod).path.endswith(".m3u8"):
-            return HLSStream.parse_variant_playlist(self.session, vod)
-
-        return {"vod": HTTPStream(self.session, vod)}
+        self.category, self.title, streamdata = data
+        if not streamdata:
+            return
 
-    def _get_streams(self):
-        root = self.session.http.get(self.url, schema=validate.Schema(
-            validate.parse_html(),
-        ))
+        self.id, streams = streamdata
 
-        return self._get_hls(root) or self._get_vod(root)
+        for streamtype, streamurl in streams:
+            if streamurl and streamtype == "live_hls":
+                return HLSStream.parse_variant_playlist(self.session, streamurl)
 
 
-__plugin__ = TV5Monde
+__plugin__ = VKplay
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tv8.py` & `streamlink-5.4.0/src/streamlink/plugins/tv8.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tv999.py` & `streamlink-5.4.0/src/streamlink/plugins/tv999.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tvibo.py` & `streamlink-5.4.0/src/streamlink/plugins/tvibo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tviplayer.py` & `streamlink-5.4.0/src/streamlink/plugins/vidio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 """
-$description Live TV channels and video on-demand service from TVI, a Portuguese free-to-air broadcaster.
-$url tviplayer.iol.pt
+$description Indonesian & international live TV channels and video on-demand service. OTT service from Vidio.
+$url vidio.com
 $type live, vod
 """
-
 import logging
 import re
+from urllib.parse import urlsplit, urlunsplit
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
+from streamlink.stream.dash import DASHStream
 from streamlink.stream.hls import HLSStream
-from streamlink.utils.url import update_qsd
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"https://tviplayer\.iol\.pt/(?:direto|programa)/",
+    r"https?://(?:www\.)?vidio\.com/",
 ))
-class TVIPlayer(Plugin):
+class Vidio(Plugin):
+    tokens_url = "https://www.vidio.com/live/{id}/tokens"
+
+    def _get_stream_token(self, stream_id, stream_type):
+        log.debug("Getting stream token")
+        return self.session.http.post(
+            self.tokens_url.format(id=stream_id),
+            params={"type": stream_type},
+            headers={"Referer": self.url},
+            schema=validate.Schema(
+                validate.parse_json(),
+                {"token": str},
+                validate.get("token"),
+            ),
+        )
+
     def _get_streams(self):
-        self.session.http.headers.update({"Referer": "https://tviplayer.iol.pt/"})
-        data = self.session.http.get(
+        stream_id, has_token, hls_url, dash_url = self.session.http.get(
             self.url,
             schema=validate.Schema(
                 validate.parse_html(),
-                validate.xml_xpath_string(".//script[contains(text(),'.m3u8')]/text()"),
-                validate.none_or_all(
-                    re.compile(r"jsonData\s*=\s*(?P<json>{.+?})\s*;", re.DOTALL),
-                    validate.none_or_all(
-                        validate.get("json"),
-                        validate.parse_json(),
-                        {
-                            "id": str,
-                            "liveType": str,
-                            "videoType": str,
-                            "videoUrl": validate.url(path=validate.endswith(".m3u8")),
-                            validate.optional("channel"): str,
-                        },
+                validate.xml_find(".//*[@data-video-id]"),
+                validate.union((
+                    validate.get("data-video-id"),
+                    validate.all(
+                        validate.get("data-video-has-token"),
+                        validate.transform(lambda val: val and val != "false"),
                     ),
-                ),
+                    validate.get("data-vjs-clip-hls-url"),
+                    validate.get("data-vjs-clip-dash-url"),
+                )),
             ),
         )
-        if not data:
-            return
-        log.debug(f"{data!r}")
 
-        if data["liveType"].upper() == "DIRETO" and data["videoType"].upper() == "LIVE":
-            geo_path = "live"
-        else:
-            geo_path = "vod"
-        data_geo = self.session.http.get(
-            f"https://services.iol.pt/direitos/rights/{geo_path}?id={data['id']}",
-            acceptable_status=(200, 403),
-            schema=validate.Schema(
-                validate.parse_json(),
-                {
-                    "code": str,
-                    "error": validate.any(None, str),
-                    "detail": str,
-                },
-            ),
-        )
-        log.debug(f"{data_geo!r}")
-        if data_geo["detail"] != "ok":
-            log.error(f"{data_geo['detail']}")
+        if dash_url and has_token:
+            token = self._get_stream_token(stream_id, "dash")
+            parsed = urlsplit(dash_url)
+            dash_url = urlunsplit(parsed._replace(path=f"{token}{parsed.path}"))
+            return DASHStream.parse_manifest(
+                self.session,
+                dash_url,
+                headers={"Referer": "https://www.vidio.com/"},
+            )
+
+        if not hls_url:
             return
 
-        wmsAuthSign = self.session.http.get(
-            "https://services.iol.pt/matrix?userId=",
-            schema=validate.Schema(str),
+        if has_token:
+            token = self._get_stream_token(stream_id, "hls")
+            hls_url = f"{hls_url}?{token}"
+
+        return HLSStream.parse_variant_playlist(
+            self.session,
+            hls_url,
+            headers={"Referer": "https://www.vidio.com/"},
         )
-        hls_url = update_qsd(data["videoUrl"], {"wmsAuthSign": wmsAuthSign})
-        return HLSStream.parse_variant_playlist(self.session, hls_url)
 
 
-__plugin__ = TVIPlayer
+__plugin__ = Vidio
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tvp.py` & `streamlink-5.4.0/src/streamlink/plugins/tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tvrby.py` & `streamlink-5.4.0/src/streamlink/plugins/tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tvrplus.py` & `streamlink-5.4.0/src/streamlink/plugins/tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/tvtoya.py` & `streamlink-5.4.0/src/streamlink/plugins/tvtoya.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/twitch.py` & `streamlink-5.4.0/src/streamlink/plugins/twitch.py`

 * *Files 1% similar despite different names*

```diff
@@ -634,15 +634,15 @@
             response, *data = self.api.access_token(is_live, channel_or_vod)
             if response != "token":
                 error, message = data
                 log.error(f"{error or 'Error'}: {message or 'Unknown error'}")
                 raise PluginError
             sig, token = data
         except (PluginError, TypeError):
-            raise NoStreamsError
+            raise NoStreamsError  # noqa: B904
 
         try:
             restricted_bitrates = self.api.parse_token(token)
         except PluginError:
             restricted_bitrates = []
 
         return sig, token, restricted_bitrates
@@ -695,15 +695,15 @@
         try:
             streams = TwitchHLSStream.parse_variant_playlist(self.session, url, start_offset=time_offset, **extra_params)
         except OSError as err:
             err = str(err)
             if "404 Client Error" in err or "Failed to parse playlist" in err:
                 return
             else:
-                raise PluginError(err)
+                raise PluginError(err) from err
 
         for name in restricted_bitrates:
             if name not in streams:
                 log.warning(f"The quality '{name}' is not available since it requires a subscription.")
 
         return streams
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/useetv.py` & `streamlink-5.4.0/src/streamlink/plugins/indihometv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 """
-$description Live TV channels and video on-demand service from UseeTV, owned by Telkom Indonesia.
-$url useetv.com
+$description Live TV channels and video on-demand service from IndiHome TV, owned by Telkom Indonesia.
+$url indihometv.com
 $type live, vod
+$region Indonesia
 """
 
-import logging
 import re
 
 from streamlink.plugin import Plugin, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.hls import HLSStream
 
 
-log = logging.getLogger(__name__)
-
-
-@pluginmatcher(re.compile(r"https?://(?:www\.)?useetv\.com/"))
-class UseeTV(Plugin):
+@pluginmatcher(re.compile(r"https?://(?:www\.)?indihometv\.com/"))
+class IndiHomeTV(Plugin):
     def _get_streams(self):
-        root = self.session.http.get(self.url, schema=validate.Schema(validate.parse_html()))
-
-        for needle, errormsg in (
-            (
-                "\"This service is not available in your Country\"",
-                "The content is not available in your region",
-            ),
-            (
-                "\"Silahkan login Menggunakan akun MyIndihome dan berlangganan minipack\"",
-                "The content is not available without a subscription",
-            ),
-        ):
-            if validate.Schema(validate.xml_xpath(".//script[contains(text(),$needle)]", needle=needle)).validate(root):
-                log.error(errormsg)
-                return
-
-        url = validate.Schema(
+        url = self.session.http.get(self.url, schema=validate.Schema(
+            validate.parse_html(),
             validate.any(
                 validate.all(
                     validate.xml_xpath_string("""
                         .//script[contains(text(), 'laylist.m3u8') or contains(text(), 'manifest.mpd')][1]/text()
                     """),
                     str,
                     re.compile(r"""(?P<q>['"])(?P<url>https://.*?/(?:[Pp]laylist\.m3u8|manifest\.mpd).+?)(?P=q)"""),
-                    validate.none_or_all(validate.get("url"), validate.url()),
+                    validate.none_or_all(
+                        validate.get("url"),
+                        validate.url(),
+                    ),
                 ),
                 validate.all(
-                    validate.xml_xpath_string(".//video[@id='video-player']/source/@src"),
-                    validate.any(None, validate.url()),
+                    validate.xml_xpath_string(".//video[@id='video-player'][1]/source[1]/@src"),
+                    validate.none_or_all(
+                        validate.url(),
+                    ),
                 ),
             ),
-        ).validate(root)
+        ))
 
         if url and ".m3u8" in url:
             return HLSStream.parse_variant_playlist(self.session, url)
         elif url and ".mpd" in url:
             return DASHStream.parse_manifest(self.session, url)
 
 
-__plugin__ = UseeTV
+__plugin__ = IndiHomeTV
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ustreamtv.py` & `streamlink-5.4.0/src/streamlink/plugins/ustreamtv.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 $url video.ibm.com
 $type live, vod
 """
 
 import logging
 import re
 from collections import deque
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from random import randint
 from threading import Event, RLock
 from typing import Any, Callable, Deque, Dict, List, NamedTuple, Optional, Union
 from urllib.parse import urljoin, urlunparse
 
 from requests import Response
 
@@ -291,15 +291,15 @@
         if count == 0:
             return
 
         # initial segment ID (needed by the workers to filter queued segments)
         if self.stream_initial_id is None:
             self.stream_initial_id = current_id
 
-        current_time = datetime.now()
+        current_time = datetime.now(timezone.utc)
 
         # lock the stream segments deques for the worker threads
         with self.stream_segments_lock:
             # interpolate and extrapolate segments from the provided id->hash data
             diff = 10 - sorted_ids[0] % 10  # if there's only one id->hash item, extrapolate until the next decimal
             for idx, segment_id in enumerate(sorted_ids):
                 idx_next = idx + 1
@@ -358,15 +358,15 @@
             self.queue(segment, self.executor.submit(self.fetch, segment, False))
 
     # noinspection PyMethodOverriding
     def fetch(self, segment: Segment, is_init: bool):  # type: ignore[override]
         if self.closed:  # pragma: no cover
             return
 
-        now = datetime.now()
+        now = datetime.now(timezone.utc)
         if segment.available_at > now:
             time_to_wait = (segment.available_at - now).total_seconds()
             log.debug(f"Waiting for {self.stream.kind} segment: {segment.num} ({time_to_wait:.01f}s)")
             if not self.reader.worker.wait(time_to_wait):
                 return
 
         try:
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/ustvnow.py` & `streamlink-5.4.0/src/streamlink/plugins/ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/vimeo.py` & `streamlink-5.4.0/src/streamlink/plugins/vimeo.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @pluginmatcher(re.compile(
     r"https?://(player\.vimeo\.com/video/\d+|(www\.)?vimeo\.com/.+)",
 ))
 class Vimeo(Plugin):
     _config_url_re = re.compile(r'(?:"config_url"|\bdata-config-url)\s*[:=]\s*(".+?")')
-    _config_re = re.compile(r"var\s+config\s*=\s*({.+?})\s*;")
+    _config_re = re.compile(r"playerConfig\s*=\s*({.+?})\s*var")
     _config_url_schema = validate.Schema(
         validate.transform(_config_url_re.search),
         validate.any(
             None,
             validate.Schema(
                 validate.get(1),
                 validate.parse_json(),
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/vinhlongtv.py` & `streamlink-5.4.0/src/streamlink/plugins/vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/vk.py` & `streamlink-5.4.0/src/streamlink/plugins/vk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 $description Russian live-streaming and video hosting social platform.
 $url vk.com
+$url vk.ru
 $type live, vod
 """
 
 import logging
 import re
 from hashlib import md5
-from urllib.parse import parse_qsl, unquote, urlparse
+from urllib.parse import parse_qsl, unquote, urlparse, urlunparse
 
 from streamlink.exceptions import NoStreamsError
 from streamlink.plugin import Plugin, PluginError, pluginmatcher
 from streamlink.plugin.api import validate
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.hls import HLSStream
 from streamlink.utils.url import update_qsd
 
 
 log = logging.getLogger(__name__)
 
 
 @pluginmatcher(re.compile(
-    r"https?://(?:\w+\.)?vk\.com/videos?(?:\?z=video)?(?P<video_id>-?\d+_\d+)",
+    r"https?://(?:\w+\.)?vk\.(?:com|ru)/videos?(?:\?z=video)?(?P<video_id>-?\d+_\d+)",
 ))
 @pluginmatcher(re.compile(
-    r"https?://(\w+\.)?vk\.com/.+",
+    r"https?://(\w+\.)?vk\.(?:com|ru)/.+",
 ))
 class VK(Plugin):
     API_URL = "https://vk.com/al_video.php"
     HASH_COOKIE = "hash429"
 
     def _get_cookies(self):
         def on_response(res, **kwargs):
@@ -39,15 +40,16 @@
                     key = md5(cookie.encode("utf-8")).hexdigest()
                     res.headers["Location"] = update_qsd(res.headers["Location"], qsd={"key": key})
                     return res
                 elif res.headers.get("X-WAF-Backend-Status") == "challenge_success":
                     self.session.http.cookies.update(res.cookies)
                     return res
 
-        self.session.http.get("https://vk.com/", hooks={"response": on_response})
+        url = urlunparse(urlparse(self.url)._replace(path="", query="", fragment=""))
+        self.session.http.get(url, hooks={"response": on_response})
 
     def _has_video_id(self):
         return any(self.matches[:-1])
 
     def follow_vk_redirect(self):
         if self._has_video_id():
             return
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/vlive.py` & `streamlink-5.4.0/src/streamlink/plugins/vlive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/vtvgo.py` & `streamlink-5.4.0/src/streamlink/plugins/vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/wasd.py` & `streamlink-5.4.0/src/streamlink/plugins/wasd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-$description Russian live streaming social platform.
+$description Russian live-streaming social platform.
 $url wasd.tv
 $type live
 """
 
 import logging
 import re
 
@@ -71,17 +71,17 @@
         log.trace("{0!r}".format(json_res))
         if not json_res:
             raise PluginError("No data returned from URL={0}".format(res.url))
 
         for stream in json_res["media_container_streams"]:
             log.debug("media_container_status: {0}, media_container_online_status: {1}".format(
                 json_res["media_container_status"], json_res["media_container_online_status"]))
-            for stream in stream["stream_media"]:
-                if stream["media_status"] == "STOPPED":
-                    hls_url = stream["media_meta"]["media_archive_url"]
-                elif stream["media_status"] == "RUNNING":
-                    hls_url = stream["media_meta"]["media_url"]
+            for stream_media in stream["stream_media"]:
+                if stream_media["media_status"] == "STOPPED":
+                    hls_url = stream_media["media_meta"]["media_archive_url"]
+                else:
+                    hls_url = stream_media["media_meta"]["media_url"]
 
                 yield from HLSStream.parse_variant_playlist(self.session, hls_url).items()
 
 
 __plugin__ = WASD
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/webtv.py` & `streamlink-5.4.0/src/streamlink/plugins/webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/welt.py` & `streamlink-5.4.0/src/streamlink/plugins/welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/wwenetwork.py` & `streamlink-5.4.0/src/streamlink/plugins/wwenetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                             headers={"Content-Type": "application/json"})
         if "authorisationToken" in data:
             self.auth_token = data["authorisationToken"]
 
         return self.auth_token
 
     @property  # type: ignore
-    @lru_cache(maxsize=128)
+    @lru_cache(maxsize=128)  # noqa: B019
     def item_config(self):
         log.debug("Loading page config")
         p = urlparse(self.url)
         res = self.session.http.get(self.page_config_url,
                                     params=dict(device="web_browser",
                                                 ff="idp,ldp",
                                                 item_detail_expand="all",
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/youtube.py` & `streamlink-5.4.0/src/streamlink/plugins/youtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     def _create_adaptive_streams(self, adaptive_formats):
         streams = {}
         adaptive_streams = {}
         audio_streams = {}
         best_audio_itag = None
 
         # Extract audio streams from the adaptive format list
-        for url, label, itag, mimeType in adaptive_formats:
+        for url, _label, itag, mimeType in adaptive_formats:
             if url is None:
                 continue
 
             # extract any high quality streams only available in adaptive formats
             adaptive_streams[itag] = url
             stream_type, stream_codec = mimeType
             stream_codec = re.sub(r"^(\w+).*$", r"\1", stream_codec)
```

### Comparing `streamlink-5.3.1/src/streamlink/plugins/yupptv.py` & `streamlink-5.4.0/src/streamlink/plugins/yupptv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/zattoo.py` & `streamlink-5.4.0/src/streamlink/plugins/zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/zdf_mediathek.py` & `streamlink-5.4.0/src/streamlink/plugins/zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/zeenews.py` & `streamlink-5.4.0/src/streamlink/plugins/zeenews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/zengatv.py` & `streamlink-5.4.0/src/streamlink/plugins/zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/plugins/zhanqi.py` & `streamlink-5.4.0/src/streamlink/plugins/zhanqi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/session.py` & `streamlink-5.4.0/src/streamlink/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,29 @@
 logging.setLoggerClass(StreamlinkLogger)
 log = logging.getLogger(__name__)
 
 
 _original_allowed_gai_family = urllib3_util_connection.allowed_gai_family  # type: ignore[attr-defined]
 
 
+def _get_deprecation_stacklevel_offset():
+    """Deal with stacklevels of both session.{g,s}et_option() and session.options.{g,s}et() calls"""
+    from inspect import currentframe
+
+    frame = currentframe().f_back.f_back
+    offset = 0
+    while frame:
+        if frame.f_code.co_filename == __file__ and frame.f_code.co_name in ("set_option", "get_option"):
+            offset += 1
+            break
+        frame = frame.f_back
+
+    return offset
+
+
 class PythonDeprecatedWarning(UserWarning):
     pass
 
 
 class StreamlinkOptions(Options):
     def __init__(self, session: "Streamlink", *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -43,22 +58,27 @@
         for keyval in value.split(delimiter):
             try:
                 key, val = keyval.split("=", 1)
                 yield key.strip(), val.strip()
             except ValueError:
                 continue
 
-    # ---- getters
-
-    def _get_http_proxy(self, key):
+    @staticmethod
+    def _deprecate_https_proxy(key: str) -> None:
         if key == "https-proxy":
             warnings.warn(
                 "The `https-proxy` option has been deprecated in favor of a single `http-proxy` option",
                 StreamlinkDeprecationWarning,
+                stacklevel=4 + _get_deprecation_stacklevel_offset(),
             )
+
+    # ---- getters
+
+    def _get_http_proxy(self, key):
+        self._deprecate_https_proxy(key)
         return self.session.http.proxies.get("https" if key == "https-proxy" else "http")
 
     def _get_http_attr(self, key):
         return getattr(self.session.http, self._OPTIONS_HTTP_ATTRS[key])
 
     # ---- setters
 
@@ -84,19 +104,15 @@
             self.set_explicit("ipv4", False)
             urllib3_util_connection.allowed_gai_family = (lambda: AF_INET6)  # type: ignore[attr-defined]
 
     def _set_http_proxy(self, key, value):
         self.session.http.proxies["http"] \
             = self.session.http.proxies["https"] \
             = update_scheme("https://", value, force=False)
-        if key == "https-proxy":
-            warnings.warn(
-                "The `https-proxy` option has been deprecated in favor of a single `http-proxy` option",
-                StreamlinkDeprecationWarning,
-            )
+        self._deprecate_https_proxy(key)
 
     def _set_http_attr(self, key, value):
         setattr(self.session.http, self._OPTIONS_HTTP_ATTRS[key], value)
 
     def _set_http_disable_dh(self, key, value):
         self.set_explicit(key, value)
         default_ciphers = [
@@ -120,14 +136,15 @@
     @staticmethod
     def _factory_set_deprecated(name: str, mapper: Callable[[Any], Any]) -> Callable[["StreamlinkOptions", str, Any], None]:
         def inner(self: "StreamlinkOptions", key: str, value: Any) -> None:
             self.set_explicit(name, mapper(value))
             warnings.warn(
                 f"`{key}` has been deprecated in favor of the `{name}` option",
                 StreamlinkDeprecationWarning,
+                stacklevel=3 + _get_deprecation_stacklevel_offset(),
             )
 
         return inner
 
     # bind explicitly with dummy context, to prevent `TypeError: 'staticmethod' object is not callable` on py<310
     _factory_set_http_attr_key_equals_value = _factory_set_http_attr_key_equals_value.__get__(object)
     _factory_set_deprecated = _factory_set_deprecated.__get__(object)
@@ -220,14 +237,15 @@
             "hls-duration": None,
             "hls-playlist-reload-attempts": 3,
             "hls-playlist-reload-time": "default",
             "hls-segment-stream-data": False,
             "hls-segment-ignore-names": [],
             "hls-segment-key-uri": None,
             "hls-audio-select": [],
+            "dash-manifest-reload-attempts": 3,
             "ffmpeg-ffmpeg": None,
             "ffmpeg-no-validation": False,
             "ffmpeg-verbose": False,
             "ffmpeg-verbose-path": None,
             "ffmpeg-fout": None,
             "ffmpeg-video-transcode": None,
             "ffmpeg-audio-transcode": None,
@@ -363,15 +381,15 @@
             * - hls-duration
               - ``float | None``
               - ``None``
               - Limit the HLS stream playback duration, rounded to the nearest HLS segment
             * - hls-playlist-reload-attempts
               - ``int``
               - ``3``
-              - Number of HLS playlist reload attempts before giving up
+              - Max number of HLS playlist reload attempts before giving up
             * - hls-playlist-reload-time
               - ``str | float``
               - ``"default"``
               - Override the HLS playlist reload time, either in seconds (``float``) or as a ``str`` keyword:
 
                 - ``segment``: duration of the last segment
                 - ``live-edge``: sum of segment durations of the ``hls-live-edge`` value minus one
@@ -391,14 +409,18 @@
                 with support for the following string template variables:
                 ``{url}``, ``{scheme}``, ``{netloc}``, ``{path}``, ``{query}``
             * - hls-audio-select
               - ``List[str]``
               - ``[]``
               - Select a specific audio source or sources when multiple audio sources are available,
                 by language code or name, or ``"*"`` (asterisk)
+            * - dash-manifest-reload-attempts
+              - ``int``
+              - ``3``
+              - Max number of DASH manifest reload attempts before giving up
             * - hls-segment-attempts *(deprecated)*
               - ``int``
               - ``3``
               - See ``stream-segment-attempts``
             * - hls-segment-threads *(deprecated)*
               - ``int``
               - ``3``
@@ -502,15 +524,15 @@
         :param key: key of the option
         """
 
         if plugin in self.plugins:
             plugincls = self.plugins[plugin]
             return plugincls.get_option(key)
 
-    @lru_cache(maxsize=128)
+    @lru_cache(maxsize=128)  # noqa: B019
     def resolve_url(
         self,
         url: str,
         follow_redirect: bool = True,
     ) -> Tuple[str, Type[Plugin], str]:
         """
         Attempts to find a plugin that can use this URL.
@@ -538,14 +560,15 @@
             # TODO: remove deprecated plugin resolver
             elif hasattr(plugin, "can_handle_url") and callable(plugin.can_handle_url) and plugin.can_handle_url(url):
                 prio = plugin.priority(url) if hasattr(plugin, "priority") and callable(plugin.priority) else NORMAL_PRIORITY
                 if prio > priority:
                     warnings.warn(
                         f"Resolved plugin {name} with deprecated can_handle_url API",
                         StreamlinkDeprecationWarning,
+                        stacklevel=1,
                     )
                     candidate = name, plugin
                     priority = prio
 
         if candidate:
             return candidate[0], candidate[1], url
 
@@ -605,15 +628,15 @@
         Attempt to load plugins from the path specified.
 
         :param path: full path to a directory where to look for plugins
         :return: success
         """
 
         success = False
-        for loader, name, ispkg in pkgutil.iter_modules([path]):
+        for _loader, name, _ispkg in pkgutil.iter_modules([path]):
             # set the full plugin module name
             # use the "streamlink.plugins." prefix even for sideloaded plugins
             module_name = f"streamlink.plugins.{name}"
             try:
                 mod = load_module(module_name, path)
             except ImportError:
                 log.exception(f"Failed to load plugin {name} from {path}\n")
```

### Comparing `streamlink-5.3.1/src/streamlink/stream/dash.py` & `streamlink-5.4.0/src/streamlink/stream/dash.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,131 +1,125 @@
 import copy
-import datetime
 import itertools
 import logging
 from collections import defaultdict
-from contextlib import contextmanager
-from pathlib import Path
+from contextlib import contextmanager, suppress
+from datetime import datetime
 from time import time
-from typing import Dict, Optional
+from typing import Any, Dict, List, Optional, Tuple
 from urllib.parse import urlparse, urlunparse
 
-from streamlink import PluginError, StreamError
+from streamlink.exceptions import PluginError, StreamError
+from streamlink.session import Streamlink
 from streamlink.stream.dash_manifest import MPD, Representation, Segment, freeze_timeline
 from streamlink.stream.ffmpegmux import FFMPEGMuxer
 from streamlink.stream.segmented import SegmentedStreamReader, SegmentedStreamWorker, SegmentedStreamWriter
 from streamlink.stream.stream import Stream
 from streamlink.utils.l10n import Language
 from streamlink.utils.parse import parse_xml
+from streamlink.utils.times import now
 
 
 log = logging.getLogger(__name__)
 
-UTC = datetime.timezone.utc
-
 
 class DASHStreamWriter(SegmentedStreamWriter):
     reader: "DASHStreamReader"
     stream: "DASHStream"
 
-    @staticmethod
-    def _get_segment_name(segment: Segment) -> str:
-        return Path(urlparse(segment.url).path).resolve().name
-
     def fetch(self, segment: Segment, retries: Optional[int] = None):
         if self.closed or not retries:
             return
 
-        try:
-            request_args = copy.deepcopy(self.reader.stream.args)
-            headers = request_args.pop("headers", {})
-            now = datetime.datetime.now(tz=UTC)
-            if segment.available_at > now:
-                time_to_wait = (segment.available_at - now).total_seconds()
-                fname = self._get_segment_name(segment)
-                log.debug(f"Waiting for segment: {fname} ({time_to_wait:.01f}s)")
-                if not self.wait(time_to_wait):
-                    log.debug(f"Waiting for segment: {fname} aborted")
-                    return
+        name = segment.name
+        available_in = segment.available_in
+        if available_in > 0:
+            log.debug(f"{self.reader.mime_type} segment {name}: waiting {available_in:.01f}s ({segment.availability})")
+            if not self.wait(available_in):
+                log.debug(f"{self.reader.mime_type} segment {name}: cancelled")
+                return
+        log.debug(f"{self.reader.mime_type} segment {name}: downloading ({segment.availability})")
+
+        request_args = copy.deepcopy(self.reader.stream.args)
+        headers = request_args.pop("headers", {})
 
-            if segment.byterange:
-                start, length = segment.byterange
-                end = str(start + length - 1) if length else ""
-                headers["Range"] = f"bytes={start}-{end}"
+        if segment.byterange:
+            start, length = segment.byterange
+            end = str(start + length - 1) if length else ""
+            headers["Range"] = f"bytes={start}-{end}"
 
+        try:
             return self.session.http.get(
                 segment.url,
                 timeout=self.timeout,
                 exception=StreamError,
                 headers=headers,
+                retries=retries,
                 **request_args,
             )
         except StreamError as err:
-            log.error(f"Failed to open segment {segment.url}: {err}")
-            return self.fetch(segment, retries - 1)
+            log.error(f"{self.reader.mime_type} segment {name}: failed ({err})")
 
     def write(self, segment, res, chunk_size=8192):
-        name = self._get_segment_name(segment)
         for chunk in res.iter_content(chunk_size):
             if self.closed:
-                log.warning(f"Download of segment: {name} aborted")
+                log.warning(f"{self.reader.mime_type} segment {segment.name}: aborted")
                 return
             self.reader.buffer.write(chunk)
 
-        log.debug(f"Download of segment: {name} complete")
+        log.debug(f"{self.reader.mime_type} segment {segment.name}: completed")
 
 
 class DASHStreamWorker(SegmentedStreamWorker):
     reader: "DASHStreamReader"
     writer: "DASHStreamWriter"
     stream: "DASHStream"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.mpd = self.stream.mpd
-        self.period = self.stream.period
+
+        self.manifest_reload_retries = self.session.options.get("dash-manifest-reload-attempts")
 
     @contextmanager
     def sleeper(self, duration):
         """
         Do something and then wait for a given duration minus the time it took doing something
         """
         s = time()
         yield
         time_to_sleep = duration - (time() - s)
         if time_to_sleep > 0:
             self.wait(time_to_sleep)
 
-    @staticmethod
-    def get_representation(mpd, representation_id, mime_type):
-        for aset in mpd.periods[0].adaptationSets:
-            for rep in aset.representations:
-                if rep.id == representation_id and rep.mimeType == mime_type:
-                    return rep
-
     def iter_segments(self):
         init = True
         back_off_factor = 1
         while not self.closed:
             # find the representation by ID
-            representation = self.get_representation(self.mpd, self.reader.representation_id, self.reader.mime_type)
+            representation = self.mpd.get_representation(self.reader.ident)
 
             if self.mpd.type == "static":
                 refresh_wait = 5
             else:
                 refresh_wait = max(
                     self.mpd.minimumUpdatePeriod.total_seconds(),
-                    self.mpd.periods[0].duration.total_seconds(),
+                    representation.period.duration.total_seconds() if representation else 0,
                 ) or 5
 
             with self.sleeper(refresh_wait * back_off_factor):
                 if not representation:
                     continue
 
-                for segment in representation.segments(init=init):
+                iter_segments = representation.segments(
+                    init=init,
+                    # sync initial timeline generation between audio and video threads
+                    timestamp=self.reader.timestamp if init else None,
+                )
+                for segment in iter_segments:
                     if self.closed:
                         break
                     yield segment
 
                 # close worker if type is not dynamic (all segments were put into writer queue)
                 if self.mpd.type != "dynamic":
                     self.close()
@@ -139,23 +133,30 @@
                 init = False
 
     def reload(self):
         if self.closed:
             return
 
         self.reader.buffer.wait_free()
-        log.debug("Reloading manifest ({0}:{1})".format(self.reader.representation_id, self.reader.mime_type))
-        res = self.session.http.get(self.mpd.url, exception=StreamError, **self.stream.args)
-
-        new_mpd = MPD(self.session.http.xml(res, ignore_ns=True),
-                      base_url=self.mpd.base_url,
-                      url=self.mpd.url,
-                      timelines=self.mpd.timelines)
+        log.debug(f"Reloading manifest {self.reader.ident!r}")
+        res = self.session.http.get(
+            self.mpd.url,
+            exception=StreamError,
+            retries=self.manifest_reload_retries,
+            **self.stream.args,
+        )
+
+        new_mpd = MPD(
+            self.session.http.xml(res, ignore_ns=True),
+            base_url=self.mpd.base_url,
+            url=self.mpd.url,
+            timelines=self.mpd.timelines,
+        )
 
-        new_rep = self.get_representation(new_mpd, self.reader.representation_id, self.reader.mime_type)
+        new_rep = new_mpd.get_representation(self.reader.ident)
         with freeze_timeline(new_mpd):
             changed = len(list(itertools.islice(new_rep.segments(), 1))) > 0
 
         if changed:
             self.mpd = new_mpd
 
         return changed
@@ -165,51 +166,55 @@
     __worker__ = DASHStreamWorker
     __writer__ = DASHStreamWriter
 
     worker: "DASHStreamWorker"
     writer: "DASHStreamWriter"
     stream: "DASHStream"
 
-    def __init__(self, stream: "DASHStream", representation_id, mime_type, *args, **kwargs):
+    def __init__(
+        self,
+        stream: "DASHStream",
+        representation: Representation,
+        timestamp: datetime,
+        *args,
+        **kwargs,
+    ):
         super().__init__(stream, *args, **kwargs)
-        self.mime_type = mime_type
-        self.representation_id = representation_id
-        log.debug("Opening DASH reader for: {0} ({1})".format(self.representation_id, self.mime_type))
+        self.ident = representation.ident
+        self.mime_type = representation.mimeType
+        self.timestamp = timestamp
 
 
 class DASHStream(Stream):
     """
     Implementation of the "Dynamic Adaptive Streaming over HTTP" protocol (MPEG-DASH)
     """
 
     __shortname__ = "dash"
 
     def __init__(
         self,
-        session,
+        session: Streamlink,
         mpd: MPD,
         video_representation: Optional[Representation] = None,
         audio_representation: Optional[Representation] = None,
-        period: float = 0,
         **args,
     ):
         """
-        :param streamlink.Streamlink session: Streamlink session instance
+        :param session: Streamlink session instance
         :param mpd: Parsed MPD manifest
         :param video_representation: Video representation
         :param audio_representation: Audio representation
-        :param period: Update period
         :param args: Additional keyword arguments passed to :meth:`requests.Session.request`
         """
 
         super().__init__(session)
         self.mpd = mpd
         self.video_representation = video_representation
         self.audio_representation = audio_representation
-        self.period = period
         self.args = args
 
     def __json__(self):
         json = dict(type=self.shortname())
 
         if self.mpd.url:
             args = self.args.copy()
@@ -226,137 +231,162 @@
     def to_url(self):
         if self.mpd.url is None:
             return super().to_url()
 
         # the MPD URL has already been prepared by the initial request in `parse_manifest`
         return self.mpd.url
 
+    @staticmethod
+    def fetch_manifest(session: Streamlink, url_or_manifest: str, **request_args) -> Tuple[str, Dict[str, Any]]:
+        if url_or_manifest.startswith("<?xml"):
+            return url_or_manifest, {}
+
+        retries = session.options.get("dash-manifest-reload-attempts")
+        args = session.http.valid_request_args(**request_args)
+        res = session.http.get(url_or_manifest, retries=retries, **args)
+        manifest: str = res.text
+        url: str = res.url
+
+        urlp = list(urlparse(url))
+        urlp[2], _ = urlp[2].rsplit("/", 1)
+        base_url: str = urlunparse(urlp)
+
+        return manifest, dict(url=url, base_url=base_url)
+
+    @staticmethod
+    def parse_mpd(manifest: str, mpd_params: Dict[str, Any]) -> MPD:
+        node = parse_xml(manifest, ignore_ns=True)
+
+        return MPD(node, **mpd_params)
+
     @classmethod
     def parse_manifest(
         cls,
-        session,
+        session: Streamlink,
         url_or_manifest: str,
+        period: int = 0,
         **args,
     ) -> Dict[str, "DASHStream"]:
         """
         Parse a DASH manifest file and return its streams.
 
-        :param streamlink.Streamlink session: Streamlink session instance
+        :param session: Streamlink session instance
         :param url_or_manifest: URL of the manifest file or an XML manifest string
+        :param period: Which MPD period to use (index number) for finding representations
         :param args: Additional keyword arguments passed to :meth:`requests.Session.request`
         """
 
-        if url_or_manifest.startswith("<?xml"):
-            mpd = MPD(parse_xml(url_or_manifest, ignore_ns=True))
-        else:
-            res = session.http.get(url_or_manifest, **session.http.valid_request_args(**args))
-            url = res.url
-
-            urlp = list(urlparse(url))
-            urlp[2], _ = urlp[2].rsplit("/", 1)
-
-            mpd = MPD(session.http.xml(res, ignore_ns=True), base_url=urlunparse(urlp), url=url)
+        manifest, mpd_params = cls.fetch_manifest(session, url_or_manifest)
 
-        video, audio = [], []
+        try:
+            mpd = cls.parse_mpd(manifest, mpd_params)
+        except Exception as err:
+            raise PluginError(f"Failed to parse MPD manifest: {err}") from err
+
+        source = mpd_params.get("url", "MPD manifest")
+        video: List[Optional[Representation]] = []
+        audio: List[Optional[Representation]] = []
 
         # Search for suitable video and audio representations
-        for aset in mpd.periods[0].adaptationSets:
-            if aset.contentProtection:
-                raise PluginError(f"{url} is protected by DRM")
+        for aset in mpd.periods[period].adaptationSets:
+            if aset.contentProtections:
+                raise PluginError(f"{source} is protected by DRM")
             for rep in aset.representations:
-                if rep.contentProtection:
-                    raise PluginError(f"{url} is protected by DRM")
+                if rep.contentProtections:
+                    raise PluginError(f"{source} is protected by DRM")
                 if rep.mimeType.startswith("video"):
                     video.append(rep)
-                elif rep.mimeType.startswith("audio"):
+                elif rep.mimeType.startswith("audio"):  # pragma: no branch
                     audio.append(rep)
 
         if not video:
-            video = [None]
-
+            video.append(None)
         if not audio:
-            audio = [None]
+            audio.append(None)
 
         locale = session.localization
         locale_lang = locale.language
         lang = None
         available_languages = set()
 
         # if the locale is explicitly set, prefer that language over others
         for aud in audio:
             if aud and aud.lang:
                 available_languages.add(aud.lang)
-                try:
+                with suppress(LookupError):
                     if locale.explicit and aud.lang and Language.get(aud.lang) == locale_lang:
                         lang = aud.lang
-                except LookupError:
-                    continue
 
         if not lang:
             # filter by the first language that appears
-            lang = audio[0] and audio[0].lang
+            lang = audio[0].lang if audio[0] else None
 
-        log.debug("Available languages for DASH audio streams: {0} (using: {1})".format(
-            ", ".join(available_languages) or "NONE",
-            lang or "n/a",
-        ))
+        log.debug(
+            f"Available languages for DASH audio streams: {', '.join(available_languages) or 'NONE'} (using: {lang or 'n/a'})",
+        )
 
         # if the language is given by the stream, filter out other languages that do not match
         if len(available_languages) > 1:
-            audio = list(filter(lambda a: a.lang is None or a.lang == lang, audio))
+            audio = [a for a in audio if a and (a.lang is None or a.lang == lang)]
 
         ret = []
         for vid, aud in itertools.product(video, audio):
             stream = DASHStream(session, mpd, vid, aud, **args)
             stream_name = []
 
             if vid:
-                stream_name.append("{:0.0f}{}".format(vid.height or vid.bandwidth_rounded, "p" if vid.height else "k"))
-            if audio and len(audio) > 1:
-                stream_name.append("a{:0.0f}k".format(aud.bandwidth))
+                stream_name.append(f"{vid.height or vid.bandwidth_rounded:0.0f}{'p' if vid.height else 'k'}")
+            if aud and len(audio) > 1:
+                stream_name.append(f"a{aud.bandwidth:0.0f}k")
             ret.append(("+".join(stream_name), stream))
 
         # rename duplicate streams
         dict_value_list = defaultdict(list)
         for k, v in ret:
             dict_value_list[k].append(v)
 
-        def sortby_bandwidth(dash_stream: DASHStream) -> int:
+        def sortby_bandwidth(dash_stream: DASHStream) -> float:
             if dash_stream.video_representation:
                 return dash_stream.video_representation.bandwidth
             if dash_stream.audio_representation:
                 return dash_stream.audio_representation.bandwidth
             return 0  # pragma: no cover
 
         ret_new = {}
         for q in dict_value_list:
             items = dict_value_list[q]
 
-            try:
+            with suppress(AttributeError):
                 items = sorted(items, key=sortby_bandwidth, reverse=True)
-            except AttributeError:
-                pass
 
             for n in range(len(items)):
                 if n == 0:
                     ret_new[q] = items[n]
                 elif n == 1:
                     ret_new[f"{q}_alt"] = items[n]
                 else:
                     ret_new[f"{q}_alt{n}"] = items[n]
+
         return ret_new
 
     def open(self):
-        if self.video_representation:
-            video = DASHStreamReader(self, self.video_representation.id, self.video_representation.mimeType)
+        video, audio = None, None
+        rep_video, rep_audio = self.video_representation, self.audio_representation
+
+        timestamp = now()
+
+        if rep_video:
+            video = DASHStreamReader(self, rep_video, timestamp)
+            log.debug(f"Opening DASH reader for: {rep_video.ident!r} - {rep_video.mimeType}")
             video.open()
 
-        if self.audio_representation:
-            audio = DASHStreamReader(self, self.audio_representation.id, self.audio_representation.mimeType)
+        if rep_audio:
+            audio = DASHStreamReader(self, rep_audio, timestamp)
+            log.debug(f"Opening DASH reader for: {rep_audio.ident!r} - {rep_audio.mimeType}")
             audio.open()
 
-        if self.video_representation and self.audio_representation:
+        if video and audio:
             return FFMPEGMuxer(self.session, video, audio, copyts=True).open()
-        elif self.video_representation:
+        elif video:
             return video
-        elif self.audio_representation:
+        elif audio:
             return audio
```

### Comparing `streamlink-5.3.1/src/streamlink/stream/dash_manifest.py` & `streamlink-5.4.0/src/streamlink/stream/dash_manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,82 @@
 import copy
 import dataclasses
-import datetime
 import logging
 import math
 import re
 from collections import defaultdict
 from contextlib import contextmanager
+from datetime import datetime, timedelta
 from itertools import count, repeat
+from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
+    Dict,
     Iterator,
     List,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
+    overload,
 )
 from urllib.parse import urljoin, urlparse, urlsplit, urlunparse, urlunsplit
 
 from isodate import Duration, parse_datetime, parse_duration  # type: ignore[import]
 
 # noinspection PyProtectedMember
 from lxml.etree import _Attrib, _Element
 
+from streamlink.utils.times import UTC, fromtimestamp, now
+
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing_extensions import Literal
 
 
 log = logging.getLogger(__name__)
 
-UTC = datetime.timezone.utc
-EPOCH_START = datetime.datetime(1970, 1, 1, tzinfo=UTC)
-ONE_SECOND = datetime.timedelta(seconds=1)
+EPOCH_START = fromtimestamp(0)
+ONE_SECOND = timedelta(seconds=1)
+
+SEGMENT_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
 @dataclasses.dataclass
 class Segment:
     url: str
-    duration: float
+    number: Optional[int] = None
+    duration: Optional[float] = None
+    available_at: datetime = EPOCH_START
     init: bool = False
     content: bool = True
-    available_at: datetime.datetime = EPOCH_START
     byterange: Optional[Tuple[int, Optional[int]]] = None
 
+    @property
+    def name(self) -> str:
+        if self.init and not self.content:
+            return "initialization"
+        if self.number is not None:
+            return str(self.number)
+        return Path(urlparse(self.url).path).resolve().name
+
+    @property
+    def available_in(self) -> float:
+        return max(0.0, (self.available_at - now()).total_seconds())
+
+    @property
+    def availability(self) -> str:
+        return f"{self.available_at.strftime(SEGMENT_TIME_FORMAT)} / {now().strftime(SEGMENT_TIME_FORMAT)}"
+
 
 @dataclasses.dataclass
 class TimelineSegment:
     t: int
     d: int
 
 
@@ -61,19 +84,16 @@
     return x
 
 
 def datetime_to_seconds(dt):
     return (dt - EPOCH_START).total_seconds()
 
 
-def count_dt(
-    firstval: Optional[datetime.datetime] = None,
-    step: datetime.timedelta = ONE_SECOND,
-) -> Iterator[datetime.datetime]:
-    current = datetime.datetime.now(tz=UTC) if firstval is None else firstval
+def count_dt(firstval: Optional[datetime] = None, step: timedelta = ONE_SECOND) -> Iterator[datetime]:
+    current = now() if firstval is None else firstval
     while True:
         yield current
         current += step
 
 
 @contextmanager
 def freeze_timeline(mpd):
@@ -93,19 +113,19 @@
     @staticmethod
     def type(mpdtype: "Literal['static', 'dynamic']") -> "Literal['static', 'dynamic']":
         if mpdtype not in ("static", "dynamic"):
             raise MPDParsingError("@type must be static or dynamic")
         return mpdtype
 
     @staticmethod
-    def duration(duration: str) -> Union[datetime.timedelta, Duration]:
+    def duration(duration: str) -> Union[timedelta, Duration]:
         return parse_duration(duration)
 
     @staticmethod
-    def datetime(dt: str) -> datetime.datetime:
+    def datetime(dt: str) -> datetime:
         return parse_datetime(dt).replace(tzinfo=UTC)
 
     @staticmethod
     def segment_template(url_template: str) -> Callable[..., str]:
         end = 0
         res = ""
         for m in _re_segment_template.finditer(url_template):
@@ -121,15 +141,15 @@
 
         a, b = frame_rate.split("/")
         return float(a) / float(b)
 
     @staticmethod
     def timedelta(timescale: float = 1):
         def _timedelta(seconds):
-            return datetime.timedelta(seconds=int(float(seconds) / float(timescale)))
+            return timedelta(seconds=int(float(seconds) / float(timescale)))
 
         return _timedelta
 
     @staticmethod
     def range(range_spec: str) -> Tuple[int, Optional[int]]:
         r = range_spec.split("-")
         if len(r) != 2:
@@ -143,28 +163,23 @@
     pass
 
 
 TMPDNode = TypeVar("TMPDNode", bound="MPDNode", covariant=True)
 TAttrDefault = TypeVar("TAttrDefault", Any, None)
 TAttrParseResult = TypeVar("TAttrParseResult")
 
+TTimelineIdent = Tuple[Optional[str], Optional[str], str]
+
 
 class MPDNode:
     __tag__: ClassVar[str]
 
     parent: "MPDNode"
 
-    def __init__(
-        self,
-        node: _Element,
-        root: "MPD",
-        parent: "MPDNode",
-        *args,
-        **kwargs,
-    ):
+    def __init__(self, node: _Element, root: "MPD", parent: "MPDNode", **kwargs) -> None:
         self.node = node
         self.root = root
         self.parent = parent
         self._base_url = kwargs.get("base_url")
         self.attributes: Set[str] = set()
         if self.__tag__ and self.node.tag.lower() != self.__tag__.lower():
             raise MPDParsingError(f"Root tag did not match the expected tag: {self.__tag__}")
@@ -176,75 +191,124 @@
     @property
     def text(self) -> Optional[str]:
         return self.node.text
 
     def __str__(self):
         return f"<{self.__tag__} {' '.join(f'@{attr}={getattr(self, attr)}' for attr in self.attributes)}>"
 
+    @overload
+    def attr(  # type: ignore[misc]  # "Overloaded function signatures 1 and 2 overlap with incompatible return types"
+        self,
+        key: str,
+        parser: None = None,
+        default: None = None,
+        required: bool = False,
+        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+    ) -> Optional[str]:  # pragma: no cover
+        pass
+
+    @overload
+    def attr(
+        self,
+        key: str,
+        parser: None,
+        default: TAttrDefault,
+        required: bool = False,
+        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+    ) -> TAttrDefault:  # pragma: no cover
+        pass
+
+    @overload
+    def attr(
+        self,
+        key: str,
+        parser: Callable[[Any], TAttrParseResult],
+        default: None = None,
+        required: bool = False,
+        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+    ) -> Optional[TAttrParseResult]:  # pragma: no cover
+        pass
+
+    @overload
     def attr(
         self,
         key: str,
-        default: TAttrDefault = None,
-        parser: Optional[Callable[[Any], TAttrParseResult]] = None,
+        parser: Callable[[Any], TAttrParseResult],
+        default: TAttrDefault,
         required: bool = False,
-        inherited: bool = False,
-    ) -> Union[TAttrParseResult, TAttrDefault, Any]:
+        inherited: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+    ) -> Union[TAttrParseResult, TAttrDefault]:  # pragma: no cover
+        pass
+
+    def attr(self, key, parser=None, default=None, required=False, inherited=None):
         self.attributes.add(key)
         if key in self.attrib:
-            value: Any = self.attrib.get(key)
+            value = self.attrib.get(key)
             if parser and callable(parser):
                 return parser(value)
             else:
                 return value
         elif inherited:
-            if self.parent and hasattr(self.parent, key) and getattr(self.parent, key):
-                return getattr(self.parent, key)
+            value = self.walk_back_get_attr(key, inherited)
+            if value is not None:
+                return value
 
-        if required:
+        if required:  # pragma: no cover
             raise MPDParsingError(f"Could not find required attribute {self.__tag__}@{key} ")
 
         return default
 
     def children(
         self,
         cls: Type[TMPDNode],
         minimum: int = 0,
         maximum: Optional[int] = None,
+        **kwargs,
     ) -> List[TMPDNode]:
         children = self.node.findall(cls.__tag__)
         if len(children) < minimum or (maximum and len(children) > maximum):
             raise MPDParsingError(f"Expected to find {self.__tag__}/{cls.__tag__} required [{minimum}..{maximum or 'unbound'})")
 
         return [
-            cls(child, root=self.root, parent=self, i=i, base_url=self.base_url)
+            cls(child, root=self.root, parent=self, i=i, base_url=self.base_url, **kwargs)
             for i, child in enumerate(children)
         ]
 
     def only_child(
         self,
         cls: Type[TMPDNode],
         minimum: int = 0,
+        **kwargs,
     ) -> Optional[TMPDNode]:
-        children = self.children(cls, minimum=minimum, maximum=1)
+        children = self.children(cls, minimum=minimum, maximum=1, **kwargs)
         return children[0] if len(children) else None
 
     def walk_back(
         self,
-        cls: Optional[Type[TMPDNode]] = None,
-        f: Callable[["MPDNode"], "MPDNode"] = _identity,
-    ) -> Iterator[Union[TMPDNode, "MPDNode"]]:
+        cls: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        mapper: Callable[["MPDNode"], Optional["MPDNode"]] = _identity,
+    ) -> Iterator["MPDNode"]:
         node = self.parent
         while node:
-            if cls is None or cls.__tag__ == node.__tag__:
-                yield f(node)
+            if cls is None or isinstance(node, cls):  # type: ignore[arg-type]
+                n = mapper(node)  # type: ignore[arg-type]
+                if n is not None:
+                    yield n
             node = node.parent
 
-    def walk_back_get_attr(self, attr: str) -> Optional[Any]:
-        parent_attrs = [getattr(n, attr) for n in self.walk_back() if hasattr(n, attr)]
-        return parent_attrs[0] if len(parent_attrs) else None
+    def walk_back_get_attr(
+        self,
+        attr: str,
+        cls: Optional[Union[Type[TMPDNode], Sequence[Type[TMPDNode]]]] = None,
+        mapper: Callable[["MPDNode"], Optional["MPDNode"]] = _identity,
+    ) -> Optional[Any]:
+        for ancestor in self.walk_back(cls, mapper):
+            value = getattr(ancestor, attr, None)
+            if value is not None:
+                return value
 
     @property
     def base_url(self):
         base_url = self._base_url
         if hasattr(self, "baseURLs") and len(self.baseURLs):
             base_url = BaseURL.join(base_url, self.baseURLs[0].url)
         return base_url
@@ -256,21 +320,21 @@
 
     Should validate the XML input and provide methods to get segment URLs for each Period, AdaptationSet and Representation.
     """
 
     __tag__ = "MPD"
 
     parent: None  # type: ignore[assignment]
+    timelines: Dict[TTimelineIdent, int]
 
-    def __init__(self, node, url=None, *args, **kwargs):
+    def __init__(self, *args, url: Optional[str] = None, **kwargs) -> None:
         # top level has no parent
-        kwargs.pop("root", None)
-        kwargs.pop("parent", None)
-        # noinspection PyTypeChecker
-        super().__init__(node, root=self, parent=None, *args, **kwargs)
+        kwargs["root"] = self
+        kwargs["parent"] = None
+        super().__init__(*args, **kwargs)
 
         # parser attributes
         self.url = url
         self.timelines = defaultdict(lambda: -1)
         self.timelines.update(kwargs.pop("timelines", {}))
 
         self.id = self.attr("id")
@@ -282,75 +346,89 @@
             "type",
             parser=MPDParsers.type,
             default="static",
         )
         self.minimumUpdatePeriod = self.attr(
             "minimumUpdatePeriod",
             parser=MPDParsers.duration,
-            default=Duration(),
+            default=timedelta(),
         )
-        self.minBufferTime = self.attr(
+        self.minBufferTime: Union[timedelta, Duration] = self.attr(
             "minBufferTime",
             parser=MPDParsers.duration,
             required=True,
         )
         self.timeShiftBufferDepth = self.attr(
             "timeShiftBufferDepth",
             parser=MPDParsers.duration,
         )
         self.availabilityStartTime = self.attr(
             "availabilityStartTime",
             parser=MPDParsers.datetime,
-            default=datetime.datetime.fromtimestamp(0, UTC),  # earliest date
+            default=EPOCH_START,
             required=self.type == "dynamic",
         )
         self.publishTime = self.attr(
             "publishTime",
             parser=MPDParsers.datetime,
             required=self.type == "dynamic",
         )
         self.availabilityEndTime = self.attr(
             "availabilityEndTime",
             parser=MPDParsers.datetime,
         )
         self.mediaPresentationDuration = self.attr(
             "mediaPresentationDuration",
             parser=MPDParsers.duration,
+            default=timedelta(),
         )
         self.suggestedPresentationDelay = self.attr(
             "suggestedPresentationDelay",
             parser=MPDParsers.duration,
+            # if there is no delay, use a delay of 3 seconds
+            # TODO: add a customizable parameter for this
+            default=timedelta(seconds=3),
         )
 
         # parse children
         location = self.children(Location)
         self.location = location[0] if location else None
         if self.location:
-            self.url = self.location.text
+            self.url = self.location.text or ""
             urlp = list(urlparse(self.url))
             if urlp[2]:
                 urlp[2], _ = urlp[2].rsplit("/", 1)
             self._base_url = urlunparse(urlp)
 
         self.baseURLs = self.children(BaseURL)
         self.periods = self.children(Period, minimum=1)
         self.programInformation = self.children(ProgramInformation)
 
+    def get_representation(self, ident: TTimelineIdent) -> Optional["Representation"]:
+        """
+        Find the first Representation instance with a matching ident
+        """
+        for period in self.periods:
+            for adaptationset in period.adaptationSets:
+                for representation in adaptationset.representations:
+                    if representation.ident == ident:
+                        return representation
+
 
 class ProgramInformation(MPDNode):
     __tag__ = "ProgramInformation"
 
 
 class BaseURL(MPDNode):
     __tag__ = "BaseURL"
 
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
-        self.url = self.text.strip()
+        self.url = (self.text or "").strip()
 
     @property
     def is_absolute(self) -> bool:
         return bool(urlparse(self.url).scheme)
 
     @staticmethod
     def join(url: str, other: str) -> str:
@@ -370,522 +448,571 @@
 class Location(MPDNode):
     __tag__ = "Location"
 
 
 class Period(MPDNode):
     __tag__ = "Period"
 
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
         self.i = kwargs.get("i", 0)
         self.id = self.attr("id")
         self.bitstreamSwitching = self.attr(
             "bitstreamSwitching",
             parser=MPDParsers.bool_str,
         )
         self.duration = self.attr(
             "duration",
             parser=MPDParsers.duration,
-            default=Duration(),
+            default=timedelta(),
         )
         self.start = self.attr(
             "start",
             parser=MPDParsers.duration,
-            default=Duration(),
+            default=timedelta(),
         )
 
-        if self.start is None and self.i == 0 and self.root.type == "static":
-            self.start = 0
+        # anchor time for segment availability
+        offset = self.start if self.root.type == "dynamic" else timedelta()
+        self.availabilityStartTime = self.root.availabilityStartTime + offset
 
         # TODO: Early Access Periods
 
         self.baseURLs = self.children(BaseURL)
-        self.segmentBase = self.only_child(SegmentBase)
+        self.segmentBase = self.only_child(SegmentBase, period=self)
+        self.segmentList = self.only_child(SegmentList, period=self)
+        self.segmentTemplate = self.only_child(SegmentTemplate, period=self)
         self.adaptationSets = self.children(AdaptationSet, minimum=1)
-        self.segmentList = self.only_child(SegmentList)
-        self.segmentTemplate = self.only_child(SegmentTemplate)
-        self.sssetIdentifier = self.only_child(AssetIdentifier)
+        self.assetIdentifier = self.only_child(AssetIdentifier)
         self.eventStream = self.children(EventStream)
         self.subset = self.children(Subset)
 
 
-class SegmentBase(MPDNode):
-    __tag__ = "SegmentBase"
-
-
 class AssetIdentifier(MPDNode):
     __tag__ = "AssetIdentifier"
 
 
 class Subset(MPDNode):
     __tag__ = "Subset"
 
 
 class EventStream(MPDNode):
     __tag__ = "EventStream"
 
 
-class Initialization(MPDNode):
-    __tag__ = "Initialization"
-
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+class _RepresentationBaseType(MPDNode):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
-        self.source_url = self.attr("sourceURL")
-        self.range = self.attr(
-            "range",
-            parser=MPDParsers.range,
+        # mimeType must be set on the AdaptationSet or Representation
+        self.mimeType: str = self.attr(  # type: ignore[assignment]
+            "mimeType",
+            required=type(self) is Representation,
+            inherited=_RepresentationBaseType,
         )
 
-
-class SegmentURL(MPDNode):
-    __tag__ = "SegmentURL"
-
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
-
-        self.media = self.attr("media")
-        self.media_range = self.attr(
-            "mediaRange",
-            parser=MPDParsers.range,
+        self.profiles = self.attr(
+            "profiles",
+            inherited=_RepresentationBaseType,
         )
-
-
-class SegmentList(MPDNode):
-    __tag__ = "SegmentList"
-
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
-
-        self.presentation_time_offset = self.attr("presentationTimeOffset")
-        self.timescale = self.attr(
-            "timescale",
+        self.width = self.attr(
+            "width",
             parser=int,
+            inherited=_RepresentationBaseType,
         )
-        self.duration = self.attr(
-            "duration",
+        self.height = self.attr(
+            "height",
             parser=int,
+            inherited=_RepresentationBaseType,
         )
-        self.start_number = self.attr(
-            "startNumber",
+        self.sar = self.attr(
+            "sar",
+            inherited=_RepresentationBaseType,
+        )
+        self.frameRate = self.attr(
+            "frameRate",
+            parser=MPDParsers.frame_rate,
+            inherited=_RepresentationBaseType,
+        )
+        self.audioSamplingRate = self.attr(
+            "audioSamplingRate",
             parser=int,
-            default=1,
+            inherited=_RepresentationBaseType,
+        )
+        self.codecs = self.attr(
+            "codecs",
+            inherited=_RepresentationBaseType,
+        )
+        self.scanType = self.attr(
+            "scanType",
+            inherited=_RepresentationBaseType,
         )
 
-        if self.duration:
-            self.duration_seconds = self.duration / float(self.timescale)
-        else:
-            self.duration_seconds = None
-
-        self.initialization = self.only_child(Initialization)
-        self.segment_urls = self.children(SegmentURL, minimum=1)
-
-    @property
-    def segments(self) -> Iterator[Segment]:
-        if self.initialization:
-            yield Segment(
-                url=self.make_url(self.initialization.source_url),
-                duration=0,
-                init=True,
-                content=False,
-                byterange=self.initialization.range,
-            )
-        for n, segment_url in enumerate(self.segment_urls, self.start_number):
-            yield Segment(
-                url=self.make_url(segment_url.media),
-                duration=self.duration_seconds,
-                byterange=segment_url.media_range,
-            )
-
-    def make_url(self, url: str) -> str:
-        return BaseURL.join(self.base_url, url)
+        self.contentProtections = self.children(ContentProtection)
 
 
-class AdaptationSet(MPDNode):
+class AdaptationSet(_RepresentationBaseType):
     __tag__ = "AdaptationSet"
 
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+    parent: Period
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
         self.id = self.attr("id")
         self.group = self.attr("group")
-        self.mimeType = self.attr("mimeType")
         self.lang = self.attr("lang")
         self.contentType = self.attr("contentType")
         self.par = self.attr("par")
-        self.minBandwidth = self.attr("minBandwidth")
-        self.maxBandwidth = self.attr("maxBandwidth")
-        self.minWidth = self.attr(
-            "minWidth",
-            parser=int,
-        )
-        self.maxWidth = self.attr(
-            "maxWidth",
-            parser=int,
-        )
-        self.minHeight = self.attr(
-            "minHeight",
-            parser=int,
-        )
-        self.maxHeight = self.attr(
-            "maxHeight",
-            parser=int,
-        )
-        self.minFrameRate = self.attr(
-            "minFrameRate",
-            parser=MPDParsers.frame_rate,
-        )
-        self.maxFrameRate = self.attr(
-            "maxFrameRate",
-            parser=MPDParsers.frame_rate,
-        )
+        self.minBandwidth = self.attr("minBandwidth", parser=int)
+        self.maxBandwidth = self.attr("maxBandwidth", parser=int)
+        self.minWidth = self.attr("minWidth", parser=int)
+        self.maxWidth = self.attr("maxWidth", parser=int)
+        self.minHeight = self.attr("minHeight", parser=int)
+        self.maxHeight = self.attr("maxHeight", parser=int)
+        self.minFrameRate = self.attr("minFrameRate", parser=MPDParsers.frame_rate)
+        self.maxFrameRate = self.attr("maxFrameRate", parser=MPDParsers.frame_rate)
         self.segmentAlignment = self.attr(
             "segmentAlignment",
             parser=MPDParsers.bool_str,
             default=False,
         )
-        self.bitstreamSwitching = self.attr(
-            "bitstreamSwitching",
-            parser=MPDParsers.bool_str,
-        )
         self.subsegmentAlignment = self.attr(
             "subsegmentAlignment",
             parser=MPDParsers.bool_str,
             default=False,
         )
         self.subsegmentStartsWithSAP = self.attr(
             "subsegmentStartsWithSAP",
             parser=int,
             default=0,
         )
+        self.bitstreamSwitching = self.attr(
+            "bitstreamSwitching",
+            parser=MPDParsers.bool_str,
+        )
 
         self.baseURLs = self.children(BaseURL)
-        self.segmentTemplate = self.only_child(SegmentTemplate)
-        self.representations = self.children(Representation, minimum=1)
-        self.contentProtection = self.children(ContentProtection)
+        self.segmentBase = self.only_child(SegmentBase, period=self.parent)
+        self.segmentList = self.only_child(SegmentList, period=self.parent)
+        self.segmentTemplate = self.only_child(SegmentTemplate, period=self.parent)
+        self.representations = self.children(Representation, minimum=1, period=self.parent)
 
 
-class SegmentTemplate(MPDNode):
-    __tag__ = "SegmentTemplate"
+class Representation(_RepresentationBaseType):
+    __tag__ = "Representation"
 
-    parent: Union["AdaptationSet", "Representation"]
+    parent: AdaptationSet
 
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+    def __init__(self, *args, period: Period, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
-        self.defaultSegmentTemplate = self.walk_back_get_attr("segmentTemplate")
+        self.period = period
 
-        self.initialization = self.attr(
-            "initialization",
-            parser=MPDParsers.segment_template,
+        self.id: str = self.attr(  # type: ignore[assignment]
+            "id",
+            required=True,
         )
-        self.media = self.attr(
-            "media",
-            parser=MPDParsers.segment_template,
+        self.bandwidth: float = self.attr(  # type: ignore[assignment]
+            "bandwidth",
+            parser=lambda b: float(b) / 1000.0,
+            required=True,
         )
-        self.duration = self.attr(
-            "duration",
+
+        self.ident = self.parent.parent.id, self.parent.id, self.id
+
+        self.baseURLs = self.children(BaseURL)
+        self.subRepresentations = self.children(SubRepresentation)
+        self.segmentBase = self.only_child(SegmentBase, period=self.period)
+        self.segmentList = self.only_child(SegmentList, period=self.period)
+        self.segmentTemplate = self.only_child(SegmentTemplate, period=self.period)
+
+    @property
+    def lang(self):
+        return self.parent.lang
+
+    @property
+    def bandwidth_rounded(self) -> float:
+        return round(self.bandwidth, 1 - int(math.log10(self.bandwidth)))
+
+    def segments(self, timestamp: Optional[datetime] = None, **kwargs) -> Iterator[Segment]:
+        """
+        Segments are yielded when they are available
+
+        Segments appear on a timeline, for dynamic content they are only available at a certain time
+        and sometimes for a limited time. For static content they are all available at the same time.
+
+        :param timestamp: Optional initial timestamp for syncing timelines of multiple substreams
+        :param kwargs: extra args to pass to the segment template
+        :return: yields Segments
+        """
+
+        # segmentBase = self.segmentBase or self.walk_back_get_attr("segmentBase")
+        segmentList = self.segmentList or self.walk_back_get_attr("segmentList")
+        segmentTemplate = self.segmentTemplate or self.walk_back_get_attr("segmentTemplate")
+
+        if segmentTemplate:
+            yield from segmentTemplate.segments(
+                self.ident,
+                self.base_url,
+                timestamp=timestamp,
+                RepresentationID=self.id,
+                Bandwidth=int(self.bandwidth * 1000),
+                **kwargs,
+            )
+        elif segmentList:
+            yield from segmentList.segments()
+        else:
+            yield Segment(
+                url=self.base_url,
+                number=None,
+                duration=self.period.duration.total_seconds() or self.root.mediaPresentationDuration.total_seconds(),
+                available_at=self.period.availabilityStartTime,
+                init=True,
+                content=True,
+                byterange=None,
+            )
+
+
+class SubRepresentation(_RepresentationBaseType):
+    __tag__ = "SubRepresentation"
+
+
+class _SegmentBaseType(MPDNode):
+    parent: Union[Period, AdaptationSet, Representation]
+
+    _ancestors = (Period, AdaptationSet, Representation)
+
+    def __init__(self, *args, period: "Period", **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+        self.period = period
+
+        self.timescale: int = self.attr(
+            "timescale",
             parser=int,
-            default=self.defaultSegmentTemplate.duration if self.defaultSegmentTemplate else None,
+            default=self._find_default("timescale", 1),
         )
-        self.timescale = self.attr(
-            "timescale",
+        self.presentationTimeOffset: timedelta = self.attr(
+            "presentationTimeOffset",
+            parser=MPDParsers.timedelta(self.timescale),
+            default=self._find_default("presentationTimeOffset", timedelta()),
+        )
+        self.availabilityTimeOffset: timedelta = self.attr(
+            "availabilityTimeOffset",
+            parser=MPDParsers.timedelta(self.timescale),
+            default=self._find_default("availabilityTimeOffset", timedelta()),
+        )
+
+        self.initialization = self.only_child(Initialization) or self._find_default("initialization")
+
+    def _find_default(self, attr: str, default: TAttrDefault = None) -> Union[TAttrDefault, Any]:
+        """Find default values from nodes of the same type on ancestor nodes"""
+        # the node attribute on each ancestor is named after its node tag, with the first character being lowercase
+        nodeattr = f"{self.__tag__[0].lower()}{self.__tag__[1:]}"
+        # start with the parent node, to avoid an unnecessary failed lookup on the current node
+        value = self.parent.walk_back_get_attr(
+            attr,
+            self._ancestors,
+            lambda node: getattr(node, nodeattr, None),
+        )
+        return default if value is None else value
+
+
+class _MultipleSegmentBaseType(_SegmentBaseType):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+        self.duration = self.attr(
+            "duration",
             parser=int,
-            default=self.defaultSegmentTemplate.timescale if self.defaultSegmentTemplate else 1,
+            default=self._find_default("duration"),
         )
-        self.startNumber = self.attr(
+        self.startNumber: int = self.attr(
             "startNumber",
             parser=int,
-            default=self.defaultSegmentTemplate.startNumber if self.defaultSegmentTemplate else 1,
-        )
-        self.presentationTimeOffset = self.attr(
-            "presentationTimeOffset",
-            parser=MPDParsers.timedelta(self.timescale),
+            default=self._find_default("startNumber", 1),
         )
 
-        if self.duration:
-            self.duration_seconds = self.duration / float(self.timescale)
-        else:
-            self.duration_seconds = None
+        self.duration_seconds = self.duration / self.timescale if self.duration else None
+
+        self.segmentTimeline = self.only_child(SegmentTimeline) or self._find_default("segmentTimeline")
 
-        self.period = list(self.walk_back(Period))[0]
 
-        # children
-        self.segmentTimeline = self.only_child(SegmentTimeline)
+class SegmentBase(_SegmentBaseType):
+    __tag__ = "SegmentBase"
+
+
+class SegmentList(_MultipleSegmentBaseType):
+    __tag__ = "SegmentList"
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+        self.segmentURLs = self.children(SegmentURL)
+
+    def segments(self) -> Iterator[Segment]:
+        if self.initialization:  # pragma: no branch
+            yield Segment(
+                url=self.make_url(self.initialization.source_url),
+                number=None,
+                duration=None,
+                available_at=self.period.availabilityStartTime,
+                init=True,
+                content=False,
+                byterange=self.initialization.range,
+            )
+        for number, segment_url in enumerate(self.segmentURLs, self.startNumber):
+            yield Segment(
+                url=self.make_url(segment_url.media),
+                number=number,
+                duration=self.duration_seconds,
+                available_at=self.period.availabilityStartTime,
+                init=False,
+                content=True,
+                byterange=segment_url.media_range,
+            )
+
+    def make_url(self, url: Optional[str]) -> str:
+        return BaseURL.join(self.base_url, url) if url else self.base_url
 
-    def segments(self, base_url: str, **kwargs) -> Iterator[Segment]:
-        if kwargs.pop("init", True):
+
+class SegmentTemplate(_MultipleSegmentBaseType):
+    __tag__ = "SegmentTemplate"
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+        self.fmt_initialization = self.attr(
+            "initialization",
+            parser=MPDParsers.segment_template,
+        )
+        self.fmt_media = self.attr(
+            "media",
+            parser=MPDParsers.segment_template,
+        )
+
+    def segments(
+        self,
+        ident: TTimelineIdent,
+        base_url: str,
+        timestamp: Optional[datetime] = None,
+        **kwargs,
+    ) -> Iterator[Segment]:
+        if kwargs.pop("init", True):  # pragma: no branch
             init_url = self.format_initialization(base_url, **kwargs)
-            if init_url:
+            if init_url:  # pragma: no branch
                 yield Segment(
                     url=init_url,
-                    duration=0,
+                    number=None,
+                    duration=None,
+                    available_at=self.period.availabilityStartTime,
                     init=True,
                     content=False,
+                    byterange=None,
                 )
-        for media_url, available_at in self.format_media(base_url, **kwargs):
+        for media_url, number, available_at in self.format_media(ident, base_url, timestamp=timestamp, **kwargs):
             yield Segment(
                 url=media_url,
+                number=number,
                 duration=self.duration_seconds,
+                available_at=available_at,
                 init=False,
                 content=True,
-                available_at=available_at,
+                byterange=None,
             )
 
     @staticmethod
     def make_url(base_url: str, url: str) -> str:
         return BaseURL.join(base_url, url)
 
-    def format_initialization(self, base_url: str, **kwargs) -> Optional[str]:
-        if self.initialization:
-            return self.make_url(base_url, self.initialization(**kwargs))
-
-    def segment_numbers(self) -> Iterator[Tuple[int, datetime.datetime]]:
+    def segment_numbers(self, timestamp: Optional[datetime] = None) -> Iterator[Tuple[int, datetime]]:
         """
         yield the segment number and when it will be available.
 
         There are two cases for segment number generation, "static" and "dynamic":
 
         In the case of static streams, the segment number starts at the startNumber and counts
         up to the number of segments that are represented by the periods-duration.
 
         In the case of dynamic streams, the segments should appear at the specified time.
         In the simplest case, the segment number is based on the time since the availabilityStartTime.
         """
 
-        log.debug(f"Generating segment numbers for {self.root.type} playlist (id={self.parent.id})")
+        if not self.duration_seconds:  # pragma: no cover
+            raise MPDParsingError("Unknown segment durations: missing duration/timescale attributes on SegmentTemplate")
+
         number_iter: Union[Iterator[int], Sequence[int]]
-        available_iter: Iterator[datetime.datetime]
+        available_iter: Iterator[datetime]
 
         if self.root.type == "static":
-            available_iter = repeat(EPOCH_START)
-            duration = self.period.duration.seconds or self.root.mediaPresentationDuration.seconds
+            available_iter = repeat(self.period.availabilityStartTime)
+            duration = self.period.duration.total_seconds() or self.root.mediaPresentationDuration.total_seconds()
             if duration:
                 number_iter = range(self.startNumber, int(duration / self.duration_seconds) + 1)
             else:
                 number_iter = count(self.startNumber)
         else:
-            now = datetime.datetime.now(UTC)
-            if self.presentationTimeOffset:
-                since_start = (now - self.presentationTimeOffset) - self.root.availabilityStartTime
-                available_start_date = self.root.availabilityStartTime + self.presentationTimeOffset + since_start
-                available_start = available_start_date
-            else:
-                since_start = now - self.root.availabilityStartTime
-                available_start = now
+            current_time = timestamp or now()
+            since_start = current_time - self.period.availabilityStartTime - self.presentationTimeOffset
 
-            # if there is no delay, use a delay of 3 seconds
-            seconds = self.root.suggestedPresentationDelay.total_seconds() if self.root.suggestedPresentationDelay else 3
-            suggested_delay = datetime.timedelta(seconds=seconds)
+            suggested_delay = self.root.suggestedPresentationDelay
+            buffer_time = self.root.minBufferTime
 
-            # the number of the segment that is available at NOW - SUGGESTED_DELAY - BUFFER_TIME
-            number_offset = int(
-                (since_start - suggested_delay - self.root.minBufferTime).total_seconds()
-                / self.duration_seconds,
-            )
+            # Segment number
+            seconds_offset = (since_start - suggested_delay - buffer_time).total_seconds()
+            number_offset = max(0, int(seconds_offset / self.duration_seconds))
             number_iter = count(self.startNumber + number_offset)
 
-            # the time the segment number is available at NOW
+            # Segment availability time
+            available_offset = timedelta(seconds=number_offset * self.duration_seconds)
+            available_start = self.period.availabilityStartTime + available_offset
             available_iter = count_dt(
                 available_start,
-                datetime.timedelta(seconds=self.duration_seconds),
+                timedelta(seconds=self.duration_seconds),
             )
 
+            log.debug(f"Stream start: {self.period.availabilityStartTime}")
+            log.debug(f"Current time: {current_time}")
+            log.debug(f"Availability: {available_start}")
+            log.debug("; ".join([
+                f"presentationTimeOffset: {self.presentationTimeOffset}",
+                f"suggestedPresentationDelay: {self.root.suggestedPresentationDelay}",
+                f"minBufferTime: {self.root.minBufferTime}",
+            ]))
+            log.debug("; ".join([
+                f"segmentDuration: {self.duration_seconds}",
+                f"segmentStart: {self.startNumber}",
+                f"segmentOffset: {number_offset} ({seconds_offset}s)",
+            ]))
+
         yield from zip(number_iter, available_iter)
 
-    def format_media(self, base_url: str, **kwargs) -> Iterator[Tuple[str, datetime.datetime]]:
-        if not self.segmentTimeline:
-            for number, available_at in self.segment_numbers():
-                url = self.make_url(base_url, self.media(Number=number, **kwargs))
-                yield url, available_at
-            return
+    def segment_timeline(self, ident: TTimelineIdent) -> Iterator[Tuple[int, TimelineSegment, datetime]]:
+        if not self.segmentTimeline:  # pragma: no cover
+            raise MPDParsingError("Missing SegmentTimeline in SegmentTemplate")
 
-        if self.parent.id is None:
-            # workaround for invalid `self.root.timelines[self.parent.id]`
-            # creates a timeline for every mimeType instead of one for both
-            self.parent.id = self.parent.mimeType
+        if self.root.type == "static":
+            yield from zip(count(self.startNumber), self.segmentTimeline.segments, repeat(self.period.availabilityStartTime))
+        else:
+            time = self.root.timelines[ident]
+            is_initial = time == -1
 
-        log.debug(f"Generating segment timeline for {self.root.type} playlist (id={self.parent.id}))")
+            publish_time = self.root.publishTime or EPOCH_START
+            threshold = publish_time - self.root.suggestedPresentationDelay
 
-        if self.root.type == "static":
-            for segment, n in zip(self.segmentTimeline.segments, count(self.startNumber)):
-                url = self.make_url(base_url, self.media(Time=segment.t, Number=n, **kwargs))
-                available_at = datetime.datetime.now(tz=UTC)  # TODO: replace with EPOCH_START ?!
-                yield url, available_at
-            return
+            # transform the timeline into a segment list
+            timeline = []
+            available_at = publish_time
 
-        # if there is no delay, use a delay of 3 seconds
-        seconds = self.root.suggestedPresentationDelay.total_seconds() if self.root.suggestedPresentationDelay else 3
-        suggested_delay = datetime.timedelta(seconds=seconds)
-        publish_time = self.root.publishTime or EPOCH_START
-
-        # transform the timeline into a segment list
-        timeline = []
-        available_at = publish_time
-        for segment, n in reversed(list(zip(self.segmentTimeline.segments, count(self.startNumber)))):
             # the last segment in the timeline is the most recent one
             # so, work backwards and calculate when each of the segments was
             # available, based on the durations relative to the publish-time
-            url = self.make_url(base_url, self.media(Time=segment.t, Number=n, **kwargs))
-            duration = datetime.timedelta(seconds=segment.d / self.timescale)
-
-            # once the suggested_delay is reach stop
-            if self.root.timelines[self.parent.id] == -1 and publish_time - available_at >= suggested_delay:
-                break
-
-            timeline.append((url, available_at, segment.t))
-
-            available_at -= duration  # walk backwards in time
-
-        # return the segments in chronological order
-        for url, available_at, t in reversed(timeline):
-            if t > self.root.timelines[self.parent.id]:
-                self.root.timelines[self.parent.id] = t
-                yield url, available_at
-
+            for number, segment in reversed(list(zip(count(self.startNumber), self.segmentTimeline.segments))):
+                # stop once the suggestedPresentationDelay is reached on the first manifest parsing
+                # or when a segment with a lower or equal time value was already returned from an earlier manifest
+                if is_initial and available_at <= threshold or segment.t <= time:
+                    break
+
+                timeline.append((number, segment, available_at))
+                available_at -= timedelta(seconds=segment.d / self.timescale)
+
+            # return the segments in chronological order
+            for number, segment, available_at in reversed(timeline):
+                self.root.timelines[ident] = segment.t
+                yield number, segment, available_at
 
-class Representation(MPDNode):
-    __tag__ = "Representation"
-
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
-
-        self.id = self.attr(
-            "id",
-            required=True,
-        )
-        self.bandwidth = self.attr(
-            "bandwidth",
-            parser=lambda b: float(b) / 1000.0,
-            required=True,
-        )
-        self.mimeType = self.attr(
-            "mimeType",
-            required=True,
-            inherited=True,
-        )
-
-        self.codecs = self.attr("codecs")
-        self.startWithSAP = self.attr("startWithSAP")
-
-        # video
-        self.width = self.attr(
-            "width",
-            parser=int,
-        )
-        self.height = self.attr(
-            "height",
-            parser=int,
-        )
-        self.frameRate = self.attr(
-            "frameRate",
-            parser=MPDParsers.frame_rate,
-        )
-
-        # audio
-        self.audioSamplingRate = self.attr(
-            "audioSamplingRate",
-            parser=int,
-        )
-        self.numChannels = self.attr(
-            "numChannels",
-            parser=int,
-        )
-
-        # subtitle
-        self.lang = self.attr(
-            "lang",
-            inherited=True,
-        )
-
-        self.baseURLs = self.children(BaseURL)
-        self.subRepresentation = self.children(SubRepresentation)
-        self.segmentBase = self.only_child(SegmentBase)
-        self.segmentList = self.children(SegmentList)
-        self.segmentTemplate = self.only_child(SegmentTemplate)
-        self.contentProtection = self.children(ContentProtection)
-
-    @property
-    def bandwidth_rounded(self) -> float:
-        return round(self.bandwidth, 1 - int(math.log10(self.bandwidth)))
-
-    def segments(self, **kwargs) -> Iterator[Segment]:
-        """
-        Segments are yielded when they are available
-
-        Segments appear on a timeline, for dynamic content they are only available at a certain time
-        and sometimes for a limited time. For static content they are all available at the same time.
-
-        :param kwargs: extra args to pass to the segment template
-        :return: yields Segments
-        """
+    def format_initialization(self, base_url: str, **kwargs) -> Optional[str]:
+        if self.fmt_initialization is not None:  # pragma: no branch
+            return self.make_url(base_url, self.fmt_initialization(**kwargs))
 
-        # segmentBase = self.segmentBase or self.walk_back_get_attr("segmentBase")
-        segmentLists = self.segmentList or self.walk_back_get_attr("segmentList")
-        segmentTemplate = self.segmentTemplate or self.walk_back_get_attr("segmentTemplate")
+    def format_media(
+        self,
+        ident: TTimelineIdent,
+        base_url: str,
+        timestamp: Optional[datetime] = None,
+        **kwargs,
+    ) -> Iterator[Tuple[str, int, datetime]]:
+        if self.fmt_media is None:  # pragma: no cover
+            return
 
-        if segmentTemplate:
-            yield from segmentTemplate.segments(
-                self.base_url,
-                RepresentationID=self.id,
-                Bandwidth=int(self.bandwidth * 1000),
-                **kwargs,
-            )
-        elif segmentLists:
-            for segmentList in segmentLists:
-                yield from segmentList.segments
+        if not self.segmentTimeline:
+            log.debug(f"Generating segment numbers for {self.root.type} playlist: {ident!r}")
+            for number, available_at in self.segment_numbers(timestamp=timestamp):
+                url = self.make_url(base_url, self.fmt_media(Number=number, **kwargs))
+                yield url, number, available_at
         else:
-            yield Segment(
-                url=self.base_url,
-                duration=0,
-                init=True,
-                content=True,
-            )
-
-
-class SubRepresentation(MPDNode):
-    __tag__ = "SubRepresentation"
+            log.debug(f"Generating segment timeline for {self.root.type} playlist: {ident!r}")
+            for number, segment, available_at in self.segment_timeline(ident):
+                url = self.make_url(base_url, self.fmt_media(Time=segment.t, Number=number, **kwargs))
+                yield url, number, available_at
 
 
 class SegmentTimeline(MPDNode):
     __tag__ = "SegmentTimeline"
 
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
         self.timescale = self.walk_back_get_attr("timescale")
 
         self.timeline_segments = self.children(_TimelineSegment)
 
     @property
     def segments(self) -> Iterator[TimelineSegment]:
         t = 0
         for tsegment in self.timeline_segments:
             if t == 0 and tsegment.t is not None:
                 t = tsegment.t
             # check the start time from MPD
-            for repeated_i in range(tsegment.r + 1):
+            for _ in range(tsegment.r + 1):
                 yield TimelineSegment(t, tsegment.d)
                 t += tsegment.d
 
 
 class _TimelineSegment(MPDNode):
     __tag__ = "S"
 
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
         self.t = self.attr("t", parser=int)
-        self.d = self.attr("d", parser=int)
+        self.d: int = self.attr("d", parser=int, required=True)  # type: ignore[assignment]
         self.r = self.attr("r", parser=int, default=0)
 
 
+class Initialization(MPDNode):
+    __tag__ = "Initialization"
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+        self.source_url = self.attr("sourceURL")
+        self.range = self.attr(
+            "range",
+            parser=MPDParsers.range,
+        )
+
+
+class SegmentURL(MPDNode):
+    __tag__ = "SegmentURL"
+
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+
+        self.media = self.attr("media")
+        self.media_range = self.attr(
+            "mediaRange",
+            parser=MPDParsers.range,
+        )
+
+
 class ContentProtection(MPDNode):
     __tag__ = "ContentProtection"
 
-    def __init__(self, node, root=None, parent=None, *args, **kwargs):
-        super().__init__(node, root, parent, *args, **kwargs)
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
 
         self.schemeIdUri = self.attr("schemeIdUri")
         self.value = self.attr("value")
         self.default_KID = self.attr("default_KID")
```

### Comparing `streamlink-5.3.1/src/streamlink/stream/ffmpegmux.py` & `streamlink-5.4.0/src/streamlink/stream/ffmpegmux.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,59 +4,62 @@
 import subprocess
 import sys
 import threading
 from contextlib import suppress
 from functools import lru_cache
 from pathlib import Path
 from shutil import which
-from typing import List, Optional, TextIO, Union
+from typing import Any, Dict, Generic, List, Optional, Sequence, TextIO, TypeVar, Union
 
 from streamlink import StreamError
 from streamlink.stream.stream import Stream, StreamIO
 from streamlink.utils.named_pipe import NamedPipe, NamedPipeBase
 from streamlink.utils.processoutput import ProcessOutput
 
 
 log = logging.getLogger(__name__)
 
 _lock_resolve_command = threading.Lock()
 
 
-class MuxedStream(Stream):
+TSubstreams = TypeVar("TSubstreams", bound=Stream)
+
+
+class MuxedStream(Stream, Generic[TSubstreams]):
     """
     Muxes multiple streams into one output stream.
     """
 
     __shortname__ = "muxed-stream"
 
     def __init__(
         self,
         session,
-        *substreams: Stream,
+        *substreams: TSubstreams,
         **options,
     ):
         """
         :param streamlink.Streamlink session: Streamlink session instance
         :param substreams: Video and/or audio streams
         :param options: Additional keyword arguments passed to :class:`ffmpegmux.FFMPEGMuxer`.
                         Subtitle streams need to be set via the ``subtitles`` keyword.
         """
 
         super().__init__(session)
-        self.substreams = substreams
-        self.subtitles = options.pop("subtitles", {})
-        self.options = options
+        self.substreams: Sequence[TSubstreams] = substreams
+        self.subtitles: Dict[str, Stream] = options.pop("subtitles", {})
+        self.options: Dict[str, Any] = options
 
     def open(self):
         fds = []
         metadata = self.options.get("metadata", {})
         maps = self.options.get("maps", [])
         # only update the maps values if they haven't been set
         update_maps = not maps
-        for i, substream in enumerate(self.substreams):
+        for substream in self.substreams:
             log.debug("Opening {0} substream".format(substream.shortname()))
             if update_maps:
                 maps.append(len(fds))
             fds.append(substream and substream.open())
 
         for i, subtitle in enumerate(self.subtitles.items()):
             language, substream = subtitle
```

### Comparing `streamlink-5.3.1/src/streamlink/stream/file.py` & `streamlink-5.4.0/src/streamlink/stream/file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/stream/filtered.py` & `streamlink-5.4.0/src/streamlink/stream/filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/stream/hls.py` & `streamlink-5.4.0/src/streamlink/stream/hls.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # noinspection PyPackageRequirements
 from Crypto.Cipher import AES
 
 # noinspection PyPackageRequirements
 from Crypto.Util.Padding import unpad
 from requests import Response
-from requests.exceptions import ChunkedEncodingError, ConnectionError, ContentDecodingError
+from requests.exceptions import ChunkedEncodingError, ConnectionError, ContentDecodingError, InvalidSchema
 
 from streamlink.buffers import RingBuffer
 from streamlink.exceptions import StreamError
 from streamlink.stream.ffmpegmux import FFMPEGMuxer, MuxedStream
 from streamlink.stream.filtered import FilteredStream
 from streamlink.stream.hls_playlist import M3U8, ByteRange, Key, Map, Media, Segment, load as load_hls_playlist
 from streamlink.stream.http import HTTPStream
@@ -108,20 +108,28 @@
                 "netloc": lambda: p.netloc,
                 "path": lambda: p.path,
                 "query": lambda: p.query,
             })
             key_uri = formatter.format(self.key_uri_override)
 
         if key_uri and self.key_uri != key_uri:
-            res = self.session.http.get(
-                key_uri,
-                exception=StreamError,
-                retries=self.retries,
-                **self.reader.request_params,
-            )
+            try:
+                res = self.session.http.get(
+                    key_uri,
+                    exception=StreamError,
+                    retries=self.retries,
+                    **self.reader.request_params,
+                )
+            except StreamError as err:
+                # FIXME: fix HTTPSession.request()
+                original_error = getattr(err, "err", None)
+                if isinstance(original_error, InvalidSchema):
+                    raise StreamError(f"Unable to find connection adapter for key URI: {key_uri}") from original_error
+                raise  # pragma: no cover
+
             res.encoding = "binary/octet-stream"
             self.key_data = res.content
             self.key_uri = key_uri
 
         iv = key.iv or self.num_to_iv(num)
 
         # Pad IV if needed
@@ -326,15 +334,15 @@
 
         log.debug("Reloading playlist")
         res = self._fetch_playlist()
 
         try:
             playlist = self._reload_playlist(res)
         except ValueError as err:
-            raise StreamError(err)
+            raise StreamError(err) from err
 
         if playlist.is_master:
             raise StreamError(f"Attempted to play a variant playlist, use 'hls://{self.stream.url}' instead")
 
         if playlist.iframes_only:
             raise StreamError("Streams containing I-frames only are not playable")
 
@@ -439,15 +447,15 @@
                 yield sequence
                 total_duration += sequence.segment.duration
                 if self.duration_limit and total_duration >= self.duration_limit:
                     log.info(f"Stopping stream early after {self.duration_limit}")
                     return
 
                 # End of stream
-                stream_end = self.playlist_end and sequence.num >= self.playlist_end
+                stream_end = self.playlist_end is not None and sequence.num >= self.playlist_end
                 if self.closed or stream_end:
                     return
 
                 self.playlist_sequence = sequence.num + 1
 
             if self.wait(self.playlist_reload_time):
                 try:
@@ -472,15 +480,15 @@
         self.request_params.pop("stream", None)
         self.request_params.pop("timeout", None)
         self.request_params.pop("url", None)
 
         super().__init__(stream)
 
 
-class MuxedHLSStream(MuxedStream):
+class MuxedHLSStream(MuxedStream["HLSStream"]):
     """
     Muxes multiple HLS video and audio streams into one output stream.
     """
 
     __shortname__ = "hls-multi"
 
     def __init__(
@@ -652,15 +660,15 @@
         audio_select = session_.options.get("hls-audio-select")
 
         res = cls._fetch_variant_playlist(session_, url, **request_params)
 
         try:
             multivariant = cls._get_variant_playlist(res)
         except ValueError as err:
-            raise OSError(f"Failed to parse playlist: {err}")
+            raise OSError(f"Failed to parse playlist: {err}") from err
 
         stream_name: Optional[str]
         stream: Union["HLSStream", "MuxedHLSStream"]
         streams: Dict[str, Union["HLSStream", "MuxedHLSStream"]] = {}
 
         for playlist in filter(lambda p: not p.is_iframe, multivariant.playlists):
             names: Dict[str, Optional[str]] = dict(name=None, pixels=None, bitrate=None)
```

### Comparing `streamlink-5.3.1/src/streamlink/stream/hls_playlist.py` & `streamlink-5.4.0/src/streamlink/stream/hls_playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         self._add_tag_callbacks()
 
     def _add_tag_callbacks(self):
         # ignore previously generated tag-callback mapping on parent classes when initializing subclasses
         if "_TAGS" in self.__class__.__dict__:
             return
         tags = {}
-        setattr(self.__class__, "_TAGS", tags)
+        self.__class__._TAGS = tags
         for name, method in inspect.getmembers(self.__class__, inspect.isfunction):
             if not name.startswith("parse_tag_"):
                 continue
             tag = name[10:].upper().replace("_", "-")
             tags[tag] = method
 
     @classmethod
```

### Comparing `streamlink-5.3.1/src/streamlink/stream/http.py` & `streamlink-5.4.0/src/streamlink/stream/http.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/stream/segmented.py` & `streamlink-5.4.0/src/streamlink/stream/segmented.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,17 +134,18 @@
         """Shuts down the thread, its executor and closes the reader (worker thread and buffer)."""
         if self.closed:  # pragma: no cover
             return
 
         log.debug("Closing writer thread")
 
         self.closed = True
+        self._wait.set()
+
         self.reader.close()
         self.executor.shutdown(wait=True, cancel_futures=True)
-        self._wait.set()
 
     def put(self, segment):
         """Adds a segment to the download pool and write queue."""
         if self.closed:  # pragma: no cover
             return
 
         if segment is None:
```

### Comparing `streamlink-5.3.1/src/streamlink/stream/stream.py` & `streamlink-5.4.0/src/streamlink/stream/stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/stream/wrappers.py` & `streamlink-5.4.0/src/streamlink/stream/wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/user_input.py` & `streamlink-5.4.0/src/streamlink/user_input.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/utils/__init__.py` & `streamlink-5.4.0/src/streamlink/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/utils/args.py` & `streamlink-5.4.0/src/streamlink/utils/args.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import re
+from typing import Optional, Type
 
 
 _filesize_re = re.compile(r"""
     (?P<size>\d+(\.\d+)?)
     (?P<modifier>[Kk]|[Mm])?
     (?:[Bb])?
 """, re.VERBOSE)
@@ -43,48 +44,52 @@
 
     modifier = match.group("modifier")
     if modifier in ("M", "m"):
         size *= 1024 * 1024
     elif modifier in ("K", "k"):
         size *= 1024
 
-    return num(int, min=0)(size)
+    return num(int, ge=1)(size)
 
 
 def keyvalue(value):
     match = _keyvalue_re.match(value)
     if not match:
         raise ValueError
 
     return match.group("key", "value")
 
 
-# noinspection PyShadowingBuiltins
-def num(type, min=None, max=None):  # noqa: A002
+def num(
+    numtype: Type[float],
+    ge: Optional[float] = None,
+    gt: Optional[float] = None,
+    le: Optional[float] = None,
+    lt: Optional[float] = None,
+):
     def func(value):
-        value = type(value)
+        value = numtype(value)
 
-        if min is not None and not (value > min):
-            raise argparse.ArgumentTypeError(
-                "{0} value must be more than {1} but is {2}".format(
-                    type.__name__, min, value,
-                ),
-            )
-
-        if max is not None and not (value <= max):
-            raise argparse.ArgumentTypeError(
-                "{0} value must be at most {1} but is {2}".format(
-                    type.__name__, max, value,
-                ),
-            )
+        if ge is not None and value < ge:
+            raise argparse.ArgumentTypeError(f"{numtype.__name__} value must be >={ge}, but is {value}")
+        if gt is not None and value <= gt:
+            raise argparse.ArgumentTypeError(f"{numtype.__name__} value must be >{gt}, but is {value}")
+        if le is not None and value > le:
+            raise argparse.ArgumentTypeError(f"{numtype.__name__} value must be <={le}, but is {value}")
+        if lt is not None and value >= lt:
+            raise argparse.ArgumentTypeError(f"{numtype.__name__} value must be <{lt}, but is {value}")
 
         return value
 
-    func.__name__ = type.__name__
+    func.__name__ = numtype.__name__
 
     return func
 
 
 __all__ = [
-    "boolean", "comma_list", "comma_list_filter", "filesize", "keyvalue",
+    "boolean",
+    "comma_list",
+    "comma_list_filter",
+    "filesize",
+    "keyvalue",
     "num",
 ]
```

### Comparing `streamlink-5.3.1/src/streamlink/utils/cache.py` & `streamlink-5.4.0/src/streamlink/utils/cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/utils/crypto.py` & `streamlink-5.4.0/src/streamlink/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/utils/data.py` & `streamlink-5.4.0/src/streamlink/utils/data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/utils/formatter.py` & `streamlink-5.4.0/src/streamlink/utils/formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 return f"{{{field_name}:{format_spec}}}"
 
         return value
 
     def _format(self, string: str, mapper: Callable[[str], str], defaults: Dict[str, str]) -> str:
         result = []
 
-        for literal_text, field_name, format_spec, conversion in _stringformatter.parse(string):
+        for literal_text, field_name, format_spec, _conversion in _stringformatter.parse(string):
             if literal_text:
                 result.append(literal_text)
 
             if field_name is None:
                 continue
 
             value = self._get_value(field_name, format_spec, defaults)
```

### Comparing `streamlink-5.3.1/src/streamlink/utils/l10n.py` & `streamlink-5.4.0/src/streamlink/utils/l10n.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
             return Country(
                 c.alpha_2,
                 c.alpha_3,
                 c.numeric,
                 c.name,
                 getattr(c, "official_name", c.name),
             )
-        except (LookupError, KeyError):
-            raise LookupError(f"Invalid country code: {country}")
+        except LookupError as err:
+            raise LookupError(f"Invalid country code: {country}") from err
 
     def __eq__(self, other):
         return (
             (self.alpha2 and self.alpha2 == other.alpha2)
             or (self.alpha3 and self.alpha3 == other.alpha3)
             or (self.numeric and self.numeric == other.numeric)
         )
@@ -72,16 +72,16 @@
             return Language(
                 # some languages don't have an alpha_2 code
                 getattr(lang, "alpha_2", ""),
                 lang.alpha_3,
                 lang.name,
                 getattr(lang, "bibliographic", ""),
             )
-        except (LookupError, KeyError):
-            raise LookupError(f"Invalid language code: {language}")
+        except LookupError as err:
+            raise LookupError(f"Invalid language code: {language}") from err
 
     def __eq__(self, other):
         return (
             (self.alpha2 and self.alpha2 == other.alpha2)
             or (self.alpha3 and self.alpha3 == other.alpha3)
             or (self.bibliographic and self.bibliographic == other.bibliographic)
         )
```

### Comparing `streamlink-5.3.1/src/streamlink/utils/named_pipe.py` & `streamlink-5.4.0/src/streamlink/utils/named_pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 _id = 0
 
 
 class NamedPipeBase(abc.ABC):
     path: Path
 
     def __init__(self):
-        global _id
+        global _id  # noqa: PLW0603
         with _lock:
             _id += 1
             self.name = f"streamlinkpipe-{os.getpid()}-{_id}-{random.randint(0, 9999)}"
         log.info(f"Creating pipe {self.name}")
         self._create()
 
     @abc.abstractmethod
```

### Comparing `streamlink-5.3.1/src/streamlink/utils/parse.py` & `streamlink-5.4.0/src/streamlink/utils/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     try:
         parsed = parser(data, *args, **kwargs)
     except Exception as err:
         snippet = repr(data)
         if len(snippet) > 35:
             snippet = f"{snippet[:35]} ..."
 
-        raise exception(f"Unable to parse {name}: {err} ({snippet})")
+        raise exception(f"Unable to parse {name}: {err} ({snippet})")  # noqa: B904
 
     if schema:
         parsed = schema.validate(parsed, name=name, exception=exception)
 
     return parsed
```

### Comparing `streamlink-5.3.1/src/streamlink/utils/processoutput.py` & `streamlink-5.4.0/src/streamlink/utils/processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink/utils/url.py` & `streamlink-5.4.0/src/streamlink/utils/url.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink.egg-info/PKG-INFO` & `streamlink-5.4.0/src/streamlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink
-Version: 5.3.1
+Version: 5.4.0
 Summary: Streamlink is a command-line utility that extracts streams from various services and pipes them into a video player of choice.
 Home-page: https://github.com/streamlink/streamlink
 Author: Streamlink
 Author-email: streamlink@protonmail.com
 License: Simplified BSD
 Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: streamlink Version: 5.3.1 Summary: Streamlink is a
+Metadata-Version: 2.1 Name: streamlink Version: 5.4.0 Summary: Streamlink is a
 command-line utility that extracts streams from various services and pipes them
 into a video player of choice. Home-page: https://github.com/streamlink/
 streamlink Author: Streamlink Author-email: streamlink@protonmail.com License:
 Simplified BSD Project-URL: Documentation, https://streamlink.github.io/
 Project-URL: Tracker, https://github.com/streamlink/streamlink/issues Project-
 URL: Source, https://github.com/streamlink/streamlink Project-URL: Funding,
 https://streamlink.github.io/latest/donate.html Classifier: Development Status
```

### Comparing `streamlink-5.3.1/src/streamlink.egg-info/SOURCES.txt` & `streamlink-5.4.0/src/streamlink.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 src/streamlink/plugins/hiplayer.py
 src/streamlink/plugins/hls.py
 src/streamlink/plugins/http.py
 src/streamlink/plugins/htv.py
 src/streamlink/plugins/huajiao.py
 src/streamlink/plugins/huya.py
 src/streamlink/plugins/idf1.py
+src/streamlink/plugins/indihometv.py
 src/streamlink/plugins/invintus.py
 src/streamlink/plugins/kugou.py
 src/streamlink/plugins/linelive.py
 src/streamlink/plugins/livestream.py
 src/streamlink/plugins/lnk.py
 src/streamlink/plugins/lrt.py
 src/streamlink/plugins/ltv_lsm_lv.py
@@ -157,15 +158,14 @@
 src/streamlink/plugins/mediavitrina.py
 src/streamlink/plugins/mildom.py
 src/streamlink/plugins/mitele.py
 src/streamlink/plugins/mixcloud.py
 src/streamlink/plugins/mjunoon.py
 src/streamlink/plugins/mrtmk.py
 src/streamlink/plugins/n13tv.py
-src/streamlink/plugins/nbcnews.py
 src/streamlink/plugins/nhkworld.py
 src/streamlink/plugins/nicolive.py
 src/streamlink/plugins/nimotv.py
 src/streamlink/plugins/nos.py
 src/streamlink/plugins/nownews.py
 src/streamlink/plugins/nrk.py
 src/streamlink/plugins/ntv.py
@@ -200,14 +200,15 @@
 src/streamlink/plugins/steam.py
 src/streamlink/plugins/streamable.py
 src/streamlink/plugins/streann.py
 src/streamlink/plugins/stv.py
 src/streamlink/plugins/svtplay.py
 src/streamlink/plugins/swisstxt.py
 src/streamlink/plugins/telefe.py
+src/streamlink/plugins/telemadrid.py
 src/streamlink/plugins/tf1.py
 src/streamlink/plugins/trovo.py
 src/streamlink/plugins/turkuvaz.py
 src/streamlink/plugins/tv360.py
 src/streamlink/plugins/tv3cat.py
 src/streamlink/plugins/tv4play.py
 src/streamlink/plugins/tv5monde.py
@@ -217,15 +218,14 @@
 src/streamlink/plugins/tviplayer.py
 src/streamlink/plugins/tvp.py
 src/streamlink/plugins/tvrby.py
 src/streamlink/plugins/tvrplus.py
 src/streamlink/plugins/tvtoya.py
 src/streamlink/plugins/twitcasting.py
 src/streamlink/plugins/twitch.py
-src/streamlink/plugins/useetv.py
 src/streamlink/plugins/ustreamtv.py
 src/streamlink/plugins/ustvnow.py
 src/streamlink/plugins/vidio.py
 src/streamlink/plugins/vimeo.py
 src/streamlink/plugins/vinhlongtv.py
 src/streamlink/plugins/vk.py
 src/streamlink/plugins/vkplay.py
@@ -371,14 +371,15 @@
 tests/plugins/test_googledrive.py
 tests/plugins/test_gulli.py
 tests/plugins/test_hiplayer.py
 tests/plugins/test_htv.py
 tests/plugins/test_huajiao.py
 tests/plugins/test_huya.py
 tests/plugins/test_idf1.py
+tests/plugins/test_indihometv.py
 tests/plugins/test_invintus.py
 tests/plugins/test_kugou.py
 tests/plugins/test_linelive.py
 tests/plugins/test_livestream.py
 tests/plugins/test_lnk.py
 tests/plugins/test_lrt.py
 tests/plugins/test_ltv_lsm_lv.py
@@ -387,15 +388,14 @@
 tests/plugins/test_mediavitrina.py
 tests/plugins/test_mildom.py
 tests/plugins/test_mitele.py
 tests/plugins/test_mixcloud.py
 tests/plugins/test_mjunoon.py
 tests/plugins/test_mrtmk.py
 tests/plugins/test_n13tv.py
-tests/plugins/test_nbcnews.py
 tests/plugins/test_nhkworld.py
 tests/plugins/test_nicolive.py
 tests/plugins/test_nimotv.py
 tests/plugins/test_nos.py
 tests/plugins/test_nownews.py
 tests/plugins/test_nrk.py
 tests/plugins/test_ntv.py
@@ -431,14 +431,15 @@
 tests/plugins/test_stream.py
 tests/plugins/test_streamable.py
 tests/plugins/test_streann.py
 tests/plugins/test_stv.py
 tests/plugins/test_svtplay.py
 tests/plugins/test_swisstxt.py
 tests/plugins/test_telefe.py
+tests/plugins/test_telemadrid.py
 tests/plugins/test_tf1.py
 tests/plugins/test_trovo.py
 tests/plugins/test_turkuvaz.py
 tests/plugins/test_tv360.py
 tests/plugins/test_tv3cat.py
 tests/plugins/test_tv4play.py
 tests/plugins/test_tv5monde.py
@@ -448,15 +449,14 @@
 tests/plugins/test_tviplayer.py
 tests/plugins/test_tvp.py
 tests/plugins/test_tvrby.py
 tests/plugins/test_tvrplus.py
 tests/plugins/test_tvtoya.py
 tests/plugins/test_twitcasting.py
 tests/plugins/test_twitch.py
-tests/plugins/test_useetv.py
 tests/plugins/test_ustreamtv.py
 tests/plugins/test_ustvnow.py
 tests/plugins/test_vidio.py
 tests/plugins/test_vimeo.py
 tests/plugins/test_vinhlongtv.py
 tests/plugins/test_vk.py
 tests/plugins/test_vkplay.py
@@ -480,23 +480,25 @@
 tests/resources/cli/config/secondary
 tests/resources/cli/config/secondary.testplugin
 tests/resources/dash/test_1.mpd
 tests/resources/dash/test_10.mpd
 tests/resources/dash/test_11_static.mpd
 tests/resources/dash/test_2.mpd
 tests/resources/dash/test_3.mpd
-tests/resources/dash/test_4.mpd
-tests/resources/dash/test_5.mpd
-tests/resources/dash/test_6_p1.mpd
-tests/resources/dash/test_6_p2.mpd
-tests/resources/dash/test_7.mpd
 tests/resources/dash/test_8.mpd
 tests/resources/dash/test_9.mpd
+tests/resources/dash/test_dynamic_timeline_continued_p1.mpd
+tests/resources/dash/test_dynamic_timeline_continued_p2.mpd
 tests/resources/dash/test_nested_baseurls.mpd
+tests/resources/dash/test_no_segment_list_or_template.mpd
+tests/resources/dash/test_segment_list.mpd
 tests/resources/dash/test_segments_byterange.mpd
+tests/resources/dash/test_segments_dynamic_number.mpd
+tests/resources/dash/test_static_no_publish_time.mpd
+tests/resources/dash/test_timeline_ids.mpd
 tests/resources/hls/test_1.m3u8
 tests/resources/hls/test_2.m3u8
 tests/resources/hls/test_date.m3u8
 tests/resources/hls/test_master.m3u8
 tests/resources/hls/test_master_twitch_vod.m3u8
 tests/stream/__init__.py
 tests/stream/test_dash.py
```

### Comparing `streamlink-5.3.1/src/streamlink_cli/argparser.py` & `streamlink-5.4.0/src/streamlink_cli/argparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,15 +515,15 @@
 
         Default is true.
         """,
     )
     player.add_argument(
         "--player-external-http-port",
         metavar="PORT",
-        type=num(int, min=0, max=65535),
+        type=num(int, ge=0, le=65535),
         default=0,
         help="""
         A fixed port to use for the external HTTP server if that mode is
         enabled. Omit or set to `0` to use a random high ( >1024) port.
         """,
     )
     player.add_argument(
@@ -600,29 +600,14 @@
 
         Example:
 
             %(prog)s --output "~/recordings/{author}/{category}/{id}-{time:%%Y%%m%%d%%H%%M%%S}.ts" <URL> [STREAM]
         """,
     )
     output.add_argument(
-        "-f", "--force",
-        action="store_true",
-        help="""
-        When using --output or --record, always write to file even if it already exists (overwrite).
-        """,
-    )
-    output.add_argument(
-        "--force-progress",
-        action="store_true",
-        help="""
-        When using --output or --record,
-        show the download progress bar even if there is no terminal.
-        """,
-    )
-    output.add_argument(
         "-O", "--stdout",
         action="store_true",
         help="""
         Write stream data to stdout instead of playing it.
         """,
     )
     output.add_argument(
@@ -679,14 +664,39 @@
 
         These characters are replaced with an underscore for the rules in use:
 
         - POSIX: `\\x00-\\x1F /`
         - Windows: `\\x00-\\x1F \\x7F " * / : < > ? \\ |`
         """,
     )
+    output.add_argument(
+        "-f", "--force",
+        action="store_true",
+        help="""
+        When using --output or --record, always write to file even if it already exists (overwrite).
+        """,
+    )
+    output.add_argument(
+        "--progress",
+        metavar="{yes,force,no}",
+        choices=("yes", "force", "no"),
+        default="yes",
+        help="""
+        When using --output or --record, show or hide the download progress bar, or force it if there's no terminal.
+
+        Default is yes.
+        """,
+    )
+    output.add_argument(
+        "--force-progress",
+        action="store_true",
+        help="""
+        Deprecated in favor of --progress=force.
+        """,
+    )
 
     stream = parser.add_argument_group("Stream options")
     stream.add_argument(
         "--url",
         dest="url_param",
         metavar="URL",
         help="""
@@ -723,39 +733,39 @@
         help="""
         If possible, translate the resolved stream to a URL and print it.
         """,
     )
     stream.add_argument(
         "--retry-streams",
         metavar="DELAY",
-        type=num(float, min=0),
+        type=num(float, gt=0),
         help="""
         Retry fetching the list of available streams until streams are found
         while waiting `DELAY` second(s) between each attempt. If unset, only one
         attempt will be made to fetch the list of streams available.
 
         The number of fetch retry attempts can be capped with --retry-max.
         """,
     )
     stream.add_argument(
         "--retry-max",
         metavar="COUNT",
-        type=num(int, min=-1),
+        type=num(int, ge=0),
         help="""
         When using --retry-streams, stop retrying the fetch after `COUNT` retry
         attempt(s). Fetch will retry infinitely if `COUNT` is zero or unset.
 
         If --retry-max is set without setting --retry-streams, the delay between
         retries will default to 1 second.
         """,
     )
     stream.add_argument(
         "--retry-open",
         metavar="ATTEMPTS",
-        type=num(int, min=0),
+        type=num(int, ge=1),
         default=1,
         help="""
         After a successful fetch, try `ATTEMPTS` time(s) to open the stream until
         giving up.
 
         Default is 1.
         """,
@@ -804,14 +814,15 @@
           --stream-sorting-excludes ">480p,>medium"
 
         """,
     )
 
     transport = parser.add_argument_group("Stream transport options")
     transport_hls = parser.add_argument_group("HLS options", parent=transport)
+    transport_dash = parser.add_argument_group("DASH options", parent=transport)
     transport_ffmpeg = parser.add_argument_group("FFmpeg options", parent=transport)
 
     transport.add_argument(
         "--ringbuffer-size",
         metavar="SIZE",
         type=filesize,
         help="""
@@ -831,51 +842,51 @@
 
         Note: A smaller size is recommended on lower end systems (such as Raspberry Pi) when playing stream types that require
         some extra processing to avoid unnecessary background processing.
         """,
     )
     transport.add_argument(
         "--stream-segment-attempts",
-        type=num(int, min=0),
+        type=num(int, ge=1),
         metavar="ATTEMPTS",
         help="""
         How many attempts should be done to download each segment before giving up.
 
         This applies to all different kinds of segmented stream types, such as DASH, HLS, etc.
 
         Default is 3.
         """,
     )
     transport.add_argument(
         "--stream-segment-threads",
-        type=num(int, max=10),
+        type=num(int, ge=1, le=10),
         metavar="THREADS",
         help="""
         The size of the thread pool used to download segments. Minimum value is `1` and maximum is `10`.
 
         This applies to all different kinds of segmented stream types, such as DASH, HLS, etc.
 
         Default is 1.
         """,
     )
     transport.add_argument(
         "--stream-segment-timeout",
-        type=num(float, min=0),
+        type=num(float, gt=0),
         metavar="TIMEOUT",
         help="""
         Segment connect and read timeout.
 
         This applies to all different kinds of segmented stream types, such as DASH, HLS, etc.
 
         Default is 10.0.
         """,
     )
     transport.add_argument(
         "--stream-timeout",
-        type=num(float, min=0),
+        type=num(float, gt=0),
         metavar="TIMEOUT",
         help="""
         Timeout for reading data from streams.
 
         This applies to all different kinds of stream types, such as DASH, HLS, HTTP, etc.
 
         Default is 60.0.
@@ -889,15 +900,15 @@
 
         Needs to be supported by the used plugin.
         """,
     )
 
     transport_hls.add_argument(
         "--hls-live-edge",
-        type=num(int, min=0),
+        type=num(int, ge=1),
         metavar="SEGMENTS",
         help="""
         Number of segments from the live stream's current live position to begin streaming.
         The size or length of each segment is determined by the streaming provider.
 
         Lower values will decrease the latency, but will also increase the chance of buffering, as there is less time for
         Streamlink to download segments and write their data to the output buffer. The number of parallel segment downloads
@@ -916,18 +927,18 @@
         action="store_true",
         help="""
         Immediately write segment data into output buffer while downloading.
         """,
     )
     transport_hls.add_argument(
         "--hls-playlist-reload-attempts",
-        type=num(int, min=0),
+        type=num(int, ge=1),
         metavar="ATTEMPTS",
         help="""
-        How many attempts should be done to reload the HLS playlist before giving up.
+        Max number of attempts when reloading the HLS playlist before giving up.
 
         Default is 3.
         """,
     )
     transport_hls.add_argument(
         "--hls-playlist-reload-time",
         metavar="TIME",
@@ -1025,19 +1036,30 @@
     transport_hls.add_argument(
         "--hls-live-restart",
         action="store_true",
         help="""
         Skip to the beginning of a live stream, or as far back as possible.
         """,
     )
+
+    transport_dash.add_argument(
+        "--dash-manifest-reload-attempts",
+        type=num(int, ge=1),
+        metavar="ATTEMPTS",
+        help="""
+        Max number of attempts when reloading the DASH manifest before giving up.
+
+        Default is 3.
+        """,
+    )
+
     transport_hls.add_argument("--hls-segment-attempts", help=argparse.SUPPRESS)
     transport_hls.add_argument("--hls-segment-threads", help=argparse.SUPPRESS)
     transport_hls.add_argument("--hls-segment-timeout", help=argparse.SUPPRESS)
     transport_hls.add_argument("--hls-timeout", help=argparse.SUPPRESS)
-
     transport.add_argument("--http-stream-timeout", help=argparse.SUPPRESS)
 
     transport_ffmpeg.add_argument(
         "--ffmpeg-ffmpeg",
         metavar="FILENAME",
         help="""
         FFMPEG is used to access or mux separate video and audio streams. You
@@ -1207,15 +1229,15 @@
 
         Expects a .crt and a .key file.
         """,
     )
     http.add_argument(
         "--http-timeout",
         metavar="TIMEOUT",
-        type=num(float, min=0),
+        type=num(float, gt=0),
         help="""
         General timeout used by all HTTP requests except the ones covered by
         other options.
 
         Default is 20.0.
         """,
     )
@@ -1269,14 +1291,15 @@
     ("hls_duration", "hls-duration", None),
     ("hls_playlist_reload_attempts", "hls-playlist-reload-attempts", None),
     ("hls_playlist_reload_time", "hls-playlist-reload-time", None),
     ("hls_segment_stream_data", "hls-segment-stream-data", None),
     ("hls_segment_ignore_names", "hls-segment-ignore-names", None),
     ("hls_segment_key_uri", "hls-segment-key-uri", None),
     ("hls_audio_select", "hls-audio-select", None),
+    ("dash_manifest_reload_attempts", "dash-manifest-reload-attempts", None),
     ("ffmpeg_ffmpeg", "ffmpeg-ffmpeg", None),
     ("ffmpeg_no_validation", "ffmpeg-no-validation", None),
     ("ffmpeg_verbose", "ffmpeg-verbose", None),
     ("ffmpeg_verbose_path", "ffmpeg-verbose-path", None),
     ("ffmpeg_fout", "ffmpeg-fout", None),
     ("ffmpeg_video_transcode", "ffmpeg-video-transcode", None),
     ("ffmpeg_audio_transcode", "ffmpeg-audio-transcode", None),
```

### Comparing `streamlink-5.3.1/src/streamlink_cli/compat.py` & `streamlink-5.4.0/src/streamlink_cli/compat.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink_cli/console.py` & `streamlink-5.4.0/src/streamlink_cli/console.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink_cli/constants.py` & `streamlink-5.4.0/src/streamlink_cli/constants.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink_cli/main.py` & `streamlink-5.4.0/src/streamlink_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import streamlink.logger as logger
 from streamlink import NoPluginError, PluginError, StreamError, Streamlink, __version__ as streamlink_version
 from streamlink.exceptions import FatalPluginError, StreamlinkDeprecationWarning
 from streamlink.plugin import Plugin, PluginOptions
 from streamlink.stream.stream import Stream, StreamIO
 from streamlink.utils.named_pipe import NamedPipe
+from streamlink.utils.times import LOCAL as LOCALTIMEZONE
 from streamlink_cli.argparser import ArgumentParser, build_parser, setup_session_options
 from streamlink_cli.compat import DeprecatedPath, importlib_metadata, stdout
 from streamlink_cli.console import ConsoleOutput, ConsoleUserInputRequester
 from streamlink_cli.constants import CONFIG_FILES, DEFAULT_STREAM_METADATA, LOG_DIR, PLUGIN_DIRS, STREAM_SYNONYMS
 from streamlink_cli.output import FileOutput, PlayerOutput
 from streamlink_cli.streamrunner import StreamRunner
 from streamlink_cli.utils import Formatter, HTTPServer, datetime
@@ -47,15 +48,15 @@
             "url": lambda: args.url,
             "plugin": lambda: plugin.module,
             "id": lambda: plugin.get_id(),
             "author": lambda: plugin.get_author(),
             "category": lambda: plugin.get_category(),
             "game": lambda: plugin.get_category(),
             "title": lambda: plugin.get_title(),
-            "time": lambda: datetime.now(),
+            "time": lambda: datetime.now(tz=LOCALTIMEZONE),
         },
         {
             "time": lambda dt, fmt: dt.strftime(fmt),
         },
     )
 
 
@@ -308,24 +309,24 @@
     """
     global stream_fd
 
     # Attempts to open the stream
     try:
         stream_fd = stream.open()
     except StreamError as err:
-        raise StreamError(f"Could not open stream: {err}")
+        raise StreamError(f"Could not open stream: {err}") from err
 
     # Read 8192 bytes before proceeding to check for errors.
     # This is to avoid opening the output unnecessarily.
     try:
         log.debug("Pre-buffering 8192 bytes")
         prebuffer = stream_fd.read(8192)
     except OSError as err:
         stream_fd.close()
-        raise StreamError(f"Failed to read data from stream: {err}")
+        raise StreamError(f"Failed to read data from stream: {err}") from err
 
     if not prebuffer:
         stream_fd.close()
         raise StreamError("No data returned from stream")
 
     return stream_fd, prebuffer
 
@@ -359,17 +360,25 @@
         else:
             console.exit(f"Failed to open output ({err}")
         return
 
     try:
         with closing(output):
             log.debug("Writing stream to output")
+            show_progress = args.progress == "force" or args.progress == "yes" and sys.stderr.isatty()
+            if args.force_progress:
+                show_progress = True
+                warnings.warn(
+                    "The --force-progress option has been deprecated in favor of --progress=force",
+                    StreamlinkDeprecationWarning,
+                    stacklevel=1,
+                )
             # TODO: finally clean up the global variable mess and refactor the streamlink_cli package
             # noinspection PyUnboundLocalVariable
-            stream_runner = StreamRunner(stream_fd, output, args.force_progress)
+            stream_runner = StreamRunner(stream_fd, output, show_progress=show_progress)
             # noinspection PyUnboundLocalVariable
             stream_runner.run(prebuffer)
     except OSError as err:
         # TODO: refactor all console.exit() calls
         console.exit(str(err))
 
     return True
@@ -407,34 +416,34 @@
         # to use these in case the main stream is not usable.
         alt_streams = list(filter(lambda k: f"{stream_name}_alt" in k, sorted(streams.keys())))
 
         file_output = args.output or args.stdout
 
         formatter = get_formatter(plugin)
 
-        for stream_name in [stream_name] + alt_streams:
-            stream = streams[stream_name]
+        for name in [stream_name] + alt_streams:
+            stream = streams[name]
             stream_type = type(stream).shortname()
 
             if stream_type in args.player_passthrough and not file_output:
-                log.info(f"Opening stream: {stream_name} ({stream_type})")
+                log.info(f"Opening stream: {name} ({stream_type})")
                 success = output_stream_passthrough(stream, formatter)
             elif args.player_external_http:
                 return output_stream_http(
                     plugin,
                     streams,
                     formatter,
                     external=True,
                     continuous=args.player_external_http_continuous,
                     port=args.player_external_http_port,
                 )
             elif args.player_continuous_http and not file_output:
                 return output_stream_http(plugin, streams, formatter)
             else:
-                log.info(f"Opening stream: {stream_name} ({stream_type})")
+                log.info(f"Opening stream: {name} ({stream_type})")
                 success = output_stream(stream, formatter)
 
             if success:
                 break
 
 
 def fetch_streams(plugin: Plugin) -> Dict[str, Stream]:
@@ -497,25 +506,21 @@
     (based on plugin.stream_weight).
 
     """
 
     delimiter = ", "
     validstreams = []
 
-    for name, stream in sorted(streams.items(),
-                               key=lambda stream: plugin.stream_weight(stream[0])):
+    for name, stream in sorted(streams.items(), key=lambda s: plugin.stream_weight(s[0])):
         if name in STREAM_SYNONYMS:
             continue
 
-        def synonymfilter(n):
-            return stream is streams[n] and n is not name
-
-        synonyms = list(filter(synonymfilter, streams.keys()))
+        synonyms = [key for key, value in streams.items() if stream is value and key != name]
 
-        if len(synonyms) > 0:
+        if synonyms:
             joined = delimiter.join(synonyms)
             name = f"{name} ({joined})"
 
         validstreams.append(name)
 
     return delimiter.join(validstreams)
 
@@ -609,14 +614,15 @@
     for directory in dirs:
         if directory.is_dir():
             success = streamlink.load_plugins(str(directory))
             if success and type(directory) is DeprecatedPath:
                 warnings.warn(
                     f"Loaded plugins from deprecated path, see CLI docs for how to migrate: {directory}",
                     StreamlinkDeprecationWarning,
+                    stacklevel=1,
                 )
         elif showwarning:
             log.warning(f"Plugin path {directory} does not exist or is not a directory!")
 
 
 def setup_args(
     parser: argparse.ArgumentParser,
@@ -657,14 +663,15 @@
     else:
         # Only load first available default config
         for config_file in filter(lambda path: path.is_file(), CONFIG_FILES):  # pragma: no branch
             if type(config_file) is DeprecatedPath:
                 warnings.warn(
                     f"Loaded config from deprecated path, see CLI docs for how to migrate: {config_file}",
                     StreamlinkDeprecationWarning,
+                    stacklevel=1,
                 )
             config_files.append(config_file)
             break
 
     if streamlink and args.url:
         # Only load first available plugin config
         with suppress(NoPluginError):
@@ -673,14 +680,15 @@
                 config_file = config_file.with_name(f"{config_file.name}.{pluginname}")
                 if not config_file.is_file():
                     continue
                 if type(config_file) is DeprecatedPath:
                     warnings.warn(
                         f"Loaded plugin config from deprecated path, see CLI docs for how to migrate: {config_file}",
                         StreamlinkDeprecationWarning,
+                        stacklevel=1,
                     )
                 config_files.append(config_file)
                 break
 
     if config_files:
         setup_args(parser, config_files, ignore_unknown=ignore_unknown)
 
@@ -830,15 +838,15 @@
             log.debug(f" {name}={value if name not in sensitive else '*' * 8}")
 
 
 def setup_logger_and_console(stream=sys.stdout, filename=None, level="info", json=False):
     global console
 
     if filename == "-":
-        filename = LOG_DIR / f"{datetime.now()}.log"
+        filename = LOG_DIR / f"{datetime.now(tz=LOCALTIMEZONE)}.log"
     elif filename:
         filename = Path(filename).expanduser().resolve()
 
     if filename:
         filename.parent.mkdir(parents=True, exist_ok=True)
 
     verbose = level in ("trace", "all")
```

### Comparing `streamlink-5.3.1/src/streamlink_cli/output.py` & `streamlink-5.4.0/src/streamlink_cli/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,16 @@
 
         if self.namedpipe or self.filename or self.http:
             self.stdin = sys.stdin
         else:
             self.stdin = subprocess.PIPE
 
         if self.quiet:
-            self.stdout = open(os.devnull, "w")
-            self.stderr = open(os.devnull, "w")
+            self.stdout = subprocess.DEVNULL
+            self.stderr = subprocess.DEVNULL
         else:
             self.stdout = sys.stdout
             self.stderr = sys.stderr
 
         if not self._re_player_args_input.search(self.args):
             self.args += f"{' ' if self.args else ''}{{{PLAYER_ARGS_INPUT_DEFAULT}}}"
 
@@ -199,26 +199,20 @@
         if is_win32:
             eargs = subprocess.list2cmdline(extra_args)
             # do not insert and extra " " when there are no extra_args
             return " ".join([cmd] + ([eargs] if eargs else []) + [args])
         return shlex.split(cmd) + extra_args + shlex.split(args)
 
     def _open(self):
-        try:
-            if self.record:
-                self.record.open()
-            if self.call and self.filename:
-                self._open_call()
-            else:
-                self._open_subprocess()
-        finally:
-            if self.quiet:
-                # Output streams no longer needed in parent process
-                self.stdout.close()
-                self.stderr.close()
+        if self.record:
+            self.record.open()
+        if self.call and self.filename:
+            self._open_call()
+        else:
+            self._open_subprocess()
 
     def _open_call(self):
         args = self._create_arguments()
         if is_win32:
             fargs = args
         else:
             fargs = subprocess.list2cmdline(args)
```

### Comparing `streamlink-5.3.1/src/streamlink_cli/streamrunner.py` & `streamlink-5.4.0/src/streamlink_cli/streamrunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     progress: Optional[Progress] = None
 
     # TODO: refactor all output implementations
     def __init__(
         self,
         stream: StreamIO,
         output: Union[PlayerOutput, FileOutput, HTTPServer],
-        force_progress: bool = False,
+        show_progress: bool = False,
     ):
         self.stream = stream
         self.output = output
         self.is_http = isinstance(output, HTTPServer)
 
         filename: Optional[Path] = None
 
@@ -95,15 +95,15 @@
 
         elif isinstance(output, FileOutput):
             if output.filename:
                 filename = output.filename
             elif output.record:
                 filename = output.record.filename
 
-        if filename and (sys.stdout.isatty() or force_progress):
+        if filename and show_progress:
             self.progress = Progress(sys.stderr, filename)
 
     def run(
         self,
         prebuffer: bytes,
         chunk_size: int = 8192,
     ) -> None:
```

### Comparing `streamlink-5.3.1/src/streamlink_cli/utils/__init__.py` & `streamlink-5.4.0/src/streamlink_cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink_cli/utils/formatter.py` & `streamlink-5.4.0/src/streamlink_cli/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink_cli/utils/http_server.py` & `streamlink-5.4.0/src/streamlink_cli/utils/http_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,50 +46,50 @@
     @property
     def url(self):
         return next(self.urls, None)
 
     def bind(self, host="127.0.0.1", port=0):
         try:
             self.socket.bind((host or "", port))
-        except OSError as err:
-            raise OSError(err)
+        except OSError:
+            raise
 
         self.socket.listen(1)
         self.bound = True
         self.host, self.port = self.socket.getsockname()
         if self.host == "0.0.0.0":
             self.host = None
 
     def open(self, timeout=30):
         self.socket.settimeout(timeout)
 
         try:
             conn, addr = self.socket.accept()
             conn.settimeout(None)
-        except socket.timeout:
-            raise OSError("Socket accept timed out")
+        except socket.timeout as err:
+            raise OSError("Socket accept timed out") from err
 
         try:
             req_data = conn.recv(1024)
-        except OSError:
-            raise OSError("Failed to read data from socket")
+        except OSError as err:
+            raise OSError("Failed to read data from socket") from err
 
         req = HTTPRequest(req_data)
         if req.command not in ("GET", "HEAD"):
             conn.send(b"HTTP/1.1 501 Not Implemented\r\n")
             conn.close()
-            raise OSError("Invalid request method: {0}".format(req.command))
+            raise OSError(f"Invalid request method: {req.command}")
 
         try:
             conn.send(b"HTTP/1.1 200 OK\r\n")
             conn.send(b"Server: Streamlink\r\n")
             conn.send(b"Content-Type: video/unknown\r\n")
             conn.send(b"\r\n")
-        except OSError:
-            raise OSError("Failed to write data to socket")
+        except OSError as err:
+            raise OSError("Failed to write data to socket") from err
 
         # We don't want to send any data on HEAD requests.
         if req.command == "HEAD":
             conn.close()
             raise OSError
 
         self.conn = conn
```

### Comparing `streamlink-5.3.1/src/streamlink_cli/utils/path.py` & `streamlink-5.4.0/src/streamlink_cli/utils/path.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink_cli/utils/player.py` & `streamlink-5.4.0/src/streamlink_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/src/streamlink_cli/utils/progress.py` & `streamlink-5.4.0/src/streamlink_cli/utils/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
         for fmt in formats:
             static.clear()
             variable.clear()
             length = 0
             # Get literal texts, static segments and variable segments from the parsed format
             # and calculate the overall length of the literal texts and static segments after substituting them.
-            for literal_text, field_name, format_spec, conversion in fmt:
+            for literal_text, field_name, format_spec, _conversion in fmt:
                 static.append(literal_text)
                 length += len(literal_text)
                 if field_name is None:
                     continue
                 if field_name not in params:
                     break
                 value_or_callable = params[field_name]
```

### Comparing `streamlink-5.3.1/src/streamlink_cli/utils/versioncheck.py` & `streamlink-5.4.0/src/streamlink_cli/utils/versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/__init__.py` & `streamlink-5.4.0/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 import signal
 
 import freezegun.config
 import pytest
 
 # import streamlink_cli as early as possible to execute its default signal overrides
 # noinspection PyUnresolvedReferences
@@ -19,14 +18,7 @@
 # in freezegun's default module ignore list (notice the trailing dots).
 freezegun.config.configure(extend_ignore_list=["_pytest.runner", "_pytest.terminal"])
 
 
 # make pytest rewrite assertions in dynamically parametrized plugin tests
 # https://docs.pytest.org/en/stable/how-to/writing_plugins.html#assertion-rewriting
 pytest.register_assert_rewrite("tests.plugins")
-
-
-windows_only = pytest.mark.skipif(os.name != "nt", reason="test only applicable on Windows")
-posix_only = pytest.mark.skipif(os.name != "posix", reason="test only applicable on a POSIX OS")
-
-
-__all__ = ["windows_only", "posix_only"]
```

### Comparing `streamlink-5.3.1/tests/cli/output/test_output.py` & `streamlink-5.4.0/tests/cli/output/test_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import unittest
 from pathlib import Path
 from unittest.mock import Mock, call, patch
 
 import pytest
 
 from streamlink_cli.output import FileOutput, PlayerOutput
-from tests import posix_only, windows_only
 
 
 @patch("streamlink_cli.output.stdout")
 class TestFileOutput(unittest.TestCase):
     @staticmethod
     def subject(filename, fd):
         fo_record = FileOutput(fd=fd)
@@ -66,20 +65,20 @@
         assert mock_fd.close.call_args_list == [call()]
         assert mock_stdout.close.call_args_list == []
         assert not fo_main.opened
         assert not fo_main.record.opened
 
         return mock_path
 
-    @posix_only
+    @pytest.mark.posix_only()
     @patch("builtins.open")
     def test_open_posix(self, mock_open: Mock, mock_stdout: Mock):
         self._test_open(mock_open, mock_stdout)
 
-    @windows_only
+    @pytest.mark.windows_only()
     @patch("streamlink_cli.output.msvcrt")
     @patch("builtins.open")
     def test_open_windows(self, mock_open: Mock, mock_msvcrt: Mock, mock_stdout: Mock):
         mock_path = self._test_open(mock_open, mock_stdout)
         assert mock_msvcrt.setmode.call_args_list == [
             call(mock_stdout.fileno(), os.O_BINARY),
             call(mock_open(mock_path, "wb").fileno(), os.O_BINARY),
```

### Comparing `streamlink-5.3.1/tests/cli/test_argparser.py` & `streamlink-5.4.0/tests/cli/test_argparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,14 @@
 
 
 @pytest.fixture(scope="module")
 def parser():
     return build_parser()
 
 
-@pytest.fixture()
-def session(monkeypatch: pytest.MonkeyPatch):
-    monkeypatch.setattr("streamlink.session.Streamlink.load_builtin_plugins", lambda _: None)
-    return Streamlink()
-
-
 @pytest.mark.filterwarnings("ignore")
 @pytest.mark.parametrize(("argv", "option", "expected"), [
     pytest.param(
         ["--locale", "xx_XX"],
         "locale",
         "xx_XX",
         id="Arg+value without mapper",
```

### Comparing `streamlink-5.3.1/tests/cli/test_cmdline.py` & `streamlink-5.4.0/tests/cli/test_cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import unittest
 from pathlib import Path
 from unittest.mock import ANY, Mock, call, patch
 
+import pytest
+
 import streamlink_cli.main
 import tests
 from streamlink import Streamlink
-from tests import posix_only, windows_only
 
 
 class CommandLineTestCase(unittest.TestCase):
     """
     Test that when invoked for the command line arguments are parsed as expected
     """
 
@@ -47,15 +48,15 @@
         assert mock_setup_streamlink.call_count == 1
         if not passthrough:
             assert mock_popen.call_args_list == [call(commandline, stderr=ANY, stdout=ANY, bufsize=ANY, stdin=ANY)]
         else:
             assert mock_call.call_args_list == [call(commandline, stderr=ANY, stdout=ANY)]
 
 
-@posix_only
+@pytest.mark.posix_only()
 class TestCommandLinePOSIX(CommandLineTestCase):
     """
     Commandline tests under POSIX-like operating systems
     """
 
     def test_open_regular_path_player(self):
         self._test_args(["streamlink", "-p", "/usr/bin/player", "http://test.se", "test"],
@@ -85,15 +86,15 @@
         """single hyphen params at the beginning of --player-args
            - https://github.com/streamlink/streamlink/issues/971 """
         self._test_args(["streamlink", "-p", "/usr/bin/player", "-a", "-v {filename}",
                          "http://test.se", "test"],
                         ["/usr/bin/player", "-v", "-"])
 
 
-@windows_only
+@pytest.mark.windows_only()
 class TestCommandLineWindows(CommandLineTestCase):
     """
     Commandline tests for Windows
     """
 
     def test_open_space_path_player(self):
         self._test_args(["streamlink", "-p", "c:\\Program Files\\Player\\player.exe", "http://test.se", "test"],
```

### Comparing `streamlink-5.3.1/tests/cli/test_cmdline_player_fifo.py` & `streamlink-5.4.0/tests/cli/test_cmdline_player_fifo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from unittest.mock import Mock, patch
 
-from tests import posix_only, windows_only
+import pytest
+
 from tests.cli.test_cmdline import CommandLineTestCase
 
 
-@posix_only
+@pytest.mark.posix_only()
 @patch("streamlink_cli.main.NamedPipe", Mock(return_value=Mock(path="/tmp/streamlinkpipe")))
 class TestCommandLineWithPlayerFifoPosix(CommandLineTestCase):
     def test_player_fifo_default(self):
         self._test_args(
             ["streamlink", "--player-fifo",
              "-p", "any-player",
              "http://test.se", "test"],
             ["any-player", "/tmp/streamlinkpipe"],
         )
 
 
-@windows_only
+@pytest.mark.windows_only()
 @patch("streamlink_cli.main.NamedPipe", Mock(return_value=Mock(path="\\\\.\\pipe\\streamlinkpipe")))
 class TestCommandLineWithPlayerFifoWindows(CommandLineTestCase):
     def test_player_fifo_default(self):
         self._test_args(
             ["streamlink", "--player-fifo",
              "-p", "any-player.exe",
              "http://test.se", "test"],
```

### Comparing `streamlink-5.3.1/tests/cli/test_cmdline_title.py` & `streamlink-5.4.0/tests/cli/test_cmdline_title.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from tests import posix_only, windows_only
+import pytest
+
 from tests.cli.test_cmdline import CommandLineTestCase
 
 
-@posix_only
+@pytest.mark.posix_only()
 class TestCommandLineWithTitlePOSIX(CommandLineTestCase):
     def test_open_player_with_title_vlc(self):
         self._test_args(["streamlink", "-p", "/usr/bin/vlc",
                          "--title", "{title} - {author} - {category}", "http://test.se", "test"],
                         ["/usr/bin/vlc", "--input-title-format", "Test Title - Tѥst Āuƭhǿr - No Category", "-"])
 
     def test_open_player_with_default_title_vlc(self):
@@ -22,15 +23,15 @@
                         ["/usr/bin/mpv", "--force-media-title=Test Title", "-"])
 
     def test_unicode_title_2444(self):
         self._test_args(["streamlink", "-p", "mpv", "-t", "★ ★ ★", "http://test.se", "test"],
                         ["mpv", "--force-media-title=★ ★ ★", "-"])
 
 
-@windows_only
+@pytest.mark.windows_only()
 class TestCommandLineWithTitleWindows(CommandLineTestCase):
     def test_open_player_with_title_vlc(self):
         self._test_args(
             ["streamlink", "-p", "c:\\Program Files\\VideoLAN\\vlc.exe",
              "--title", "{title} - {author} - {category}", "http://test.se", "test"],
             "c:\\Program Files\\VideoLAN\\vlc.exe --input-title-format \"Test Title - Tѥst Āuƭhǿr - No Category\" -",
         )
```

### Comparing `streamlink-5.3.1/tests/cli/test_console.py` & `streamlink-5.4.0/tests/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/cli/test_main.py` & `streamlink-5.4.0/tests/cli/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import datetime
 import logging
 import os
 import re
 import sys
 import unittest
+from argparse import Namespace
+from io import BytesIO
 from pathlib import Path, PosixPath, WindowsPath
 from textwrap import dedent
 from unittest.mock import Mock, call, patch
 
 import freezegun
 import pytest
 
 import streamlink_cli.main
 import tests.resources
-from streamlink.exceptions import PluginError, StreamError
+from streamlink.exceptions import PluginError, StreamError, StreamlinkDeprecationWarning
 from streamlink.session import Streamlink
 from streamlink.stream.stream import Stream
 from streamlink_cli.compat import stdout
 from streamlink_cli.main import (
     Formatter,
     NoPluginError,
     check_file_output,
@@ -25,15 +26,14 @@
     format_valid_streams,
     handle_stream,
     handle_url,
     output_stream,
     resolve_stream_name,
 )
 from streamlink_cli.output import FileOutput, PlayerOutput
-from tests import posix_only, windows_only
 from tests.plugin.testplugin import TestPlugin as _TestPlugin
 
 
 # TODO: rewrite the entire mess
 
 
 class FakePlugin(_TestPlugin):
@@ -472,39 +472,87 @@
         handle_stream(plugin, streams, "best")
         assert mock_output_stream.call_count == 1
         paramStream, paramFormatter = mock_output_stream.call_args[0]
         assert paramStream is stream
         assert isinstance(paramFormatter, Formatter)
 
 
-class TestCLIMainOutputStream(unittest.TestCase):
-    @patch("streamlink_cli.main.args", Mock(retry_open=2))
-    @patch("streamlink_cli.main.log")
-    @patch("streamlink_cli.main.console")
-    def test_stream_failure_no_output_open(self, mock_console: Mock, mock_log: Mock):
+class TestCLIMainOutputStream:
+    def test_stream_failure_no_output_open(self, caplog: pytest.LogCaptureFixture):
         output = Mock()
         stream = Mock(
             __str__=lambda _: "fake-stream",
             open=Mock(side_effect=StreamError("failure")),
         )
-        formatter = Formatter({})
+        formatter = Mock()
 
-        with patch("streamlink_cli.main.output", Mock()), \
+        caplog.set_level(1, "streamlink.cli")
+
+        with patch("streamlink_cli.main.args", Namespace(retry_open=2)), \
+             patch("streamlink_cli.main.console") as mock_console, \
+             patch("streamlink_cli.main.output"), \
              patch("streamlink_cli.main.create_output", return_value=output):
             output_stream(stream, formatter)
 
-        assert mock_log.error.call_args_list == [
-            call("Try 1/2: Could not open stream fake-stream (Could not open stream: failure)"),
-            call("Try 2/2: Could not open stream fake-stream (Could not open stream: failure)"),
+        assert [(record.levelname, record.module, record.message) for record in caplog.records] == [
+            ("error", "main", "Try 1/2: Could not open stream fake-stream (Could not open stream: failure)"),
+            ("error", "main", "Try 2/2: Could not open stream fake-stream (Could not open stream: failure)"),
         ]
         assert mock_console.exit.call_args_list == [
             call("Could not open stream fake-stream, tried 2 times, exiting"),
         ]
         assert not output.open.called, "Does not open the output on stream error"
 
+    @pytest.mark.parametrize(
+        ("args", "isatty", "deprecation", "expected"),
+        [
+            ({"progress": "yes", "force_progress": False}, True, False, True),
+            ({"progress": "no", "force_progress": False}, True, False, False),
+            ({"progress": "yes", "force_progress": False}, False, False, False),
+            ({"progress": "no", "force_progress": False}, False, False, False),
+            ({"progress": "force", "force_progress": False}, False, False, True),
+            ({"progress": "yes", "force_progress": True}, False, True, True),
+            ({"progress": "no", "force_progress": True}, False, True, True),
+        ],
+    )
+    def test_show_progress(
+        self,
+        caplog: pytest.LogCaptureFixture,
+        recwarn: pytest.WarningsRecorder,
+        args: dict,
+        isatty: bool,
+        deprecation: bool,
+        expected: bool,
+    ):
+        streamio = BytesIO(b"0" * 8192 * 2)
+        stream = Mock(open=Mock(return_value=streamio))
+        output = Mock()
+        formatter = Mock()
+
+        caplog.set_level(1, "streamlink.cli")
+
+        with patch("streamlink_cli.main.sys.stderr.isatty", return_value=isatty), \
+             patch("streamlink_cli.main.args", Namespace(retry_open=1, **args)), \
+             patch("streamlink_cli.main.console") as mock_console, \
+             patch("streamlink_cli.main.output"), \
+             patch("streamlink_cli.main.create_output", return_value=output), \
+             patch("streamlink_cli.main.StreamRunner") as mock_streamrunner:
+            assert output_stream(stream, formatter)
+
+        assert not mock_console.exit.called
+        assert [(record.levelname, record.module, record.message) for record in caplog.records] == [
+            ("debug", "main", "Pre-buffering 8192 bytes"),
+            ("debug", "main", "Writing stream to output"),
+        ]
+        assert [(record.category, str(record.message)) for record in recwarn.list] == ([(
+            StreamlinkDeprecationWarning,
+            "The --force-progress option has been deprecated in favor of --progress=force",
+        )] if deprecation else [])
+        assert mock_streamrunner.call_args_list == [call(streamio, output, show_progress=expected)]
+
 
 class _TestCLIMainLogging(unittest.TestCase):
     # stop test execution at the setup_signals() call, as we're not interested in what comes afterwards
     class StopTest(Exception):
         pass
 
     @classmethod
@@ -634,15 +682,15 @@
     def test_pipe_json(self, mock_stdout: Mock, mock_stderr: Mock):
         self.subject(["streamlink", "--stdout", "--json"], mock_stderr)
         assert mock_stdout.write.mock_calls == []
         assert mock_stderr.write.mock_calls == self._write_call_console_msg_json
 
 
 class TestCLIMainLoggingInfos(_TestCLIMainLogging):
-    @posix_only
+    @pytest.mark.posix_only()
     @patch("streamlink_cli.main.log")
     def test_log_root_warning(self, mock_log):
         self.subject(["streamlink"], euid=0)
         assert mock_log.info.mock_calls == [call("streamlink is running as root! Be careful!")]
 
     @patch("streamlink_cli.main.log")
     @patch("streamlink_cli.main.streamlink_version", "streamlink")
@@ -771,15 +819,15 @@
         self.write_file_and_assert(
             mock_mkdir=path.mkdir,
             mock_write=mock_open(str(path), "a").write,
             mock_stdout=mock_stdout,
         )
 
 
-@posix_only
+@pytest.mark.posix_only()
 class TestCLIMainLoggingLogfilePosix(_TestCLIMainLogging):
     @patch("sys.stdout")
     @patch("builtins.open")
     @patch("pathlib.Path.mkdir", Mock())
     def test_logfile_path_absolute(self, mock_open, mock_stdout):
         self.subject(["streamlink", "--logfile", "/foo/bar"])
         self.write_file_and_assert(
@@ -799,26 +847,26 @@
             mock_write=mock_open("/foo/bar", "a").write,
             mock_stdout=mock_stdout,
         )
 
     @patch("sys.stdout")
     @patch("builtins.open")
     @patch("pathlib.Path.mkdir", Mock())
-    @freezegun.freeze_time(datetime.datetime(2000, 1, 2, 3, 4, 5))
+    @freezegun.freeze_time("2000-01-02T03:04:05Z")
     def test_logfile_path_auto(self, mock_open, mock_stdout):
         with patch("streamlink_cli.constants.LOG_DIR", PosixPath("/foo")):
             self.subject(["streamlink", "--logfile", "-"])
         self.write_file_and_assert(
             mock_mkdir=PosixPath("/foo").mkdir,
             mock_write=mock_open("/foo/2000-01-02_03-04-05.log", "a").write,
             mock_stdout=mock_stdout,
         )
 
 
-@windows_only
+@pytest.mark.windows_only()
 class TestCLIMainLoggingLogfileWindows(_TestCLIMainLogging):
     @patch("sys.stdout")
     @patch("builtins.open")
     @patch("pathlib.Path.mkdir", Mock())
     def test_logfile_path_absolute(self, mock_open, mock_stdout):
         self.subject(["streamlink", "--logfile", "C:\\foo\\bar"])
         self.write_file_and_assert(
@@ -838,15 +886,15 @@
             mock_write=mock_open("C:\\foo\\bar", "a").write,
             mock_stdout=mock_stdout,
         )
 
     @patch("sys.stdout")
     @patch("builtins.open")
     @patch("pathlib.Path.mkdir", Mock())
-    @freezegun.freeze_time(datetime.datetime(2000, 1, 2, 3, 4, 5))
+    @freezegun.freeze_time("2000-01-02T03:04:05Z")
     def test_logfile_path_auto(self, mock_open, mock_stdout):
         with patch("streamlink_cli.constants.LOG_DIR", WindowsPath("C:\\foo")):
             self.subject(["streamlink", "--logfile", "-"])
         self.write_file_and_assert(
             mock_mkdir=WindowsPath("C:\\foo").mkdir,
             mock_write=mock_open("C:\\foo\\2000-01-02_03-04-05.log", "a").write,
             mock_stdout=mock_stdout,
```

### Comparing `streamlink-5.3.1/tests/cli/test_main_formatter.py` & `streamlink-5.4.0/tests/cli/test_main_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/cli/test_main_setup_config_args.py` & `streamlink-5.4.0/tests/cli/test_main_setup_config_args.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/cli/test_streamrunner.py` & `streamlink-5.4.0/tests/cli/test_streamrunner.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,20 +98,14 @@
 
 @pytest.fixture(autouse=True)
 def _logging(caplog: pytest.LogCaptureFixture):
     assert streamrunnerlogger.name == "streamlink.cli"
     caplog.set_level(1, "streamlink")
 
 
-@pytest.fixture(autouse=True)
-def _isatty(request: pytest.FixtureRequest):
-    with patch("sys.stdout.isatty", return_value=getattr(request, "param", False)):
-        yield
-
-
 @pytest.fixture()
 def stream():
     stream = FakeStream()
     yield stream
     assert stream.closed
 
 
@@ -171,14 +165,15 @@
     def output(self, player_process: Mock):
         with patch("subprocess.Popen") as mock_popen, \
              patch("streamlink_cli.output.sleep"):
             mock_popen.return_value = player_process
             output = FakePlayerOutput("mocked")
             output.open()
             yield output
+            output.close()
 
     @pytest.fixture()
     def stream_runner(self, stream: FakeStream, output: FakePlayerOutput):
         with patch("streamlink_cli.streamrunner.PlayerPollThread", EventedPlayerPollThread):
             stream_runner = StreamRunner(stream, output)
             assert isinstance(stream_runner.playerpoller, EventedPlayerPollThread)
             assert not stream_runner.playerpoller.is_alive()
@@ -558,22 +553,14 @@
         expectedlogs = (
             ([("streamrunner", "info", "HTTP connection closed")] if logs else [])
             + [("streamrunner", "info", "Stream ended")]
         )
         assert [(record.module, record.levelname, record.message) for record in caplog.records] == expectedlogs
 
 
-@pytest.mark.parametrize(
-    ("_isatty", "force_progress"),
-    [
-        pytest.param(False, True, id="No TTY, force"),
-        pytest.param(True, False, id="TTY, no force"),
-    ],
-    indirect=["_isatty"],
-)
 class TestHasProgress:
     @pytest.mark.parametrize(
         "output",
         [
             pytest.param(
                 FakePlayerOutput("mocked"),
                 id="Player output without record",
@@ -587,17 +574,16 @@
                 id="HTTPServer",
             ),
         ],
     )
     def test_no_progress(
         self,
         output: Union[FakePlayerOutput, FakeFileOutput, FakeHTTPServer],
-        force_progress: bool,
     ):
-        stream_runner = FakeStreamRunner(StreamIO(), output, force_progress)
+        stream_runner = FakeStreamRunner(StreamIO(), output, show_progress=True)
         assert not stream_runner.progress
 
     @pytest.mark.parametrize(
         ("output", "expected"),
         [
             pytest.param(
                 FakePlayerOutput("mocked", record=FakeFileOutput(Path("record"))),
@@ -620,33 +606,32 @@
                 id="FileOutput with file name and record",
             ),
         ],
     )
     def test_has_progress(
         self,
         output: Union[FakePlayerOutput, FakeFileOutput],
-        force_progress: bool,
         expected: Path,
     ):
-        stream_runner = FakeStreamRunner(StreamIO(), output, force_progress)
+        stream_runner = FakeStreamRunner(StreamIO(), output, show_progress=True)
         assert stream_runner.progress
         assert not stream_runner.progress.is_alive()
         assert stream_runner.progress.stream is sys.stderr
         assert stream_runner.progress.path == expected
 
 
 class TestProgress:
     @pytest.fixture()
     def output(self):
         return FakeFileOutput(Path("filename"))
 
     @pytest.fixture()
     def stream_runner(self, stream: FakeStream, output: FakeFileOutput):
         with patch("streamlink_cli.streamrunner.Progress", FakeProgress):
-            stream_runner = FakeStreamRunner(stream, output, True)
+            stream_runner = FakeStreamRunner(stream, output, show_progress=True)
             assert not stream_runner.playerpoller
             assert not stream_runner.is_http
             assert isinstance(stream_runner.progress, FakeProgress)
             assert stream_runner.progress.path == Path("filename")
             assert not stream_runner.progress.is_alive()
             yield stream_runner
             assert not stream_runner.progress.is_alive()
```

### Comparing `streamlink-5.3.1/tests/cli/utils/test_formatter.py` & `streamlink-5.4.0/tests/cli/utils/test_formatter.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/cli/utils/test_path.py` & `streamlink-5.4.0/tests/cli/utils/test_path.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 import os
 from pathlib import Path
 from unittest.mock import patch
 
 import pytest
 
 from streamlink_cli.utils.path import replace_chars, replace_path
-from tests import posix_only, windows_only
 
 
 @pytest.mark.parametrize("char", list(range(32)))
 def test_replace_chars_unprintable(char: int):
     assert replace_chars(f"foo{chr(char)}{chr(char)}bar") == "foo_bar", "Replaces unprintable characters"
 
 
-@posix_only
+@pytest.mark.posix_only()
 @pytest.mark.parametrize("char", "/".split())
 def test_replace_chars_posix(char: str):
     assert replace_chars(f"foo{char}{char}bar") == "foo_bar", "Replaces multiple unsupported characters in a row"
 
 
-@windows_only
+@pytest.mark.windows_only()
 @pytest.mark.parametrize("char", "\x7f\"*/:<>?\\|".split())
 def test_replace_chars_windows(char: str):
     assert replace_chars(f"foo{char}{char}bar") == "foo_bar", "Replaces multiple unsupported characters in a row"
 
 
-@posix_only
+@pytest.mark.posix_only()
 def test_replace_chars_posix_all():
     assert replace_chars("".join(chr(i) for i in range(32)) + "/") == "_"
 
 
-@windows_only
+@pytest.mark.windows_only()
 def test_replace_chars_windows_all():
     assert replace_chars("".join(chr(i) for i in range(32)) + "\x7f\"*/:<>?\\|") == "_"
 
 
-@posix_only
+@pytest.mark.posix_only()
 def test_replace_chars_posix_override():
     all_chars = "".join(chr(i) for i in range(32)) + "\x7f\"*:/<>?\\|"
     assert replace_chars(all_chars) == "_\x7f\"*:_<>?\\|"
     assert replace_chars(all_chars, "posix") == "_\x7f\"*:_<>?\\|"
     assert replace_chars(all_chars, "unix") == "_\x7f\"*:_<>?\\|"
     assert replace_chars(all_chars, "windows") == "_"
     assert replace_chars(all_chars, "win32") == "_"
 
 
-@windows_only
+@pytest.mark.windows_only()
 def test_replace_chars_windows_override():
     all_chars = "".join(chr(i) for i in range(32)) + "\x7f\"*:/<>?\\|"
     assert replace_chars(all_chars) == "_"
     assert replace_chars(all_chars, "posix") == "_\x7f\"*:_<>?\\|"
     assert replace_chars(all_chars, "unix") == "_\x7f\"*:_<>?\\|"
     assert replace_chars(all_chars, "windows") == "_"
     assert replace_chars(all_chars, "win32") == "_"
@@ -64,19 +63,19 @@
         return dict(foo=".", bar="..").get(s, s)
 
     path = Path("foo", ".", "bar", "..", "baz")
     expected = Path("_", ".", "_", "..", "baz")
     assert replace_path(path, mapper) == expected, "Only replaces mapped parts which are in the special parts tuple"
 
 
-@posix_only
+@pytest.mark.posix_only()
 def test_replace_path_expanduser_posix():
     with patch.object(os, "environ", {"HOME": "/home/foo"}):
         assert replace_path("~/bar", lambda s: s) == Path("/home/foo/bar")
         assert replace_path("foo/bar", lambda s: dict(foo="~").get(s, s)) == Path("~/bar")
 
 
-@windows_only
+@pytest.mark.windows_only()
 def test_replace_path_expanduser_windows():
     with patch.object(os, "environ", {"USERPROFILE": "C:\\Users\\foo"}):
         assert replace_path("~\\bar", lambda s: s) == Path("C:\\Users\\foo\\bar")
         assert replace_path("foo\\bar", lambda s: dict(foo="~").get(s, s)) == Path("~\\bar")
```

### Comparing `streamlink-5.3.1/tests/cli/utils/test_progress.py` & `streamlink-5.4.0/tests/cli/utils/test_progress.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from time import time
 from unittest.mock import Mock, call, patch
 
 import freezegun
 import pytest
 
 from streamlink_cli.utils.progress import Progress, ProgressFormatter
-from tests import posix_only, windows_only
 
 
 class TestProgressFormatter:
     @pytest.fixture(scope="class")
     def params(self):
         return dict(
             written="WRITTEN",
@@ -179,24 +178,24 @@
     def stream(self):
         return StringIO()
 
     @pytest.fixture()
     def progress(self, stream: StringIO):
         return Progress(stream, Mock())
 
-    @posix_only
+    @pytest.mark.posix_only()
     def test_print_posix(self, progress: Progress, stream: StringIO):
         progress.print_inplace("foo")
         progress.print_inplace("barbaz")
         progress.print_inplace("0123456789")
         progress.print_inplace("abcdefghijk")
         progress.print_end()
         assert stream.getvalue() == "\rfoo       \rbarbaz    \r0123456789\rabcdefghijk\n"
 
-    @windows_only
+    @pytest.mark.windows_only()
     def test_print_windows(self, progress: Progress, stream: StringIO):
         progress.print_inplace("foo")
         progress.print_inplace("barbaz")
         progress.print_inplace("0123456789")
         progress.print_inplace("abcdefghijk")
         progress.print_end()
         assert stream.getvalue() == "\rfoo      \rbarbaz   \r0123456789\rabcdefghijk\n"
```

### Comparing `streamlink-5.3.1/tests/cli/utils/test_versioncheck.py` & `streamlink-5.4.0/tests/cli/utils/test_versioncheck.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/mixins/stream_hls.py` & `streamlink-5.4.0/tests/mixins/stream_hls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 from binascii import hexlify
 from functools import partial
 from threading import Event, Thread
 from typing import List
+from unittest.mock import patch
 
 import requests_mock
 
 from streamlink import Streamlink
 from streamlink.stream.hls import HLSStream, HLSStreamWriter as _HLSStreamWriter
 from tests.testutils.handshake import Handshake
 
@@ -159,15 +160,15 @@
             if cm.error:
                 return
 
     def reset(self):
         self.data.clear()
 
     def close(self):
-        self.reader.buffer.close()
+        self.reader.close()
         self.read_once.set()
         # allow reader thread to terminate
         self.handshake.go()
 
 
 class TestMixinStreamHLS(unittest.TestCase):
     __stream__ = HLSStream
@@ -175,31 +176,38 @@
 
     session: Streamlink
     stream: HLSStream
     thread: HLSStreamReadThread
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+        # FIXME: fix HTTPSession.request()
+        # don't sleep on mocked HTTP request failures
+        self._patch_http_retry_sleep = patch("streamlink.plugin.api.http_session.time.sleep")
         self.mocker = requests_mock.Mocker()
         self.mocks = {}
 
     def setUp(self):
         super().setUp()
+
+        self._patch_http_retry_sleep.start()
         self.mocker.start()
 
     def tearDown(self):
         super().tearDown()
 
         # close read thread and make sure that all threads have terminated before moving on
         self.close()
         self.await_close()
 
         self.mocker.stop()
         self.mocks.clear()
 
+        self._patch_http_retry_sleep.stop()
+
     def mock(self, method, url, *args, **kwargs):
         self.mocks[url] = self.mocker.request(method, url, *args, **kwargs)
 
     def get_mock(self, item):
         return self.mocks[self.url(item)]
 
     def called(self, item, once=False):
@@ -222,15 +230,15 @@
         thread.join(timeout)
         assert self.thread.reader.closed, "Stream reader is closed"
 
     # make write calls on the write-thread and wait until it has finished
     def await_write(self, write_calls=1, timeout=TIMEOUT_AWAIT_WRITE) -> None:
         writer: EventedHLSStreamWriter = self.thread.reader.writer  # type: ignore[assignment]
         assert writer.is_alive()
-        for write_call in range(write_calls):
+        for _ in range(write_calls):
             assert writer.handshake.step(timeout)
 
     # make one read call on the read thread and wait until it has finished
     def await_read(self, read_all=False, timeout=TIMEOUT_AWAIT_READ):
         thread = self.thread
         thread.read_all = read_all
```

### Comparing `streamlink-5.3.1/tests/plugin/testplugin.py` & `streamlink-5.4.0/tests/plugin/testplugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     def _get_streams(self):
         if "empty" in self.url:
             return
 
         if "UnsortableStreamNames" in self.url:
             def gen():
-                for i in range(3):
+                for _ in range(3):
                     yield "vod", HTTPStream(self.session, "http://test.se/stream")
 
             return gen()
 
         if "NoStreamsError" in self.url:
             raise NoStreamsError
```

### Comparing `streamlink-5.3.1/tests/plugins/__init__.py` & `streamlink-5.4.0/tests/plugins/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,16 @@
     def classnames(self):
         yield _plugin_can_handle_url_classnames
         _plugin_can_handle_url_classnames.add(self.__class__.__name__)
 
     # ---- tests
 
     def test_class_setup(self):
-        assert issubclass(getattr(self, "__plugin__"), Plugin), "Test has a __plugin__ that is a subclass of the Plugin class"
+        assert hasattr(self, "__plugin__"), "Test has a __plugin__ attribute"
+        assert issubclass(self.__plugin__, Plugin), "Test has a __plugin__ that is a subclass of the Plugin class"
         assert len(self.should_match) + len(self.should_match_groups) > 0, "Test has at least one positive URL"
 
     def test_class_name(self, classnames: Set[str]):
         assert self.__class__.__name__ not in classnames
 
     # ---- all tests below are parametrized dynamically via conftest.py
```

### Comparing `streamlink-5.3.1/tests/plugins/conftest.py` & `streamlink-5.4.0/tests/plugins/conftest.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_abematv.py` & `streamlink-5.4.0/tests/plugins/test_abematv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_adultswim.py` & `streamlink-5.4.0/tests/plugins/test_adultswim.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_afreeca.py` & `streamlink-5.4.0/tests/plugins/test_afreeca.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_albavision.py` & `streamlink-5.4.0/tests/plugins/test_albavision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_aloula.py` & `streamlink-5.4.0/tests/plugins/test_aloula.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_ard_mediathek.py` & `streamlink-5.4.0/tests/plugins/test_ard_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_artetv.py` & `streamlink-5.4.0/tests/plugins/test_artetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_atpchallenger.py` & `streamlink-5.4.0/tests/plugins/test_atpchallenger.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_atresplayer.py` & `streamlink-5.4.0/tests/plugins/test_atresplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_bbciplayer.py` & `streamlink-5.4.0/tests/plugins/test_bbciplayer.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_bfmtv.py` & `streamlink-5.4.0/tests/plugins/test_bfmtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_bigo.py` & `streamlink-5.4.0/tests/plugins/test_bigo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_blazetv.py` & `streamlink-5.4.0/tests/plugins/test_blazetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_bloomberg.py` & `streamlink-5.4.0/tests/plugins/test_bloomberg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_booyah.py` & `streamlink-5.4.0/tests/plugins/test_booyah.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_cbsnews.py` & `streamlink-5.4.0/tests/plugins/test_cbsnews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_cdnbg.py` & `streamlink-5.4.0/tests/plugins/test_cdnbg.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_ceskatelevize.py` & `streamlink-5.4.0/tests/plugins/test_ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_cinergroup.py` & `streamlink-5.4.0/tests/plugins/test_cinergroup.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_cmmedia.py` & `streamlink-5.4.0/tests/plugins/test_cmmedia.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_crunchyroll.py` & `streamlink-5.4.0/tests/plugins/test_crunchyroll.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_dailymotion.py` & `streamlink-5.4.0/tests/plugins/test_dailymotion.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_dash.py` & `streamlink-5.4.0/tests/plugins/test_dash.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_delfi.py` & `streamlink-5.4.0/tests/plugins/test_delfi.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_deutschewelle.py` & `streamlink-5.4.0/tests/plugins/test_deutschewelle.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_dogan.py` & `streamlink-5.4.0/tests/plugins/test_dogan.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_drdk.py` & `streamlink-5.4.0/tests/plugins/test_drdk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_euronews.py` & `streamlink-5.4.0/tests/plugins/test_euronews.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_facebook.py` & `streamlink-5.4.0/tests/plugins/test_facebook.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_filmon.py` & `streamlink-5.4.0/tests/plugins/test_filmon.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import datetime
+from datetime import datetime, timezone
 from unittest.mock import patch
 
 import freezegun
 import pytest
 
 from streamlink import Streamlink
 from streamlink.plugins.filmon import Filmon, FilmOnAPI, FilmOnHLS
@@ -38,43 +38,43 @@
         ("http://www.filmon.tv/vod/view/10250-0-crime-boss?extra", (None, None, "10250-0-crime-boss")),
         ("http://www.filmon.tv/vod/view/10250-0-crime-boss&extra", (None, None, "10250-0-crime-boss")),
     ]
 
 
 @pytest.fixture()
 def filmonhls():
-    with freezegun.freeze_time(datetime.datetime(2000, 1, 1, 0, 0, 0, 0)), \
+    with freezegun.freeze_time("2000-01-01T00:00:00Z"), \
          patch("streamlink.plugins.filmon.FilmOnHLS._get_stream_data", return_value=[]):
         session = Streamlink()
         api = FilmOnAPI(session)
         yield FilmOnHLS(session, "http://fake/one.m3u8", api=api, channel="test")
 
 
 def test_filmonhls_to_url(filmonhls):
-    filmonhls.watch_timeout = datetime.datetime(2000, 1, 1, 0, 0, 0, 0).timestamp()
+    filmonhls.watch_timeout = datetime(2000, 1, 1, 0, 0, 0, 0, timezone.utc).timestamp()
     assert filmonhls.to_url() == "http://fake/one.m3u8"
 
 
 def test_filmonhls_to_url_updated(filmonhls):
-    filmonhls.watch_timeout = datetime.datetime(1999, 12, 31, 23, 59, 59, 9999).timestamp()
+    filmonhls.watch_timeout = datetime(1999, 12, 31, 23, 59, 59, 9999, timezone.utc).timestamp()
 
     filmonhls._get_stream_data.return_value = [
-        ("high", "http://fake/two.m3u8", datetime.datetime(2000, 1, 1, 0, 0, 0, 0).timestamp()),
+        ("high", "http://fake/two.m3u8", datetime(2000, 1, 1, 0, 0, 0, 0, timezone.utc).timestamp()),
     ]
     assert filmonhls.to_url() == "http://fake/two.m3u8"
 
-    filmonhls.watch_timeout = datetime.datetime(1999, 12, 31, 23, 59, 59, 9999).timestamp()
+    filmonhls.watch_timeout = datetime(1999, 12, 31, 23, 59, 59, 9999, timezone.utc).timestamp()
     filmonhls._get_stream_data.return_value = [
-        ("high", "http://another-fake/three.m3u8", datetime.datetime(2000, 1, 1, 0, 0, 0, 0).timestamp()),
+        ("high", "http://another-fake/three.m3u8", datetime(2000, 1, 1, 0, 0, 0, 0, timezone.utc).timestamp()),
     ]
     assert filmonhls.to_url() == "http://fake/three.m3u8"
 
 
 def test_filmonhls_to_url_missing_quality(filmonhls):
-    filmonhls.watch_timeout = datetime.datetime(1999, 12, 31, 23, 59, 59, 9999).timestamp()
+    filmonhls.watch_timeout = datetime(1999, 12, 31, 23, 59, 59, 9999, timezone.utc).timestamp()
 
     filmonhls._get_stream_data.return_value = [
-        ("low", "http://fake/two.m3u8", datetime.datetime(2000, 1, 1, 0, 0, 0, 0).timestamp()),
+        ("low", "http://fake/two.m3u8", datetime(2000, 1, 1, 0, 0, 0, 0, timezone.utc).timestamp()),
     ]
     with pytest.raises(TypeError) as cm:
         filmonhls.to_url()
     assert str(cm.value) == "Stream has expired and cannot be translated to a URL"
```

### Comparing `streamlink-5.3.1/tests/plugins/test_goltelevision.py` & `streamlink-5.4.0/tests/plugins/test_goltelevision.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_gulli.py` & `streamlink-5.4.0/tests/plugins/test_gulli.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_htv.py` & `streamlink-5.4.0/tests/plugins/test_htv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_idf1.py` & `streamlink-5.4.0/tests/plugins/test_idf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_invintus.py` & `streamlink-5.4.0/tests/plugins/test_invintus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_kugou.py` & `streamlink-5.4.0/tests/plugins/test_kugou.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_livestream.py` & `streamlink-5.4.0/tests/plugins/test_livestream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_lnk.py` & `streamlink-5.4.0/tests/plugins/test_lnk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_lrt.py` & `streamlink-5.4.0/tests/plugins/test_lrt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_ltv_lsm_lv.py` & `streamlink-5.4.0/tests/plugins/test_ltv_lsm_lv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_mdstrm.py` & `streamlink-5.4.0/tests/plugins/test_mdstrm.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_mediaklikk.py` & `streamlink-5.4.0/tests/plugins/test_mediaklikk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_mediavitrina.py` & `streamlink-5.4.0/tests/plugins/test_mediavitrina.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_mitele.py` & `streamlink-5.4.0/tests/plugins/test_mitele.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_mixcloud.py` & `streamlink-5.4.0/tests/plugins/test_mixcloud.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_n13tv.py` & `streamlink-5.4.0/tests/plugins/test_n13tv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_nicolive.py` & `streamlink-5.4.0/tests/plugins/test_nicolive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_nos.py` & `streamlink-5.4.0/tests/plugins/test_nos.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_nrk.py` & `streamlink-5.4.0/tests/plugins/test_nrk.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_olympicchannel.py` & `streamlink-5.4.0/tests/plugins/test_olympicchannel.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_oneplusone.py` & `streamlink-5.4.0/tests/plugins/test_oneplusone.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_onetv.py` & `streamlink-5.4.0/tests/plugins/test_onetv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_pandalive.py` & `streamlink-5.4.0/tests/plugins/test_pandalive.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_picarto.py` & `streamlink-5.4.0/tests/plugins/test_picarto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_pluto.py` & `streamlink-5.4.0/tests/plugins/test_pluto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_pluzz.py` & `streamlink-5.4.0/tests/plugins/test_pluzz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_radionet.py` & `streamlink-5.4.0/tests/plugins/test_radionet.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_raiplay.py` & `streamlink-5.4.0/tests/plugins/test_raiplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_reuters.py` & `streamlink-5.4.0/tests/plugins/test_reuters.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_rtbf.py` & `streamlink-5.4.0/tests/plugins/test_rtbf.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_rtpplay.py` & `streamlink-5.4.0/tests/plugins/test_rtpplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_rtve.py` & `streamlink-5.4.0/tests/plugins/test_rtve.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_ruv.py` & `streamlink-5.4.0/tests/plugins/test_ruv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_sbscokr.py` & `streamlink-5.4.0/tests/plugins/test_sbscokr.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_showroom.py` & `streamlink-5.4.0/tests/plugins/test_showroom.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_steam.py` & `streamlink-5.4.0/tests/plugins/test_steam.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_stream.py` & `streamlink-5.4.0/tests/plugins/test_stream.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_streann.py` & `streamlink-5.4.0/tests/plugins/test_streann.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_svtplay.py` & `streamlink-5.4.0/tests/plugins/test_svtplay.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_swisstxt.py` & `streamlink-5.4.0/tests/plugins/test_swisstxt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_telefe.py` & `streamlink-5.4.0/tests/plugins/test_telefe.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_tf1.py` & `streamlink-5.4.0/tests/plugins/test_tf1.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_trovo.py` & `streamlink-5.4.0/tests/plugins/test_trovo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_turkuvaz.py` & `streamlink-5.4.0/tests/plugins/test_turkuvaz.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_tv4play.py` & `streamlink-5.4.0/tests/plugins/test_tv4play.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_tv5monde.py` & `streamlink-5.4.0/tests/plugins/test_tv5monde.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tests.plugins import PluginCanHandleUrl
 
 
 class TestPluginCanHandleUrlTV5Monde(PluginCanHandleUrl):
     __plugin__ = TV5Monde
 
     should_match = [
-        "http://live.tv5monde.com/fbs.html",
-        "https://www.tv5monde.com/emissions/episode/version-francaise-vf-83",
-        "https://revoir.tv5monde.com/toutes-les-videos/cinema/je-ne-reve-que-de-vous",
-        "https://revoir.tv5monde.com/toutes-les-videos/documentaires/des-russes-blancs-des-russes-blancs",
+        "https://live.tv5monde.com/fbs.html",
+        "https://europe.tv5monde.com/fr/direct",
+        "https://maghreb-orient.tv5monde.com/fr/direct",
+        "https://revoir.tv5monde.com/toutes-les-videos/documentaires/sauver-notre-dame-sauver-notre-dame-14-04-2020",
         "https://information.tv5monde.com/video/la-diplomatie-francaise-est-elle-en-crise",
-        "https://afrique.tv5monde.com/videos/exclusivites-web/les-tutos-de-magloire/season-1/episode-1",
+        "https://afrique.tv5monde.com/videos/afrykas-et-la-boite-magique",
         "https://www.tivi5mondeplus.com/conte-nous/episode-25",
     ]
```

### Comparing `streamlink-5.3.1/tests/plugins/test_tvp.py` & `streamlink-5.4.0/tests/plugins/test_tvp.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_tvrby.py` & `streamlink-5.4.0/tests/plugins/test_tvrby.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_tvrplus.py` & `streamlink-5.4.0/tests/plugins/test_tvrplus.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_twitch.py` & `streamlink-5.4.0/tests/plugins/test_twitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from unittest.mock import MagicMock, call, patch
 
 import pytest
 import requests_mock
 
 from streamlink import Streamlink
 from streamlink.exceptions import NoStreamsError
@@ -48,15 +48,15 @@
 
     should_not_match = [
         "https://www.twitch.tv",
         "https://www.twitch.tv/",
     ]
 
 
-DATETIME_BASE = datetime(2000, 1, 1, 0, 0, 0, 0)
+DATETIME_BASE = datetime(2000, 1, 1, 0, 0, 0, 0, timezone.utc)
 DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
 class TagDateRangeAd(Tag):
     def __init__(self, start=DATETIME_BASE, duration=1, attrid="stitched-ad-1234", classname="twitch-stitched-ad", custom=None):
         attrs = {
             "ID": self.val_quoted_string(attrid),
```

### Comparing `streamlink-5.3.1/tests/plugins/test_ustreamtv.py` & `streamlink-5.4.0/tests/plugins/test_ustreamtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_ustvnow.py` & `streamlink-5.4.0/tests/plugins/test_ustvnow.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_vimeo.py` & `streamlink-5.4.0/tests/plugins/test_vimeo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_vinhlongtv.py` & `streamlink-5.4.0/tests/plugins/test_vinhlongtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_vk.py` & `streamlink-5.4.0/tests/plugins/test_vk.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,93 @@
+from contextlib import nullcontext
+
 import pytest
 import requests_mock as rm
 
 from streamlink import Streamlink
 from streamlink.exceptions import NoStreamsError
 from streamlink.plugins.vk import VK
 from tests.plugins import PluginCanHandleUrl
 
 
+does_not_raise = nullcontext()
+
+
 class TestPluginCanHandleUrlVK(PluginCanHandleUrl):
     __plugin__ = VK
 
     should_match = [
-        "https://vk.com/video-9944999_456239622",
         "http://vk.com/video-24136539_456239830",
+        "http://vk.ru/video-24136539_456239830",
+        "https://vk.com/video-9944999_456239622",
+        "https://vk.ru/video-9944999_456239622",
         "https://www.vk.com/video-34453259_456240574",
+        "https://www.vk.ru/video-34453259_456240574",
         "https://vk.com/videos-24136539?z=video-24136539_456241155%2Fpl_-24136539_-2",
         "https://vk.com/video?z=video-15755094_456245149%2Fpl_cat_lives",
         "https://vk.com/video?z=video132886594_167211693%2Fpl_cat_8",
         "https://vk.com/video132886594_167211693",
         "https://vk.com/videos132886594?z=video132886594_167211693",
         "https://vk.com/video-73154028_456239128",
         "https://vk.com/dota2?w=wall-126093223_1057924",
         "https://vk.com/search?c%5Bq%5D=dota&c%5Bsection%5D=auto&z=video295508334_171402661",
     ]
 
     should_not_match = [
         "https://vk.com/",
+        "https://vk.ru/",
     ]
 
 
-@pytest.mark.parametrize(("url", "newurl"), [
+@pytest.mark.parametrize(("url", "newurl", "raises"), [
     # canonical video URL
     pytest.param(
         "https://vk.com/video-24136539_456241176",
         "https://vk.com/video-24136539_456241176",
+        does_not_raise,
     ),
 
     # video ID from URL
     pytest.param(
         "https://vk.com/videos-24136539?z=video-24136539_456241181%2Fpl_-24136539_-2",
         "https://vk.com/video-24136539_456241181",
+        does_not_raise,
     ),
     pytest.param(
         "https://vk.com/videos132886594?z=video132886594_167211693",
         "https://vk.com/video132886594_167211693",
+        does_not_raise,
     ),
     pytest.param(
         "https://vk.com/search?c%5Bq%5D=dota&c%5Bsection%5D=auto&z=video295508334_171402661",
         "https://vk.com/video295508334_171402661",
+        does_not_raise,
     ),
 
     # video ID from HTTP request
     pytest.param(
         "https://vk.com/dota2?w=wall-126093223_1057924",
         "https://vk.com/video-126093223_1057924",
+        does_not_raise,
     ),
 
     # no video ID
     pytest.param(
         "https://vk.com/videos-0123456789?z=",
         "",
-        marks=pytest.mark.xfail(raises=NoStreamsError),
+        pytest.raises(NoStreamsError),
     ),
     pytest.param(
         "https://vk.com/video/for_kids?z=video%2Fpl_-22277933_51053000",
         "",
-        marks=pytest.mark.xfail(raises=NoStreamsError),
+        pytest.raises(NoStreamsError),
     ),
 ])
-def test_url_redirect(url: str, newurl: str, requests_mock):
+def test_url_redirect(url: str, newurl: str, raises: nullcontext, requests_mock: rm.Mocker):
     session = Streamlink()
+    # noinspection PyTypeChecker
     plugin: VK = VK(session, url)
     requests_mock.register_uri(rm.ANY, rm.ANY, exc=rm.exceptions.InvalidRequest)
     requests_mock.get(url, text=f"""<!DOCTYPE html><html><head><meta property="og:url" content="{newurl}"/></head></html>""")
-    plugin.follow_vk_redirect()
-    assert plugin.url == newurl
+    with raises:
+        plugin.follow_vk_redirect()
+        assert plugin.url == newurl
```

### Comparing `streamlink-5.3.1/tests/plugins/test_vtvgo.py` & `streamlink-5.4.0/tests/plugins/test_vtvgo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_webtv.py` & `streamlink-5.4.0/tests/plugins/test_webtv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_welt.py` & `streamlink-5.4.0/tests/plugins/test_welt.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_youtube.py` & `streamlink-5.4.0/tests/plugins/test_youtube.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_zattoo.py` & `streamlink-5.4.0/tests/plugins/test_zattoo.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_zdf_mediathek.py` & `streamlink-5.4.0/tests/plugins/test_zdf_mediathek.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/plugins/test_zengatv.py` & `streamlink-5.4.0/tests/plugins/test_zengatv.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/__init__.py` & `streamlink-5.4.0/tests/resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                 el.tag = el.tag.split("}", 1)[1]
         return it.root
     except Exception as err:  # pragma: no cover
         snippet = repr(data)
         if len(snippet) > 35:
             snippet = f"{snippet[:35]} ..."
 
-        raise ValueError("Unable to parse XML: {0} ({1})".format(err, snippet))
+        raise ValueError(f"Unable to parse XML: {err} ({snippet})") from err
 
 
 @contextmanager
 def text(path, encoding="utf8"):
     with codecs.open(os.path.join(__here__, path), "r", encoding=encoding) as resource_fh:
         yield resource_fh
```

### Comparing `streamlink-5.3.1/tests/resources/dash/test_1.mpd` & `streamlink-5.4.0/tests/resources/dash/test_1.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/dash/test_10.mpd` & `streamlink-5.4.0/tests/resources/dash/test_10.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/dash/test_11_static.mpd` & `streamlink-5.4.0/tests/resources/dash/test_11_static.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/dash/test_2.mpd` & `streamlink-5.4.0/tests/resources/dash/test_2.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/dash/test_3.mpd` & `streamlink-5.4.0/tests/resources/dash/test_3.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/dash/test_4.mpd` & `streamlink-5.4.0/tests/resources/dash/test_segments_dynamic_number.mpd`

 * *Files 19% similar despite different names*

#### Comparing `streamlink-5.3.1/tests/resources/dash/test_4.mpd` & `streamlink-5.4.0/tests/resources/dash/test_segments_dynamic_number.mpd`

```diff
@@ -1,29 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
-<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="urn:mpeg:dash:schema:mpd:2011" xmlns:cenc="urn:mpeg:cenc:2013" xsi:schemaLocation="urn:mpeg:dash:schema:mpd:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" type="dynamic" publishTime="2018-05-10T09:27:09" minimumUpdatePeriod="PT10S" availabilityStartTime="2018-05-04T13:20:07Z" minBufferTime="PT2S" suggestedPresentationDelay="PT40S" timeShiftBufferDepth="PT24H0M0S" profiles="urn:mpeg:dash:profile:isoff-live:2011">
-  <Period start="PT0S" id="1">
+<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:cenc="urn:mpeg:cenc:2013" xmlns="urn:mpeg:dash:schema:mpd:2011" xsi:schemaLocation="urn:mpeg:dash:schema:mpd:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" type="dynamic" availabilityStartTime="2000-01-01T00:00:00Z" publishTime="2000-01-01T00:00:00Z" minimumUpdatePeriod="PT10S" minBufferTime="PT2S" suggestedPresentationDelay="PT40S" timeShiftBufferDepth="PT24H0M0S" profiles="urn:mpeg:dash:profile:isoff-live:2011">
+  <Period id="1" start="PT1M30S">
     <AdaptationSet mimeType="video/mp4" frameRate="25/1" segmentAlignment="true" subsegmentAlignment="true" startWithSAP="1" subsegmentStartsWithSAP="1" bitstreamSwitching="false">
-      <SegmentTemplate timescale="90000" duration="450000" startNumber="1"/>
+      <SegmentTemplate timescale="90000" duration="450000" startNumber="100"/>
       <Representation id="1" width="1280" height="720" bandwidth="2400000" codecs="avc1.64001f">
-        <SegmentTemplate duration="450000" startNumber="1" media="hd-5_$Number%09d$.mp4" initialization="hd-5-init.mp4"/>
+        <SegmentTemplate media="hd-5_$Number%09d$.mp4" initialization="hd-5-init.mp4"/>
       </Representation>
       <Representation id="2" width="1280" height="720" bandwidth="1250000" codecs="avc1.64001f">
-        <SegmentTemplate duration="450000" startNumber="1" media="hd-4_$Number%09d$.mp4" initialization="hd-4-init.mp4"/>
+        <SegmentTemplate media="hd-4_$Number%09d$.mp4" initialization="hd-4-init.mp4"/>
       </Representation>
       <Representation id="3" width="640" height="360" bandwidth="950000" codecs="avc1.4d401e">
-        <SegmentTemplate duration="450000" startNumber="1" media="hd-3_$Number%09d$.mp4" initialization="hd-3-init.mp4"/>
+        <SegmentTemplate media="hd-3_$Number%09d$.mp4" initialization="hd-3-init.mp4"/>
       </Representation>
       <Representation id="4" width="640" height="360" bandwidth="650000" codecs="avc1.4d401e">
-        <SegmentTemplate duration="450000" startNumber="1" media="hd-2_$Number%09d$.mp4" initialization="hd-2-init.mp4"/>
+        <SegmentTemplate media="hd-2_$Number%09d$.mp4" initialization="hd-2-init.mp4"/>
       </Representation>
       <Representation id="5" width="640" height="360" bandwidth="350000" codecs="avc1.4d401e">
-        <SegmentTemplate duration="450000" startNumber="1" media="hd-1_$Number%09d$.mp4" initialization="hd-1-init.mp4"/>
+        <SegmentTemplate media="hd-1_$Number%09d$.mp4" initialization="hd-1-init.mp4"/>
       </Representation>
       <Representation id="6" width="160" height="90" bandwidth="110000" codecs="avc1.4d400b">
-        <SegmentTemplate duration="450000" startNumber="1" media="hd-0_$Number%09d$.mp4" initialization="hd-0-init.mp4"/>
+        <SegmentTemplate media="hd-0_$Number%09d$.mp4" initialization="hd-0-init.mp4"/>
       </Representation>
     </AdaptationSet>
     <AdaptationSet mimeType="audio/mp4" lang="rus" segmentAlignment="0">
       <SegmentTemplate timescale="48000" media="hd-audio_$Number%09d$.mp4" initialization="hd-audio-init.mp4" duration="240000" startNumber="1"/>
       <Representation id="7" bandwidth="96000" audioSamplingRate="48000" codecs="mp4a.40.2"/>
     </AdaptationSet>
     <AdaptationSet mimeType="application/mp4" lang="rus">
```

### Comparing `streamlink-5.3.1/tests/resources/dash/test_5.mpd` & `streamlink-5.4.0/tests/resources/dash/test_static_no_publish_time.mpd`

 * *Files 4% similar despite different names*

#### Comparing `streamlink-5.3.1/tests/resources/dash/test_5.mpd` & `streamlink-5.4.0/tests/resources/dash/test_static_no_publish_time.mpd`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- Created with Unified Streaming Platform(version=1.7.10) -->
-<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="urn:mpeg:dash:schema:mpd:2011" xsi:schemaLocation="urn:mpeg:dash:schema:mpd:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" type="static" mediaPresentationDuration="PT1M23.847347S" maxSegmentDuration="PT3S" minBufferTime="PT10S" profiles="urn:mpeg:dash:profile:isoff-live:2011">
-  <Period>
+<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="urn:mpeg:dash:schema:mpd:2011" xsi:schemaLocation="urn:mpeg:dash:schema:mpd:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" type="static" availabilityStartTime="2020-01-01T00:00:00Z" mediaPresentationDuration="PT1M23.847347S" maxSegmentDuration="PT3S" minBufferTime="PT10S" profiles="urn:mpeg:dash:profile:isoff-live:2011">
+  <Period start="PT12M34S">
     <BaseURL>dash/</BaseURL>
     <AdaptationSet group="1" contentType="audio" lang="en" minBandwidth="128000" maxBandwidth="152000" segmentAlignment="true" audioSamplingRate="44100" mimeType="audio/mp4" codecs="mp4a.40.2">
       <AudioChannelConfiguration schemeIdUri="urn:mpeg:dash:23003:3:audio_channel_configuration:2011" value="2"/>
       <SegmentTemplate timescale="44100" initialization="150633-$RepresentationID$.dash" media="150633-$RepresentationID$-$Time$.dash" startNumber="1">
         <SegmentTimeline>
           <S t="0" d="90113"/>
           <S d="88064" r="5"/>
```

### Comparing `streamlink-5.3.1/tests/resources/dash/test_6_p1.mpd` & `streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

 * *Files 3% similar despite different names*

#### Comparing `streamlink-5.3.1/tests/resources/dash/test_6_p1.mpd` & `streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p1.mpd`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<MPD xmlns="urn:mpeg:dash:schema:mpd:2011" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" type="dynamic" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-live:2011" minBufferTime="PT5S" suggestedPresentationDelay="PT5S" availabilityStartTime="2018-01-01T00:00:00Z" publishTime="2018-01-01T13:00:00Z" minimumUpdatePeriod="PT5S" maxSegmentDuration="PT1S" timeShiftBufferDepth="PT30S">
-  <Location>http://test.se/</Location>
+<MPD xmlns="urn:mpeg:dash:schema:mpd:2011" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-live:2011" type="dynamic" minBufferTime="PT5S" suggestedPresentationDelay="PT5S" availabilityStartTime="2018-01-01T00:00:00Z" publishTime="2018-01-01T13:00:00Z" minimumUpdatePeriod="PT5S" maxSegmentDuration="PT1S" timeShiftBufferDepth="PT30S">
+  <Location>http://test/</Location>
   <Period id="1" start="PT3600.0S">
     <AdaptationSet mimeType="video/mp4" contentType="video" id="4" maxWidth="1920" maxHeight="1080" maxFrameRate="25" segmentAlignment="true" startWithSAP="1" subsegmentAlignment="true" subsegmentStartsWithSAP="1">
       <Representation id="video" width="512" height="288" bandwidth="505000" codecs="avc1.420015">
         <SegmentTemplate initialization="$RepresentationID$/init.mp4" media="$RepresentationID$/$Time$.mp4" timescale="1000">
           <SegmentTimeline>
             <S t="1000000" d="1000" r="10"/>
           </SegmentTimeline>
```

### Comparing `streamlink-5.3.1/tests/resources/dash/test_6_p2.mpd` & `streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

 * *Files 4% similar despite different names*

#### Comparing `streamlink-5.3.1/tests/resources/dash/test_6_p2.mpd` & `streamlink-5.4.0/tests/resources/dash/test_dynamic_timeline_continued_p2.mpd`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<MPD xmlns="urn:mpeg:dash:schema:mpd:2011" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" type="dynamic" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-live:2011" minBufferTime="PT5S" suggestedPresentationDelay="PT5S" availabilityStartTime="2018-01-01T00:00:00Z" publishTime="2018-01-01T13:00:05Z" minimumUpdatePeriod="PT5S" maxSegmentDuration="PT1S" timeShiftBufferDepth="PT30S">
-  <Location>http://test.se/</Location>
+<MPD xmlns="urn:mpeg:dash:schema:mpd:2011" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-live:2011" type="dynamic" minBufferTime="PT5S" suggestedPresentationDelay="PT5S" availabilityStartTime="2018-01-01T00:00:00Z" publishTime="2018-01-01T13:00:05Z" minimumUpdatePeriod="PT5S" maxSegmentDuration="PT1S" timeShiftBufferDepth="PT30S">
+  <Location>http://test/</Location>
   <Period id="1" start="PT3600.0S">
     <AdaptationSet mimeType="video/mp4" contentType="video" id="4" maxWidth="1920" maxHeight="1080" maxFrameRate="25" segmentAlignment="true" startWithSAP="1" subsegmentAlignment="true" subsegmentStartsWithSAP="1">
       <Representation id="video" width="512" height="288" bandwidth="505000" codecs="avc1.420015">
         <SegmentTemplate initialization="$RepresentationID$/init.mp4" media="$RepresentationID$/$Time$.mp4" timescale="1000">
           <SegmentTimeline>
             <S t="1005000" d="1000" r="10"/>
           </SegmentTimeline>
```

### Comparing `streamlink-5.3.1/tests/resources/dash/test_7.mpd` & `streamlink-5.4.0/tests/resources/dash/test_segment_list.mpd`

 * *Files 10% similar despite different names*

#### Comparing `streamlink-5.3.1/tests/resources/dash/test_7.mpd` & `streamlink-5.4.0/tests/resources/dash/test_segment_list.mpd`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
-<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="urn:mpeg:dash:schema:mpd:2011" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-main:2011" type="static" publishTime="2018-06-25T18:01:58Z" mediaPresentationDuration="PT53M18.059S" minBufferTime="PT1.5S">
+<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns="urn:mpeg:dash:schema:mpd:2011" xmlns:xlink="http://www.w3.org/1999/xlink" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-main:2011" type="static" availabilityStartTime="2020-01-01T00:00:00Z" publishTime="2018-06-25T18:01:58Z" mediaPresentationDuration="PT53M18.059S" minBufferTime="PT1.5S">
   <ProgramInformation>
     <Title>test/dash.smil</Title>
   </ProgramInformation>
-  <Period id="0" start="PT0.0S">
+  <Period id="0" start="PT12M34S">
     <AdaptationSet id="0" group="1" mimeType="video/mp4" maxWidth="1920" maxHeight="1080" par="16:9" frameRate="25" segmentAlignment="true" startWithSAP="1" subsegmentAlignment="true" subsegmentStartsWithSAP="1">
       <Representation id="p0va0br4332748" codecs="avc1.640028" width="1920" height="1080" sar="1:1" bandwidth="4332748">
         <SegmentList presentationTimeOffset="0" timescale="90000" duration="900000" startNumber="1">
           <Initialization sourceURL="chunk_ctvideo_ridp0va0br4332748_cinit_mpd.m4s"/>
           <SegmentURL media="chunk_ctvideo_ridp0va0br4332748_cn1_mpd.m4s"/>
           <SegmentURL media="chunk_ctvideo_ridp0va0br4332748_cn2_mpd.m4s"/>
           <SegmentURL media="chunk_ctvideo_ridp0va0br4332748_cn3_mpd.m4s"/>
```

### Comparing `streamlink-5.3.1/tests/resources/dash/test_8.mpd` & `streamlink-5.4.0/tests/resources/dash/test_8.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/dash/test_9.mpd` & `streamlink-5.4.0/tests/resources/dash/test_9.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-5.4.0/tests/resources/dash/test_nested_baseurls.mpd`

 * *Files 2% similar despite different names*

#### Comparing `streamlink-5.3.1/tests/resources/dash/test_nested_baseurls.mpd` & `streamlink-5.4.0/tests/resources/dash/test_nested_baseurls.mpd`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
-<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="urn:mpeg:dash:schema:mpd:2011" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-live:2011" type="static" mediaPresentationDuration="PT0H0M6.00S" minBufferTime="PT6.0S">
+<MPD xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns="urn:mpeg:dash:schema:mpd:2011" xsi:schemaLocation="urn:mpeg:DASH:schema:MPD:2011 http://standards.iso.org/ittf/PubliclyAvailableStandards/MPEG-DASH_schema_files/DASH-MPD.xsd" profiles="urn:mpeg:dash:profile:isoff-live:2011" type="static" availabilityStartTime="2020-01-01T00:00:00Z" mediaPresentationDuration="PT0H0M6.00S" minBufferTime="PT6.0S">
   <BaseURL>https://hostname/</BaseURL>
-  <Period id="0" start="PT0.0S">
+  <Period id="0" start="PT12M34S">
     <BaseURL>period/</BaseURL>
     <AdaptationSet id="0" mimeType="video/mp4" maxWidth="1920" maxHeight="1080" par="16:9" frameRate="60" segmentAlignment="true" startWithSAP="1" subsegmentAlignment="true" subsegmentStartsWithSAP="1">
       <SegmentTemplate presentationTimeOffset="0" timescale="90000" duration="540000" startNumber="1" media="media_$RepresentationID$-$Number$.m4s" initialization="init_$RepresentationID$.m4s"/>
       <Representation id="video_5000kbps" codecs="avc1.640028" width="1920" height="1080" sar="1:1" bandwidth="5000000"/>
       <Representation id="video_9000kbps" codecs="avc1.640028" width="1920" height="1080" sar="1:1" bandwidth="9000000">
         <BaseURL>representation/</BaseURL>
       </Representation>
```

### Comparing `streamlink-5.3.1/tests/resources/dash/test_segments_byterange.mpd` & `streamlink-5.4.0/tests/resources/dash/test_segments_byterange.mpd`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/hls/test_1.m3u8` & `streamlink-5.4.0/tests/resources/hls/test_1.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/hls/test_2.m3u8` & `streamlink-5.4.0/tests/resources/hls/test_2.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/hls/test_date.m3u8` & `streamlink-5.4.0/tests/resources/hls/test_date.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/hls/test_master.m3u8` & `streamlink-5.4.0/tests/resources/hls/test_master.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/resources/hls/test_master_twitch_vod.m3u8` & `streamlink-5.4.0/tests/resources/hls/test_master_twitch_vod.m3u8`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/stream/test_dash.py` & `streamlink-5.4.0/tests/stream/test_dash.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,294 +1,305 @@
-import unittest
+from datetime import datetime, timezone
 from typing import List
-from unittest.mock import ANY, MagicMock, Mock, call, patch
+from unittest.mock import ANY, Mock, call
 
+import freezegun
 import pytest
+import requests_mock as rm
+from lxml.etree import ParseError
 
-from streamlink import PluginError
+from streamlink.exceptions import PluginError
+from streamlink.session import Streamlink
 from streamlink.stream.dash import DASHStream, DASHStreamWorker
-from streamlink.stream.dash_manifest import MPD
+from streamlink.stream.dash_manifest import MPD, MPDParsingError
+from streamlink.utils.parse import parse_xml as original_parse_xml
 from tests.resources import text, xml
 
 
-class TestDASHStream(unittest.TestCase):
-    def setUp(self):
-        self.session = MagicMock()
-        self.test_url = "http://test.bar/foo.mpd"
-        self.session.http.get.return_value = Mock(url=self.test_url)
+@pytest.fixture()
+def timestamp():
+    with freezegun.freeze_time("2000-01-01T00:00:00Z"):
+        yield datetime.now(timezone.utc)
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_video_only(self, mpdClass):
+
+class TestDASHStreamParseManifest:
+    @pytest.fixture(autouse=True)
+    def _response(self, request: pytest.FixtureRequest, requests_mock: rm.Mocker):
+        invalid = requests_mock.register_uri(rm.ANY, rm.ANY, exc=rm.exceptions.InvalidRequest("Invalid request"))
+        response = requests_mock.register_uri("GET", "http://test/manifest.mpd", **getattr(request, "param", {}))
+        called_once = "nomockedhttprequest" not in request.keywords
+        yield
+        assert not invalid.called
+        assert response.called_once is called_once
+
+    @pytest.fixture()
+    def parse_xml(self, monkeypatch: pytest.MonkeyPatch):
+        parse_xml = Mock(return_value=Mock())
+        monkeypatch.setattr("streamlink.stream.dash.parse_xml", parse_xml)
+        return parse_xml
+
+    @pytest.fixture()
+    def mpd(self, monkeypatch: pytest.MonkeyPatch, parse_xml: Mock):
+        mpd = Mock()
+        monkeypatch.setattr("streamlink.stream.dash.MPD", mpd)
+        return mpd
+
+    @pytest.mark.parametrize(("se_parse_xml", "se_mpd"), [
+        (ParseError, None),
+        (None, MPDParsingError),
+    ])
+    def test_parse_fail(self, session: Streamlink, mpd: Mock, parse_xml: Mock, se_parse_xml, se_mpd):
+        parse_xml.side_effect = se_parse_xml
+        mpd.side_effect = se_mpd
+
+        with pytest.raises(PluginError) as cm:
+            DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert str(cm.value).startswith("Failed to parse MPD manifest: ")
+
+    def test_video_only(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=720),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080),
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["720p", "1080p"])
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_audio_only(self, mpdClass):
+    def test_audio_only(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="audio/mp4", bandwidth=128.0, lang="en"),
-                Mock(id="2", contentProtection=None, mimeType="audio/mp4", bandwidth=256.0, lang="en"),
+                Mock(id="1", contentProtections=None, mimeType="audio/mp4", bandwidth=128.0, lang="en"),
+                Mock(id="2", contentProtections=None, mimeType="audio/mp4", bandwidth=256.0, lang="en"),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["a128k", "a256k"])
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_audio_single(self, mpdClass):
+    def test_audio_single(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=720),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080),
-                Mock(id="3", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
+                Mock(id="3", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["720p", "1080p"])
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_audio_multi(self, mpdClass):
+    def test_audio_multi(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=720),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080),
-                Mock(id="3", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
-                Mock(id="4", contentProtection=None, mimeType="audio/aac", bandwidth=256.0, lang="en"),
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
+                Mock(id="3", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
+                Mock(id="4", contentProtections=None, mimeType="audio/aac", bandwidth=256.0, lang="en"),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["720p+a128k", "1080p+a128k", "720p+a256k", "1080p+a256k"])
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_audio_multi_lang(self, mpdClass):
+    def test_audio_multi_lang(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=720),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080),
-                Mock(id="3", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
-                Mock(id="4", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="es"),
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
+                Mock(id="3", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
+                Mock(id="4", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="es"),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["720p", "1080p"])
+        assert getattr(streams["720p"].audio_representation, "lang", None) == "en"
+        assert getattr(streams["1080p"].audio_representation, "lang", None) == "en"
 
-        assert streams["720p"].audio_representation.lang == "en"
-        assert streams["1080p"].audio_representation.lang == "en"
-
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_audio_multi_lang_alpha3(self, mpdClass):
+    def test_audio_multi_lang_alpha3(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=720),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080),
-                Mock(id="3", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="eng"),
-                Mock(id="4", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="spa"),
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
+                Mock(id="3", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="eng"),
+                Mock(id="4", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="spa"),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["720p", "1080p"])
+        assert getattr(streams["720p"].audio_representation, "lang", None) == "eng"
+        assert getattr(streams["1080p"].audio_representation, "lang", None) == "eng"
 
-        assert streams["720p"].audio_representation.lang == "eng"
-        assert streams["1080p"].audio_representation.lang == "eng"
-
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_audio_invalid_lang(self, mpdClass):
+    def test_audio_invalid_lang(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=720),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080),
-                Mock(id="3", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="en_no_voice"),
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
+                Mock(id="3", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="en_no_voice"),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["720p", "1080p"])
+        assert getattr(streams["720p"].audio_representation, "lang", None) == "en_no_voice"
+        assert getattr(streams["1080p"].audio_representation, "lang", None) == "en_no_voice"
 
-        assert streams["720p"].audio_representation.lang == "en_no_voice"
-        assert streams["1080p"].audio_representation.lang == "en_no_voice"
-
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_audio_multi_lang_locale(self, mpdClass):
-        self.session.localization.language.alpha2 = "es"
-        self.session.localization.explicit = True
+    def test_audio_multi_lang_locale(self, monkeypatch: pytest.MonkeyPatch, session: Streamlink, mpd: Mock):
+        session.set_option("locale", "es_ES")
 
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=720),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080),
-                Mock(id="3", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
-                Mock(id="4", contentProtection=None, mimeType="audio/aac", bandwidth=128.0, lang="es"),
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=720),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080),
+                Mock(id="3", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="en"),
+                Mock(id="4", contentProtections=None, mimeType="audio/aac", bandwidth=128.0, lang="es"),
             ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
         assert sorted(streams.keys()) == sorted(["720p", "1080p"])
+        assert getattr(streams["720p"].audio_representation, "lang", None) == "es"
+        assert getattr(streams["1080p"].audio_representation, "lang", None) == "es"
 
-        assert streams["720p"].audio_representation.lang == "es"
-        assert streams["1080p"].audio_representation.lang == "es"
-
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_drm_adaptationset(self, mpdClass):
+    # Verify the fix for https://github.com/streamlink/streamlink/issues/3365
+    def test_duplicated_resolutions(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection="DRM",
-            representations=[],
+            contentProtections=None,
+            representations=[
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=1080, bandwidth=128.0),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080, bandwidth=64.0),
+                Mock(id="3", contentProtections=None, mimeType="video/mp4", height=1080, bandwidth=32.0),
+                Mock(id="4", contentProtections=None, mimeType="video/mp4", height=720),
+            ],
         )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
-        with pytest.raises(PluginError):
-            DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
+        assert sorted(streams.keys()) == sorted(["720p", "1080p", "1080p_alt", "1080p_alt2"])
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_drm_representation(self, mpdClass):
+    # Verify the fix for https://github.com/streamlink/streamlink/issues/4217
+    def test_duplicated_resolutions_sorted_bandwidth(self, session: Streamlink, mpd: Mock):
         adaptationset = Mock(
-            contentProtection=None,
+            contentProtections=None,
             representations=[
-                Mock(id="1", contentProtection="DRM"),
-            ],
-        )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
+                Mock(id="1", contentProtections=None, mimeType="video/mp4", height=1080, bandwidth=64.0),
+                Mock(id="2", contentProtections=None, mimeType="video/mp4", height=1080, bandwidth=128.0),
+                Mock(id="3", contentProtections=None, mimeType="video/mp4", height=1080, bandwidth=32.0),
+            ],
+        )
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
+
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
+        assert getattr(streams["1080p"].video_representation, "bandwidth", None) == pytest.approx(128.0)
+        assert getattr(streams["1080p_alt"].video_representation, "bandwidth", None) == pytest.approx(64.0)
+        assert getattr(streams["1080p_alt2"].video_representation, "bandwidth", None) == pytest.approx(32.0)
+
+    @pytest.mark.parametrize("adaptationset", [
+        pytest.param(
+            Mock(contentProtections="DRM", representations=[]),
+            id="ContentProtection on AdaptationSet",
+        ),
+        pytest.param(
+            Mock(contentProtections=None, representations=[Mock(id="1", contentProtections="DRM")]),
+            id="ContentProtection on Representation",
+        ),
+    ])
+    def test_contentprotection(self, session: Streamlink, mpd: Mock, adaptationset: Mock):
+        mpd.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
 
         with pytest.raises(PluginError):
-            DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+            DASHStream.parse_manifest(session, "http://test/manifest.mpd")
 
-    def test_parse_manifest_string(self):
+    @pytest.mark.nomockedhttprequest()
+    def test_string(self, session: Streamlink, mpd: Mock, parse_xml: Mock):
         with text("dash/test_9.mpd") as mpd_txt:
             test_manifest = mpd_txt.read()
+        parse_xml.side_effect = original_parse_xml
+        mpd.side_effect = MPD
 
-        streams = DASHStream.parse_manifest(self.session, test_manifest)
-        assert list(streams.keys()) == ["2500k"]
-
-    @patch("streamlink.stream.dash.DASHStreamReader")
-    @patch("streamlink.stream.dash.FFMPEGMuxer")
-    def test_stream_open_video_only(self, muxer, reader):
-        stream = DASHStream(self.session, Mock(), Mock(id=1, mimeType="video/mp4"))
-        open_reader = reader.return_value = Mock()
-
-        stream.open()
-
-        reader.assert_called_with(stream, 1, "video/mp4")
-        open_reader.open.assert_called_with()
-        muxer.assert_not_called()
-
-    @patch("streamlink.stream.dash.DASHStreamReader")
-    @patch("streamlink.stream.dash.FFMPEGMuxer")
-    def test_stream_open_video_audio(self, muxer, reader):
-        stream = DASHStream(self.session, Mock(), Mock(id=1, mimeType="video/mp4"), Mock(id=2, mimeType="audio/mp3", lang="en"))
-        open_reader = reader.return_value = Mock()
-
-        stream.open()
-
-        assert reader.mock_calls == [
-            call(stream, 1, "video/mp4"),
-            call().open(),
-            call(stream, 2, "audio/mp3"),
-            call().open(),
-        ]
-        assert muxer.mock_calls == [
-            call(self.session, open_reader, open_reader, copyts=True),
-            call().open(),
-        ]
-
-    @patch("streamlink.stream.dash.MPD")
-    def test_segments_number_time(self, mpdClass):
+        streams = DASHStream.parse_manifest(session, test_manifest)
+        assert mpd.call_args_list == [call(ANY)]
+        assert list(streams.keys()) == ["480p"]
+
+    # TODO: Move this test to test_dash_parser and properly test segment URLs.
+    #       This test currently achieves nothing... (manifest fixture added in 7aada92)
+    def test_segments_number_time(self, session: Streamlink, mpd: Mock):
         with xml("dash/test_9.mpd") as mpd_xml:
-            mpdClass.return_value = MPD(mpd_xml, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+            mpd.return_value = MPD(mpd_xml, base_url="http://test", url="http://test/manifest.mpd")
 
-            streams = DASHStream.parse_manifest(self.session, self.test_url)
-            mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        streams = DASHStream.parse_manifest(session, "http://test/manifest.mpd")
+        assert mpd.call_args_list == [call(ANY, url="http://test/manifest.mpd", base_url="http://test")]
+        assert list(streams.keys()) == ["480p"]
 
-            assert list(streams.keys()) == ["2500k"]
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_with_duplicated_resolutions(self, mpdClass):
-        """
-            Verify the fix for https://github.com/streamlink/streamlink/issues/3365
-        """
-        adaptationset = Mock(
-            contentProtection=None,
-            representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=1080, bandwidth=128.0),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080, bandwidth=64.0),
-                Mock(id="3", contentProtection=None, mimeType="video/mp4", height=1080, bandwidth=32.0),
-                Mock(id="4", contentProtection=None, mimeType="video/mp4", height=720),
-            ],
-        )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
-
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
-
-        assert sorted(streams.keys()) == sorted(["720p", "1080p", "1080p_alt", "1080p_alt2"])
+class TestDASHStreamOpen:
+    @pytest.fixture()
+    def reader(self, monkeypatch: pytest.MonkeyPatch):
+        reader = Mock()
+        monkeypatch.setattr("streamlink.stream.dash.DASHStreamReader", reader)
+        return reader
 
-    @patch("streamlink.stream.dash.MPD")
-    def test_parse_manifest_with_duplicated_resolutions_sorted_bandwidth(self, mpdClass):
-        """
-            Verify the fix for https://github.com/streamlink/streamlink/issues/4217
-        """
-        adaptationset = Mock(
-            contentProtection=None,
-            representations=[
-                Mock(id="1", contentProtection=None, mimeType="video/mp4", height=1080, bandwidth=64.0),
-                Mock(id="2", contentProtection=None, mimeType="video/mp4", height=1080, bandwidth=128.0),
-                Mock(id="3", contentProtection=None, mimeType="video/mp4", height=1080, bandwidth=32.0),
-            ],
-        )
-        mpdClass.return_value = Mock(periods=[Mock(adaptationSets=[adaptationset])])
+    @pytest.fixture()
+    def muxer(self, monkeypatch: pytest.MonkeyPatch):
+        muxer = Mock()
+        monkeypatch.setattr("streamlink.stream.dash.FFMPEGMuxer", muxer)
+        return muxer
+
+    def test_stream_open_video_only(self, session: Streamlink, timestamp: datetime, muxer: Mock, reader: Mock):
+        rep_video = Mock(ident=(None, None, "1"), mimeType="video/mp4")
+        stream = DASHStream(session, Mock(), rep_video)
+        stream.open()
 
-        streams = DASHStream.parse_manifest(self.session, self.test_url)
-        mpdClass.assert_called_with(ANY, base_url="http://test.bar", url="http://test.bar/foo.mpd")
+        assert reader.call_args_list == [call(stream, rep_video, timestamp)]
+        reader_video = reader(stream, rep_video, timestamp)
+        assert reader_video.open.called_once
+        assert muxer.call_args_list == []
+
+    def test_stream_open_video_audio(self, session: Streamlink, timestamp: datetime, muxer: Mock, reader: Mock):
+        rep_video = Mock(ident=(None, None, "1"), mimeType="video/mp4")
+        rep_audio = Mock(ident=(None, None, "2"), mimeType="audio/mp3", lang="en")
+        stream = DASHStream(session, Mock(), rep_video, rep_audio)
+        stream.open()
 
-        assert streams["1080p"].video_representation.bandwidth == pytest.approx(128.0)
-        assert streams["1080p_alt"].video_representation.bandwidth == pytest.approx(64.0)
-        assert streams["1080p_alt2"].video_representation.bandwidth == pytest.approx(32.0)
+        assert reader.call_args_list == [call(stream, rep_video, timestamp), call(stream, rep_audio, timestamp)]
+        reader_video = reader(stream, rep_video, timestamp)
+        reader_audio = reader(stream, rep_audio, timestamp)
+        assert reader_video.open.called_once
+        assert reader_audio.open.called_once
+        assert muxer.call_args_list == [call(session, reader_video, reader_audio, copyts=True)]
+        assert reader_video.timestamp is reader_audio.timestamp
 
 
 class TestDASHStreamWorker:
     @pytest.fixture()
     def mock_time(self, monkeypatch: pytest.MonkeyPatch) -> Mock:
         mock = Mock(return_value=1)
         monkeypatch.setattr("streamlink.stream.dash.time", mock)
@@ -297,135 +308,125 @@
     @pytest.fixture(autouse=True)
     def mock_wait(self, monkeypatch: pytest.MonkeyPatch) -> Mock:
         mock = Mock(return_value=True)
         monkeypatch.setattr("streamlink.stream.dash.DASHStreamWorker.wait", mock)
         return mock
 
     @pytest.fixture()
-    def representation(self) -> Mock:
-        return Mock(id=1, mimeType="video/mp4", height=720)
-
-    @pytest.fixture()
     def segments(self) -> List[Mock]:
         return [
             Mock(url="init_segment"),
             Mock(url="first_segment"),
             Mock(url="second_segment"),
         ]
 
     @pytest.fixture()
-    def mpd(self, representation) -> Mock:
+    def mpd(self) -> Mock:
+        representation = Mock(
+            ident=(None, None, "1"),
+            mimeType="video/mp4",
+            height=720,
+        )
+        adaptationset = Mock(
+            contentProtections=None,
+            representations=[representation],
+        )
+        period = Mock(
+            duration=Mock(total_seconds=Mock(return_value=0)),
+            adaptationSets=[adaptationset],
+        )
+        representation.period = period
+
         return Mock(
             publishTime=1,
             minimumUpdatePeriod=Mock(total_seconds=Mock(return_value=0)),
-            periods=[
-                Mock(
-                    duration=Mock(total_seconds=Mock(return_value=0)),
-                    adaptationSets=[
-                        Mock(
-                            contentProtection=None,
-                            representations=[representation],
-                        ),
-                    ],
-                ),
-            ],
+            periods=[period],
+            get_representation=Mock(return_value=representation),
         )
 
     @pytest.fixture()
-    def worker(self, mpd):
-        reader = MagicMock(representation_id=1, mime_type="video/mp4")
+    def representation(self, mpd) -> Mock:
+        return mpd.periods[0].adaptationSets[0].representations[0]
+
+    @pytest.fixture()
+    def worker(self, timestamp: datetime, mpd: Mock):
+        stream = Mock(
+            mpd=mpd,
+            period=0,
+            args={},
+        )
+        reader = Mock(
+            stream=stream,
+            ident=(None, None, "1"),
+            timestamp=timestamp,
+        )
         worker = DASHStreamWorker(reader)
-        worker.mpd = mpd
+
         return worker
 
     def test_dynamic_reload(
         self,
         monkeypatch: pytest.MonkeyPatch,
+        timestamp: datetime,
         worker: DASHStreamWorker,
         representation: Mock,
         segments: List[Mock],
         mpd: Mock,
     ):
         mpd.dynamic = True
         mpd.type = "dynamic"
         monkeypatch.setattr("streamlink.stream.dash.MPD", lambda *args, **kwargs: mpd)
 
         segment_iter = worker.iter_segments()
 
         representation.segments.return_value = segments[:1]
         assert next(segment_iter) is segments[0]
-        assert representation.segments.call_args_list == [call(init=True)]
+        assert representation.segments.call_args_list == [call(init=True, timestamp=timestamp)]
         assert not worker._wait.is_set()
 
         representation.segments.reset_mock()
         representation.segments.return_value = segments[1:]
         assert [next(segment_iter), next(segment_iter)] == segments[1:]
-        assert representation.segments.call_args_list == [call(), call(init=False)]
+        assert representation.segments.call_args_list == [call(), call(init=False, timestamp=None)]
         assert not worker._wait.is_set()
 
     def test_static(
         self,
         worker: DASHStreamWorker,
+        timestamp: datetime,
         representation: Mock,
         segments: List[Mock],
         mpd: Mock,
     ):
         mpd.dynamic = False
         mpd.type = "static"
 
         representation.segments.return_value = segments
         assert list(worker.iter_segments()) == segments
-        assert representation.segments.call_args_list == [call(init=True)]
+        assert representation.segments.call_args_list == [call(init=True, timestamp=timestamp)]
         assert worker._wait.is_set()
 
+    # Verify the fix for https://github.com/streamlink/streamlink/issues/2873
     @pytest.mark.parametrize("duration", [
         0,
         204.32,
     ])
     def test_static_refresh_wait(
         self,
-        duration: float,
+        timestamp: datetime,
         mock_wait: Mock,
         mock_time: Mock,
         worker: DASHStreamWorker,
         representation: Mock,
         segments: List[Mock],
         mpd: Mock,
+        duration: float,
     ):
-        """
-            Verify the fix for https://github.com/streamlink/streamlink/issues/2873
-        """
         mpd.dynamic = False
         mpd.type = "static"
         mpd.periods[0].duration.total_seconds.return_value = duration
 
         representation.segments.return_value = segments
         assert list(worker.iter_segments()) == segments
-        assert representation.segments.call_args_list == [call(init=True)]
+        assert representation.segments.call_args_list == [call(init=True, timestamp=timestamp)]
         assert mock_wait.call_args_list == [call(5)]
         assert worker._wait.is_set()
-
-    def test_duplicate_rep_id(self):
-        representation_vid = Mock(id=1, mimeType="video/mp4", height=720)
-        representation_aud = Mock(id=1, mimeType="audio/aac", lang="en")
-
-        mpd = Mock(
-            dynamic=False,
-            publishTime=1,
-            periods=[
-                Mock(
-                    adaptationSets=[
-                        Mock(
-                            contentProtection=None,
-                            representations=[representation_vid],
-                        ),
-                        Mock(
-                            contentProtection=None,
-                            representations=[representation_aud],
-                        ),
-                    ],
-                ),
-            ],
-        )
-
-        assert DASHStreamWorker.get_representation(mpd, 1, "video/mp4") is representation_vid
-        assert DASHStreamWorker.get_representation(mpd, 1, "audio/aac") is representation_aud
```

### Comparing `streamlink-5.3.1/tests/stream/test_ffmpegmux.py` & `streamlink-5.4.0/tests/stream/test_ffmpegmux.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
 @pytest.fixture(autouse=True)
 def _logger(caplog: pytest.LogCaptureFixture):
     caplog.set_level(1, "streamlink")
 
 
 @pytest.fixture()
-def session():
-    with patch("streamlink.session.Streamlink.load_builtin_plugins"):
-        yield Streamlink({"ffmpeg-no-validation": True})
+def session(session: Streamlink):
+    session.set_option("ffmpeg-no-validation", True)
+
+    return session
 
 
 class TestCommand:
     def test_cache(self, session: Streamlink):
         with patch("streamlink.stream.ffmpegmux.which", return_value="some_value") as mock:
             assert FFMPEGMuxer.command(session) == "some_value"
             assert FFMPEGMuxer.command(session) == "some_value"
```

### Comparing `streamlink-5.3.1/tests/stream/test_file.py` & `streamlink-5.4.0/tests/stream/test_file.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/stream/test_hls.py` & `streamlink-5.4.0/tests/stream/test_hls.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from threading import Event
 from unittest.mock import Mock, call, patch
 
 import pytest
 import requests_mock
 from Crypto.Cipher import AES
 from Crypto.Util.Padding import pad
+from requests.exceptions import InvalidSchema
 
 from streamlink.session import Streamlink
-from streamlink.stream.hls import HLSStream, HLSStreamReader
+from streamlink.stream.hls import HLSStream, HLSStreamReader, MuxedHLSStream
 from streamlink.stream.hls_playlist import M3U8Parser
 from tests.mixins.stream_hls import EventedHLSStreamWriter, Playlist, Segment, Tag, TestMixinStreamHLS
 from tests.resources import text
 
 
 class EncryptedBase:
     content: bytes
@@ -129,14 +130,22 @@
 class TestHLSStream(TestMixinStreamHLS, unittest.TestCase):
     def get_session(self, options=None, *args, **kwargs):
         session = super().get_session(options)
         session.set_option("hls-live-edge", 3)
 
         return session
 
+    def test_playlist_end(self):
+        thread, segments = self.subject([
+            # media sequence = 0
+            Playlist(0, [Segment(0)], end=True),
+        ])
+
+        assert self.await_read(read_all=True) == self.content(segments), "Stream ends and read-all handshake doesn't time out"
+
     def test_offset_and_duration(self):
         thread, segments = self.subject([
             Playlist(1234, [Segment(0), Segment(1, duration=0.5), Segment(2, duration=0.5), Segment(3)], end=True),
         ], streamoptions={"start_offset": 1, "duration": 1})
 
         data = self.await_read(read_all=True)
         assert data == self.content(segments, cond=lambda s: 0 < s.num < 3), "Respects the offset and duration"
@@ -268,65 +277,97 @@
     def get_session(self, options=None, *args, **kwargs):
         session = super().get_session(options)
         session.set_option("hls-live-edge", 3)
         session.set_option("http-headers", {"X-FOO": "BAR"})
 
         return session
 
-    def gen_key(self, aes_key=None, aes_iv=None, method="AES-128", uri=None, keyformat="identity", keyformatversions=1):
+    def gen_key(
+        self,
+        aes_key=None,
+        aes_iv=None,
+        method="AES-128",
+        uri=None,
+        keyformat="identity",
+        keyformatversions=1,
+        mock=None,
+    ):
         aes_key = aes_key or os.urandom(16)
         aes_iv = aes_iv or os.urandom(16)
 
         key = TagKey(method=method, uri=uri, iv=aes_iv, keyformat=keyformat, keyformatversions=keyformatversions)
-        self.mock("GET", key.url(self.id()), content=aes_key)
+        self.mock("GET", key.url(self.id()), **(mock if mock else {"content": aes_key}))
 
         return aes_key, aes_iv, key
 
     @patch("streamlink.stream.hls.log")
     def test_hls_encrypted_invalid_method(self, mock_log: Mock):
         aesKey, aesIv, key = self.gen_key(method="INVALID")
 
         self.subject([
             Playlist(0, [key, SegmentEnc(1, aesKey, aesIv)], end=True),
         ])
         self.await_write()
 
-        assert self.thread.reader.writer.closed
+        self.thread.close()
+        self.await_close()
+
         assert b"".join(self.thread.data) == b""
         assert mock_log.error.mock_calls == [
             call("Failed to create decryptor: Unable to decrypt cipher INVALID"),
         ]
 
     @patch("streamlink.stream.hls.log")
     def test_hls_encrypted_missing_uri(self, mock_log: Mock):
         aesKey, aesIv, key = self.gen_key(uri=False)
 
         self.subject([
             Playlist(0, [key, SegmentEnc(1, aesKey, aesIv)], end=True),
         ])
         self.await_write()
 
-        assert self.thread.reader.writer.closed
+        self.thread.close()
+        self.await_close()
+
         assert b"".join(self.thread.data) == b""
         assert mock_log.error.mock_calls == [
             call("Failed to create decryptor: Missing URI for decryption key"),
         ]
 
+    @patch("streamlink.stream.hls.log")
+    def test_hls_encrypted_missing_adapter(self, mock_log: Mock):
+        aesKey, aesIv, key = self.gen_key(uri="foo://bar/baz", mock={"exc": InvalidSchema})
+
+        self.subject([
+            Playlist(0, [key, SegmentEnc(1, aesKey, aesIv)], end=True),
+        ])
+        self.await_write()
+
+        self.thread.close()
+        self.await_close()
+
+        assert b"".join(self.thread.data) == b""
+        assert mock_log.error.mock_calls == [
+            call("Failed to create decryptor: Unable to find connection adapter for key URI: foo://bar/baz"),
+        ]
+
     def test_hls_encrypted_aes128(self):
         aesKey, aesIv, key = self.gen_key()
         long = b"Test cipher block chaining mode by using a long bytes string"
 
         # noinspection PyTypeChecker
         thread, segments = self.subject([
             Playlist(0, [key] + [SegmentEnc(num, aesKey, aesIv) for num in range(0, 4)]),
             Playlist(4, [key] + [SegmentEnc(num, aesKey, aesIv, content=long) for num in range(4, 8)], end=True),
         ])
 
         self.await_write(3 + 4)
         data = self.await_read(read_all=True)
+        self.await_close()
+
         expected = self.content(segments, prop="content_plain", cond=lambda s: s.num >= 1)
         assert data == expected, "Decrypts the AES-128 identity stream"
         assert self.called(key, once=True), "Downloads encryption key only once"
         assert self.get_mock(key).last_request._request.headers.get("X-FOO") == "BAR"
         assert not any(self.called(s) for s in segments.values() if s.num < 1), "Skips first segment"
         assert all(self.called(s) for s in segments.values() if s.num >= 1), "Downloads all remaining segments"
         assert self.get_mock(segments[1]).last_request._request.headers.get("X-FOO") == "BAR"
@@ -342,14 +383,16 @@
         thread, segments = self.subject([
             Playlist(0, [key, map1] + [SegmentEnc(num, aesKey, aesIv) for num in range(0, 2)]),
             Playlist(2, [key, map2] + [SegmentEnc(num, aesKey, aesIv) for num in range(2, 4)], end=True),
         ])
 
         self.await_write(2 * 2 + 2 * 2)
         data = self.await_read(read_all=True)
+        self.await_close()
+
         assert data == self.content([
             map1, segments[0], map1, segments[1], map2, segments[2], map2, segments[3],
         ], prop="content_plain")
 
     def test_hls_encrypted_aes128_key_uri_override(self):
         aesKey, aesIv, key = self.gen_key(uri="http://real-mocked/{namespace}/encryption.key?foo=bar")
         aesKeyInvalid = bytes(ord(aesKey[i:i + 1]) ^ 0xFF for i in range(16))
@@ -359,14 +402,16 @@
         thread, segments = self.subject([
             Playlist(0, [key_invalid] + [SegmentEnc(num, aesKey, aesIv) for num in range(0, 4)]),
             Playlist(4, [key_invalid] + [SegmentEnc(num, aesKey, aesIv) for num in range(4, 8)], end=True),
         ], options={"hls-segment-key-uri": "{scheme}://real-{netloc}{path}?{query}"})
 
         self.await_write(3 + 4)
         data = self.await_read(read_all=True)
+        self.await_close()
+
         expected = self.content(segments, prop="content_plain", cond=lambda s: s.num >= 1)
         assert data == expected, "Decrypts stream from custom key"
         assert not self.called(key_invalid), "Skips encryption key"
         assert self.called(key, once=True), "Downloads custom encryption key"
         assert self.get_mock(key).last_request._request.headers.get("X-FOO") == "BAR"
 
     @patch("streamlink.stream.hls.log")
@@ -377,18 +422,20 @@
             Playlist(0, [
                 key,
                 SegmentEnc(0, aesKey, aesIv, append=b"?"),
                 SegmentEnc(1, aesKey, aesIv),
             ], end=True),
         ])
         self.await_write()
-        assert self.thread.reader.writer.closed is not True
+        assert thread.reader.writer.is_alive()
 
         self.await_write()
         data = self.await_read(read_all=True)
+        self.await_close()
+
         assert data == self.content([segments[1]], prop="content_plain")
         assert mock_log.error.mock_calls == [
             call("Error while decrypting segment 0: Data must be padded to 16 byte boundary in CBC mode"),
         ]
 
     @patch("streamlink.stream.hls.log")
     def test_hls_encrypted_aes128_incorrect_padding_length(self, mock_log: Mock):
@@ -399,18 +446,20 @@
             Playlist(0, [
                 key,
                 SegmentEnc(0, aesKey, aesIv, padding=padding),
                 SegmentEnc(1, aesKey, aesIv),
             ], end=True),
         ])
         self.await_write()
-        assert self.thread.reader.writer.closed is not True
+        assert thread.reader.writer.is_alive()
 
         self.await_write()
         data = self.await_read(read_all=True)
+        self.await_close()
+
         assert data == self.content([segments[1]], prop="content_plain")
         assert mock_log.error.mock_calls == [call("Error while decrypting segment 0: Padding is incorrect.")]
 
     @patch("streamlink.stream.hls.log")
     def test_hls_encrypted_aes128_incorrect_padding_content(self, mock_log: Mock):
         aesKey, aesIv, key = self.gen_key()
 
@@ -419,18 +468,20 @@
             Playlist(0, [
                 key,
                 SegmentEnc(0, aesKey, aesIv, padding=padding),
                 SegmentEnc(1, aesKey, aesIv),
             ], end=True),
         ])
         self.await_write()
-        assert self.thread.reader.writer.closed is not True
+        assert thread.reader.writer.is_alive()
 
         self.await_write()
         data = self.await_read(read_all=True)
+        self.await_close()
+
         assert data == self.content([segments[1]], prop="content_plain")
         assert mock_log.error.mock_calls == [call("Error while decrypting segment 0: PKCS#7 padding is incorrect.")]
 
 
 @patch("streamlink.stream.hls.HLSStreamWorker.wait", Mock(return_value=True))
 class TestHlsPlaylistReloadTime(TestMixinStreamHLS, unittest.TestCase):
     segments = [
@@ -443,15 +494,15 @@
     def get_session(self, options=None, reload_time=None, *args, **kwargs):
         return super().get_session(dict(options or {}, **{
             "hls-live-edge": 3,
             "hls-playlist-reload-time": reload_time,
         }))
 
     def subject(self, *args, **kwargs):
-        thread, segments = super().subject(start=False, *args, **kwargs)
+        thread, segments = super().subject(*args, start=False, **kwargs)
 
         # mock the worker thread's _playlist_reload_time method, so that the main thread can wait on its call
         playlist_reload_time_called = Event()
         orig_playlist_reload_time = thread.reader.worker._playlist_reload_time
 
         def mocked_playlist_reload_time(*args, **kwargs):
             playlist_reload_time_called.set()
@@ -573,114 +624,59 @@
         assert self.await_read(read_all=True) == b""
         self.await_close()
         assert self.thread.reader.buffer.closed, "Closes the stream on initial playlist parsing error"
         assert mock_log.debug.mock_calls == [call("Reloading playlist")]
         assert mock_log.error.mock_calls == [call("Streams containing I-frames only are not playable")]
 
 
-@patch("streamlink.stream.hls.FFMPEGMuxer.is_usable", Mock(return_value=True))
-class TestHlsExtAudio(unittest.TestCase):
-    @property
-    def playlist(self):
-        with text("hls/test_2.m3u8") as pl:
-            return pl.read()
-
-    def run_streamlink(self, playlist, audio_select=None):
-        streamlink = Streamlink()
-
-        if audio_select:
-            streamlink.set_option("hls-audio-select", audio_select)
-
-        return HLSStream.parse_variant_playlist(streamlink, playlist)
-
-    def test_hls_ext_audio_not_selected(self):
-        master_url = "http://mocked/path/master.m3u8"
-
-        with requests_mock.Mocker() as mock:
-            mock.get(master_url, text=self.playlist)
-            master_stream = self.run_streamlink(master_url)["video"]
-
-        with pytest.raises(AttributeError):
-            master_stream.substreams
-
-        assert master_stream.url == "http://mocked/path/playlist.m3u8"
-
-    def test_hls_ext_audio_en(self):
-        """
-        m3u8 with ext audio but no options should not download additional streams
-        :return:
-        """
-
-        master_url = "http://mocked/path/master.m3u8"
-        expected = ["http://mocked/path/playlist.m3u8", "http://mocked/path/en.m3u8"]
-
-        with requests_mock.Mocker() as mock:
-            mock.get(master_url, text=self.playlist)
-            master_stream = self.run_streamlink(master_url, "en")
-
-        substreams = master_stream["video"].substreams
-        result = [x.url for x in substreams]
-
-        # Check result
-        assert result == expected
-
-    def test_hls_ext_audio_es(self):
-        """
-        m3u8 with ext audio but no options should not download additional streams
-        :return:
-        """
-
-        master_url = "http://mocked/path/master.m3u8"
-        expected = ["http://mocked/path/playlist.m3u8", "http://mocked/path/es.m3u8"]
-
-        with requests_mock.Mocker() as mock:
-            mock.get(master_url, text=self.playlist)
-            master_stream = self.run_streamlink(master_url, "es")
-
-        substreams = master_stream["video"].substreams
-
-        result = [x.url for x in substreams]
-
-        # Check result
-        assert result == expected
-
-    def test_hls_ext_audio_all(self):
-        """
-        m3u8 with ext audio but no options should not download additional streams
-        :return:
-        """
-
-        master_url = "http://mocked/path/master.m3u8"
-        expected = ["http://mocked/path/playlist.m3u8", "http://mocked/path/en.m3u8", "http://mocked/path/es.m3u8"]
-
-        with requests_mock.Mocker() as mock:
-            mock.get(master_url, text=self.playlist)
-            master_stream = self.run_streamlink(master_url, "en,es")
-
-        substreams = master_stream["video"].substreams
-
-        result = [x.url for x in substreams]
-
-        # Check result
-        assert result == expected
-
-    def test_hls_ext_audio_wildcard(self):
-        master_url = "http://mocked/path/master.m3u8"
-        expected = ["http://mocked/path/playlist.m3u8", "http://mocked/path/en.m3u8", "http://mocked/path/es.m3u8"]
-
-        with requests_mock.Mocker() as mock:
-            mock.get(master_url, text=self.playlist)
-            master_stream = self.run_streamlink(master_url, "*")
-
-        substreams = master_stream["video"].substreams
-
-        result = [x.url for x in substreams]
+class TestHlsExtAudio:
+    @pytest.fixture(autouse=True)
+    def _is_usable(self, monkeypatch: pytest.MonkeyPatch):
+        monkeypatch.setattr("streamlink.stream.hls.FFMPEGMuxer.is_usable", Mock(return_value=True))
+
+    @pytest.fixture(autouse=True)
+    def _playlist(self):
+        with text("hls/test_2.m3u8") as playlist, \
+             requests_mock.Mocker() as mock_requests:
+            mock_requests.get("http://mocked/path/master.m3u8", text=playlist.read())
+            yield
+
+    @pytest.fixture()
+    def stream(self, session: Streamlink):
+        streams = HLSStream.parse_variant_playlist(session, "http://mocked/path/master.m3u8")
+        assert "video" in streams
+
+        return streams["video"]
+
+    def test_no_selection(self, stream: HLSStream):
+        assert not isinstance(stream, MuxedHLSStream)
+        assert stream.url == "http://mocked/path/playlist.m3u8"
+
+    @pytest.mark.parametrize(("session", "selection"), [
+        pytest.param({"hls-audio-select": ["en"]}, "http://mocked/path/en.m3u8", id="English"),
+        pytest.param({"hls-audio-select": ["es"]}, "http://mocked/path/es.m3u8", id="Spanish"),
+    ], indirect=["session"])
+    def test_selection(self, session: Streamlink, stream: MuxedHLSStream, selection: str):
+        assert isinstance(stream, MuxedHLSStream)
+        assert [substream.url for substream in stream.substreams] == [
+            "http://mocked/path/playlist.m3u8",
+            selection,
+        ]
 
-        # Check result
-        assert result == expected
+    @pytest.mark.parametrize("session", [
+        pytest.param({"hls-audio-select": ["*"]}, id="wildcard"),
+        pytest.param({"hls-audio-select": ["en", "es"]}, id="multiple locales"),
+    ], indirect=["session"])
+    def test_multiple(self, session: Streamlink, stream: MuxedHLSStream):
+        assert isinstance(stream, MuxedHLSStream)
+        assert [substream.url for substream in stream.substreams] == [
+            "http://mocked/path/playlist.m3u8",
+            "http://mocked/path/en.m3u8",
+            "http://mocked/path/es.m3u8",
+        ]
 
 
 class TestM3U8ParserLogging:
     @pytest.mark.parametrize(("loglevel", "has_logs"), [("trace", False), ("all", True)])
     def test_log(self, caplog: pytest.LogCaptureFixture, loglevel: str, has_logs: bool):
         caplog.set_level(loglevel, "streamlink")
```

### Comparing `streamlink-5.3.1/tests/stream/test_hls_filtered.py` & `streamlink-5.4.0/tests/stream/test_hls_filtered.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/stream/test_hls_playlist.py` & `streamlink-5.4.0/tests/stream/test_hls_playlist.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/stream/test_stream_json.py` & `streamlink-5.4.0/tests/stream/test_stream_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.file import FileStream
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 from streamlink.stream.stream import Stream
 
 
-@pytest.fixture(scope="module")
-def session():
-    session = Streamlink()
+@pytest.fixture()
+def session(session: Streamlink):
     session.set_option("http-cookies", {"sessioncookiekey": "sessioncookieval"})
     session.set_option("http-headers", {"sessionheaderkey": "sessionheaderval"})
     session.set_option("http-query-params", {"sessionqueryparamkey": "sessionqueryparamval"})
 
     return session
```

### Comparing `streamlink-5.3.1/tests/stream/test_stream_to_url.py` & `streamlink-5.4.0/tests/stream/test_stream_to_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 from unittest.mock import Mock
 
 import pytest
 
-from streamlink import Streamlink
 from streamlink.stream.dash import DASHStream
 from streamlink.stream.file import FileStream
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 from streamlink.stream.stream import Stream
 
 
 @pytest.fixture(scope="module")
-def session():
-    return Streamlink()
-
-
-@pytest.fixture(scope="module")
 def common_args():
     return dict(
         params={"queryparamkey": "queryparamval"},
         unknown="invalid",
     )
```

### Comparing `streamlink-5.3.1/tests/stream/test_stream_wrappers.py` & `streamlink-5.4.0/tests/stream/test_stream_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/test_api_http_session.py` & `streamlink-5.4.0/tests/test_api_http_session.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/test_api_validate.py` & `streamlink-5.4.0/tests/test_api_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 
 
 def assert_validationerror(exception, expected):
     assert str(exception) == dedent(expected).strip("\n")
 
 
 def test_text_is_str(recwarn: pytest.WarningsRecorder):
-    assert "text" not in getattr(validate, "__dict__")
-    assert "text" in getattr(validate, "__all__")
+    assert "text" not in getattr(validate, "__dict__", {})
+    assert "text" in getattr(validate, "__all__", [])
     assert validate.text is str, "Exports text as str alias for backwards compatiblity"
-    assert [(record.category, str(record.message)) for record in recwarn.list] == [
+    assert [(record.category, str(record.message), record.filename) for record in recwarn.list] == [
         (
             StreamlinkDeprecationWarning,
             "`streamlink.plugin.api.validate.text` is deprecated. Use `str` instead.",
+            __file__,
         ),
     ]
 
 
 class TestSchema:
     @pytest.fixture(scope="class")
     def schema(self):
@@ -640,15 +641,15 @@
         def __repr__(self):
             return self.__class__.__name__
 
     @pytest.fixture()
     def obj(self):
         obj1 = self.Subject()
         obj2 = self.Subject()
-        setattr(obj1, "bar", obj2)
+        obj1.bar = obj2
 
         return obj1
 
     def test_success(self, obj):
         schema = validate.attr({"foo": validate.transform(lambda num: num + 1)})
         newobj = validate.validate(schema, obj)
         assert obj.foo == 1
```

### Comparing `streamlink-5.3.1/tests/test_api_websocket.py` & `streamlink-5.4.0/tests/test_api_websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,22 +20,14 @@
 ])
 def test_opcode_export(name, value):
     assert getattr(WebsocketClient, name) == value
 
 
 class TestWebsocketClient:
     @pytest.fixture()
-    def session(self, request: pytest.FixtureRequest):
-        with patch("streamlink.session.Streamlink.load_builtin_plugins"):
-            session = Streamlink()
-            for key, value in getattr(request, "param", {}).items():
-                session.set_option(key, value)
-            yield session
-
-    @pytest.fixture()
     def websocketapp(self):
         with patch("streamlink.plugin.api.websocket.WebSocketApp") as mock_websocketapp:
             yield mock_websocketapp
 
     @pytest.fixture()
     def client(self, request: pytest.FixtureRequest, session: Streamlink, websocketapp: Mock):
         with patch("streamlink.plugin.api.websocket.certify_where", side_effect=Mock(return_value="/path/to/cacert.pem")):
```

### Comparing `streamlink-5.3.1/tests/test_buffers.py` & `streamlink-5.4.0/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/test_cache.py` & `streamlink-5.4.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/test_logger.py` & `streamlink-5.4.0/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import warnings
+from datetime import timezone
 from inspect import currentframe, getframeinfo
 from io import StringIO
 from pathlib import Path
 from typing import Iterable, Tuple, Type
 from unittest.mock import patch
 
 import freezegun
@@ -20,15 +21,16 @@
 
 @pytest.fixture()
 def log(request, output: StringIO):
     params = getattr(request, "param", {})
     params.setdefault("format", "[{name}][{levelname}] {message}")
     params.setdefault("style", "{")
     fakeroot = logging.getLogger("streamlink.test")
-    with patch("streamlink.logger.root", fakeroot):
+    with patch("streamlink.logger.root", fakeroot), \
+         patch("streamlink.utils.times.LOCAL", timezone.utc):
         logger.basicConfig(stream=output, **params)
         yield fakeroot
         logger.capturewarnings(False)
 
 
 class TestLogging:
     @pytest.fixture()
@@ -148,20 +150,20 @@
     def test_datefmt_default(self, log: logging.Logger, output: StringIO):
         log.setLevel("info")
         log.info("test")
         assert output.getvalue() == "[03:04:05][test][info] test\n"
 
     @freezegun.freeze_time("2000-01-02T03:04:05.123456Z")
     @pytest.mark.parametrize("log", [
-        {"format": "[{asctime}][{name}][{levelname}] {message}", "datefmt": "%H:%M:%S.%f"},
+        {"format": "[{asctime}][{name}][{levelname}] {message}", "datefmt": "%H:%M:%S.%f%z"},
     ], indirect=True)
     def test_datefmt_custom(self, log: logging.Logger, output: StringIO):
         log.setLevel("info")
         log.info("test")
-        assert output.getvalue() == "[03:04:05.123456][test][info] test\n"
+        assert output.getvalue() == "[03:04:05.123456+0000][test][info] test\n"
 
 
 class TestCaptureWarnings:
     @staticmethod
     def _warn(messages: Iterable[Tuple[str, Type[Warning]]], filterwarnings=None):
         frame = currentframe()
         assert frame
```

### Comparing `streamlink-5.3.1/tests/test_options.py` & `streamlink-5.4.0/tests/test_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,16 +238,20 @@
         @pluginargument("foo-foo", is_global=True)
         @pluginargument("bar-bar", default=456)
         @pluginargument("baz-baz", default=789, help=argparse.SUPPRESS)
         class FakePlugin(Plugin):
             def _get_streams(self):  # pragma: no cover
                 pass
 
-        assert [(record.category, str(record.message)) for record in recwarn.list] == [
-            (StreamlinkDeprecationWarning, "Defining global plugin arguments is deprecated. Use the session options instead."),
+        assert [(record.category, str(record.message), record.filename) for record in recwarn.list] == [
+            (
+                StreamlinkDeprecationWarning,
+                "Defining global plugin arguments is deprecated. Use the session options instead.",
+                __file__,
+            ),
         ]
 
         session = Mock()
         parser = ArgumentParser()
         parser.add_argument("--foo-foo", default=123)
 
         session.plugins = {"plugin": FakePlugin}
```

### Comparing `streamlink-5.3.1/tests/test_plugin.py` & `streamlink-5.4.0/tests/test_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,20 @@
         session = Mock()
         with patch("streamlink.plugin.plugin.Cache") as mock_cache, \
              patch.object(DeprecatedPlugin, "load_cookies") as mock_load_cookies:
             plugin = DeprecatedPlugin(session, "http://localhost")  # type: ignore[call-arg]
 
         assert isinstance(plugin, DeprecatedPlugin)
         assert plugin.custom_attribute == "HTTP://LOCALHOST"
-        assert [(record.category, str(record.message)) for record in recwarn.list] == [
-            (FutureWarning, "Initialized test_plugin plugin with deprecated constructor"),
+        assert [(record.category, str(record.message), record.filename) for record in recwarn.list] == [
+            (
+                FutureWarning,
+                "Initialized test_plugin plugin with deprecated constructor",
+                __file__,
+            ),
         ]
 
         assert plugin.session is session
         assert plugin.url == "http://localhost"
 
         assert plugin.module == "test_plugin"
 
@@ -286,18 +290,14 @@
         rest={"HttpOnly": None},
         rfc2109=False,
     )
 
 
 class TestCookies:
     @pytest.fixture()
-    def session(self):
-        return Streamlink()
-
-    @pytest.fixture()
     def pluginclass(self):
         class MyPlugin(FakePlugin):
             __module__ = "myplugin"
 
         return MyPlugin
 
     @pytest.fixture()
```

### Comparing `streamlink-5.3.1/tests/test_plugin_userinput.py` & `streamlink-5.4.0/tests/test_plugin_userinput.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,14 @@
     console_input = ConsoleUserInputRequester(Mock())
     session = Streamlink({"user-input-requester": console_input})
     assert session.get_option("user-input-requester") is console_input
 
 
 class TestPluginUserInput:
     @pytest.fixture()
-    def session(self):
-        return Streamlink()
-
-    @pytest.fixture()
     def testplugin(self, session: Streamlink):
         return _TestPlugin(session, "http://example.com/stream")
 
     @pytest.fixture()
     def console_input(self, request, session: Streamlink):
         isatty: bool = request.param
         with patch("streamlink_cli.console.sys.stdin.isatty", return_value=isatty):
```

### Comparing `streamlink-5.3.1/tests/test_plugins.py` & `streamlink-5.4.0/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/test_session.py` & `streamlink-5.4.0/tests/test_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,27 @@
 from unittest.mock import Mock, call, patch
 
 import pytest
 import requests_mock
 import urllib3
 
 import tests.plugin
-from streamlink import NoPluginError, Streamlink
-from streamlink.exceptions import StreamlinkDeprecationWarning
+from streamlink.exceptions import NoPluginError, StreamlinkDeprecationWarning
 from streamlink.plugin import HIGH_PRIORITY, LOW_PRIORITY, NO_PRIORITY, NORMAL_PRIORITY, Plugin, pluginmatcher
+from streamlink.session import Streamlink
 from streamlink.stream.hls import HLSStream
 from streamlink.stream.http import HTTPStream
 
 
 PATH_TESTPLUGINS = Path(tests.plugin.__path__[0])
 PATH_TESTPLUGINS_OVERRIDE = PATH_TESTPLUGINS / "override"
 
 _original_allowed_gai_family = urllib3.util.connection.allowed_gai_family  # type: ignore[attr-defined]
 
 
-@pytest.fixture()
-def session():
-    with patch("streamlink.session.Streamlink.load_builtin_plugins"):
-        yield Streamlink()
-
-
 class EmptyPlugin(Plugin):
     def _get_streams(self):
         pass  # pragma: no cover
 
 
 # TODO: rewrite using pytest
 class TestSession(unittest.TestCase):
@@ -420,18 +414,19 @@
     def _no_deprecation(self, recwarn: pytest.WarningsRecorder):
         yield
         assert recwarn.list == []
 
     @pytest.fixture()
     def _logs_deprecation(self, recwarn: pytest.WarningsRecorder):
         yield
-        assert [(record.category, str(record.message)) for record in recwarn.list] == [
+        assert [(record.category, str(record.message), record.filename) for record in recwarn.list] == [
             (
                 StreamlinkDeprecationWarning,
                 "The `https-proxy` option has been deprecated in favor of a single `http-proxy` option",
+                __file__,
             ),
         ]
 
     @pytest.mark.usefixtures("_no_deprecation")
     def test_https_proxy_default(self, session: Streamlink):
         session.set_option("http-proxy", "http://testproxy.com")
 
@@ -483,14 +478,24 @@
 
     @pytest.mark.usefixtures("_logs_deprecation")
     def test_get_https_proxy(self, session: Streamlink):
         session.http.proxies["http"] = "http://testproxy1.com"
         session.http.proxies["https"] = "http://testproxy2.com"
         assert session.get_option("https-proxy") == "http://testproxy2.com"
 
+    @pytest.mark.usefixtures("_logs_deprecation")
+    def test_https_proxy_get_directly(self, session: Streamlink):
+        # The DeprecationWarning's origin must point to this call, even without the set_option() wrapper
+        session.options.get("https-proxy")
+
+    @pytest.mark.usefixtures("_logs_deprecation")
+    def test_https_proxy_set_directly(self, session: Streamlink):
+        # The DeprecationWarning's origin must point to this call, even without the set_option() wrapper
+        session.options.set("https-proxy", "https://foo")
+
 
 class TestOptionsKeyEqualsValue:
     @pytest.fixture()
     def option(self, request, session: Streamlink):
         option, attr = request.param
         httpsessionattr = getattr(session.http, attr)
         assert session.get_option(option) is httpsessionattr
```

### Comparing `streamlink-5.3.1/tests/test_streamlink_api.py` & `streamlink-5.4.0/tests/test_streamlink_api.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/testutils/handshake.py` & `streamlink-5.4.0/tests/testutils/handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/testutils/test_handshake.py` & `streamlink-5.4.0/tests/testutils/test_handshake.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_cache.py` & `streamlink-5.4.0/tests/utils/test_cache.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_crypto.py` & `streamlink-5.4.0/tests/utils/test_crypto.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_data.py` & `streamlink-5.4.0/tests/utils/test_data.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_formatter.py` & `streamlink-5.4.0/tests/utils/test_formatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import datetime, timezone
 from unittest.mock import Mock, patch
 
 import pytest
 from freezegun import freeze_time
 
 from streamlink.utils.formatter import Formatter
 
@@ -23,15 +23,15 @@
     @pytest.fixture()
     def formatter(self, prop: Mock, obj: Obj):
         with freeze_time("2000-01-02T03:04:05.000006Z"):
             yield Formatter(
                 {
                     "prop": prop,
                     "obj": lambda: obj,
-                    "time": datetime.now,
+                    "time": lambda: datetime.now(timezone.utc),
                     "empty": lambda: "",
                     "none": lambda: None,
                 },
                 {
                     "time": lambda dt, fmt: dt.strftime(fmt),
                 },
             )
@@ -53,20 +53,21 @@
 
         defaults = dict(prop="PROP", obj="OBJ", empty="EMPTY", none="NONE")
         assert formatter.format("'{prop}' '{obj}' '{empty}' '{none}'", defaults) == "'prop' 'obj' '' 'NONE'"
         assert formatter.cache == dict(prop="prop", obj=obj, empty="", none=None)
         assert prop.call_count == 1
 
     def test_format_spec(self, formatter: Formatter):
-        assert formatter.format("{time}") == "2000-01-02 03:04:05.000006"
-        assert formatter.cache == dict(time=datetime(2000, 1, 2, 3, 4, 5, 6, None))
+        assert formatter.format("{time}") == "2000-01-02 03:04:05.000006+00:00"
+        assert formatter.cache == dict(time=datetime(2000, 1, 2, 3, 4, 5, 6, timezone.utc))
         assert formatter.format("{time:%Y}") == "2000"
         assert formatter.format("{time:%Y-%m-%d}") == "2000-01-02"
         assert formatter.format("{time:%H:%M:%S}") == "03:04:05"
+        assert formatter.format("{time:%Z}") == "UTC"
         with patch("datetime.datetime.strftime", side_effect=ValueError):
             assert formatter.format("{time:foo:bar}") == "{time:foo:bar}"
-        assert formatter.cache == dict(time=datetime(2000, 1, 2, 3, 4, 5, 6, None))
+        assert formatter.cache == dict(time=datetime(2000, 1, 2, 3, 4, 5, 6, timezone.utc))
 
         assert formatter.format("{prop:foo}") == "prop"
         assert formatter.format("{none:foo}") == ""
         assert formatter.format("{unknown:format}") == "{unknown:format}"
         assert formatter.format("{unknown:format}", {"unknown": "known"}) == "known"
```

### Comparing `streamlink-5.3.1/tests/utils/test_l10n.py` & `streamlink-5.4.0/tests/utils/test_l10n.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_module.py` & `streamlink-5.4.0/tests/utils/test_module.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_named_pipe.py` & `streamlink-5.4.0/tests/utils/test_named_pipe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import threading
 import unittest
 from unittest.mock import Mock, call, patch
 
 import pytest
 
 from streamlink.utils.named_pipe import NamedPipe, NamedPipeBase, NamedPipePosix, NamedPipeWindows
-from tests import posix_only, windows_only
 
 
 try:
     from ctypes import byref, c_ulong, create_string_buffer, windll  # type: ignore[attr-defined]
 except ImportError:
     pass
 
@@ -74,15 +73,15 @@
         NamedPipe()
         assert mock_log.info.mock_calls == [
             call("Creating pipe streamlinkpipe-12345-1-67890"),
             call("Creating pipe streamlinkpipe-12345-2-67890"),
         ]
 
 
-@posix_only
+@pytest.mark.posix_only()
 class TestNamedPipePosix(unittest.TestCase):
     def test_export(self):
         assert NamedPipe is NamedPipePosix
 
     @patch("streamlink.utils.named_pipe.os.mkfifo")
     def test_create(self, mock_mkfifo):
         mock_mkfifo.side_effect = OSError
@@ -117,15 +116,15 @@
         assert not pipe.path.is_fifo()
         reader.done.wait(4000)
         assert reader.error is None
         assert reader.data == b"foobar"
         assert not reader.is_alive()
 
 
-@windows_only
+@pytest.mark.windows_only()
 class TestNamedPipeWindows(unittest.TestCase):
     def test_export(self):
         assert NamedPipe is NamedPipeWindows
 
     @patch("streamlink.utils.named_pipe.windll.kernel32")
     def test_create(self, mock_kernel32):
         mock_kernel32.CreateNamedPipeW.return_value = NamedPipeWindows.INVALID_HANDLE_VALUE
```

### Comparing `streamlink-5.3.1/tests/utils/test_parse.py` & `streamlink-5.4.0/tests/utils/test_parse.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_processoutput.py` & `streamlink-5.4.0/tests/utils/test_processoutput.py`

 * *Files identical despite different names*

### Comparing `streamlink-5.3.1/tests/utils/test_url.py` & `streamlink-5.4.0/tests/utils/test_url.py`

 * *Files identical despite different names*

