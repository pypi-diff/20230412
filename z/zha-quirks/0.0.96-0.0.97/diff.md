# Comparing `tmp/zha-quirks-0.0.96.tar.gz` & `tmp/zha-quirks-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zha-quirks-0.0.96.tar", last modified: Fri Apr  7 21:11:04 2023, max compression
+gzip compressed data, was "zha-quirks-0.0.97.tar", last modified: Wed Apr 12 01:26:30 2023, max compression
```

## Comparing `zha-quirks-0.0.96.tar` & `zha-quirks-0.0.97.tar`

### file list

```diff
@@ -1,374 +1,375 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32824 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.343397 zha-quirks-0.0.96/zha_quirks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-07 21:11:04.000000 zha-quirks-0.0.96/zha_quirks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-07 21:11:04.000000 zha-quirks-0.0.96/zha_quirks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:11:04.000000 zha-quirks-0.0.96/zha_quirks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 21:11:04.000000 zha-quirks-0.0.96/zha_quirks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 21:11:04.000000 zha-quirks-0.0.96/zha_quirks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.343397 zha-quirks-0.0.96/zhaquirks/
--rw-r--r--   0 runner    (1001) docker     (123)    13690 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.343397 zha-quirks-0.0.96/zhaquirks/adeo/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/adeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/adeo/color_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.343397 zha-quirks-0.0.96/zhaquirks/aduro/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/aduro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/aduro/adurolightncc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.343397 zha-quirks-0.0.96/zhaquirks/aurora/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/aurora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/aurora/aurora_dimmer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.343397 zha-quirks-0.0.96/zhaquirks/bitron/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/bitron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/bitron/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.343397 zha-quirks-0.0.96/zhaquirks/bosch/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/bosch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/bosch/isw_zdl1_wp11g.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2184 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/bosch/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.347398 zha-quirks-0.0.96/zhaquirks/centralite/
--rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/cl_3130.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2221 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/cl_3157100.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3134 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/cl_3300S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3643 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/cl_3305S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/cl_3310S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3457 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/cl_3321S.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2793 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/cl_3460L.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5941 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/ias.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/centralite/motionandtemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.347398 zha-quirks-0.0.96/zhaquirks/danfoss/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/danfoss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/danfoss/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.347398 zha-quirks-0.0.96/zhaquirks/develco/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/develco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/develco/air_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/develco/heat_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/develco/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/develco/open_close.py
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/develco/smoke_alarm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.347398 zha-quirks-0.0.96/zhaquirks/echostar/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/echostar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/echostar/bell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.347398 zha-quirks-0.0.96/zhaquirks/ecolink/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ecolink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ecolink/contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.347398 zha-quirks-0.0.96/zhaquirks/edpwithus/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/edpwithus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/edpwithus/redy_plug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.351398 zha-quirks-0.0.96/zhaquirks/elko/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/elko/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/elko/smart_super_thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.351398 zha-quirks-0.0.96/zhaquirks/eurotronic/
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/eurotronic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/eurotronic/spzb0001.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.351398 zha-quirks-0.0.96/zhaquirks/feibit/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/feibit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/feibit/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.351398 zha-quirks-0.0.96/zhaquirks/gledopto/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/gledopto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/gledopto/glc009.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/gledopto/glc009p.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/gledopto/gls007z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/gledopto/soposhgu10.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.351398 zha-quirks-0.0.96/zhaquirks/heiman/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/heiman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/heiman/smoke.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.351398 zha-quirks-0.0.96/zhaquirks/hivehome/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/hivehome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/hivehome/mot003V0.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/hivehome/mot003V6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.355398 zha-quirks-0.0.96/zhaquirks/ikea/
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/blinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/cctlightzha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/fivebtnremote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/fourbtnremote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/motionzha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/opencloseremote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/shortcutbtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/starkvind.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/symfonisk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/symfonisk2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/tradfriplug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ikea/twobtnremote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.355398 zha-quirks-0.0.96/zhaquirks/iluminize/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/iluminize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/iluminize/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/iluminize/dim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.355398 zha-quirks-0.0.96/zhaquirks/imagic/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/imagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/imagic/gs1117s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/imagic/im1116s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.355398 zha-quirks-0.0.96/zhaquirks/innr/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/innr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/innr/innr_sp120_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/innr/innr_sp234_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/innr/rs228t.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.355398 zha-quirks-0.0.96/zhaquirks/inovelli/
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/inovelli/VZM31SN.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/inovelli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/inovelli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.355398 zha-quirks-0.0.96/zhaquirks/insta/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/insta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/insta/nexentro_pushbutton_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/keenhome/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/keenhome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/keenhome/sv02612mp13.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/keenhome/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/kof/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/kof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/kof/kof_mr101z.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/konke/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/konke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/konke/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/konke/magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/konke/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/konke/temp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/lds/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lds/cctswitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/ledvance/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ledvance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ledvance/a19rgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/ledvance/flexrgbw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/legrand/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/legrand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/legrand/dimmer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/lidl/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lidl/TS0501A.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lidl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lidl/cct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lidl/rgbcct.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lidl/ts011f_plug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/linkind/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/linkind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/linkind/a001082.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/linkind/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/lixee/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lixee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lixee/zlinky.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.359398 zha-quirks-0.0.96/zhaquirks/lutron/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lutron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/lutron/lzl4bwhl01remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/mli/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/mli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/mli/tint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/mli/tintE14rgbcct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/netvox/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/netvox/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/netvox/z308e3ed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/nodon/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/nodon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/nodon/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/nue/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/nue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/nue/auwz02000.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/orvibo/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/orvibo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/orvibo/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/orvibo/motion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/osram/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/a19rgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/cla60tw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/flexrgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/gardenpolesrgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/lightifyx4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/osramplug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/smartplusac05347.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/switchmini.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/osram/tunablewhite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/paulmann/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/paulmann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/paulmann/fourbtnremote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/philio/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philio/pst03a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/philips/
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philips/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philips/rdm001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philips/rom001.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philips/rwl022.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/philips/rwlfirstgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/plaid/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/plaid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/plaid/soil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.363398 zha-quirks-0.0.96/zhaquirks/salus/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/salus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/salus/sp600.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/samjin/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/samjin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/samjin/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/samjin/button2.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/samjin/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/samjin/multi2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/sengled/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sengled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sengled/e1e_g7f.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/sercomm/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sercomm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sercomm/szwtd02n.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/siglis/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/siglis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/siglis/zigfred.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/sinope/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sinope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sinope/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sinope/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sinope/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    15193 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sinope/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/smartthings/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2165 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/moisturev4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/multi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/multiv4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/pgc313.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/pgc314.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3337 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartthings/tag_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/smartwings/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartwings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/smartwings/wm25lz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/sonoff/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sonoff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sonoff/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.367398 zha-quirks-0.0.96/zhaquirks/sourcingandcreation/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sourcingandcreation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/sourcingandcreation/smart_button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.371398 zha-quirks-0.0.96/zhaquirks/terncy/
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/terncy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/terncy/pp01.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/terncy/sd01.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.371398 zha-quirks-0.0.96/zhaquirks/texasinstruments/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/texasinstruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/texasinstruments/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.371398 zha-quirks-0.0.96/zhaquirks/thirdreality/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/thirdreality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/thirdreality/button.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/thirdreality/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.371398 zha-quirks-0.0.96/zhaquirks/trust/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/trust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/trust/zpir8000.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.375398 zha-quirks-0.0.96/zhaquirks/tuya/
--rw-r--r--   0 runner    (1001) docker     (123)    56142 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.375398 zha-quirks-0.0.96/zhaquirks/tuya/air/
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/air/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/air/ts0601_air_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.375398 zha-quirks-0.0.96/zhaquirks/tuya/mcu/
--rw-r--r--   0 runner    (1001) docker     (123)    21928 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/mcu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/sm0202_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    32600 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts000x.py
--rw-r--r--   0 runner    (1001) docker     (123)    40283 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts001x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0041.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0042.py
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0043.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0044.py
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0046.py
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts004f.py
--rw-r--r--   0 runner    (1001) docker     (123)    43413 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts011f_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts011f_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0121_plug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0201.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0210.py
--rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0211.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0501_fan_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0501b.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0501bs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_co.py
--rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_din_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_electric_heating.py
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_garage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_haozee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_motion.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_rcbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    70498 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_trv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_trv_sas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts0601_valve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts110e.py
--rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/tuya/ts130f.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.379398 zha-quirks-0.0.96/zhaquirks/universalelectronics/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/universalelectronics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/universalelectronics/contact_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.379398 zha-quirks-0.0.96/zhaquirks/visonic/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/visonic/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/visonic/mct340e.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.379398 zha-quirks-0.0.96/zhaquirks/waxman/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/waxman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/waxman/leaksmart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.379398 zha-quirks-0.0.96/zhaquirks/xbee/
--rw-r--r--   0 runner    (1001) docker     (123)    20282 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xbee/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xbee/xbee3_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xbee/xbee_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.379398 zha-quirks-0.0.96/zhaquirks/xiaomi/
--rw-r--r--   0 runner    (1001) docker     (123)    26618 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/ctrl_ln.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/ctrl_neutral.py
--rw-r--r--   0 runner    (1001) docker     (123)    11957 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/cube_aqgl01.py
--rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/feeder_acn001.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/illumination.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/light_aqcn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/magnet_acn001.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/magnet_aq2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_ac01.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_ac02.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_agl02.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_agl04.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_aq2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_aq2b.py
--rw-r--r--   0 runner    (1001) docker     (123)    57648 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/opple_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    13787 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/opple_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/plug.py
--rw-r--r--   0 runner    (1001) docker     (123)    11622 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/plug_eu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/plug_maus01.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/relay_c2acn01.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_b186acn01.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_b286acn01.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_e1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_h1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/roller_curtain_e1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/switch_aq2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/thermostat_agl001.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/tvoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/vibration_aq1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/water_acn001.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/wleak_aq1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/zhaquirks/xiaomi/mija/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/mija/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/mija/motion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/mija/sensor_ht.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/mija/sensor_magnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/mija/sensor_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/xiaomi/mija/smoke.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/zhaquirks/yale/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/yale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/yale/realliving.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/zhaquirks/zen/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/zen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/zen/thermostat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:11:04.387398 zha-quirks-0.0.96/zhaquirks/zhongxing/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/zhongxing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-07 21:11:02.000000 zha-quirks-0.0.96/zhaquirks/zhongxing/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32824 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zha_quirks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33259 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-12 01:26:30.000000 zha-quirks-0.0.97/zha_quirks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/adeo/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/adeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8369 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/adeo/color_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/aduro/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aduro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aduro/adurolightncc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/aurora/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aurora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/aurora/aurora_dimmer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/bitron/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bitron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bitron/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/bosch/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bosch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bosch/isw_zdl1_wp11g.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2184 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/bosch/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/centralite/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2948 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3130.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2221 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3157100.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3134 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3300S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3643 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3305S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2607 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3310S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3457 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3321S.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2793 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/cl_3460L.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5941 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/ias.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3296 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/centralite/motionandtemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/danfoss/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/danfoss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/danfoss/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/develco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/heat_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/open_close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/develco/smoke_alarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/echostar/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/echostar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/echostar/bell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/ecolink/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ecolink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ecolink/contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/edpwithus/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/edpwithus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/edpwithus/redy_plug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.734132 zha-quirks-0.0.97/zhaquirks/elko/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/elko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/elko/smart_super_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/eurotronic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/eurotronic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/eurotronic/spzb0001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/feibit/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/feibit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/feibit/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/gledopto/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/glc009.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/glc009p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/gls007z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/glsd001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/gledopto/soposhgu10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/heiman/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/heiman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/heiman/smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/hivehome/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/hivehome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/hivehome/mot003V0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/hivehome/mot003V6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/ikea/
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/cctlightzha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/fivebtnremote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/fourbtnremote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/motionzha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/opencloseremote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/shortcutbtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/starkvind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/symfonisk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/symfonisk2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/tradfriplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ikea/twobtnremote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/iluminize/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/iluminize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/iluminize/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/iluminize/dim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/imagic/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/imagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/imagic/gs1117s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/imagic/im1116s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/innr/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/innr_sp120_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/innr_sp234_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/innr/rs228t.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.738132 zha-quirks-0.0.97/zhaquirks/inovelli/
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/inovelli/VZM31SN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/inovelli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/inovelli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/insta/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/insta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/insta/nexentro_pushbutton_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/keenhome/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/keenhome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/keenhome/sv02612mp13.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/keenhome/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/kof/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/kof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/kof/kof_mr101z.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/konke/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/konke/temp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lds/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lds/cctswitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/ledvance/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ledvance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ledvance/a19rgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/ledvance/flexrgbw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/legrand/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/legrand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/legrand/dimmer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lidl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/TS0501A.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/cct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/rgbcct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lidl/ts011f_plug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/linkind/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/linkind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/linkind/a001082.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/linkind/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lixee/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lixee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10598 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lixee/zlinky.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/lutron/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lutron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/lutron/lzl4bwhl01remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/mli/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/mli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/mli/tint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/mli/tintE14rgbcct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/netvox/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/netvox/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/netvox/z308e3ed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/nodon/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nodon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nodon/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/nue/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/nue/auwz02000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.742132 zha-quirks-0.0.97/zhaquirks/orvibo/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/orvibo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/orvibo/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/orvibo/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/osram/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/a19rgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/cla60tw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/flexrgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/gardenpolesrgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/lightifyx4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/osramplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/smartplusac05347.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/switchmini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/osram/tunablewhite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/paulmann/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/paulmann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/paulmann/fourbtnremote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/philio/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philio/pst03a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/philips/
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rdm001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rom001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rwl022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/philips/rwlfirstgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/plaid/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/plaid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/plaid/soil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/salus/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/salus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/salus/sp600.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/samjin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/button2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/samjin/multi2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/sengled/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sengled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sengled/e1e_g7f.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/sercomm/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sercomm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sercomm/szwtd02n.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/siglis/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/siglis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19161 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/siglis/zigfred.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.746132 zha-quirks-0.0.97/zhaquirks/sinope/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14842 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15193 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sinope/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/smartthings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2165 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/moisturev4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/multi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/multiv4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/pgc313.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/pgc314.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3337 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartthings/tag_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/smartwings/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartwings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/smartwings/wm25lz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/sonoff/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sonoff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sonoff/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/sourcingandcreation/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sourcingandcreation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/sourcingandcreation/smart_button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/terncy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/terncy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/terncy/pp01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/terncy/sd01.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/texasinstruments/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/texasinstruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/texasinstruments/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/thirdreality/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/thirdreality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/thirdreality/button.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3709 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/thirdreality/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.750132 zha-quirks-0.0.97/zhaquirks/trust/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/trust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/trust/zpir8000.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/tuya/
+-rw-r--r--   0 runner    (1001) docker     (123)    56166 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/tuya/air/
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/air/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/air/ts0601_air_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/tuya/mcu/
+-rw-r--r--   0 runner    (1001) docker     (123)    21915 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/mcu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/sm0202_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32600 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts000x.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40283 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts001x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0041.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0042.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0043.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0046.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts004f.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43413 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts011f_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts011f_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0121_plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0210.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4266 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0211.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0501_fan_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0501b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0501bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_co.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20111 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_din_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_electric_heating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_garage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_haozee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_rcbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13444 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24769 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70494 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11139 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv_sas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts0601_valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts110e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/tuya/ts130f.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/universalelectronics/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/universalelectronics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/universalelectronics/contact_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/visonic/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/visonic/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2337 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/visonic/mct340e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/waxman/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/waxman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/waxman/leaksmart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/xbee/
+-rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/xbee3_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xbee/xbee_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.754132 zha-quirks-0.0.97/zhaquirks/xiaomi/
+-rw-r--r--   0 runner    (1001) docker     (123)    26618 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.758132 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_ln.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_neutral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11956 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube_aqgl01.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10772 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/feeder_acn001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/illumination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/light_aqcn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_acn001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_aq2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl04.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57638 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_eu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_maus01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/relay_c2acn01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b186acn01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b286acn01.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_e1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10324 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_h1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/roller_curtain_e1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/switch_aq2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/thermostat_agl001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/tvoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/vibration_aq1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/water_acn001.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/wleak_aq1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.758132 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/motion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_ht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_magnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/xiaomi/mija/smoke.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.758132 zha-quirks-0.0.97/zhaquirks/yale/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/yale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/yale/realliving.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/zhaquirks/zen/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zen/thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 01:26:30.762132 zha-quirks-0.0.97/zhaquirks/zhongxing/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zhongxing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-12 01:26:29.000000 zha-quirks-0.0.97/zhaquirks/zhongxing/motion.py
```

### Comparing `zha-quirks-0.0.96/LICENSE.md` & `zha-quirks-0.0.97/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/PKG-INFO` & `zha-quirks-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha-quirks
-Version: 0.0.96
+Version: 0.0.97
 Summary: Library implementing Zigpy quirks for ZHA in Home Assistant
 Home-page: https://github.com/dmulcahey/zha-device-handlers
 Author: David F. Mulcahey
 Author-email: david.mulcahey@icloud.com
 License: Apache License Version 2.0
 Keywords: zha quirks homeassistant hass
 Platform: UNKNOWN
```

### Comparing `zha-quirks-0.0.96/README.md` & `zha-quirks-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/setup.cfg` & `zha-quirks-0.0.97/setup.cfg`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/setup.py` & `zha-quirks-0.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup module for ZHAQuirks."""
 
 import pathlib
 
 from setuptools import find_packages, setup
 
-VERSION = "0.0.96"
+VERSION = "0.0.97"
 
 
 setup(
     name="zha-quirks",
     version=VERSION,
     description="Library implementing Zigpy quirks for ZHA in Home Assistant",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
```

### Comparing `zha-quirks-0.0.96/zha_quirks.egg-info/PKG-INFO` & `zha-quirks-0.0.97/zha_quirks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zha-quirks
-Version: 0.0.96
+Version: 0.0.97
 Summary: Library implementing Zigpy quirks for ZHA in Home Assistant
 Home-page: https://github.com/dmulcahey/zha-device-handlers
 Author: David F. Mulcahey
 Author-email: david.mulcahey@icloud.com
 License: Apache License Version 2.0
 Keywords: zha quirks homeassistant hass
 Platform: UNKNOWN
```

### Comparing `zha-quirks-0.0.96/zha_quirks.egg-info/SOURCES.txt` & `zha-quirks-0.0.97/zha_quirks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 zhaquirks/eurotronic/spzb0001.py
 zhaquirks/feibit/__init__.py
 zhaquirks/feibit/switch.py
 zhaquirks/gledopto/__init__.py
 zhaquirks/gledopto/glc009.py
 zhaquirks/gledopto/glc009p.py
 zhaquirks/gledopto/gls007z.py
+zhaquirks/gledopto/glsd001.py
 zhaquirks/gledopto/soposhgu10.py
 zhaquirks/heiman/__init__.py
 zhaquirks/heiman/smoke.py
 zhaquirks/hivehome/__init__.py
 zhaquirks/hivehome/mot003V0.py
 zhaquirks/hivehome/mot003V6.py
 zhaquirks/ikea/__init__.py
```

### Comparing `zha-quirks-0.0.96/zhaquirks/__init__.py` & `zha-quirks-0.0.97/zhaquirks/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import asyncio
 import importlib
 import logging
 import pathlib
 import pkgutil
-from typing import Any, Dict, List, Optional, Union
+from typing import Any
 
 import zigpy.device
 import zigpy.endpoint
 from zigpy.quirks import CustomCluster, CustomDevice
 import zigpy.types as t
 from zigpy.util import ListenableMixin
 from zigpy.zcl import foundation
@@ -104,19 +104,18 @@
 
 class EventableCluster(CustomCluster):
     """Cluster that generates events."""
 
     def handle_cluster_request(
         self,
         hdr: foundation.ZCLHeader,
-        args: List[Any],
+        args: list[Any],
         *,
-        dst_addressing: Optional[
-            Union[t.Addressing.Group, t.Addressing.IEEE, t.Addressing.NWK]
-        ] = None,
+        dst_addressing: None
+        | (t.Addressing.Group | t.Addressing.IEEE | t.Addressing.NWK) = None,
     ):
         """Send cluster requests as events."""
         if (
             self.server_commands is not None
             and self.server_commands.get(hdr.command_id) is not None
         ):
             self.listener_event(
@@ -153,15 +152,15 @@
 
     COORDINATOR_GROUP_ID = 0x30  # Group id with only coordinator as a member
 
     async def bind(self):
         """Bind cluster to a group."""
         # Ensure coordinator is a member of the group
         application = self._endpoint.device.application
-        coordinator = application.get_device(application.ieee)
+        coordinator = application.get_device(application.state.node_info.ieee)
         await coordinator.add_to_group(
             self.COORDINATOR_GROUP_ID,
             name="Coordinator Group - Created by ZHAQuirks",
         )
 
         # Bind cluster to group
         dstaddr = zdotypes.MultiAddress()
@@ -255,19 +254,18 @@
     """
 
     send_occupancy_event: bool = False
 
     def handle_cluster_request(
         self,
         hdr: foundation.ZCLHeader,
-        args: List[Any],
+        args: list[Any],
         *,
-        dst_addressing: Optional[
-            Union[t.Addressing.Group, t.Addressing.IEEE, t.Addressing.NWK]
-        ] = None,
+        dst_addressing: None
+        | (t.Addressing.Group | t.Addressing.IEEE | t.Addressing.NWK) = None,
     ):
         """Handle the cluster command."""
         # check if the command is for a zone status change of ZoneStatus.Alarm_1 or ZoneStatus.Alarm_2
         if hdr.command_id == ZONE_STATUS_CHANGE_COMMAND and args[0] & 3:
             if self._timer_handle:
                 self._timer_handle.cancel()
             self._timer_handle = self._loop.call_later(self.reset_s, self._turn_off)
@@ -345,19 +343,19 @@
             self.endpoint.device.motion_bus.listener_event(MOTION_EVENT)
             self._timer_handle = self._loop.call_later(self.reset_s, self._turn_off)
 
 
 class QuickInitDevice(CustomDevice):
     """Devices with quick initialization from quirk signature."""
 
-    signature: Optional[Dict[str, Any]] = None
+    signature: dict[str, Any] | None = None
 
     @classmethod
     def from_signature(
-        cls, device: zigpy.device.Device, model: Optional[str] = None
+        cls, device: zigpy.device.Device, model: str | None = None
     ) -> zigpy.device.Device:
         """Update device accordingly to quirk signature."""
 
         assert isinstance(cls.signature, dict)
         if model is None:
             model = cls.signature[MODEL]
         manufacturer = cls.signature.get(MANUFACTURER)
@@ -388,19 +386,57 @@
         device.status = zigpy.device.Status.ENDPOINTS_INIT
         device.manufacturer = manufacturer
         device.model = model
 
         return device
 
 
+class NoReplyMixin:
+    """A simple mixin.
+
+    Allows a cluster to have configurable list of command
+    ids that do not generate an explicit reply.
+    """
+
+    void_input_commands: set[int] = {}
+
+    async def command(self, command, *args, expect_reply=None, **kwargs):
+        """Override the default Cluster command.
+
+        expect_reply behavior is based on void_input_commands.
+        Note that this method changes the default value of
+        expect_reply to None. This allows the caller to explicitly force
+        expect_reply to true.
+        """
+
+        if expect_reply is None and command in self.void_input_commands:
+            cmd_expect_reply = False
+        elif expect_reply is None:
+            cmd_expect_reply = True  # the default
+        else:
+            cmd_expect_reply = expect_reply
+
+        rsp = await super().command(
+            command, *args, expect_reply=cmd_expect_reply, **kwargs
+        )
+
+        if expect_reply is None and command in self.void_input_commands:
+            # Pretend we received a default reply
+            return foundation.GENERAL_COMMANDS[
+                foundation.GeneralCommand.Default_Response
+            ].schema(command_id=command, status=foundation.Status.SUCCESS)
+
+        return rsp
+
+
 def setup(custom_quirks_path: str | None = None) -> None:
     """Register all quirks with zigpy, including optional custom quirks."""
 
     # Import all quirks in the `zhaquirks` package first
-    for importer, modname, _ispkg in pkgutil.walk_packages(
+    for _importer, modname, _ispkg in pkgutil.walk_packages(
         path=__path__,
         prefix=__name__ + ".",
     ):
         _LOGGER.debug("Loading quirks module %r", modname)
         importlib.import_module(modname)
 
     if custom_quirks_path is None:
```

### Comparing `zha-quirks-0.0.96/zhaquirks/adeo/color_controller.py` & `zha-quirks-0.0.97/zhaquirks/adeo/color_controller.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/aduro/adurolightncc.py` & `zha-quirks-0.0.97/zhaquirks/aduro/adurolightncc.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/aurora/aurora_dimmer.py` & `zha-quirks-0.0.97/zhaquirks/aurora/aurora_dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/bitron/thermostat.py` & `zha-quirks-0.0.97/zhaquirks/bitron/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/bosch/isw_zdl1_wp11g.py` & `zha-quirks-0.0.97/zhaquirks/bosch/isw_zdl1_wp11g.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/bosch/motion.py` & `zha-quirks-0.0.97/zhaquirks/bosch/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/__init__.py` & `zha-quirks-0.0.97/zhaquirks/centralite/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/cl_3130.py` & `zha-quirks-0.0.97/zhaquirks/centralite/cl_3130.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/cl_3157100.py` & `zha-quirks-0.0.97/zhaquirks/centralite/cl_3157100.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/cl_3300S.py` & `zha-quirks-0.0.97/zhaquirks/centralite/cl_3300S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/cl_3305S.py` & `zha-quirks-0.0.97/zhaquirks/centralite/cl_3305S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/cl_3310S.py` & `zha-quirks-0.0.97/zhaquirks/centralite/cl_3310S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/cl_3321S.py` & `zha-quirks-0.0.97/zhaquirks/centralite/cl_3321S.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/cl_3460L.py` & `zha-quirks-0.0.97/zhaquirks/centralite/cl_3460L.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/ias.py` & `zha-quirks-0.0.97/zhaquirks/centralite/ias.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/motion.py` & `zha-quirks-0.0.97/zhaquirks/centralite/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/centralite/motionandtemp.py` & `zha-quirks-0.0.97/zhaquirks/centralite/motionandtemp.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/const.py` & `zha-quirks-0.0.97/zhaquirks/const.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/danfoss/thermostat.py` & `zha-quirks-0.0.97/zhaquirks/danfoss/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/develco/__init__.py` & `zha-quirks-0.0.97/zhaquirks/develco/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/develco/air_quality.py` & `zha-quirks-0.0.97/zhaquirks/develco/air_quality.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/develco/heat_alarm.py` & `zha-quirks-0.0.97/zhaquirks/develco/heat_alarm.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/develco/motion.py` & `zha-quirks-0.0.97/zhaquirks/develco/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/develco/open_close.py` & `zha-quirks-0.0.97/zhaquirks/develco/open_close.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/develco/smoke_alarm.py` & `zha-quirks-0.0.97/zhaquirks/develco/smoke_alarm.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/echostar/bell.py` & `zha-quirks-0.0.97/zhaquirks/echostar/bell.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ecolink/contact.py` & `zha-quirks-0.0.97/zhaquirks/ecolink/contact.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/edpwithus/redy_plug.py` & `zha-quirks-0.0.97/zhaquirks/edpwithus/redy_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/elko/__init__.py` & `zha-quirks-0.0.97/zhaquirks/elko/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/elko/smart_super_thermostat.py` & `zha-quirks-0.0.97/zhaquirks/elko/smart_super_thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/eurotronic/__init__.py` & `zha-quirks-0.0.97/zhaquirks/eurotronic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
             rar = foundation.ReadAttributeRecord(
                 SYSTEM_MODE_ATTR, foundation.Status.SUCCESS, foundation.TypeValue()
             )
             rar.value.value = 0x4
             success.append(rar)
 
         if OCCUPIED_HEATING_SETPOINT_ATTR in attributes:
-
             _LOGGER.debug("intercepting OCC_HS")
 
             values = await super().read_attributes_raw(
                 [CURRENT_TEMP_SETPOINT_ATTR], manufacturer=MANUFACTURER
             )
 
             if len(values) == 2:
@@ -131,15 +130,14 @@
                 error.extend(values[1])
 
         return success, error
 
     def write_attributes(self, attributes, manufacturer=None):
         """Override wrong writes to thermostat attributes."""
         if "system_mode" in attributes:
-
             host_flags = self._attr_cache.get(HOST_FLAGS_ATTR, 1)
             _LOGGER.debug("current host_flags: %s", host_flags)
 
             if attributes.get("system_mode") == 0x0:
                 return super().write_attributes(
                     {"host_flags": host_flags | SET_OFF_MODE_FLAG}, MANUFACTURER
                 )
```

### Comparing `zha-quirks-0.0.96/zhaquirks/eurotronic/spzb0001.py` & `zha-quirks-0.0.97/zhaquirks/eurotronic/spzb0001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/feibit/switch.py` & `zha-quirks-0.0.97/zhaquirks/feibit/switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/gledopto/glc009.py` & `zha-quirks-0.0.97/zhaquirks/gledopto/glc009.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/gledopto/glc009p.py` & `zha-quirks-0.0.97/zhaquirks/gledopto/glc009p.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/gledopto/gls007z.py` & `zha-quirks-0.0.97/zhaquirks/gledopto/gls007z.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/gledopto/soposhgu10.py` & `zha-quirks-0.0.97/zhaquirks/gledopto/soposhgu10.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/heiman/smoke.py` & `zha-quirks-0.0.97/zhaquirks/heiman/smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/hivehome/mot003V0.py` & `zha-quirks-0.0.97/zhaquirks/hivehome/mot003V0.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/hivehome/mot003V6.py` & `zha-quirks-0.0.97/zhaquirks/hivehome/mot003V6.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/__init__.py` & `zha-quirks-0.0.97/zhaquirks/ikea/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Ikea module."""
 import logging
 
 from zigpy.quirks import CustomCluster
 import zigpy.types as t
 from zigpy.zcl import foundation
 from zigpy.zcl.clusters.general import PowerConfiguration, Scenes
-from zigpy.zcl.clusters.lightlink import LightLink
 
 from zhaquirks import DoublingPowerConfigurationCluster, EventableCluster
 
 _LOGGER = logging.getLogger(__name__)
 
 IKEA = "IKEA of Sweden"
 IKEA_CLUSTER_ID = 0xFC7C  # decimal = 64636
@@ -24,41 +23,14 @@
 BATTERY_SIZE = PowerConfiguration.attributes_by_name["battery_size"].id
 BATTERY_QUANTITY = PowerConfiguration.attributes_by_name["battery_quantity"].id
 BATTERY_RATED_VOLTAGE = PowerConfiguration.attributes_by_name[
     "battery_rated_voltage"
 ].id
 
 
-class LightLinkCluster(CustomCluster, LightLink):
-    """Ikea LightLink cluster."""
-
-    async def bind(self):
-        """Bind LightLink cluster to coordinator."""
-        application = self._endpoint.device.application
-        try:
-            coordinator = application.get_device(application.ieee)
-        except KeyError:
-            _LOGGER.warning("Aborting - unable to locate required coordinator device.")
-            return
-        group_list = await self.get_group_identifiers(0)
-        try:
-            group_record = group_list[2]
-            group_id = group_record[0].group_id
-        except IndexError:
-            _LOGGER.warning(
-                "unable to locate required group info - falling back to group 0x0000."
-            )
-            group_id = 0x0000
-        status = await coordinator.add_to_group(
-            group_id,
-            name="Default Lightlink Group",
-        )
-        return [status]
-
-
 class ScenesCluster(CustomCluster, Scenes):
     """Ikea Scenes cluster."""
 
     server_commands = Scenes.server_commands.copy()
     server_commands.update(
         {
             0x0007: foundation.ZCLCommandDef(
```

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/blinds.py` & `zha-quirks-0.0.97/zhaquirks/ikea/blinds.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/cctlightzha.py` & `zha-quirks-0.0.97/zhaquirks/ikea/cctlightzha.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/dimmer.py` & `zha-quirks-0.0.97/zhaquirks/ikea/dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/fivebtnremote.py` & `zha-quirks-0.0.97/zhaquirks/ikea/fivebtnremote.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     TURN_ON,
 )
 from zhaquirks.ikea import (
     IKEA,
     IKEA_CLUSTER_ID,
     WWAH_CLUSTER_ID,
     DoublingPowerConfig1CRCluster,
-    LightLinkCluster,
     PowerConfig1CRCluster,
     ScenesCluster,
 )
 
 
 class IkeaTradfriRemote1(CustomDevice):
     """Custom device representing ZLL version of IKEA five button remote."""
@@ -99,15 +98,15 @@
                 DEVICE_TYPE: zll.DeviceType.SCENE_CONTROLLER,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     DoublingPowerConfigurationCluster,
                     Identify.cluster_id,
                     Alarms.cluster_id,
                     Diagnostic.cluster_id,
-                    LightLinkCluster,
+                    LightLink.cluster_id,
                 ],
                 OUTPUT_CLUSTERS: [
                     Identify.cluster_id,
                     Groups.cluster_id,
                     ScenesCluster,
                     OnOff.cluster_id,
                     LevelControl.cluster_id,
@@ -305,15 +304,15 @@
                 PROFILE_ID: zha.PROFILE_ID,
                 DEVICE_TYPE: zha.DeviceType.COLOR_SCENE_CONTROLLER,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     DoublingPowerConfig1CRCluster,
                     Identify.cluster_id,
                     Alarms.cluster_id,
-                    LightLinkCluster,
+                    LightLink.cluster_id,
                 ],
                 OUTPUT_CLUSTERS: [
                     Identify.cluster_id,
                     Groups.cluster_id,
                     ScenesCluster,
                     OnOff.cluster_id,
                     LevelControl.cluster_id,
```

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/fourbtnremote.py` & `zha-quirks-0.0.97/zhaquirks/ikea/fourbtnremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/motion.py` & `zha-quirks-0.0.97/zhaquirks/ikea/motion.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     DEVICE_TYPE,
     ENDPOINTS,
     INPUT_CLUSTERS,
     MODELS_INFO,
     OUTPUT_CLUSTERS,
     PROFILE_ID,
 )
-from zhaquirks.ikea import IKEA, DoublingPowerConfig2CRCluster, LightLinkCluster
+from zhaquirks.ikea import IKEA, DoublingPowerConfig2CRCluster
 
 
 class IkeaTradfriMotion(CustomDevice):
     """Custom device representing IKEA of Sweden TRADFRI remote control."""
 
     signature = {
         # <SimpleDescriptor endpoint=1 profile=49246 device_type=2128
@@ -63,15 +63,15 @@
                 DEVICE_TYPE: zll.DeviceType.ON_OFF_SENSOR,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     DoublingPowerConfig2CRCluster,
                     Identify.cluster_id,
                     Alarms.cluster_id,
                     Diagnostic.cluster_id,
-                    LightLinkCluster,
+                    LightLink.cluster_id,
                 ],
                 OUTPUT_CLUSTERS: [
                     Identify.cluster_id,
                     Groups.cluster_id,
                     OnOff.cluster_id,
                     Ota.cluster_id,
                     LightLink.cluster_id,
```

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/motionzha.py` & `zha-quirks-0.0.97/zhaquirks/ikea/motionzha.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/opencloseremote.py` & `zha-quirks-0.0.97/zhaquirks/ikea/opencloseremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/shortcutbtn.py` & `zha-quirks-0.0.97/zhaquirks/ikea/shortcutbtn.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/starkvind.py` & `zha-quirks-0.0.97/zhaquirks/ikea/starkvind.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/symfonisk.py` & `zha-quirks-0.0.97/zhaquirks/ikea/symfonisk.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/symfonisk2.py` & `zha-quirks-0.0.97/zhaquirks/ikea/symfonisk2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/tradfriplug.py` & `zha-quirks-0.0.97/zhaquirks/ikea/tradfriplug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ikea/twobtnremote.py` & `zha-quirks-0.0.97/zhaquirks/ikea/twobtnremote.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,20 +36,15 @@
     OUTPUT_CLUSTERS,
     PARAMS,
     PROFILE_ID,
     SHORT_PRESS,
     TURN_OFF,
     TURN_ON,
 )
-from zhaquirks.ikea import (
-    IKEA,
-    IKEA_CLUSTER_ID,
-    DoublingPowerConfig1CRCluster,
-    LightLinkCluster,
-)
+from zhaquirks.ikea import IKEA, IKEA_CLUSTER_ID, DoublingPowerConfig1CRCluster
 
 
 class IkeaTradfriRemote2Btn(CustomDevice):
     """Custom device representing IKEA of Sweden TRADFRI remote control."""
 
     signature = {
         # <SimpleDescriptor endpoint=1 profile=260 device_type=2080
@@ -179,15 +174,15 @@
                 PROFILE_ID: zll.PROFILE_ID,
                 DEVICE_TYPE: zll.DeviceType.CONTROLLER,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     DoublingPowerConfig1CRCluster,
                     Identify.cluster_id,
                     Alarms.cluster_id,
-                    LightLinkCluster,
+                    LightLink.cluster_id,
                     IKEA_CLUSTER_ID,
                 ],
                 OUTPUT_CLUSTERS: [
                     Identify.cluster_id,
                     Groups.cluster_id,
                     OnOff.cluster_id,
                     LevelControl.cluster_id,
```

### Comparing `zha-quirks-0.0.96/zhaquirks/iluminize/cct.py` & `zha-quirks-0.0.97/zhaquirks/iluminize/cct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/iluminize/dim.py` & `zha-quirks-0.0.97/zhaquirks/iluminize/dim.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/imagic/gs1117s.py` & `zha-quirks-0.0.97/zhaquirks/imagic/gs1117s.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/imagic/im1116s.py` & `zha-quirks-0.0.97/zhaquirks/imagic/im1116s.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/innr/innr_sp120_plug.py` & `zha-quirks-0.0.97/zhaquirks/innr/innr_sp120_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/innr/innr_sp234_plug.py` & `zha-quirks-0.0.97/zhaquirks/innr/innr_sp234_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/innr/rs228t.py` & `zha-quirks-0.0.97/zhaquirks/innr/rs228t.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/inovelli/VZM31SN.py` & `zha-quirks-0.0.97/zhaquirks/inovelli/VZM31SN.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/inovelli/__init__.py` & `zha-quirks-0.0.97/zhaquirks/inovelli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,19 +104,22 @@
             0x0010: ("disable_remote_control", t.uint8_t, True),
             0x0011: ("load_level_indicator_timeout", t.uint8_t, True),
             0x0012: ("active_power_reports", t.uint8_t, True),
             0x0013: ("periodic_power_and_energy_reports", t.uint8_t, True),
             0x0014: ("active_energy_reports", t.uint16_t, True),
             0x0015: ("power_type", t.uint8_t, True),
             0x0016: ("switch_type", t.uint8_t, True),
+            0x0019: ("increased_non_neutral_output", t.Bool, True),
             0x0032: ("button_delay", t.uint8_t, True),
             0x0033: ("device_bind_number", t.uint8_t, True),
             0x0034: ("smart_bulb_mode", t.Bool, True),
-            0x0035: ("double_tap_up_for_max_brightness", t.Bool, True),
-            0x0036: ("double_tap_down_for_min_brightness", t.Bool, True),
+            0x0035: ("double_tap_up_enabled", t.Bool, True),
+            0x0036: ("double_tap_down_enabled", t.Bool, True),
+            0x0037: ("double_tap_up_level", t.uint8_t, True),
+            0x0038: ("double_tap_down_level", t.uint8_t, True),
             0x003C: ("default_led1_strip_color_when_on", t.uint8_t, True),
             0x003D: ("default_led1_strip_color_when_off", t.uint8_t, True),
             0x003E: ("default_led1_strip_intensity_when_on", t.uint8_t, True),
             0x003F: ("default_led1_strip_intensity_when_off", t.uint8_t, True),
             0x0041: ("default_led2_strip_color_when_on", t.uint8_t, True),
             0x0042: ("default_led2_strip_color_when_off", t.uint8_t, True),
             0x0043: ("default_led2_strip_intensity_when_on", t.uint8_t, True),
@@ -141,14 +144,17 @@
             0x005B: ("default_led7_strip_color_when_off", t.uint8_t, True),
             0x005C: ("default_led7_strip_intensity_when_on", t.uint8_t, True),
             0x005D: ("default_led7_strip_intensity_when_off", t.uint8_t, True),
             0x005F: ("led_color_when_on", t.uint8_t, True),
             0x0060: ("led_color_when_off", t.uint8_t, True),
             0x0061: ("led_intensity_when_on", t.uint8_t, True),
             0x0062: ("led_intensity_when_off", t.uint8_t, True),
+            0x0064: ("led_scaling_mode", t.Bool, True),
+            0x007B: ("aux_switch_scenes", t.Bool, True),
+            0x007D: ("binding_off_to_on_sync_level", t.Bool, True),
             0x0100: ("local_protection", t.Bool, True),
             0x0101: ("remote_protection", t.Bool, True),
             0x0102: ("output_mode", t.Bool, True),
             0x0103: ("on_off_led_mode", t.Bool, True),
             0x0104: ("firmware_progress_led", t.Bool, True),
             0x0105: ("relay_click_in_on_off_mode", t.Bool, True),
             0x0106: ("disable_clear_notifications_double_tap", t.Bool, True),
```

### Comparing `zha-quirks-0.0.96/zhaquirks/inovelli/types.py` & `zha-quirks-0.0.97/zhaquirks/inovelli/types.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/insta/nexentro_pushbutton_interface.py` & `zha-quirks-0.0.97/zhaquirks/insta/nexentro_pushbutton_interface.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/keenhome/sv02612mp13.py` & `zha-quirks-0.0.97/zhaquirks/keenhome/sv02612mp13.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/keenhome/weather.py` & `zha-quirks-0.0.97/zhaquirks/keenhome/weather.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/kof/kof_mr101z.py` & `zha-quirks-0.0.97/zhaquirks/nodon/switch.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,156 +1,133 @@
-"""Module to handle quirks of the King of Fans MR101Z ceiling fan receiver.
-
-The King of Fans ceiling fan receiver does not generate default replies. This
-module overrides all server commands that do not have a mandatory reply to not
-expect replies at all.
-"""
-
-from __future__ import annotations
-
+"""NodOn on/off switch two channels."""
 from zigpy.profiles import zha
-from zigpy.quirks import CustomCluster, CustomDevice
-from zigpy.zcl import foundation
+from zigpy.quirks import CustomDevice
 from zigpy.zcl.clusters.general import (
     Basic,
+    GreenPowerProxy,
     Groups,
     Identify,
     LevelControl,
     OnOff,
+    OnOffConfiguration,
     Ota,
     Scenes,
 )
-from zigpy.zcl.clusters.hvac import Fan
+from zigpy.zcl.clusters.lightlink import LightLink
 
 from zhaquirks.const import (
     DEVICE_TYPE,
     ENDPOINTS,
     INPUT_CLUSTERS,
-    MANUFACTURER,
+    MODELS_INFO,
     OUTPUT_CLUSTERS,
     PROFILE_ID,
 )
 
-
-class NoReplyMixin:
-    """A simple mixin.
-
-    Allows a cluster to have configurable list of command
-    ids that do not generate an explicit reply.
-    """
-
-    void_input_commands: set[int] = {}
-
-    async def command(self, command, *args, expect_reply=None, **kwargs):
-        """Override the default Cluster command.
-
-        expect_reply behavior is based on void_input_commands.
-        Note that this method changes the default value of
-        expect_reply to None. This allows the caller to explicitly force
-        expect_reply to true.
-        """
-
-        if expect_reply is None and command in self.void_input_commands:
-            cmd_expect_reply = False
-        elif expect_reply is None:
-            cmd_expect_reply = True  # the default
-        else:
-            cmd_expect_reply = expect_reply
-
-        rsp = await super(NoReplyMixin, self).command(
-            command, *args, expect_reply=cmd_expect_reply, **kwargs
-        )
-
-        if expect_reply is None and command in self.void_input_commands:
-            # Pretend we received a default reply
-            return foundation.GENERAL_COMMANDS[
-                foundation.GeneralCommand.Default_Response
-            ].schema(command_id=command, status=foundation.Status.SUCCESS)
-
-        return rsp
-
-
-class KofBasic(NoReplyMixin, CustomCluster, Basic):
-    """KOF Basic Cluster."""
-
-    void_input_commands = {
-        Basic.commands_by_name["reset_fact_default"].id,
-    }
-
-
-class KofIdentify(NoReplyMixin, CustomCluster, Identify):
-    """KOF Identify Cluster."""
-
-    void_input_commands = {
-        Identify.commands_by_name["identify"].id,
-        Identify.commands_by_name["trigger_effect"].id,
-    }
-
-
-class KofGroups(NoReplyMixin, CustomCluster, Groups):
-    """KOF Group Cluster."""
-
-    # Remove All Groups, Add Group If Identifying
-    void_input_commands = {
-        Groups.commands_by_name["remove_all"].id,
-        Groups.commands_by_name["add_if_identifying"].id,
-    }
-
-
-class KofScenes(NoReplyMixin, CustomCluster, Scenes):
-    """KOF Scene Cluster."""
-
-    void_input_commands = {Scenes.commands_by_name["recall"].id}
+WWAH_CLUSTER_ID = 0xFC57
 
 
-class KofOnOff(NoReplyMixin, CustomCluster, OnOff):
-    """KOF On Off Cluster."""
-
-    void_input_commands = {cmd.id for cmd in OnOff.commands_by_name.values()}
-
-
-class KofLevelControl(NoReplyMixin, CustomCluster, LevelControl):
-    """KOF Level Control Cluster."""
-
-    void_input_commands = {cmd.id for cmd in LevelControl.commands_by_name.values()}
-
-
-class CeilingFan(CustomDevice):
-    """Ceiling Fan Device."""
+class NodOnSIN4220(CustomDevice):
+    """NodOn on/off switch two channels."""
 
     signature = {
+        MODELS_INFO: [("NodOn", "SIN-4-2-20")],
         ENDPOINTS: {
+            # <SimpleDescriptor endpoint=1 profile=260 device_type=256
+            # input_clusters=[0, 3, 4, 5, 6, 7, 8, 4096, 64599]
+            # output_clusters=[3, 6, 25]>
             1: {
                 PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: 14,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     Identify.cluster_id,
                     Groups.cluster_id,
                     Scenes.cluster_id,
                     OnOff.cluster_id,
+                    OnOffConfiguration.cluster_id,
                     LevelControl.cluster_id,
-                    Fan.cluster_id,
+                    LightLink.cluster_id,
+                    WWAH_CLUSTER_ID,
+                ],
+                OUTPUT_CLUSTERS: [
+                    Identify.cluster_id,
+                    OnOff.cluster_id,
+                    Ota.cluster_id,
                 ],
-                OUTPUT_CLUSTERS: [Identify.cluster_id, Ota.cluster_id],
-            }
+            },
+            # <SimpleDescriptor endpoint=1 profile=260 device_type=256
+            # input_clusters=[0, 3, 4, 5, 6, 7, 8]
+            # output_clusters=[3, 6]>
+            2: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
+                INPUT_CLUSTERS: [
+                    Basic.cluster_id,
+                    Identify.cluster_id,
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    OnOff.cluster_id,
+                    OnOffConfiguration.cluster_id,
+                    LevelControl.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [
+                    Identify.cluster_id,
+                    OnOff.cluster_id,
+                ],
+            },
+            # <SimpleDescriptor endpoint=242 profile=41440 device_type=102
+            # input_clusters=[33]
+            # output_clusters=[33]
+            242: {
+                PROFILE_ID: 41440,
+                DEVICE_TYPE: 102,
+                INPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+                OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+            },
         },
-        MANUFACTURER: "King Of Fans,  Inc.",
     }
-
     replacement = {
         ENDPOINTS: {
             1: {
-                DEVICE_TYPE: zha.DeviceType.DIMMABLE_LIGHT,
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
                 INPUT_CLUSTERS: [
-                    KofBasic,
-                    KofIdentify,
-                    KofGroups,
-                    KofScenes,
-                    KofOnOff,
-                    KofLevelControl,
-                    Fan,
-                ],
-                OUTPUT_CLUSTERS: [Identify, Ota],
-            }
-        }
+                    Basic.cluster_id,
+                    Identify.cluster_id,
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    OnOff.cluster_id,
+                    OnOffConfiguration.cluster_id,
+                    LightLink.cluster_id,
+                    WWAH_CLUSTER_ID,
+                ],
+                OUTPUT_CLUSTERS: [
+                    Identify.cluster_id,
+                    OnOff.cluster_id,
+                    Ota.cluster_id,
+                ],
+            },
+            2: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
+                INPUT_CLUSTERS: [
+                    Basic.cluster_id,
+                    Identify.cluster_id,
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    OnOff.cluster_id,
+                    OnOffConfiguration.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [
+                    Identify.cluster_id,
+                    OnOff.cluster_id,
+                ],
+            },
+            242: {
+                PROFILE_ID: 41440,
+                DEVICE_TYPE: 102,
+                INPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+                OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+            },
+        },
     }
```

### Comparing `zha-quirks-0.0.96/zhaquirks/konke/__init__.py` & `zha-quirks-0.0.97/zhaquirks/konke/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/konke/button.py` & `zha-quirks-0.0.97/zhaquirks/konke/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/konke/magnet.py` & `zha-quirks-0.0.97/zhaquirks/konke/magnet.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/konke/motion.py` & `zha-quirks-0.0.97/zhaquirks/konke/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/konke/temp.py` & `zha-quirks-0.0.97/zhaquirks/konke/temp.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/lds/cctswitch.py` & `zha-quirks-0.0.97/zhaquirks/lds/cctswitch.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     MODELS_INFO,
     OUTPUT_CLUSTERS,
     PARAMS,
     PROFILE_ID,
     SHORT_PRESS,
     TURN_ON,
 )
-from zhaquirks.lds import MANUFACTURER, LightLinkCluster
+from zhaquirks.lds import MANUFACTURER
 
 
 class CCTSwitch(CustomDevice):
     """Custom device representing CCTSwitch-D0001 remote control."""
 
     signature = {
         # <SimpleDescriptor endpoint = 1 profile = 260 device_type = 2048
@@ -77,15 +77,15 @@
             1: {
                 PROFILE_ID: zha.PROFILE_ID,
                 DEVICE_TYPE: zha.DeviceType.COLOR_CONTROLLER,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     PowerConfiguration.cluster_id,
                     Identify.cluster_id,
-                    LightLinkCluster,
+                    LightLink.cluster_id,
                     0xFD01,
                 ],
                 OUTPUT_CLUSTERS: [
                     Identify.cluster_id,
                     Groups.cluster_id,
                     OnOff.cluster_id,
                     LevelControl.cluster_id,
```

### Comparing `zha-quirks-0.0.96/zhaquirks/ledvance/a19rgbw.py` & `zha-quirks-0.0.97/zhaquirks/ledvance/a19rgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/ledvance/flexrgbw.py` & `zha-quirks-0.0.97/zhaquirks/ledvance/flexrgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/legrand/dimmer.py` & `zha-quirks-0.0.97/zhaquirks/legrand/dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/lidl/TS0501A.py` & `zha-quirks-0.0.97/zhaquirks/lidl/TS0501A.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/lidl/cct.py` & `zha-quirks-0.0.97/zhaquirks/lidl/cct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/lidl/rgbcct.py` & `zha-quirks-0.0.97/zhaquirks/lidl/rgbcct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/lidl/ts011f_plug.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0046.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,169 +1,165 @@
-"""LIDL TS011F plug."""
-from __future__ import annotations
+"""Tuya 6 Button Remote."""
 
-import asyncio
-import logging
-
-import zigpy
 from zigpy.profiles import zha
-from zigpy.quirks import CustomCluster
-import zigpy.types as t
-from zigpy.zcl.clusters.general import (
-    Basic,
-    GreenPowerProxy,
-    Groups,
-    Identify,
-    OnOff,
-    Ota,
-    Scenes,
-    Time,
-)
+from zigpy.zcl.clusters.general import Basic, OnOff, Ota, PowerConfiguration, Time
 
 from zhaquirks.const import (
+    BUTTON_1,
+    BUTTON_2,
+    BUTTON_3,
+    BUTTON_4,
+    BUTTON_5,
+    BUTTON_6,
+    COMMAND,
     DEVICE_TYPE,
+    DOUBLE_PRESS,
+    ENDPOINT_ID,
     ENDPOINTS,
     INPUT_CLUSTERS,
+    LONG_PRESS,
     MODEL,
     OUTPUT_CLUSTERS,
     PROFILE_ID,
+    SHORT_PRESS,
 )
-from zhaquirks.tuya.ts011f_plug import Plug_3AC_4USB
+from zhaquirks.tuya import (
+    TuyaNoBindPowerConfigurationCluster,
+    TuyaSmartRemoteOnOffCluster,
+    TuyaZBE000Cluster,
+)
+from zhaquirks.tuya.mcu import EnchantedDevice
 
-_LOGGER = logging.getLogger(__name__)
 
+class Tuya6ButtonTriggers:
+    """Tuya 6-button remote device triggers."""
 
-async def cast_tuya_magic_spell_task(
-    dev: zigpy.device.Device, tries: int = 100, rejoin: bool = False
-) -> None:
-    """Initialize device so that all endpoints become available."""
-    import inspect
-
-    basic_cluster = dev.endpoints[1].in_clusters[0]
-
-    # The magic spell is needed only once.
-    # TODO: Improve by doing this only once (successfully).
-
-    # Magic spell - part 1
-    # Note: attribute order is important
-    attr_to_read = [
-        "manufacturer",
-        "zcl_version",
-        "app_version",
-        "model",
-        "power_source",
-        0xFFFE,
-    ]
-    if "tries" in inspect.getfullargspec(basic_cluster.read_attributes)[0]:
-        _LOGGER.debug(f"Cast Tuya Magic Spell on {dev.ieee!r} with {tries} tries")
-        res = await basic_cluster.read_attributes(attr_to_read, tries=tries)
-    else:
-        _LOGGER.debug(f"Cast Tuya Magic Spell on {dev.ieee!r}")
-        res = await basic_cluster.read_attributes(attr_to_read)
-
-    _LOGGER.debug(f"Tuya Magic Spell result {res!r} for {dev.ieee!r}")
-
-    # Magic spell - part 2 (skipped - does not seem to be needed)
-    # attr_to_write={0xffde:13}
-    # basic_cluster.write_attributes(attr_to_write)
-
-    if rejoin:
-        # Leave with rejoin - may need to be adjuste to work everywhere
-        # or require a minimum zigpy version
-        # This should have the device leave and rejoin immediately triggering
-        # the discovery of the endpoints that appear after the magic trick
-
-        # Note: this is not validated yet and disabled by default
-        _LOGGER.debug(f"Send leave with rejoin request to {dev.ieee!r}")
-        res = await dev.zdo.request(0x0034, dev.ieee, 0x01, tries)
-        _LOGGER.debug(f"Leave with rejoin result {res!r} for {dev.ieee!r}")
-
-        app = dev.application
-        # Delete the device from the database
-        app.listener_event("device_removed", dev)
-
-        # Delete the device from zigpy
-        app.devices.pop(dev.ieee, None)
-
-
-def cast_tuya_magic_spell(dev: zigpy.device.Device, tries: int = 3) -> None:
-    """Set up the magic spell asynchronously."""
-
-    # Note for sleepy devices the number of tries may need to be increased to 100.
-
-    dev._magic_spell_task = asyncio.create_task(
-        cast_tuya_magic_spell_task(dev, tries=tries)
-    )
-
-
-class TuyaBasicCluster(CustomCluster, Basic):
-    """Provide Tuya Basic Cluster with magic spell."""
-
-    attributes = Basic.attributes.copy()
-    attributes.update(
-        {
-            0xFFDE: ("tuya_FFDE", t.uint8_t, True),
-            # 0xffe0: ("tuya_FFE0", TODO.Array, True),
-            # 0xffe1: ("tuya_FFE1", TODO.Array, True),
-            0xFFE2: ("tuya_FFE2", t.uint8_t, True),
-            # 0xffe3: ("tuya_FFE3", TODO.Array, True),
-        }
-    )
-
-    async def bind(self):
-        """Bind cluster."""
-
-        _LOGGER.debug(
-            f"Requesting Tuya Magic Spell for {self.ieee!r} in basic bind method"
-        )
-        tries = 3
-        await asyncio.create_task(cast_tuya_magic_spell_task(self, tries=tries))
-
-        return await super().bind()
-
-
-class Lidl_Plug_3AC_4USB(Plug_3AC_4USB):
-    """LIDL 3 outlets + 4 USB with restore power state support."""
-
-    def __init__(self, *args, **kwargs):
-        """Initialize with task."""
-        super().__init__(*args, **kwargs)
-
-        # Use 'external' version that could be called from cluster
-        # customiation
-        cast_tuya_magic_spell(self, tries=3)
+    device_automation_triggers = {
+        (SHORT_PRESS, BUTTON_1): {ENDPOINT_ID: 1, COMMAND: SHORT_PRESS},
+        (LONG_PRESS, BUTTON_1): {ENDPOINT_ID: 1, COMMAND: LONG_PRESS},
+        (DOUBLE_PRESS, BUTTON_1): {ENDPOINT_ID: 1, COMMAND: DOUBLE_PRESS},
+        (SHORT_PRESS, BUTTON_2): {ENDPOINT_ID: 2, COMMAND: SHORT_PRESS},
+        (LONG_PRESS, BUTTON_2): {ENDPOINT_ID: 2, COMMAND: LONG_PRESS},
+        (DOUBLE_PRESS, BUTTON_2): {ENDPOINT_ID: 2, COMMAND: DOUBLE_PRESS},
+        (SHORT_PRESS, BUTTON_3): {ENDPOINT_ID: 3, COMMAND: SHORT_PRESS},
+        (LONG_PRESS, BUTTON_3): {ENDPOINT_ID: 3, COMMAND: LONG_PRESS},
+        (DOUBLE_PRESS, BUTTON_3): {ENDPOINT_ID: 3, COMMAND: DOUBLE_PRESS},
+        (SHORT_PRESS, BUTTON_4): {ENDPOINT_ID: 4, COMMAND: SHORT_PRESS},
+        (LONG_PRESS, BUTTON_4): {ENDPOINT_ID: 4, COMMAND: LONG_PRESS},
+        (DOUBLE_PRESS, BUTTON_4): {ENDPOINT_ID: 4, COMMAND: DOUBLE_PRESS},
+        (SHORT_PRESS, BUTTON_5): {ENDPOINT_ID: 5, COMMAND: SHORT_PRESS},
+        (LONG_PRESS, BUTTON_5): {ENDPOINT_ID: 5, COMMAND: LONG_PRESS},
+        (DOUBLE_PRESS, BUTTON_5): {ENDPOINT_ID: 5, COMMAND: DOUBLE_PRESS},
+        (SHORT_PRESS, BUTTON_6): {ENDPOINT_ID: 6, COMMAND: SHORT_PRESS},
+        (LONG_PRESS, BUTTON_6): {ENDPOINT_ID: 6, COMMAND: LONG_PRESS},
+        (DOUBLE_PRESS, BUTTON_6): {ENDPOINT_ID: 6, COMMAND: DOUBLE_PRESS},
+    }
+
+
+class TuyaSmartRemote0046(EnchantedDevice, Tuya6ButtonTriggers):
+    """Tuya 6-button remote device with time on out cluster."""
 
     signature = {
-        MODEL: "TS011F",
+        # SizePrefixedSimpleDescriptor(endpoint=1, profile=260, device_type=0, device_version=1, input_clusters=[0, 1, 6, 57344], output_clusters=[10, 25]))
+        # SizePrefixedSimpleDescriptor(endpoint=2, profile=260, device_type=0, device_version=1, input_clusters=[1, 6], output_clusters=[])
+        # SizePrefixedSimpleDescriptor(endpoint=3, profile=260, device_type=0, device_version=1, input_clusters=[1, 6], output_clusters=[])
+        # SizePrefixedSimpleDescriptor(endpoint=4, profile=260, device_type=0, device_version=1, input_clusters=[1, 6], output_clusters=[])
+        MODEL: "TS0046",
         ENDPOINTS: {
-            # <SimpleDescriptor endpoint=1 profile=260 device_type=266
-            # device_version=1
-            # input_clusters=[0, 3, 4, 5, 6]
-            # output_clusters=[10, 25]>
             1: {
                 PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_SWITCH,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
-                    Identify.cluster_id,
-                    Groups.cluster_id,
-                    Scenes.cluster_id,
+                    PowerConfiguration.cluster_id,
                     OnOff.cluster_id,
+                    TuyaZBE000Cluster.cluster_id,
                 ],
                 OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
             },
-            # <SimpleDescriptor endpoint=242 profile=41440 device_type=97
-            # device_version=1
-            # input_clusters=[]
-            # output_clusters=[33]>
-            242: {
-                PROFILE_ID: 41440,
-                DEVICE_TYPE: 97,
+            2: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_SWITCH,
+                INPUT_CLUSTERS: [
+                    PowerConfiguration.cluster_id,
+                    OnOff.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [],
+            },
+            3: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_SWITCH,
+                INPUT_CLUSTERS: [
+                    PowerConfiguration.cluster_id,
+                    OnOff.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [],
+            },
+            4: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_SWITCH,
+                INPUT_CLUSTERS: [
+                    PowerConfiguration.cluster_id,
+                    OnOff.cluster_id,
+                ],
+                OUTPUT_CLUSTERS: [],
+            },
+        },
+    }
+    replacement = {
+        ENDPOINTS: {
+            1: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.REMOTE_CONTROL,
+                INPUT_CLUSTERS: [
+                    Basic.cluster_id,
+                    TuyaNoBindPowerConfigurationCluster,
+                    TuyaZBE000Cluster,
+                ],
+                OUTPUT_CLUSTERS: [
+                    TuyaSmartRemoteOnOffCluster,
+                    Time.cluster_id,
+                    Ota.cluster_id,
+                ],
+            },
+            2: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.REMOTE_CONTROL,
                 INPUT_CLUSTERS: [],
-                OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+                OUTPUT_CLUSTERS: [
+                    TuyaSmartRemoteOnOffCluster,
+                ],
+            },
+            3: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.REMOTE_CONTROL,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [
+                    TuyaSmartRemoteOnOffCluster,
+                ],
+            },
+            4: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.REMOTE_CONTROL,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [
+                    TuyaSmartRemoteOnOffCluster,
+                ],
+            },
+            5: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.REMOTE_CONTROL,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [
+                    TuyaSmartRemoteOnOffCluster,
+                ],
+            },
+            6: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.REMOTE_CONTROL,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [
+                    TuyaSmartRemoteOnOffCluster,
+                ],
             },
         },
     }
-
-    # Uncomment to try TuyaBasicCluster implementation
-    # Rename __init__ to disabled__init__ as well
-    # replacement[1][INPUT_CLUSTERS][0] = TuyaBasicCluster
```

### Comparing `zha-quirks-0.0.96/zhaquirks/linkind/a001082.py` & `zha-quirks-0.0.97/zhaquirks/linkind/a001082.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/linkind/motion.py` & `zha-quirks-0.0.97/zhaquirks/linkind/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/lixee/zlinky.py` & `zha-quirks-0.0.97/zhaquirks/lixee/zlinky.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/lutron/lzl4bwhl01remote.py` & `zha-quirks-0.0.97/zhaquirks/lutron/lzl4bwhl01remote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/mli/tint.py` & `zha-quirks-0.0.97/zhaquirks/mli/tint.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/mli/tintE14rgbcct.py` & `zha-quirks-0.0.97/zhaquirks/mli/tintE14rgbcct.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/netvox/z308e3ed.py` & `zha-quirks-0.0.97/zhaquirks/netvox/z308e3ed.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/nodon/switch.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0121_plug.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,133 +1,187 @@
-"""NodOn on/off switch two channels."""
+"""Tuya TS0121 plug."""
 from zigpy.profiles import zha
 from zigpy.quirks import CustomDevice
-from zigpy.zcl.clusters.general import (
-    Basic,
-    GreenPowerProxy,
-    Groups,
-    Identify,
-    LevelControl,
-    OnOff,
-    OnOffConfiguration,
-    Ota,
-    Scenes,
-)
-from zigpy.zcl.clusters.lightlink import LightLink
+from zigpy.zcl.clusters.general import Basic, Groups, Identify, OnOff, Ota, Scenes, Time
+from zigpy.zcl.clusters.homeautomation import ElectricalMeasurement
+from zigpy.zcl.clusters.smartenergy import Metering
 
 from zhaquirks.const import (
     DEVICE_TYPE,
     ENDPOINTS,
     INPUT_CLUSTERS,
-    MODELS_INFO,
+    MODEL,
     OUTPUT_CLUSTERS,
     PROFILE_ID,
 )
-
-WWAH_CLUSTER_ID = 0xFC57
+from zhaquirks.tuya import (
+    TuyaNewManufCluster,
+    TuyaZBE000Cluster,
+    TuyaZBElectricalMeasurement,
+    TuyaZBExternalSwitchTypeCluster,
+    TuyaZBMeteringCluster,
+    TuyaZBOnOffAttributeCluster,
+)
 
 
-class NodOnSIN4220(CustomDevice):
-    """NodOn on/off switch two channels."""
+class Plug(CustomDevice):
+    """Tuya TS0121 plug with restore tuya power state support."""
 
     signature = {
-        MODELS_INFO: [("NodOn", "SIN-4-2-20")],
+        MODEL: "TS0121",
         ENDPOINTS: {
-            # <SimpleDescriptor endpoint=1 profile=260 device_type=256
-            # input_clusters=[0, 3, 4, 5, 6, 7, 8, 4096, 64599]
-            # output_clusters=[3, 6, 25]>
+            # <SimpleDescriptor endpoint=1 profile=260 device_type=81
+            # device_version=1
+            # input_clusters=[0, 4, 5, 6, 9, 1794, 2820]
+            # output_clusters=[10, 25]>
             1: {
                 PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
+                DEVICE_TYPE: zha.DeviceType.SMART_PLUG,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
-                    Identify.cluster_id,
                     Groups.cluster_id,
                     Scenes.cluster_id,
                     OnOff.cluster_id,
-                    OnOffConfiguration.cluster_id,
-                    LevelControl.cluster_id,
-                    LightLink.cluster_id,
-                    WWAH_CLUSTER_ID,
-                ],
-                OUTPUT_CLUSTERS: [
-                    Identify.cluster_id,
-                    OnOff.cluster_id,
-                    Ota.cluster_id,
+                    Metering.cluster_id,
+                    ElectricalMeasurement.cluster_id,
                 ],
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
             },
-            # <SimpleDescriptor endpoint=1 profile=260 device_type=256
-            # input_clusters=[0, 3, 4, 5, 6, 7, 8]
-            # output_clusters=[3, 6]>
-            2: {
+        },
+    }
+    replacement = {
+        ENDPOINTS: {
+            1: {
                 PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
+                DEVICE_TYPE: zha.DeviceType.SMART_PLUG,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
-                    Identify.cluster_id,
                     Groups.cluster_id,
                     Scenes.cluster_id,
-                    OnOff.cluster_id,
-                    OnOffConfiguration.cluster_id,
-                    LevelControl.cluster_id,
+                    TuyaZBOnOffAttributeCluster,
+                    TuyaZBMeteringCluster,
+                    TuyaZBElectricalMeasurement,
                 ],
-                OUTPUT_CLUSTERS: [
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
+            },
+        },
+    }
+
+
+class TS0121B(CustomDevice):
+    """Tuya TS0121 plug with restore tuya power state support and ZGP endpoint."""
+
+    signature = {
+        MODEL: "TS0121",
+        ENDPOINTS: {
+            1: {
+                PROFILE_ID: zha.PROFILE_ID,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
+                INPUT_CLUSTERS: [
+                    Basic.cluster_id,
                     Identify.cluster_id,
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
                     OnOff.cluster_id,
+                    Metering.cluster_id,
+                    ElectricalMeasurement.cluster_id,
+                    TuyaZBE000Cluster.cluster_id,
+                    TuyaZBExternalSwitchTypeCluster.cluster_id,
                 ],
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
             },
-            # <SimpleDescriptor endpoint=242 profile=41440 device_type=102
-            # input_clusters=[33]
-            # output_clusters=[33]
             242: {
-                PROFILE_ID: 41440,
-                DEVICE_TYPE: 102,
-                INPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
-                OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+                PROFILE_ID: 0xA1E0,
+                DEVICE_TYPE: 0x0061,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [0x0021],
             },
         },
     }
     replacement = {
         ENDPOINTS: {
             1: {
                 PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
+                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     Identify.cluster_id,
                     Groups.cluster_id,
                     Scenes.cluster_id,
-                    OnOff.cluster_id,
-                    OnOffConfiguration.cluster_id,
-                    LightLink.cluster_id,
-                    WWAH_CLUSTER_ID,
-                ],
-                OUTPUT_CLUSTERS: [
-                    Identify.cluster_id,
-                    OnOff.cluster_id,
-                    Ota.cluster_id,
+                    TuyaZBOnOffAttributeCluster,
+                    TuyaZBMeteringCluster,
+                    TuyaZBElectricalMeasurement,
+                    TuyaZBE000Cluster,
+                    TuyaZBExternalSwitchTypeCluster,
                 ],
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
             },
-            2: {
+            242: {
+                PROFILE_ID: 0xA1E0,
+                DEVICE_TYPE: 0x0061,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [0x0021],
+            },
+        },
+    }
+
+
+class TS0121_Var03(CustomDevice):
+    """Tuya TS0121 plug DeviceType.MAIN_POWER_OUTLET."""
+
+    signature = {
+        MODEL: "TS0121",
+        ENDPOINTS: {
+            1: {
+                # "profile_id": 260,
+                # "device_type": "0x0009",
+                # "in_clusters": ["0x0000","0x0003","0x0004","0x0005","0x0006","0x0702","0x0b04","0xef00"],
+                # "out_clusters": ["0x000a","0x0019"]
                 PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.ON_OFF_LIGHT,
+                DEVICE_TYPE: zha.DeviceType.MAIN_POWER_OUTLET,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     Identify.cluster_id,
                     Groups.cluster_id,
                     Scenes.cluster_id,
                     OnOff.cluster_id,
-                    OnOffConfiguration.cluster_id,
+                    Metering.cluster_id,
+                    ElectricalMeasurement.cluster_id,
+                    TuyaNewManufCluster.cluster_id,
                 ],
-                OUTPUT_CLUSTERS: [
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
+            },
+            242: {
+                # "profile_id": 41440,
+                # "device_type": "0x0061",
+                # "in_clusters": [],
+                # "out_clusters": ["0x0021"]
+                PROFILE_ID: 0xA1E0,
+                DEVICE_TYPE: 0x0061,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [0x0021],
+            },
+        },
+    }
+    replacement = {
+        ENDPOINTS: {
+            1: {
+                INPUT_CLUSTERS: [
+                    Basic.cluster_id,
                     Identify.cluster_id,
-                    OnOff.cluster_id,
+                    Groups.cluster_id,
+                    Scenes.cluster_id,
+                    TuyaZBOnOffAttributeCluster,
+                    TuyaZBMeteringCluster,
+                    TuyaZBElectricalMeasurement,
+                    TuyaNewManufCluster,
                 ],
+                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
             },
             242: {
-                PROFILE_ID: 41440,
-                DEVICE_TYPE: 102,
-                INPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
-                OUTPUT_CLUSTERS: [GreenPowerProxy.cluster_id],
+                PROFILE_ID: 0xA1E0,
+                DEVICE_TYPE: 0x0061,
+                INPUT_CLUSTERS: [],
+                OUTPUT_CLUSTERS: [0x0021],
             },
         },
     }
```

### Comparing `zha-quirks-0.0.96/zhaquirks/nue/auwz02000.py` & `zha-quirks-0.0.97/zhaquirks/nue/auwz02000.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/orvibo/dimmer.py` & `zha-quirks-0.0.97/zhaquirks/orvibo/dimmer.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/orvibo/motion.py` & `zha-quirks-0.0.97/zhaquirks/orvibo/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/a19rgbw.py` & `zha-quirks-0.0.97/zhaquirks/osram/a19rgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/cla60tw.py` & `zha-quirks-0.0.97/zhaquirks/osram/cla60tw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/flexrgbw.py` & `zha-quirks-0.0.97/zhaquirks/osram/flexrgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/gardenpolesrgbw.py` & `zha-quirks-0.0.97/zhaquirks/osram/gardenpolesrgbw.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/lightifyx4.py` & `zha-quirks-0.0.97/zhaquirks/osram/lightifyx4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/osramplug.py` & `zha-quirks-0.0.97/zhaquirks/osram/osramplug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/smartplusac05347.py` & `zha-quirks-0.0.97/zhaquirks/osram/smartplusac05347.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/switchmini.py` & `zha-quirks-0.0.97/zhaquirks/osram/switchmini.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/osram/tunablewhite.py` & `zha-quirks-0.0.97/zhaquirks/osram/tunablewhite.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/paulmann/fourbtnremote.py` & `zha-quirks-0.0.97/zhaquirks/paulmann/fourbtnremote.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/philio/pst03a.py` & `zha-quirks-0.0.97/zhaquirks/philio/pst03a.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/philips/__init__.py` & `zha-quirks-0.0.97/zhaquirks/philips/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/philips/motion.py` & `zha-quirks-0.0.97/zhaquirks/philips/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/philips/rdm001.py` & `zha-quirks-0.0.97/zhaquirks/philips/rdm001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/philips/rom001.py` & `zha-quirks-0.0.97/zhaquirks/philips/rom001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/philips/rwl022.py` & `zha-quirks-0.0.97/zhaquirks/philips/rwl022.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/philips/rwlfirstgen.py` & `zha-quirks-0.0.97/zhaquirks/philips/rwlfirstgen.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/plaid/soil.py` & `zha-quirks-0.0.97/zhaquirks/plaid/soil.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/salus/sp600.py` & `zha-quirks-0.0.97/zhaquirks/salus/sp600.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/samjin/__init__.py` & `zha-quirks-0.0.97/zhaquirks/samjin/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,9 +35,9 @@
         if hdr.command_id == 0:
             state = args[0] & 3
             event_args = {
                 PRESS_TYPE: CLICK_TYPES[state],
                 COMMAND_ID: hdr.command_id,
                 ARGS: args,
             }
-            action = "button_{}".format(CLICK_TYPES[state])
+            action = f"button_{CLICK_TYPES[state]}"
             self.listener_event(ZHA_SEND_EVENT, action, event_args)
```

### Comparing `zha-quirks-0.0.96/zhaquirks/samjin/button.py` & `zha-quirks-0.0.97/zhaquirks/samjin/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/samjin/button2.py` & `zha-quirks-0.0.97/zhaquirks/samjin/button2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/samjin/multi2.py` & `zha-quirks-0.0.97/zhaquirks/samjin/multi2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sengled/e1e_g7f.py` & `zha-quirks-0.0.97/zhaquirks/sengled/e1e_g7f.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sercomm/szwtd02n.py` & `zha-quirks-0.0.97/zhaquirks/sercomm/szwtd02n.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/siglis/zigfred.py` & `zha-quirks-0.0.97/zhaquirks/siglis/zigfred.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sinope/__init__.py` & `zha-quirks-0.0.97/zhaquirks/sinope/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sinope/light.py` & `zha-quirks-0.0.97/zhaquirks/sinope/light.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sinope/sensor.py` & `zha-quirks-0.0.97/zhaquirks/sinope/sensor.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sinope/switch.py` & `zha-quirks-0.0.97/zhaquirks/sinope/switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sinope/thermostat.py` & `zha-quirks-0.0.97/zhaquirks/sinope/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/__init__.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/moisturev4.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/moisturev4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/motion.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/multi.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/multi.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/multiv4.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/multiv4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/pgc313.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/pgc313.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/pgc314.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/pgc314.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartthings/tag_v4.py` & `zha-quirks-0.0.97/zhaquirks/smartthings/tag_v4.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/smartwings/wm25lz.py` & `zha-quirks-0.0.97/zhaquirks/smartwings/wm25lz.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     MODELS_INFO,
     OUTPUT_CLUSTERS,
     PROFILE_ID,
 )
 
 
 class InvertedWindowCoveringCluster(CustomCluster, WindowCovering):
-    """This WindowCovering cluster implementation inverts the commands for up and down."""
+    """WindowCovering cluster implementation that inverts the commands for up and down."""
 
     CMD_UP_OPEN = WindowCovering.commands_by_name["up_open"].id
     CMD_DOWN_CLOSE = WindowCovering.commands_by_name["down_close"].id
 
     async def command(
         self,
         command_id: foundation.GeneralCommand | int | t.uint8_t,
```

### Comparing `zha-quirks-0.0.96/zhaquirks/sonoff/button.py` & `zha-quirks-0.0.97/zhaquirks/sonoff/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/sourcingandcreation/smart_button.py` & `zha-quirks-0.0.97/zhaquirks/sourcingandcreation/smart_button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/terncy/__init__.py` & `zha-quirks-0.0.97/zhaquirks/terncy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             if (state, count) in self._last_clicks:
                 return  # ignore repeated event for single action.
             else:
                 self._last_clicks.append((state, count))
             if state > 5:
                 state = 5
             event_args = {PRESS_TYPE: CLICK_TYPES[state], "count": count, VALUE: state}
-            action = "button_{}".format(CLICK_TYPES[state])
+            action = f"button_{CLICK_TYPES[state]}"
             self.listener_event(ZHA_SEND_EVENT, action, event_args)
         elif hdr.command_id == 4:  # motion event
             state = args[2]
             side = SIDE_LOOKUP[state]
             if side == LEFT:
                 self.endpoint.device.motion_left_bus.listener_event(MOTION_EVENT)
             elif side == RIGHT:
```

### Comparing `zha-quirks-0.0.96/zhaquirks/terncy/pp01.py` & `zha-quirks-0.0.97/zhaquirks/terncy/pp01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/terncy/sd01.py` & `zha-quirks-0.0.97/zhaquirks/terncy/sd01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/texasinstruments/router.py` & `zha-quirks-0.0.97/zhaquirks/texasinstruments/router.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/thirdreality/button.py` & `zha-quirks-0.0.97/zhaquirks/thirdreality/button.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/thirdreality/switch.py` & `zha-quirks-0.0.97/zhaquirks/thirdreality/switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/trust/zpir8000.py` & `zha-quirks-0.0.97/zhaquirks/trust/zpir8000.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/__init__.py` & `zha-quirks-0.0.97/zhaquirks/tuya/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 TUYA_LEVEL_COMMAND = 514
 
 COVER_EVENT = "cover_event"
 LEVEL_EVENT = "level_event"
 TUYA_MCU_COMMAND = "tuya_mcu_command"
 
 # Rotating for remotes
-STOP = "stop"  # To constans
+STOP = "stop"  # To constants
 
 # ---------------------------------------------------------
 # Value for dp_type
 # ---------------------------------------------------------
 # ID    Name            Description
 # ---------------------------------------------------------
 # 0x00 	DP_TYPE_RAW 	?
@@ -212,15 +212,15 @@
 
         if value is None:
             return
         elif isinstance(value, (t.bitmap8, t.bitmap16, t.bitmap32)):
             self.dp_type = TuyaDPType.BITMAP
         elif isinstance(value, (bool, t.Bool)):
             self.dp_type = TuyaDPType.BOOL
-        elif isinstance(value, enum.Enum):
+        elif isinstance(value, enum.Enum):  # type: ignore # noqa
             self.dp_type = TuyaDPType.ENUM
         elif isinstance(value, int):
             self.dp_type = TuyaDPType.VALUE
         elif isinstance(value, str):
             self.dp_type = TuyaDPType.STRING
         else:
             self.dp_type = TuyaDPType.RAW
```

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/air/__init__.py` & `zha-quirks-0.0.97/zhaquirks/tuya/air/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/air/ts0601_air_quality.py` & `zha-quirks-0.0.97/zhaquirks/tuya/air/ts0601_air_quality.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/mcu/__init__.py` & `zha-quirks-0.0.97/zhaquirks/tuya/mcu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,14 @@
         """Defer attributes writing to the set_data tuya command."""
 
         await super().write_attributes(attributes, manufacturer)
 
         records = self._write_attr_records(attributes)
 
         for record in records:
-
             self.debug("write_attributes --> record: %s", record)
 
             cluster_data = TuyaClusterData(
                 endpoint_id=self.endpoint.endpoint_id,
                 cluster_name=self.ep_attribute,
                 cluster_attr=self.attributes[record.attrid].name,
                 attr_value=record.value.value,
@@ -144,15 +143,15 @@
                 # is converted from HEX -> BIN -> XX.XX.XXXX -> DEC (x.y.z)
                 # example: 0x98 -> 10011000 -> 10.01.1000 -> 2.1.8
                 # https://developer.tuya.com/en/docs/iot-device-dev/firmware-version-description?id=K9zzuc5n2gff8#title-1-Zigbee%20firmware%20versions
                 major = self.version_raw >> 6
                 minor = (self.version_raw & 63) >> 4
                 release = self.version_raw & 15
 
-                return "{}.{}.{}".format(major, minor, release)
+                return f"{major}.{minor}.{release}"
 
             return None
 
     class TuyaConnectionStatus(t.Struct):
         """Tuya connection status data."""
 
         tsn: t.uint8_t
```

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/sm0202_motion.py` & `zha-quirks-0.0.97/zhaquirks/tuya/sm0202_motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts000x.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts000x.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts001x.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts001x.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0041.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0041.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0042.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0042.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0043.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0043.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0044.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0044.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts004f.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts004f.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts011f_plug.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts011f_plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts011f_switch.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts011f_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0121_plug.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_switch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,213 @@
-"""Tuya TS0121 plug."""
+"""Xiaomi mija button device."""
+import asyncio
+import logging
+
 from zigpy.profiles import zha
-from zigpy.quirks import CustomDevice
-from zigpy.zcl.clusters.general import Basic, Groups, Identify, OnOff, Ota, Scenes, Time
-from zigpy.zcl.clusters.homeautomation import ElectricalMeasurement
-from zigpy.zcl.clusters.smartenergy import Metering
+from zigpy.zcl.clusters.general import (
+    Basic,
+    Groups,
+    Identify,
+    LevelControl,
+    OnOff,
+    Ota,
+    Scenes,
+)
 
+from zhaquirks import CustomCluster
 from zhaquirks.const import (
+    ARGS,
+    BUTTON,
+    CLICK_TYPE,
+    COMMAND,
+    COMMAND_CLICK,
+    COMMAND_DOUBLE,
+    COMMAND_FURIOUS,
+    COMMAND_HOLD,
+    COMMAND_QUAD,
+    COMMAND_RELEASE,
+    COMMAND_SINGLE,
+    COMMAND_TRIPLE,
     DEVICE_TYPE,
+    DOUBLE_PRESS,
     ENDPOINTS,
     INPUT_CLUSTERS,
-    MODEL,
+    LONG_PRESS,
+    LONG_RELEASE,
+    MODELS_INFO,
+    NODE_DESCRIPTOR,
     OUTPUT_CLUSTERS,
     PROFILE_ID,
+    QUADRUPLE_PRESS,
+    QUINTUPLE_PRESS,
+    SHORT_PRESS,
+    SKIP_CONFIGURATION,
+    TRIPLE_PRESS,
+    UNKNOWN,
+    ZHA_SEND_EVENT,
 )
-from zhaquirks.tuya import (
-    TuyaNewManufCluster,
-    TuyaZBE000Cluster,
-    TuyaZBElectricalMeasurement,
-    TuyaZBExternalSwitchTypeCluster,
-    TuyaZBMeteringCluster,
-    TuyaZBOnOffAttributeCluster,
+from zhaquirks.xiaomi import (
+    LUMI,
+    XIAOMI_NODE_DESC,
+    BasicCluster,
+    XiaomiPowerConfiguration,
+    XiaomiQuickInitDevice,
 )
 
+XIAOMI_CLUSTER_ID = 0xFFFF
 
-class Plug(CustomDevice):
-    """Tuya TS0121 plug with restore tuya power state support."""
+_LOGGER = logging.getLogger(__name__)
 
-    signature = {
-        MODEL: "TS0121",
-        ENDPOINTS: {
-            # <SimpleDescriptor endpoint=1 profile=260 device_type=81
-            # device_version=1
-            # input_clusters=[0, 4, 5, 6, 9, 1794, 2820]
-            # output_clusters=[10, 25]>
-            1: {
-                PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.SMART_PLUG,
-                INPUT_CLUSTERS: [
-                    Basic.cluster_id,
-                    Groups.cluster_id,
-                    Scenes.cluster_id,
-                    OnOff.cluster_id,
-                    Metering.cluster_id,
-                    ElectricalMeasurement.cluster_id,
-                ],
-                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
-            },
-        },
-    }
-    replacement = {
-        ENDPOINTS: {
-            1: {
-                PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.SMART_PLUG,
-                INPUT_CLUSTERS: [
-                    Basic.cluster_id,
-                    Groups.cluster_id,
-                    Scenes.cluster_id,
-                    TuyaZBOnOffAttributeCluster,
-                    TuyaZBMeteringCluster,
-                    TuyaZBElectricalMeasurement,
-                ],
-                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
-            },
-        },
-    }
+CLICK_TYPE_MAP = {
+    2: COMMAND_DOUBLE,
+    3: COMMAND_TRIPLE,
+    4: COMMAND_QUAD,
+    128: COMMAND_FURIOUS,
+}
+
+
+class MijaButton(XiaomiQuickInitDevice):
+    """Mija button device."""
+
+    def __init__(self, *args, **kwargs):
+        """Init."""
+        self.battery_size = 10
+        super().__init__(*args, **kwargs)
+
+    class MijaOnOff(CustomCluster, OnOff):
+        """Mija on off cluster."""
+
+        cluster_id = OnOff.cluster_id
+        hold_duration: float = 1.0
+
+        def __init__(self, *args, **kwargs):
+            """Init."""
+            self._current_state = {}
+            self._loop = asyncio.get_running_loop()
+            self._timer_handle = None
+            super().__init__(*args, **kwargs)
+
+        def _update_attribute(self, attrid, value):
+            click_type = False
+
+            # Handle Mija OnOff
+            if attrid == 0:
+                value = not value
+
+                if value:
+                    if self._timer_handle:
+                        self._timer_handle.cancel()
+                    self._timer_handle = self._loop.call_later(
+                        self.hold_duration, self._hold_timeout
+                    )
+                else:
+                    if self._timer_handle:
+                        self._timer_handle.cancel()
+                        self._timer_handle = None
+                        click_type = COMMAND_SINGLE
+                    else:
+                        self.listener_event(ZHA_SEND_EVENT, COMMAND_RELEASE, [])
+
+            # Handle Multi Clicks
+            elif attrid == 32768:
+                click_type = CLICK_TYPE_MAP.get(value, UNKNOWN)
+
+            if click_type:
+                self.listener_event(
+                    ZHA_SEND_EVENT, COMMAND_CLICK, {CLICK_TYPE: click_type}
+                )
+
+            super()._update_attribute(attrid, value)
 
+        def _hold_timeout(self):
+            """Handle hold timeout."""
 
-class TS0121B(CustomDevice):
-    """Tuya TS0121 plug with restore tuya power state support and ZGP endpoint."""
+            self._timer_handle = None
+            self.listener_event(ZHA_SEND_EVENT, COMMAND_HOLD, [])
 
     signature = {
-        MODEL: "TS0121",
+        # Endpoints:
+        #   1: profile=0x104, device_type=DeviceType.DIMMER_SWITCH
+        #     Input Clusters:
+        #       Basic (0)
+        #       Identify (3)
+        #       Ota (25)
+        #       Manufacturer Specific (65535)
+        #     Output Clusters:
+        #       Basic (0)
+        #       Identify (3)
+        #       Groups (4)
+        #       Scenes (5)
+        #       On/Off (6)
+        #       Level control (8)
+        #       Ota (25)
+        MODELS_INFO: [(LUMI, "lumi.sensor_switch")],
+        NODE_DESCRIPTOR: XIAOMI_NODE_DESC,
         ENDPOINTS: {
             1: {
                 PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
+                DEVICE_TYPE: zha.DeviceType.DIMMER_SWITCH,
                 INPUT_CLUSTERS: [
                     Basic.cluster_id,
                     Identify.cluster_id,
-                    Groups.cluster_id,
-                    Scenes.cluster_id,
-                    OnOff.cluster_id,
-                    Metering.cluster_id,
-                    ElectricalMeasurement.cluster_id,
-                    TuyaZBE000Cluster.cluster_id,
-                    TuyaZBExternalSwitchTypeCluster.cluster_id,
+                    Ota.cluster_id,
+                    XIAOMI_CLUSTER_ID,
                 ],
-                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
-            },
-            242: {
-                PROFILE_ID: 0xA1E0,
-                DEVICE_TYPE: 0x0061,
-                INPUT_CLUSTERS: [],
-                OUTPUT_CLUSTERS: [0x0021],
-            },
-        },
-    }
-    replacement = {
-        ENDPOINTS: {
-            1: {
-                PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.ON_OFF_PLUG_IN_UNIT,
-                INPUT_CLUSTERS: [
+                OUTPUT_CLUSTERS: [
                     Basic.cluster_id,
                     Identify.cluster_id,
                     Groups.cluster_id,
                     Scenes.cluster_id,
-                    TuyaZBOnOffAttributeCluster,
-                    TuyaZBMeteringCluster,
-                    TuyaZBElectricalMeasurement,
-                    TuyaZBE000Cluster,
-                    TuyaZBExternalSwitchTypeCluster,
+                    OnOff.cluster_id,
+                    LevelControl.cluster_id,
+                    Ota.cluster_id,
                 ],
-                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
-            },
-            242: {
-                PROFILE_ID: 0xA1E0,
-                DEVICE_TYPE: 0x0061,
-                INPUT_CLUSTERS: [],
-                OUTPUT_CLUSTERS: [0x0021],
-            },
+            }
         },
     }
 
-
-class TS0121_Var03(CustomDevice):
-    """Tuya TS0121 plug DeviceType.MAIN_POWER_OUTLET."""
-
-    signature = {
-        MODEL: "TS0121",
+    replacement = {
+        SKIP_CONFIGURATION: True,
         ENDPOINTS: {
             1: {
-                # "profile_id": 260,
-                # "device_type": "0x0009",
-                # "in_clusters": ["0x0000","0x0003","0x0004","0x0005","0x0006","0x0702","0x0b04","0xef00"],
-                # "out_clusters": ["0x000a","0x0019"]
-                PROFILE_ID: zha.PROFILE_ID,
-                DEVICE_TYPE: zha.DeviceType.MAIN_POWER_OUTLET,
+                DEVICE_TYPE: zha.DeviceType.REMOTE_CONTROL,
                 INPUT_CLUSTERS: [
-                    Basic.cluster_id,
                     Identify.cluster_id,
-                    Groups.cluster_id,
+                    BasicCluster,
+                    XiaomiPowerConfiguration,
+                ],
+                OUTPUT_CLUSTERS: [
+                    BasicCluster,
                     Scenes.cluster_id,
-                    OnOff.cluster_id,
-                    Metering.cluster_id,
-                    ElectricalMeasurement.cluster_id,
-                    TuyaNewManufCluster.cluster_id,
+                    Groups.cluster_id,
+                    MijaOnOff,
+                    LevelControl.cluster_id,
+                    Ota.cluster_id,
                 ],
-                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
-            },
-            242: {
-                # "profile_id": 41440,
-                # "device_type": "0x0061",
-                # "in_clusters": [],
-                # "out_clusters": ["0x0021"]
-                PROFILE_ID: 0xA1E0,
-                DEVICE_TYPE: 0x0061,
-                INPUT_CLUSTERS: [],
-                OUTPUT_CLUSTERS: [0x0021],
-            },
+            }
         },
     }
-    replacement = {
-        ENDPOINTS: {
-            1: {
-                INPUT_CLUSTERS: [
-                    Basic.cluster_id,
-                    Identify.cluster_id,
-                    Groups.cluster_id,
-                    Scenes.cluster_id,
-                    TuyaZBOnOffAttributeCluster,
-                    TuyaZBMeteringCluster,
-                    TuyaZBElectricalMeasurement,
-                    TuyaNewManufCluster,
-                ],
-                OUTPUT_CLUSTERS: [Time.cluster_id, Ota.cluster_id],
-            },
-            242: {
-                PROFILE_ID: 0xA1E0,
-                DEVICE_TYPE: 0x0061,
-                INPUT_CLUSTERS: [],
-                OUTPUT_CLUSTERS: [0x0021],
-            },
+
+    device_automation_triggers = {
+        (SHORT_PRESS, SHORT_PRESS): {
+            COMMAND: COMMAND_CLICK,
+            ARGS: {CLICK_TYPE: COMMAND_SINGLE},
+        },
+        (LONG_PRESS, BUTTON): {COMMAND: COMMAND_HOLD},
+        (LONG_RELEASE, BUTTON): {COMMAND: COMMAND_RELEASE},
+        (DOUBLE_PRESS, DOUBLE_PRESS): {
+            COMMAND: COMMAND_CLICK,
+            ARGS: {CLICK_TYPE: COMMAND_DOUBLE},
+        },
+        (TRIPLE_PRESS, TRIPLE_PRESS): {
+            COMMAND: COMMAND_CLICK,
+            ARGS: {CLICK_TYPE: COMMAND_TRIPLE},
+        },
+        (QUADRUPLE_PRESS, QUADRUPLE_PRESS): {
+            COMMAND: COMMAND_CLICK,
+            ARGS: {CLICK_TYPE: COMMAND_QUAD},
+        },
+        (QUINTUPLE_PRESS, QUINTUPLE_PRESS): {
+            COMMAND: COMMAND_CLICK,
+            ARGS: {CLICK_TYPE: COMMAND_FURIOUS},
         },
     }
```

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0201.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0201.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0210.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0210.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0211.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0211.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0501_fan_switch.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0501_fan_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0501b.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0501b.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0501bs.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0501bs.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_co.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_co.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_cover.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_cover.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_dimmer.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_dimmer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,14 @@
     TuyaOnOffNM,
 )
 
 
 class TuyaInWallLevelControlNM(NoManufacturerCluster, TuyaInWallLevelControl):
     """Tuya Level cluster for inwall dimmable device with NoManufacturerID."""
 
-    pass
-
 
 # --- DEVICE SUMMARY ---
 # TuyaSingleSwitchDimmer: 0x00, 0x04, 0x05, 0xEF00; 0x000A, 0x0019
 # TuyaDoubleSwitchDimmer: 0x00, 0x04, 0x05, 0xEF00; 0x000A, 0x0019
 # - Dimmer with Green Power Proxy: Endpoint=242 profile=41440 device_type=0x0061, output_clusters: 0x0021 -
 # TuyaSingleSwitchDimmerGP: 0x00, 0x04, 0x05, 0xEF00; 0x000A, 0x0019
 # TuyaDoubleSwitchDimmerGP: 0x00, 0x04, 0x05, 0xEF00; 0x000A, 0x0019
```

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_din_power.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_din_power.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_electric_heating.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_electric_heating.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_garage.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_garage.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_gas.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_gas.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_haozee.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_haozee.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_illuminance.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_illuminance.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_motion.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_rcbo.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_rcbo.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_sensor.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_siren.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_siren.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_smoke.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_switch.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_switch.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_trv.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,14 @@
                 MOES_MODE_ATTR: self._attr_cache.get(
                     self.attributes_by_name["operation_preset"].id, 2
                 )
             }
         if attribute in self.WORKDAY_SCHEDULE_ATTRS:
             data = data144()
             for num, (attr, default) in enumerate(self.WORKDAY_SCHEDULE_ATTRS.items()):
-
                 if num % 3 == 0:
                     if attr == attribute:
                         val = round(value / 100)
                     else:
                         val = round(
                             self._attr_cache.get(
                                 self.attributes_by_name[attr].id, default
@@ -535,15 +534,14 @@
                         )
 
                 data.append(val)
             return {MOES_SCHEDULE_WORKDAY_ATTR: data}
         if attribute in self.WEEKEND_SCHEDULE_ATTRS:
             data = data144()
             for num, (attr, default) in enumerate(self.WEEKEND_SCHEDULE_ATTRS.items()):
-
                 if num % 3 == 0:
                     if attr == attribute:
                         val = round(value / 100)
                     else:
                         val = round(
                             self._attr_cache.get(
                                 self.attributes_by_name[attr].id, default
@@ -870,15 +868,14 @@
         manufacturer: Optional[Union[int, t.uint16_t]] = None,
         expect_reply: bool = True,
         tsn: Optional[Union[int, t.uint8_t]] = None,
     ):
         """Override the default Cluster command."""
 
         if command_id in (0x0000, 0x0001, 0x0002):
-
             if command_id == 0x0000:
                 value = False
             elif command_id == 0x0001:
                 value = True
             else:
                 attrid = self.attributes_by_name["on_off"].id
                 success, _ = await self.read_attributes(
@@ -1253,15 +1250,14 @@
         manufacturer: Optional[Union[int, t.uint16_t]] = None,
         expect_reply: bool = True,
         tsn: Optional[Union[int, t.uint8_t]] = None,
     ):
         """Override the default Cluster command."""
 
         if command_id in (0x0000, 0x0001, 0x0002):
-
             if command_id == 0x0000:
                 value = False
             elif command_id == 0x0001:
                 value = True
             else:
                 attrid = self.attributes_by_name["on_off"].id
                 success, _ = await self.read_attributes(
```

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_trv_sas.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_trv_sas.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts0601_valve.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts0601_valve.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,16 +184,15 @@
         6: "_dp_2_attr_update",
         11: "_dp_2_attr_update",
         108: "_dp_2_attr_update",
         109: "_dp_2_attr_update",
     }
 
     async def bind(self):
-        """
-        Bind cluster.
+        """Bind cluster.
 
         When adding this device tuya gateway issues factory reset,
         we just need to reset the frost lock, because its state is unknown to us.
         """
         result = await super().bind()
         await self.write_attributes({self.attributes_by_name["frost_lock_reset"].id: 0})
         return result
```

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts110e.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts110e.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/tuya/ts130f.py` & `zha-quirks-0.0.97/zhaquirks/tuya/ts130f.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/universalelectronics/contact_sensor.py` & `zha-quirks-0.0.97/zhaquirks/universalelectronics/contact_sensor.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/visonic/mct340e.py` & `zha-quirks-0.0.97/zhaquirks/visonic/mct340e.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/waxman/leaksmart.py` & `zha-quirks-0.0.97/zhaquirks/waxman/leaksmart.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xbee/__init__.py` & `zha-quirks-0.0.97/zhaquirks/xbee/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,17 +443,15 @@
             (fut,) = self._awaiting.pop(args.frame_id)
             try:
                 status = ATCommandResult(args.status)
             except ValueError:
                 status = ATCommandResult.ERROR
 
             if status:
-                fut.set_exception(
-                    RuntimeError("AT Command response: {}".format(status.name))
-                )
+                fut.set_exception(RuntimeError(f"AT Command response: {status.name}"))
                 return
 
             response_type = AT_COMMANDS[args.cmd.decode("ascii")]
             if response_type is None or len(args.value) == 0:
                 fut.set_result(None)
                 return
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xbee/types.py` & `zha-quirks-0.0.97/zhaquirks/xbee/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Types used to serialize and deserialize XBee commands."""
+from __future__ import annotations
 
 
 class Bytes(bytes):
     """Bytes serializable class."""
 
     def serialize(self):
         """Serialize Bytes."""
@@ -67,15 +68,15 @@
         digital_pins = list(reversed(digital_pins))
         analog_pins = [
             (int.from_bytes(analog_mask, byteorder="big") >> bit) & 1
             for bit in range(8 - 1, -1, -1)
         ]
         analog_pins = list(reversed(analog_pins))
         if 1 in digital_pins:
-            digital_samples = [
+            digital_samples: list[int | None] = [
                 (int.from_bytes(digital_sample, byteorder="big") >> bit) & 1
                 for bit in range(num_bits - 1, -1, -1)
             ]
             digital_samples = list(reversed(digital_samples))
             sample_index = 6
         else:
             # skip digital samples block
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xbee/xbee3_io.py` & `zha-quirks-0.0.97/zhaquirks/xbee/xbee3_io.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xbee/xbee_io.py` & `zha-quirks-0.0.97/zhaquirks/xbee/xbee_io.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/__init__.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/__init__.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/ctrl_ln.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_ln.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/ctrl_neutral.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/ctrl_neutral.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/cube.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,14 @@
             super()._update_attribute(attrid, value)
             if attrid == STATUS_TYPE_ATTR:
                 self._current_state[STATUS_TYPE_ATTR] = action = MOVEMENT_TYPE.get(
                     value
                 )
                 event_args = {VALUE: value}
                 if action is not None:
-
                     if action in (SLIDE, KNOCK):
                         event_args[DESCRIPTION] = MOVEMENT_TYPE_DESCRIPTION[value]
                         event_args[ACTIVATED_FACE] = SIDES[value]
 
                     if action == FLIP:
                         if value > 108:
                             event_args[FLIP_DEGREES] = 180
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/cube_aqgl01.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/cube_aqgl01.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,14 @@
 
     def _update_attribute(self, attrid, value):
         super()._update_attribute(attrid, value)
         if attrid == STATUS_TYPE_ATTR:
             self._current_state[STATUS_TYPE_ATTR] = action = MOVEMENT_TYPE.get(value)
             event_args = {VALUE: value}
             if action is not None:
-
                 if action in (SLIDE, KNOCK):
                     event_args[DESCRIPTION] = MOVEMENT_TYPE_DESCRIPTION[value]
                     event_args[ACTIVATED_FACE] = SIDES[value]
 
                 if action == FLIP:
                     if value > 108:
                         event_args[FLIP_DEGREES] = 180
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/feeder_acn001.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/feeder_acn001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/illumination.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/illumination.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/light_aqcn2.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/light_aqcn2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/magnet_acn001.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_acn001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/magnet_aq2.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/magnet_aq2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_ac01.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_ac02.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_ac02.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         super().__init__(*args, **kwargs)
         if self.ATTR_ID not in self._attr_cache:
             # put a default value so the sensor is created
             self._update_attribute(self.ATTR_ID, 0)
 
     def illuminance_reported(self, value):
         """Illuminance reported."""
-        if 0 > value or value > 0xFFDC:
+        if value < 0 or value > 0xFFDC:
             _LOGGER.debug(
                 "Received invalid illuminance value: %s - setting illuminance to 0",
                 value,
             )
             value = 0
         super().illuminance_reported(value)
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_agl02.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl02.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_agl04.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_agl04.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_aq2.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/motion_aq2b.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/motion_aq2b.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/opple_remote.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             self._current_state = PRESS_TYPES.get(value)
             event_args = {
                 BUTTON: self.endpoint.endpoint_id,
                 PRESS_TYPE: self._current_state,
                 ATTR_ID: attrid,
                 VALUE: value,
             }
-            action = "{}_{}".format(self.endpoint.endpoint_id, self._current_state)
+            action = f"{self.endpoint.endpoint_id}_{self._current_state}"
             self.listener_event(ZHA_SEND_EVENT, action, event_args)
             # show something in the sensor in HA
             super()._update_attribute(0, action)
 
 
 class OppleCluster(CustomCluster):
     """Opple cluster."""
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/opple_switch.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/opple_switch.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             self._current_state = PRESS_TYPES.get(value)
             event_args = {
                 BUTTON: self.endpoint.endpoint_id,
                 PRESS_TYPE: self._current_state,
                 ATTR_ID: attrid,
                 VALUE: value,
             }
-            action = "{}_{}".format(self.endpoint.endpoint_id, self._current_state)
+            action = f"{self.endpoint.endpoint_id}_{self._current_state}"
             self.listener_event(ZHA_SEND_EVENT, action, event_args)
             # show something in the sensor in HA
             super()._update_attribute(0, action)
 
 
 class XiaomiOpple2ButtonSwitchBase(XiaomiCustomDevice):
     """Xiaomi Opple 2 Button Switch."""
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/plug.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/plug_eu.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_eu.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,15 @@
 
 XIAOMI_PROFILE_ID = 0xA1E0
 XIAOMI_DEVICE_TYPE = 0x61
 OPPLE_MFG_CODE = 0x115F
 
 
 async def remove_from_ep(dev: zigpy.device.Device) -> None:
-    """
-    Remove devices that are in group 0 by default, so IKEA devices don't control them.
+    """Remove devices that are in group 0 by default, so IKEA devices don't control them.
 
     This is only needed for newer firmware versions. Only a downgrade will fully fix this but this should improve it.
     See https://github.com/zigpy/zha-device-handlers/pull/1656#issuecomment-1244750465 for details.
     """
 
     endpoint = dev.endpoints.get(1)
     if endpoint is not None:
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/plug_maus01.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/plug_maus01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/relay_c2acn01.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/relay_c2acn01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_b186acn01.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b186acn01.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_b286acn01.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_b286acn01.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 button = ENDPOINT_MAP.get(self.endpoint.endpoint_id)
                 event_args = {
                     BUTTON: button,
                     PRESS_TYPE: self._current_state,
                     ATTR_ID: attrid,
                     VALUE: value,
                 }
-                action = "{}_{}".format(button, self._current_state)
+                action = f"{button}_{self._current_state}"
                 self.listener_event(ZHA_SEND_EVENT, action, event_args)
                 # show something in the sensor in HA
                 super()._update_attribute(0, action)
 
     signature = {
         # <SimpleDescriptor endpoint=1 profile=260 device_type=24321
         # device_version=1
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_e1.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_e1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/remote_h1.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/remote_h1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/roller_curtain_e1.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/roller_curtain_e1.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
         self._update_attribute(0x0041, float(0x064))  # max_present_value
         self._update_attribute(0x0045, 0.0)  # min_present_value
         self._update_attribute(0x0051, 0)  # out_of_service
         self._update_attribute(0x006A, 1.0)  # resolution
         self._update_attribute(0x006F, 0x00)  # status_flags
 
     def _update_attribute(self, attrid: int, value: Any) -> None:
-
         super()._update_attribute(attrid, value)
 
         if attrid == PRESENT_VALUE:
             self.endpoint.window_covering._update_attribute(
                 CURRENT_POSITION_LIFT_PERCENTAGE, (100 - value)
             )
```

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_ht_agl02.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/sensor_switch_aq3.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/smoke.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/switch_aq2.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/switch_aq2.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/thermostat_agl001.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/thermostat_agl001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/tvoc.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/tvoc.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/vibration_aq1.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/vibration_aq1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/water_acn001.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/water_acn001.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/weather.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/weather.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/aqara/wleak_aq1.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/aqara/wleak_aq1.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/mija/motion.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/motion.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/mija/sensor_ht.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_ht.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/mija/sensor_magnet.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/sensor_magnet.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/xiaomi/mija/smoke.py` & `zha-quirks-0.0.97/zhaquirks/xiaomi/mija/smoke.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/yale/realliving.py` & `zha-quirks-0.0.97/zhaquirks/yale/realliving.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/zen/thermostat.py` & `zha-quirks-0.0.97/zhaquirks/zen/thermostat.py`

 * *Files identical despite different names*

### Comparing `zha-quirks-0.0.96/zhaquirks/zhongxing/motion.py` & `zha-quirks-0.0.97/zhaquirks/zhongxing/motion.py`

 * *Files identical despite different names*

