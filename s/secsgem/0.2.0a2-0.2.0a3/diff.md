# Comparing `tmp/secsgem-0.2.0a2.tar.gz` & `tmp/secsgem-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secsgem-0.2.0a2.tar", max compression
+gzip compressed data, was "secsgem-0.2.0a3.tar", max compression
```

## Comparing `secsgem-0.2.0a2.tar` & `secsgem-0.2.0a3.tar`

### file list

```diff
@@ -1,280 +1,329 @@
--rw-r--r--   0        0        0    26444 2023-04-05 08:11:04.401621 secsgem-0.2.0a2/LICENSE
--rw-r--r--   0        0        0     2164 2023-04-05 08:11:04.401621 secsgem-0.2.0a2/README.md
--rw-r--r--   0        0        0     1328 2023-04-05 08:11:04.401621 secsgem-0.2.0a2/pyproject.toml
--rw-r--r--   0        0        0      756 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/common/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/common/callbacks.py
--rw-r--r--   0        0        0     1591 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/common/codec_jis_x_0201.py
--rw-r--r--   0        0        0     5412 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/common/events.py
--rw-r--r--   0        0        0    13116 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/common/fysom.py
--rw-r--r--   0        0        0     2768 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/common/helpers.py
--rw-r--r--   0        0        0     2118 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/__init__.py
--rw-r--r--   0        0        0     1910 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/alarm.py
--rw-r--r--   0        0        0     1978 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/collection_event.py
--rw-r--r--   0        0        0     1600 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/collection_event_link.py
--rw-r--r--   0        0        0     1573 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/collection_event_report.py
--rw-r--r--   0        0        0     2200 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/data_value.py
--rw-r--r--   0        0        0     2839 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/equipment_constant.py
--rw-r--r--   0        0        0    43608 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/equipmenthandler.py
--rw-r--r--   0        0        0    13109 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/handler.py
--rw-r--r--   0        0        0     9742 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/hosthandler.py
--rw-r--r--   0        0        0     2052 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/remote_command.py
--rw-r--r--   0        0        0     2356 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/gem/status_variable.py
--rw-r--r--   0        0        0     1718 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/__init__.py
--rw-r--r--   0        0        0     5571 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/active_connection.py
--rw-r--r--   0        0        0    10898 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/connection.py
--rw-r--r--   0        0        0     6111 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/connectionmanager.py
--rw-r--r--   0        0        0     3377 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/connectionstatemachine.py
--rw-r--r--   0        0        0     1583 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/deselect_req_header.py
--rw-r--r--   0        0        0     1586 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/deselect_rsp_header.py
--rw-r--r--   0        0        0    21904 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/handler.py
--rw-r--r--   0        0        0     2870 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/header.py
--rw-r--r--   0        0        0     1583 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/linktest_req_header.py
--rw-r--r--   0        0        0     1587 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/linktest_rsp_header.py
--rw-r--r--   0        0        0     2869 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/multi_passive_connection.py
--rw-r--r--   0        0        0     6666 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/multi_passive_server.py
--rw-r--r--   0        0        0     4093 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/packet.py
--rw-r--r--   0        0        0     5113 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/passive_connection.py
--rw-r--r--   0        0        0     1749 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/reject_req_header.py
--rw-r--r--   0        0        0     1570 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/select_req_header.py
--rw-r--r--   0        0        0     1573 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/select_rsp_header.py
--rw-r--r--   0        0        0     1591 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/separate_req_header.py
--rw-r--r--   0        0        0     2076 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/hsms/stream_function_header.py
--rw-r--r--   0        0        0     1001 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/__init__.py
--rw-r--r--   0        0        0     2365 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/acka.py
--rw-r--r--   0        0        0     2574 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ackc10.py
--rw-r--r--   0        0        0     1828 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ackc5.py
--rw-r--r--   0        0        0     2026 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ackc6.py
--rw-r--r--   0        0        0     3850 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ackc7.py
--rw-r--r--   0        0        0     4220 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/alcd.py
--rw-r--r--   0        0        0     2058 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/aled.py
--rw-r--r--   0        0        0     1797 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/alid.py
--rw-r--r--   0        0        0     1143 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/altx.py
--rw-r--r--   0        0        0     3419 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/attrdata.py
--rw-r--r--   0        0        0     2809 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/attrid.py
--rw-r--r--   0        0        0     3265 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/attrreln.py
--rw-r--r--   0        0        0     2422 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/base.py
--rw-r--r--   0        0        0     1244 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/bcequ.py
--rw-r--r--   0        0        0     1496 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/binlt.py
--rw-r--r--   0        0        0     1405 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ceed.py
--rw-r--r--   0        0        0     2683 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ceid.py
--rw-r--r--   0        0        0     1396 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/colct.py
--rw-r--r--   0        0        0     1982 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/commack.py
--rw-r--r--   0        0        0     2370 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/cpack.py
--rw-r--r--   0        0        0     2164 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/cpname.py
--rw-r--r--   0        0        0     2264 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/cpval.py
--rw-r--r--   0        0        0     4525 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/dataid.py
--rw-r--r--   0        0        0     2426 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/datalength.py
--rw-r--r--   0        0        0     1047 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/datlc.py
--rw-r--r--   0        0        0     2884 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/drack.py
--rw-r--r--   0        0        0     1817 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/dsid.py
--rw-r--r--   0        0        0     1138 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/dutms.py
--rw-r--r--   0        0        0     1761 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/dvname.py
--rw-r--r--   0        0        0     2210 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/dvval.py
--rw-r--r--   0        0        0     2606 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/eac.py
--rw-r--r--   0        0        0     2019 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ecdef.py
--rw-r--r--   0        0        0     1892 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ecid.py
--rw-r--r--   0        0        0     2019 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ecmax.py
--rw-r--r--   0        0        0     2019 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ecmin.py
--rw-r--r--   0        0        0     1077 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ecname.py
--rw-r--r--   0        0        0     2096 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ecv.py
--rw-r--r--   0        0        0     1785 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/edid.py
--rw-r--r--   0        0        0     2085 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/erack.py
--rw-r--r--   0        0        0     4961 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/errcode.py
--rw-r--r--   0        0        0     4410 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/errtext.py
--rw-r--r--   0        0        0     1483 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/exid.py
--rw-r--r--   0        0        0     1146 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/exmessage.py
--rw-r--r--   0        0        0     1170 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/exrecvra.py
--rw-r--r--   0        0        0     1332 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/extype.py
--rw-r--r--   0        0        0     1217 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/ffrot.py
--rw-r--r--   0        0        0     1283 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/fnloc.py
--rw-r--r--   0        0        0     2183 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/grant5.py
--rw-r--r--   0        0        0     3186 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/grnt1.py
--rw-r--r--   0        0        0     3510 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/hcack.py
--rw-r--r--   0        0        0     2988 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/idtyp.py
--rw-r--r--   0        0        0     1759 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/length.py
--rw-r--r--   0        0        0     3087 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/lrack.py
--rw-r--r--   0        0        0     2136 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/maper.py
--rw-r--r--   0        0        0     2215 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/mapft.py
--rw-r--r--   0        0        0     2517 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/mdack.py
--rw-r--r--   0        0        0     1616 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/mdln.py
--rw-r--r--   0        0        0     1082 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/mexp.py
--rw-r--r--   0        0        0     1367 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/mhead.py
--rw-r--r--   0        0        0     3834 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/mid.py
--rw-r--r--   0        0        0     1387 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/mlcl.py
--rw-r--r--   0        0        0     1310 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/nulbc.py
--rw-r--r--   0        0        0     2575 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/objack.py
--rw-r--r--   0        0        0     1674 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/objid.py
--rw-r--r--   0        0        0     2336 2023-04-05 08:11:04.405621 secsgem-0.2.0a2/secsgem/secs/data_items/objspec.py
--rw-r--r--   0        0        0     1953 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/objtype.py
--rw-r--r--   0        0        0     1751 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/oflack.py
--rw-r--r--   0        0        0     2215 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/onlack.py
--rw-r--r--   0        0        0     2720 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/orloc.py
--rw-r--r--   0        0        0     2045 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/ppbody.py
--rw-r--r--   0        0        0     3000 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/ppgnt.py
--rw-r--r--   0        0        0     2459 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/ppid.py
--rw-r--r--   0        0        0     3543 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/praxi.py
--rw-r--r--   0        0        0     1393 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/prdct.py
--rw-r--r--   0        0        0     1393 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/rcmd.py
--rw-r--r--   0        0        0     1519 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/refp.py
--rw-r--r--   0        0        0     1393 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/rowct.py
--rw-r--r--   0        0        0     1122 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/rpsel.py
--rw-r--r--   0        0        0     2808 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/rptid.py
--rw-r--r--   0        0        0     1411 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/rsinf.py
--rw-r--r--   0        0        0     1685 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/sdack.py
--rw-r--r--   0        0        0     2022 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/sdbin.py
--rw-r--r--   0        0        0     1103 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/shead.py
--rw-r--r--   0        0        0     1622 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/softrev.py
--rw-r--r--   0        0        0     1407 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/strp.py
--rw-r--r--   0        0        0     2145 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/sv.py
--rw-r--r--   0        0        0     1889 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/svid.py
--rw-r--r--   0        0        0     1074 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/svname.py
--rw-r--r--   0        0        0     1973 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/text.py
--rw-r--r--   0        0        0     1285 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/tid.py
--rw-r--r--   0        0        0     1144 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/time.py
--rw-r--r--   0        0        0     1553 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/timestamp.py
--rw-r--r--   0        0        0     1265 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/units.py
--rw-r--r--   0        0        0     2333 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/v.py
--rw-r--r--   0        0        0     2210 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/vid.py
--rw-r--r--   0        0        0     1539 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/xdies.py
--rw-r--r--   0        0        0     1416 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/xypos.py
--rw-r--r--   0        0        0     1539 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/data_items/ydies.py
--rw-r--r--   0        0        0     2659 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/__init__.py
--rw-r--r--   0        0        0     5849 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/base.py
--rw-r--r--   0        0        0     1399 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s00f00.py
--rw-r--r--   0        0        0     1407 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f00.py
--rw-r--r--   0        0        0     1405 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f01.py
--rw-r--r--   0        0        0     1894 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f02.py
--rw-r--r--   0        0        0     1716 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f03.py
--rw-r--r--   0        0        0     1778 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f04.py
--rw-r--r--   0        0        0     1753 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f11.py
--rw-r--r--   0        0        0     2227 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f12.py
--rw-r--r--   0        0        0     1920 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f13.py
--rw-r--r--   0        0        0     2204 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f14.py
--rw-r--r--   0        0        0     1399 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f15.py
--rw-r--r--   0        0        0     1593 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f16.py
--rw-r--r--   0        0        0     1398 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f17.py
--rw-r--r--   0        0        0     1599 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s01f18.py
--rw-r--r--   0        0        0     1407 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f00.py
--rw-r--r--   0        0        0     1750 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f13.py
--rw-r--r--   0        0        0     1722 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f14.py
--rw-r--r--   0        0        0     2121 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f15.py
--rw-r--r--   0        0        0     1593 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f16.py
--rw-r--r--   0        0        0     1406 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f17.py
--rw-r--r--   0        0        0     1583 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f18.py
--rw-r--r--   0        0        0     1759 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f29.py
--rw-r--r--   0        0        0     3099 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f30.py
--rw-r--r--   0        0        0     2578 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f33.py
--rw-r--r--   0        0        0     1606 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f34.py
--rw-r--r--   0        0        0     2395 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f35.py
--rw-r--r--   0        0        0     1608 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f36.py
--rw-r--r--   0        0        0     1902 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f37.py
--rw-r--r--   0        0        0     1615 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f38.py
--rw-r--r--   0        0        0     2433 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f41.py
--rw-r--r--   0        0        0     2587 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s02f42.py
--rw-r--r--   0        0        0     1407 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f00.py
--rw-r--r--   0        0        0     2151 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f01.py
--rw-r--r--   0        0        0     1597 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f02.py
--rw-r--r--   0        0        0     1816 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f03.py
--rw-r--r--   0        0        0     1602 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f04.py
--rw-r--r--   0        0        0     1675 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f05.py
--rw-r--r--   0        0        0     2252 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f06.py
--rw-r--r--   0        0        0     1427 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f07.py
--rw-r--r--   0        0        0     2260 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f08.py
--rw-r--r--   0        0        0     2517 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f09.py
--rw-r--r--   0        0        0     1408 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f10.py
--rw-r--r--   0        0        0     2143 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f11.py
--rw-r--r--   0        0        0     1409 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f12.py
--rw-r--r--   0        0        0     1818 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f13.py
--rw-r--r--   0        0        0     2542 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f14.py
--rw-r--r--   0        0        0     2553 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f15.py
--rw-r--r--   0        0        0     1420 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f16.py
--rw-r--r--   0        0        0     1575 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f17.py
--rw-r--r--   0        0        0     2548 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s05f18.py
--rw-r--r--   0        0        0     1407 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f00.py
--rw-r--r--   0        0        0     1853 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f05.py
--rw-r--r--   0        0        0     1595 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f06.py
--rw-r--r--   0        0        0     1584 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f07.py
--rw-r--r--   0        0        0     3259 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f08.py
--rw-r--r--   0        0        0     2611 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f11.py
--rw-r--r--   0        0        0     1599 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f12.py
--rw-r--r--   0        0        0     1578 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f15.py
--rw-r--r--   0        0        0     2616 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f16.py
--rw-r--r--   0        0        0     1615 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f19.py
--rw-r--r--   0        0        0     1686 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f20.py
--rw-r--r--   0        0        0     1625 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f21.py
--rw-r--r--   0        0        0     2040 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s06f22.py
--rw-r--r--   0        0        0     1407 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f00.py
--rw-r--r--   0        0        0     1813 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f01.py
--rw-r--r--   0        0        0     1592 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f02.py
--rw-r--r--   0        0        0     1860 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f03.py
--rw-r--r--   0        0        0     1606 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f04.py
--rw-r--r--   0        0        0     1571 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f05.py
--rw-r--r--   0        0        0     1860 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f06.py
--rw-r--r--   0        0        0     1694 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f17.py
--rw-r--r--   0        0        0     1617 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f18.py
--rw-r--r--   0        0        0     1443 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f19.py
--rw-r--r--   0        0        0     1704 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s07f20.py
--rw-r--r--   0        0        0     1407 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f00.py
--rw-r--r--   0        0        0     1614 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f01.py
--rw-r--r--   0        0        0     1616 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f03.py
--rw-r--r--   0        0        0     1618 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f05.py
--rw-r--r--   0        0        0     1604 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f07.py
--rw-r--r--   0        0        0     1617 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f09.py
--rw-r--r--   0        0        0     1607 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f11.py
--rw-r--r--   0        0        0     1800 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s09f13.py
--rw-r--r--   0        0        0     1410 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s10f00.py
--rw-r--r--   0        0        0     1783 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s10f01.py
--rw-r--r--   0        0        0     1601 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s10f02.py
--rw-r--r--   0        0        0     1790 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s10f03.py
--rw-r--r--   0        0        0     1622 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s10f04.py
--rw-r--r--   0        0        0     1410 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f00.py
--rw-r--r--   0        0        0     4078 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f01.py
--rw-r--r--   0        0        0     1596 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f02.py
--rw-r--r--   0        0        0     3038 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f03.py
--rw-r--r--   0        0        0     4054 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f04.py
--rw-r--r--   0        0        0     2258 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f05.py
--rw-r--r--   0        0        0     1603 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f06.py
--rw-r--r--   0        0        0     2596 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f07.py
--rw-r--r--   0        0        0     1603 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f08.py
--rw-r--r--   0        0        0     2262 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f09.py
--rw-r--r--   0        0        0     1599 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f10.py
--rw-r--r--   0        0        0     2588 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f11.py
--rw-r--r--   0        0        0     1608 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f12.py
--rw-r--r--   0        0        0     1821 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f13.py
--rw-r--r--   0        0        0     2591 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f14.py
--rw-r--r--   0        0        0     1821 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f15.py
--rw-r--r--   0        0        0     2257 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f16.py
--rw-r--r--   0        0        0     2088 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f17.py
--rw-r--r--   0        0        0     2601 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f18.py
--rw-r--r--   0        0        0     1812 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s12f19.py
--rw-r--r--   0        0        0     1410 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s14f00.py
--rw-r--r--   0        0        0     3335 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s14f01.py
--rw-r--r--   0        0        0     4281 2023-04-05 08:11:04.409621 secsgem-0.2.0a2/secsgem/secs/functions/s14f02.py
--rw-r--r--   0        0        0     2730 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/functions/s14f03.py
--rw-r--r--   0        0        0     4281 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/functions/s14f04.py
--rw-r--r--   0        0        0    14727 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/handler.py
--rw-r--r--   0        0        0     1311 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/__init__.py
--rw-r--r--   0        0        0     6592 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/array.py
--rw-r--r--   0        0        0     3883 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/base.py
--rw-r--r--   0        0        0     7121 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/base_number.py
--rw-r--r--   0        0        0     6513 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/base_text.py
--rw-r--r--   0        0        0     6685 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/binary.py
--rw-r--r--   0        0        0     6681 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/boolean.py
--rw-r--r--   0        0        0     8755 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/dynamic.py
--rw-r--r--   0        0        0     1190 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/f4.py
--rw-r--r--   0        0        0     1192 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/f8.py
--rw-r--r--   0        0        0     2417 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/functions.py
--rw-r--r--   0        0        0     1182 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/i1.py
--rw-r--r--   0        0        0     1186 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/i2.py
--rw-r--r--   0        0        0     1196 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/i4.py
--rw-r--r--   0        0        0     1214 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/i8.py
--rw-r--r--   0        0        0     1261 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/jis8.py
--rw-r--r--   0        0        0     8800 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/list_type.py
--rw-r--r--   0        0        0     1233 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/string.py
--rw-r--r--   0        0        0     1183 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/u1.py
--rw-r--r--   0        0        0     1185 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/u2.py
--rw-r--r--   0        0        0     1190 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/u4.py
--rw-r--r--   0        0        0     1200 2023-04-05 08:11:04.413621 secsgem-0.2.0a2/secsgem/secs/variables/u8.py
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 secsgem-0.2.0a2/PKG-INFO
+-rw-r--r--   0        0        0    26444 2023-04-12 06:57:27.336893 secsgem-0.2.0a3/LICENSE
+-rw-r--r--   0        0        0     2164 2023-04-12 06:57:27.336893 secsgem-0.2.0a3/README.md
+-rw-r--r--   0        0        0     1442 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/pyproject.toml
+-rw-r--r--   0        0        0      756 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/__init__.py
+-rw-r--r--   0        0        0     1123 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/__init__.py
+-rw-r--r--   0        0        0     3636 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/callbacks.py
+-rw-r--r--   0        0        0     1651 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/codec_jis_x_0201.py
+-rw-r--r--   0        0        0     5908 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/events.py
+-rw-r--r--   0        0        0    13116 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/fysom.py
+-rw-r--r--   0        0        0     2867 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/common/helpers.py
+-rw-r--r--   0        0        0     2118 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/__init__.py
+-rw-r--r--   0        0        0     2202 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/alarm.py
+-rw-r--r--   0        0        0     2200 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/collection_event.py
+-rw-r--r--   0        0        0     1823 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/collection_event_link.py
+-rw-r--r--   0        0        0     1764 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/collection_event_report.py
+-rw-r--r--   0        0        0     2450 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/data_value.py
+-rw-r--r--   0        0        0     3232 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/equipment_constant.py
+-rw-r--r--   0        0        0    47111 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/equipmenthandler.py
+-rw-r--r--   0        0        0    13257 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/handler.py
+-rw-r--r--   0        0        0    10249 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/hosthandler.py
+-rw-r--r--   0        0        0     2249 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/remote_command.py
+-rw-r--r--   0        0        0     2356 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/gem/status_variable.py
+-rw-r--r--   0        0        0     1718 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/__init__.py
+-rw-r--r--   0        0        0     5571 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/active_connection.py
+-rw-r--r--   0        0        0    10898 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/connection.py
+-rw-r--r--   0        0        0     6111 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/connectionmanager.py
+-rw-r--r--   0        0        0     3377 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/connectionstatemachine.py
+-rw-r--r--   0        0        0     1583 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/deselect_req_header.py
+-rw-r--r--   0        0        0     1586 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/deselect_rsp_header.py
+-rw-r--r--   0        0        0    21678 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/handler.py
+-rw-r--r--   0        0        0     2870 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/header.py
+-rw-r--r--   0        0        0     1583 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/linktest_req_header.py
+-rw-r--r--   0        0        0     1587 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/linktest_rsp_header.py
+-rw-r--r--   0        0        0     2869 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/multi_passive_connection.py
+-rw-r--r--   0        0        0     6666 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/multi_passive_server.py
+-rw-r--r--   0        0        0     4093 2023-04-12 06:57:27.340893 secsgem-0.2.0a3/secsgem/hsms/packet.py
+-rw-r--r--   0        0        0     5168 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/passive_connection.py
+-rw-r--r--   0        0        0     1749 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/reject_req_header.py
+-rw-r--r--   0        0        0     1570 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/select_req_header.py
+-rw-r--r--   0        0        0     1573 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/select_rsp_header.py
+-rw-r--r--   0        0        0     1591 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/separate_req_header.py
+-rw-r--r--   0        0        0     2076 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/hsms/stream_function_header.py
+-rw-r--r--   0        0        0     1001 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/__init__.py
+-rw-r--r--   0        0        0     5646 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/__init__.py
+-rw-r--r--   0        0        0     1119 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/abs.py
+-rw-r--r--   0        0        0     1434 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/acka.py
+-rw-r--r--   0        0        0     2449 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc10.py
+-rw-r--r--   0        0        0     1792 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc5.py
+-rw-r--r--   0        0        0     1792 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc6.py
+-rw-r--r--   0        0        0     3262 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ackc7.py
+-rw-r--r--   0        0        0     4279 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/alcd.py
+-rw-r--r--   0        0        0     2051 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/aled.py
+-rw-r--r--   0        0        0     1863 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/alid.py
+-rw-r--r--   0        0        0     1218 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/altx.py
+-rw-r--r--   0        0        0     2297 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/attrdata.py
+-rw-r--r--   0        0        0     1621 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/attrid.py
+-rw-r--r--   0        0        0     3261 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/attrreln.py
+-rw-r--r--   0        0        0     2541 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/base.py
+-rw-r--r--   0        0        0     1266 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/bcequ.py
+-rw-r--r--   0        0        0     1518 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/binlt.py
+-rw-r--r--   0        0        0     1332 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ceed.py
+-rw-r--r--   0        0        0     2155 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ceid.py
+-rw-r--r--   0        0        0     1066 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cename.py
+-rw-r--r--   0        0        0     2795 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cepack.py
+-rw-r--r--   0        0        0     2103 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cepval.py
+-rw-r--r--   0        0        0     2481 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cmda.py
+-rw-r--r--   0        0        0     1396 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/colct.py
+-rw-r--r--   0        0        0     1976 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/commack.py
+-rw-r--r--   0        0        0     2430 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cpack.py
+-rw-r--r--   0        0        0     1900 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cpname.py
+-rw-r--r--   0        0        0     1869 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/cpval.py
+-rw-r--r--   0        0        0     2215 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dataid.py
+-rw-r--r--   0        0        0     1634 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/datalength.py
+-rw-r--r--   0        0        0     1043 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/datlc.py
+-rw-r--r--   0        0        0     2878 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/drack.py
+-rw-r--r--   0        0        0     1685 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dsid.py
+-rw-r--r--   0        0        0     1060 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dsper.py
+-rw-r--r--   0        0        0     1128 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dutms.py
+-rw-r--r--   0        0        0     1695 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dvname.py
+-rw-r--r--   0        0        0     2078 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dvval.py
+-rw-r--r--   0        0        0     1069 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/dvvalname.py
+-rw-r--r--   0        0        0     2587 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/eac.py
+-rw-r--r--   0        0        0     2020 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecdef.py
+-rw-r--r--   0        0        0     1893 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecid.py
+-rw-r--r--   0        0        0     2020 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecmax.py
+-rw-r--r--   0        0        0     2020 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecmin.py
+-rw-r--r--   0        0        0     1068 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecname.py
+-rw-r--r--   0        0        0     2152 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ecv.py
+-rw-r--r--   0        0        0     1785 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/edid.py
+-rw-r--r--   0        0        0     2078 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/erack.py
+-rw-r--r--   0        0        0    17058 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/errcode.py
+-rw-r--r--   0        0        0     1381 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/errtext.py
+-rw-r--r--   0        0        0     1490 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/exid.py
+-rw-r--r--   0        0        0     1137 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/exmessage.py
+-rw-r--r--   0        0        0     1177 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/exrecvra.py
+-rw-r--r--   0        0        0     1125 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/extype.py
+-rw-r--r--   0        0        0     1140 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/fcnid.py
+-rw-r--r--   0        0        0     1213 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ffrot.py
+-rw-r--r--   0        0        0     1279 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/fnloc.py
+-rw-r--r--   0        0        0     2177 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/grant6.py
+-rw-r--r--   0        0        0     3179 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/grnt1.py
+-rw-r--r--   0        0        0     3503 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/hcack.py
+-rw-r--r--   0        0        0     2981 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/idtyp.py
+-rw-r--r--   0        0        0     1627 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/length.py
+-rw-r--r--   0        0        0     3868 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitack.py
+-rw-r--r--   0        0        0     1221 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitid.py
+-rw-r--r--   0        0        0     1972 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitmax.py
+-rw-r--r--   0        0        0     1972 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/limitmin.py
+-rw-r--r--   0        0        0     2043 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/lowerdb.py
+-rw-r--r--   0        0        0     3081 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/lrack.py
+-rw-r--r--   0        0        0     2792 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/lvack.py
+-rw-r--r--   0        0        0     2130 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/maper.py
+-rw-r--r--   0        0        0     2208 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mapft.py
+-rw-r--r--   0        0        0     2510 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mdack.py
+-rw-r--r--   0        0        0     1226 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mdln.py
+-rw-r--r--   0        0        0     1088 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mexp.py
+-rw-r--r--   0        0        0     1360 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mhead.py
+-rw-r--r--   0        0        0     2024 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mid.py
+-rw-r--r--   0        0        0     1387 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/mlcl.py
+-rw-r--r--   0        0        0     1332 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/nulbc.py
+-rw-r--r--   0        0        0     1974 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objack.py
+-rw-r--r--   0        0        0     1608 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objid.py
+-rw-r--r--   0        0        0     1204 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objspec.py
+-rw-r--r--   0        0        0     1491 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/objtype.py
+-rw-r--r--   0        0        0     1745 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/oflack.py
+-rw-r--r--   0        0        0     2209 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/onlack.py
+-rw-r--r--   0        0        0     2731 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/orloc.py
+-rw-r--r--   0        0        0     1847 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ppbody.py
+-rw-r--r--   0        0        0     2927 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ppgnt.py
+-rw-r--r--   0        0        0     1574 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/ppid.py
+-rw-r--r--   0        0        0     3536 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/praxi.py
+-rw-r--r--   0        0        0     1393 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/prdct.py
+-rw-r--r--   0        0        0     1394 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rcmd.py
+-rw-r--r--   0        0        0     1388 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/refp.py
+-rw-r--r--   0        0        0     1700 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/repgsz.py
+-rw-r--r--   0        0        0     1393 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rowct.py
+-rw-r--r--   0        0        0     1118 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rpsel.py
+-rw-r--r--   0        0        0     2016 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rptid.py
+-rw-r--r--   0        0        0     2397 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rsda.py
+-rw-r--r--   0        0        0     1991 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rsdc.py
+-rw-r--r--   0        0        0     1426 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rsinf.py
+-rw-r--r--   0        0        0     2122 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/rspack.py
+-rw-r--r--   0        0        0     1678 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/sdack.py
+-rw-r--r--   0        0        0     2016 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/sdbin.py
+-rw-r--r--   0        0        0     1096 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/shead.py
+-rw-r--r--   0        0        0     1607 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/smpln.py
+-rw-r--r--   0        0        0     1008 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/softrev.py
+-rw-r--r--   0        0        0     1053 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/stime.py
+-rw-r--r--   0        0        0     2459 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/strack.py
+-rw-r--r--   0        0        0     1138 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/strid.py
+-rw-r--r--   0        0        0     1423 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/strp.py
+-rw-r--r--   0        0        0     2146 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/sv.py
+-rw-r--r--   0        0        0     1890 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/svid.py
+-rw-r--r--   0        0        0     1065 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/svname.py
+-rw-r--r--   0        0        0     1841 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/text.py
+-rw-r--r--   0        0        0     2947 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/tiaack.py
+-rw-r--r--   0        0        0     1146 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/tid.py
+-rw-r--r--   0        0        0     1085 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/time.py
+-rw-r--r--   0        0        0     1230 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/timestamp.py
+-rw-r--r--   0        0        0     1693 2023-04-12 06:57:27.344893 secsgem-0.2.0a3/secsgem/secs/data_items/totsmp.py
+-rw-r--r--   0        0        0     1756 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/trid.py
+-rw-r--r--   0        0        0     1256 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/units.py
+-rw-r--r--   0        0        0     2043 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/upperdb.py
+-rw-r--r--   0        0        0     2267 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/v.py
+-rw-r--r--   0        0        0     2210 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/vid.py
+-rw-r--r--   0        0        0     2523 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/vlaack.py
+-rw-r--r--   0        0        0     1539 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/xdies.py
+-rw-r--r--   0        0        0     1432 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/xypos.py
+-rw-r--r--   0        0        0     1539 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/data_items/ydies.py
+-rw-r--r--   0        0        0    10811 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/__init__.py
+-rw-r--r--   0        0        0     6099 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/base.py
+-rw-r--r--   0        0        0     1399 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s00f00.py
+-rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f00.py
+-rw-r--r--   0        0        0     1405 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f01.py
+-rw-r--r--   0        0        0     2127 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f02.py
+-rw-r--r--   0        0        0     1716 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f03.py
+-rw-r--r--   0        0        0     1778 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f04.py
+-rw-r--r--   0        0        0     1753 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f11.py
+-rw-r--r--   0        0        0     2297 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f12.py
+-rw-r--r--   0        0        0     2153 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f13.py
+-rw-r--r--   0        0        0     2485 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f14.py
+-rw-r--r--   0        0        0     1399 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f15.py
+-rw-r--r--   0        0        0     1594 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f16.py
+-rw-r--r--   0        0        0     1398 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f17.py
+-rw-r--r--   0        0        0     1600 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f18.py
+-rw-r--r--   0        0        0     1695 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f21.py
+-rw-r--r--   0        0        0     2138 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f22.py
+-rw-r--r--   0        0        0     1701 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f23.py
+-rw-r--r--   0        0        0     2297 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s01f24.py
+-rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f00.py
+-rw-r--r--   0        0        0     1750 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f13.py
+-rw-r--r--   0        0        0     1722 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f14.py
+-rw-r--r--   0        0        0     2152 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f15.py
+-rw-r--r--   0        0        0     1594 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f16.py
+-rw-r--r--   0        0        0     1406 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f17.py
+-rw-r--r--   0        0        0     1576 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f18.py
+-rw-r--r--   0        0        0     1569 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f21.py
+-rw-r--r--   0        0        0     1591 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f22.py
+-rw-r--r--   0        0        0     2665 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f23.py
+-rw-r--r--   0        0        0     1615 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f24.py
+-rw-r--r--   0        0        0     1571 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f25.py
+-rw-r--r--   0        0        0     1568 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f26.py
+-rw-r--r--   0        0        0     1759 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f29.py
+-rw-r--r--   0        0        0     3308 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f30.py
+-rw-r--r--   0        0        0     2662 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f33.py
+-rw-r--r--   0        0        0     1607 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f34.py
+-rw-r--r--   0        0        0     2465 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f35.py
+-rw-r--r--   0        0        0     1609 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f36.py
+-rw-r--r--   0        0        0     1937 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f37.py
+-rw-r--r--   0        0        0     1616 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f38.py
+-rw-r--r--   0        0        0     2496 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f41.py
+-rw-r--r--   0        0        0     2644 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f42.py
+-rw-r--r--   0        0        0     2267 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f43.py
+-rw-r--r--   0        0        0     2963 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f44.py
+-rw-r--r--   0        0        0     3470 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f45.py
+-rw-r--r--   0        0        0     3147 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f46.py
+-rw-r--r--   0        0        0     1697 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f47.py
+-rw-r--r--   0        0        0     3848 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f48.py
+-rw-r--r--   0        0        0     2870 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f49.py
+-rw-r--r--   0        0        0     2655 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s02f50.py
+-rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f00.py
+-rw-r--r--   0        0        0     2139 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f01.py
+-rw-r--r--   0        0        0     1598 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f02.py
+-rw-r--r--   0        0        0     1851 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f03.py
+-rw-r--r--   0        0        0     1603 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f04.py
+-rw-r--r--   0        0        0     1675 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f05.py
+-rw-r--r--   0        0        0     2270 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f06.py
+-rw-r--r--   0        0        0     1411 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f07.py
+-rw-r--r--   0        0        0     2278 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f08.py
+-rw-r--r--   0        0        0     2667 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f09.py
+-rw-r--r--   0        0        0     1408 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f10.py
+-rw-r--r--   0        0        0     2310 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f11.py
+-rw-r--r--   0        0        0     1409 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f12.py
+-rw-r--r--   0        0        0     1853 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f13.py
+-rw-r--r--   0        0        0     2566 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f14.py
+-rw-r--r--   0        0        0     2852 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f15.py
+-rw-r--r--   0        0        0     1420 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f16.py
+-rw-r--r--   0        0        0     1576 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f17.py
+-rw-r--r--   0        0        0     2603 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s05f18.py
+-rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f00.py
+-rw-r--r--   0        0        0     2374 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f01.py
+-rw-r--r--   0        0        0     1596 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f02.py
+-rw-r--r--   0        0        0     1888 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f05.py
+-rw-r--r--   0        0        0     1596 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f06.py
+-rw-r--r--   0        0        0     1580 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f07.py
+-rw-r--r--   0        0        0     3424 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f08.py
+-rw-r--r--   0        0        0     2783 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f11.py
+-rw-r--r--   0        0        0     1600 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f12.py
+-rw-r--r--   0        0        0     1577 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f15.py
+-rw-r--r--   0        0        0     2788 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f16.py
+-rw-r--r--   0        0        0     1614 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f19.py
+-rw-r--r--   0        0        0     1686 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f20.py
+-rw-r--r--   0        0        0     1624 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f21.py
+-rw-r--r--   0        0        0     2075 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f22.py
+-rw-r--r--   0        0        0     1584 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f23.py
+-rw-r--r--   0        0        0     1595 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s06f24.py
+-rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f00.py
+-rw-r--r--   0        0        0     1848 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f01.py
+-rw-r--r--   0        0        0     1593 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f02.py
+-rw-r--r--   0        0        0     1895 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f03.py
+-rw-r--r--   0        0        0     1607 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f04.py
+-rw-r--r--   0        0        0     1572 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f05.py
+-rw-r--r--   0        0        0     1895 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f06.py
+-rw-r--r--   0        0        0     1694 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f17.py
+-rw-r--r--   0        0        0     1618 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f18.py
+-rw-r--r--   0        0        0     1427 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f19.py
+-rw-r--r--   0        0        0     1704 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s07f20.py
+-rw-r--r--   0        0        0     1407 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f00.py
+-rw-r--r--   0        0        0     1615 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f01.py
+-rw-r--r--   0        0        0     1617 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f03.py
+-rw-r--r--   0        0        0     1619 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f05.py
+-rw-r--r--   0        0        0     1605 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f07.py
+-rw-r--r--   0        0        0     1618 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f09.py
+-rw-r--r--   0        0        0     1608 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f11.py
+-rw-r--r--   0        0        0     1835 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s09f13.py
+-rw-r--r--   0        0        0     1410 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f00.py
+-rw-r--r--   0        0        0     1818 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f01.py
+-rw-r--r--   0        0        0     1602 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f02.py
+-rw-r--r--   0        0        0     1825 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f03.py
+-rw-r--r--   0        0        0     1623 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s10f04.py
+-rw-r--r--   0        0        0     1410 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f00.py
+-rw-r--r--   0        0        0     4534 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f01.py
+-rw-r--r--   0        0        0     1597 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f02.py
+-rw-r--r--   0        0        0     3302 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f03.py
+-rw-r--r--   0        0        0     4510 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f04.py
+-rw-r--r--   0        0        0     2281 2023-04-12 06:57:27.348893 secsgem-0.2.0a3/secsgem/secs/functions/s12f05.py
+-rw-r--r--   0        0        0     1604 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f06.py
+-rw-r--r--   0        0        0     2711 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f07.py
+-rw-r--r--   0        0        0     1604 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f08.py
+-rw-r--r--   0        0        0     2285 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f09.py
+-rw-r--r--   0        0        0     1600 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f10.py
+-rw-r--r--   0        0        0     2703 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f11.py
+-rw-r--r--   0        0        0     1609 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f12.py
+-rw-r--r--   0        0        0     1856 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f13.py
+-rw-r--r--   0        0        0     2706 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f14.py
+-rw-r--r--   0        0        0     1856 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f15.py
+-rw-r--r--   0        0        0     2280 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f16.py
+-rw-r--r--   0        0        0     2109 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f17.py
+-rw-r--r--   0        0        0     2696 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f18.py
+-rw-r--r--   0        0        0     1847 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s12f19.py
+-rw-r--r--   0        0        0     1410 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f00.py
+-rw-r--r--   0        0        0     3293 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f01.py
+-rw-r--r--   0        0        0     4411 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f02.py
+-rw-r--r--   0        0        0     2963 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f03.py
+-rw-r--r--   0        0        0     4411 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/functions/s14f04.py
+-rw-r--r--   0        0        0    16343 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/handler.py
+-rw-r--r--   0        0        0     1387 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/__init__.py
+-rw-r--r--   0        0        0     6592 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/array.py
+-rw-r--r--   0        0        0     4112 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/base.py
+-rw-r--r--   0        0        0     7238 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/base_number.py
+-rw-r--r--   0        0        0     6513 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/base_text.py
+-rw-r--r--   0        0        0     6685 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/binary.py
+-rw-r--r--   0        0        0     6681 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/boolean.py
+-rw-r--r--   0        0        0     8973 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/dynamic.py
+-rw-r--r--   0        0        0     1190 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/f4.py
+-rw-r--r--   0        0        0     1192 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/f8.py
+-rw-r--r--   0        0        0     2417 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/functions.py
+-rw-r--r--   0        0        0     1182 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i1.py
+-rw-r--r--   0        0        0     1186 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i2.py
+-rw-r--r--   0        0        0     1196 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i4.py
+-rw-r--r--   0        0        0     1214 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/i8.py
+-rw-r--r--   0        0        0     1261 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/jis8.py
+-rw-r--r--   0        0        0     8800 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/list_type.py
+-rw-r--r--   0        0        0     1233 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/string.py
+-rw-r--r--   0        0        0     1183 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u1.py
+-rw-r--r--   0        0        0     1185 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u2.py
+-rw-r--r--   0        0        0     1190 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u4.py
+-rw-r--r--   0        0        0     1200 2023-04-12 06:57:27.352893 secsgem-0.2.0a3/secsgem/secs/variables/u8.py
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 secsgem-0.2.0a3/PKG-INFO
```

### Comparing `secsgem-0.2.0a2/LICENSE` & `secsgem-0.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/README.md` & `secsgem-0.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/pyproject.toml` & `secsgem-0.2.0a3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secsgem"
-version = "0.2.0-alpha.2"
+version = "0.2.0-alpha.3"
 description = "Python SECS/GEM implementation"
 readme = "README.md"
 
 authors = ["Benjamin Parzella <bparzella@gmail.com>"]
 
 license = "LGPL-2.1-or-later"
 
@@ -32,17 +32,22 @@
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 python-dateutil = "^2.8.1"
 transitions = "^0.9.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
-coverage = "^7.2.2"
+pytest = "^7.3.0"
+coverage = "^7.2.3"
 prospector = "^1.9.0"
+mypy = "^1.2.0"
+Jinja2 = "^3.1.2"
+PyYAML = "^6.0"
+types-PyYAML = "^6.0.12.9"
+types-python-dateutil = "^2.8.19.12"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --doctest-report ndiff"
 testpaths = [
     "tests",
     "secsgem"
 ]
```

### Comparing `secsgem-0.2.0a2/secsgem/__init__.py` & `secsgem-0.2.0a3/secsgem/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/common/__init__.py` & `secsgem-0.2.0a3/secsgem/common/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/common/callbacks.py` & `secsgem-0.2.0a3/secsgem/common/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,39 +10,40 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Contains callback handling routines."""
+import typing
 
 
 class _CallbackCallWrapper:
-    def __init__(self, handler, name):
+    def __init__(self, handler: "CallbackHandler", name: str):
         self.name = name
         self.handler = handler
 
     def __call__(self, *args, **kwargs):
         return self.handler._call(self.name, *args, **kwargs)  # noqa
 
 
 class CallbackHandler:
     """
     Handler for callbacks for HSMS/SECS/GEM events.
 
     This handler manages callbacks for events that can happen on a handler for a connection.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the handler."""
-        self._callbacks = {}
-        self.target = None
+        self._callbacks: typing.Dict[str, typing.Callable] = {}
+        self.target: object = None
         self._object_intitialized = True
 
-    def __setattr__(self, name, value):
+    def __setattr__(self, name: str, value: typing.Callable):
         """
         Set an item as object member.
 
         :param name: Name of the callback
         :param value: Callback
         """
         if '_object_intitialized' not in self.__dict__ or name in self.__dict__:
@@ -51,15 +52,15 @@
 
         if value is None:
             if name in self._callbacks:
                 del self._callbacks[name]
         else:
             self._callbacks[name] = value
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> typing.Callable:
         """
         Get a callable function for an event.
 
         :param name: Name of the event
         :return: Callable representation of the callback
         """
         return _CallbackCallWrapper(self, name)
@@ -76,23 +77,23 @@
             if self._counter < len(self._keys):
                 i = self._counter
                 self._counter += 1
                 return self._keys[i]
 
             raise StopIteration()
 
-    def __iter__(self):
+    def __iter__(self) -> _CallbacksIter:
         """
         Get an iterator for the callbacks.
 
         :return: Callback iterator.
         """
         return self._CallbacksIter(self._callbacks.keys())
 
-    def __contains__(self, callback):
+    def __contains__(self, callback: str) -> bool:
         """
         Check if a callback is present.
 
         :param callback: Name of the event
         :return: True if callback present
         """
         if callback in self._callbacks:
@@ -100,15 +101,15 @@
 
         delegate_handler = getattr(self.target, "_on_" + callback, None)
         if callable(delegate_handler):
             return True
 
         return False
 
-    def _call(self, callback, *args, **kwargs):
+    def _call(self, callback: str, *args, **kwargs) -> typing.Any:
         if callback in self._callbacks:
             return self._callbacks[callback](*args, **kwargs)
 
         delegate_handler = getattr(self.target, "_on_" + callback, None)
         if callable(delegate_handler):
             return delegate_handler(*args, **kwargs)
```

### Comparing `secsgem-0.2.0a2/secsgem/common/codec_jis_x_0201.py` & `secsgem-0.2.0a3/secsgem/common/codec_jis_x_0201.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """JIS X 0201 Codec required for JIS8 encoding of JIS8."""
 
 import codecs
 
-jis8_decoding_map = codecs.make_identity_dict(range(256))
+jis8_decoding_map = codecs.make_identity_dict(range(256))  # type: ignore[attr-defined]
 jis8_decoding_map.update({
     0x005C: 0x00A5,  # Yen Sign
     0x007E: 0x203E,  # Overline
 })
 
 for i in range(0x00A1, 0x00E0):
     jis8_decoding_map[i] = i + 0xFEC0
 
-jis8_encoding_map = codecs.make_encoding_map(jis8_decoding_map)
+jis8_encoding_map = codecs.make_encoding_map(jis8_decoding_map)  # type: ignore[attr-defined]
 
 
 def _jis_x_0201_encode(data, errors='strict'):
     return codecs.charmap_encode(data, errors, jis8_encoding_map)
 
 
 def _jis_x_0201_decode(data, errors='strict'):
```

### Comparing `secsgem-0.2.0a2/secsgem/common/events.py` & `secsgem-0.2.0a3/secsgem/common/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,60 +10,61 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Contains helper functions."""
+import typing
 
 
 class Event:
     """Class to handle the callbacks for a single event."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the event class."""
-        self._callbacks = []
+        self._callbacks: typing.List[typing.Callable[[typing.Dict[str, typing.Any]], None]] = []
 
-    def __iadd__(self, other):
+    def __iadd__(self, other: typing.Callable[[typing.Dict[str, typing.Any]], None]) -> "Event":
         """Add a new callback to event."""
         self._callbacks.append(other)
         return self
 
-    def __isub__(self, other):
+    def __isub__(self, other: typing.Callable[[typing.Dict[str, typing.Any]], None]) -> "Event":
         """Remove a callback from event."""
         self._callbacks.remove(other)
         return self
 
-    def __call__(self, data):
+    def __call__(self, data: typing.Dict[str, typing.Any]):
         """Raise the event and call all callbacks."""
         for callback in self._callbacks:
             callback(data)
 
-    def __len__(self):
+    def __len__(self) -> int:
         """Return the number of callbacks."""
         return len(self._callbacks)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Generate representation for an object."""
         return f"{self.__class__.__name__}: {self._callbacks}"
 
 
 class Targets:
     """Class to handle a list of objects as target for events."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the target class."""
-        self._targets = []
+        self._targets: typing.List[object] = []
 
-    def __iadd__(self, other):
+    def __iadd__(self, other: object) -> "Targets":
         """Add a targets."""
         self._targets.append(other)
         return self
 
-    def __isub__(self, other):
+    def __isub__(self, other: object) -> "Targets":
         """Remove a target."""
         self._targets.remove(other)
         return self
 
     class _TargetsIter:
         def __init__(self, values):
             self._values = values
@@ -78,48 +79,48 @@
             if self._counter < len(self._values):
                 i = self._counter
                 self._counter += 1
                 return self._values[i]
 
             raise StopIteration()
 
-    def __iter__(self):
+    def __iter__(self) -> _TargetsIter:
         """Return the iterator."""
         return self._TargetsIter(self._targets)
 
 
 class EventProducer:
     """Manages the consumers for the events and handles firing events."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize the event producer class."""
         self._targets = Targets()
-        self._events = {}
+        self._events: typing.Dict[str, Event] = {}
 
-    def __getattr__(self, name):
+    def __getattr__(self, name: str) -> Event:
         """Get an event as member of the EventProducer object."""
         if name not in self._events:
             self._events[name] = Event()
 
         return self._events[name]
 
-    def __iadd__(self, other):
+    def __iadd__(self, other) -> "EventProducer":
         """Add a the callbacks and targets of another EventProducer to this one."""
         for event_name in other._events:  # noqa
             if event_name not in self._events:
                 self._events[event_name] = Event()
 
             for callback in other._events[event_name]._callbacks:  # noqa
                 self._events[event_name] += callback
 
         for target in other._targets:  # noqa
             self._targets += target
         return self
 
-    def fire(self, event, data):
+    def fire(self, event: str, data: typing.Dict[str, typing.Any]):
         """
         Fire a event.
 
         calls all the available handlers for a specific event
 
         :param event: name of the event
         :type event: string
@@ -134,15 +135,15 @@
             specific_handler = getattr(target, "_on_event_" + event, None)
             if callable(specific_handler):
                 specific_handler(data)
 
         if event in self._events:
             self._events[event](data)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Generate representation for an object."""
         return f"{self.__class__.__name__}: {self._events}"
 
     class _EventsIter:
         def __init__(self, keys):
             self._keys = list(keys)
             self._counter = 0
@@ -156,20 +157,20 @@
             if self._counter < len(self._keys):
                 i = self._counter
                 self._counter += 1
                 return self._keys[i]
 
             raise StopIteration()
 
-    def __iter__(self):
+    def __iter__(self) -> _EventsIter:
         """Return the iterator."""
         return self._EventsIter([event for event, event_value in self._events.items() if len(event_value) > 0])
 
     @property
-    def targets(self):
+    def targets(self) -> Targets:
         """Targets used as consumer for this producer."""
         return self._targets
 
     @targets.setter
-    def targets(self, value):
+    def targets(self, value: Targets):
         if self._targets != value:
             raise AttributeError("can't set attribute")
```

### Comparing `secsgem-0.2.0a2/secsgem/common/fysom.py` & `secsgem-0.2.0a3/secsgem/common/fysom.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/common/helpers.py` & `secsgem-0.2.0a3/secsgem/common/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Contains helper functions."""
-
 import errno
 import sys
 import types
 
 
-def format_hex(text):
+def format_hex(text: bytes) -> str:
     """
     Return byte arrays (string) formated as hex numbers.
 
     **Example**::
 
         >>> import secsgem.common
         >>>
@@ -37,72 +36,72 @@
     :type text: string
     :returns: Formated text
     :rtype: string
     """
     return ":".join(f"{c:02x}" for c in bytearray(text))
 
 
-def is_windows():
+def is_windows() -> bool:
     """
     Return True if running on windows.
 
     :returns: Is windows system
     :rtype: bool
     """
     if sys.platform == "win32":  # pragma: no cover
         return True
 
     return False
 
 
-def function_name(function):
+def function_name(function) -> str:
     """
     Get name of function or method.
 
     :returns: function/method name
     :rtype: string
     """
     if isinstance(function, types.FunctionType):
         return function.__name__
 
     return function.__self__.__class__.__name__ + "." + function.__name__
 
 
-def indent_line(line, spaces=2):
+def indent_line(line: str, spaces: int = 2) -> str:
     """
     Indent line by a number of spaces.
 
     :param line: input text
     :type line: string
     :param spaces: number of spaces to prepend
     :type spaces: integer
     :returns: indented text
     :rtype: string
     """
-    return (' ' * spaces) + line
+    return f"{' ' * spaces}{line}"
 
 
-def indent_block(block, spaces=2):
+def indent_block(block: str, spaces: int = 2) -> str:
     """
     Indent a multiline string by a number of spaces.
 
     :param block: input text
     :type block: string
     :param spaces: number of spaces to prepend to each line
     :type spaces: integer
     :returns: indented text
     :rtype: string
     """
     lines = block.split('\n')
-    lines = filter(None, lines)
-    lines = map(lambda line, spc=spaces: indent_line(line, spc), lines)
-    return '\n'.join(lines)
+    lines_filter = filter(None, lines)
+    indented_lines = [indent_line(line, spaces) for line in lines_filter]
+    return '\n'.join(indented_lines)
 
 
-def is_errorcode_ewouldblock(errorcode):
+def is_errorcode_ewouldblock(errorcode: int) -> bool:
     """
     Check if the errorcode is a would-block error.
 
     :param errorcode: Code of the error
     :return: True if blocking error code
     """
     if errorcode in (errno.EAGAIN, errno.EWOULDBLOCK):
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/__init__.py` & `secsgem-0.2.0a3/secsgem/gem/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/gem/alarm.py` & `secsgem-0.2.0a3/secsgem/gem/alarm.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,30 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Wrapper for GEM alarm."""
+import typing
 
 import secsgem.secs
 
 
 class Alarm:
     """Alarm definition."""
 
-    def __init__(self, alid, name, text, code, ce_on, ce_off, **kwargs):
+    def __init__(self,
+                 alid: typing.Union[str, int],
+                 name: str,
+                 text: str,
+                 code: int,
+                 ce_on: typing.Union[str, int],
+                 ce_off: typing.Union[str, int],
+                 **kwargs):
         """
         Initialize an alarm.
 
         You can manually set the secs-type of the id with the 'id_type' keyword argument.
 
         :param alid: ID of the alarm
         :type alid: various
@@ -43,14 +51,16 @@
         self.text = text
         self.code = code
         self.ce_on = ce_on
         self.ce_off = ce_off
         self.enabled = False
         self.set = False
 
+        self.id_type: typing.Type[secsgem.secs.variables.Base]
+        
         if isinstance(self.alid, int):
             self.id_type = secsgem.secs.variables.U4
         else:
             self.id_type = secsgem.secs.variables.String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/collection_event.py` & `secsgem-0.2.0a3/secsgem/gem/collection_event.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,22 +10,27 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Wrapper for GEM collection event."""
+import typing
 
-import secsgem.secs
+import secsgem.secs.variables
 
 
 class CollectionEvent:
     """Collection event definition."""
 
-    def __init__(self, ceid, name, data_values, **kwargs):
+    def __init__(self,
+                 ceid: typing.Union[int, str],
+                 name: str,
+                 data_values: typing.List[typing.Union[int, str]],
+                 **kwargs):
         """
         Initialize a collection event.
 
         You can manually set the secs-type of the id with the 'id_type' keyword argument.
 
         Custom parameters can be set with the keyword arguments,
         they will be passed to the GemEquipmentHandlers callback
@@ -40,14 +45,16 @@
         :param data_values: data values available for this event
         :type data_values: list of DVIDs
         """
         self.ceid = ceid
         self.name = name
         self.data_values = data_values
 
+        self.id_type: typing.Type[secsgem.secs.variables.Base]
+
         if isinstance(self.ceid, int):
             self.id_type = secsgem.secs.variables.U4
         else:
             self.id_type = secsgem.secs.variables.String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/collection_event_link.py` & `secsgem-0.2.0a3/secsgem/gem/collection_event_link.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,20 +10,26 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Wrapper for GEM collection event link."""
+import typing
 
+from .collection_event import CollectionEvent
+from .collection_event_report import CollectionEventReport
 
 class CollectionEventLink:
     """Representation for registered/linked collection event."""
 
-    def __init__(self, ce, reports, **kwargs):
+    def __init__(self,
+                 ce: CollectionEvent,
+                 reports: typing.List[CollectionEventReport],
+                 **kwargs):
         """
         Initialize a collection event link.
 
         :param ce: ID of the collection event
         :type ce: :class:`gem.CollectionEvent`
         :param reports: list of the linked reports
         :type reports: list of :class:`gem.CollectionEventReport`
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/collection_event_report.py` & `secsgem-0.2.0a3/secsgem/gem/collection_event_report.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,35 +10,41 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Wrapper for GEM collection event report."""
+import typing
 
 import secsgem.secs
 
 
 class CollectionEventReport:
     """Report definition for registered collection events."""
 
-    def __init__(self, rptid, variables, **kwargs):
+    def __init__(self,
+                 rptid: typing.Union[int, str],
+                 variables: typing.List[typing.Union[int, str]], 
+                 **kwargs):
         """
         Initialize a collection event report.
 
         You can manually set the secs-type of the id with the 'id_type' keyword argument.
 
         :param rptid: ID of the report
         :type rptid: various
         :param vars: long name of the collection event
         :type vars: string
         """
         self.rptid = rptid
         self.vars = variables
 
+        self.id_type: typing.Type[secsgem.secs.variables.Base]
+
         if isinstance(self.rptid, int):
             self.id_type = secsgem.secs.variables.U4
         else:
             self.id_type = secsgem.secs.variables.String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/data_value.py` & `secsgem-0.2.0a3/secsgem/gem/data_value.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,28 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Wrapper for GEM data value."""
+import typing
 
 import secsgem.secs
 
 
 class DataValue:
     """Data value definition."""
 
-    def __init__(self, dvid, name, value_type, use_callback=True, **kwargs):
+    def __init__(self,
+                 dvid: typing.Union[int, str],
+                 name: str,
+                 value_type: typing.Type[secsgem.secs.variables.Base],
+                 use_callback: bool = True,
+                 **kwargs):
         """
         Initialize a data value.
 
         You can manually set the secs-type of the id with the 'id_type' keyword argument.
 
         Custom parameters can be set with the keyword arguments,
         they will be passed to the GemEquipmentHandlers callback
@@ -44,14 +50,16 @@
         """
         self.dvid = dvid
         self.name = name
         self.value_type = value_type
         self.use_callback = use_callback
         self.value = 0
 
+        self.id_type: typing.Type[secsgem.secs.variables.Base]
+        
         if isinstance(self.dvid, int):
             self.id_type = secsgem.secs.variables.U4
         else:
             self.id_type = secsgem.secs.variables.String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/equipment_constant.py` & `secsgem-0.2.0a3/secsgem/gem/equipment_constant.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,22 +10,32 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Wrapper for GEM equipment constant."""
+import typing
 
 import secsgem.secs
 
 
 class EquipmentConstant:
     """Equipment constant definition."""
 
-    def __init__(self, ecid, name, min_value, max_value, default_value, unit, value_type, use_callback=True, **kwargs):
+    def __init__(self,
+                 ecid: typing.Union[int, str],
+                 name: str,
+                 min_value: typing.Union[int, float],
+                 max_value: typing.Union[int, float],
+                 default_value: typing.Union[int, float],
+                 unit: str,
+                 value_type: typing.Type[secsgem.secs.variables.Base],
+                 use_callback: bool = True,
+                 **kwargs):
         """
         Initialize an equipment constant.
 
         You can manually set the secs-type of the id with the 'id_type' keyword argument.
 
         Custom parameters can be set with the keyword arguments,
         they will be passed to the GemEquipmentHandlers callbacks
@@ -57,14 +67,16 @@
         self.max_value = max_value
         self.default_value = default_value
         self.unit = unit
         self.value_type = value_type
         self.use_callback = use_callback
         self.value = default_value
 
+        self.id_type: typing.Type[secsgem.secs.variables.Base]
+
         if isinstance(self.ecid, int):
             self.id_type = secsgem.secs.variables.U4
         else:
             self.id_type = secsgem.secs.variables.String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/equipmenthandler.py` & `secsgem-0.2.0a3/secsgem/gem/equipmenthandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,30 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Handler for GEM equipment."""
-
 from datetime import datetime
+import typing
 
 from dateutil.tz import tzlocal
 
 import secsgem.common
+import secsgem.hsms
 import secsgem.secs.variables
 import secsgem.secs.data_items
 
 from .status_variable import StatusVariable
+from .alarm import Alarm
 from .collection_event import CollectionEvent
 from .collection_event_link import CollectionEventLink
 from .collection_event_report import CollectionEventReport
+from .data_value import DataValue
 from .equipment_constant import EquipmentConstant
 from .remote_command import RemoteCommand
 from .handler import GemHandler
 
 
 ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT = 1
 ECID_TIME_FORMAT = 2
@@ -51,83 +54,75 @@
 RCMD_START = "START"
 RCMD_STOP = "STOP"
 
 
 class GemEquipmentHandler(GemHandler):
     """Baseclass for creating equipment models. Inherit from this class and override required functions."""
 
-    def __init__(self, address, port, active, session_id, name, custom_connection_handler=None,
-                 initial_control_state="ATTEMPT_ONLINE", initial_online_control_state="REMOTE"):
+    def __init__(self,
+                 connection: secsgem.hsms.HsmsHandler,
+                 initial_control_state: str = "ATTEMPT_ONLINE",
+                 initial_online_control_state: str = "REMOTE"):
         """
         Initialize a gem equipment handler.
 
-        :param address: IP address of remote host
+        :param connection: Base connection
         :type address: string
-        :param port: TCP port of remote host
-        :type port: integer
-        :param active: Is the connection active (*True*) or passive (*False*)
-        :type active: boolean
-        :param session_id: session / device ID to use for connection
-        :type session_id: integer
-        :param name: Name of the underlying configuration
-        :type name: string
-        :param custom_connection_handler: object for connection handling (ie multi server)
-        :type custom_connection_handler: :class:`secsgem.hsms.connections.HsmsMultiPassiveServer`
         :param initial_control_state: initial state for the control state model, one of ["EQUIPMENT_OFFLINE",
         "ATTEMPT_ONLINE", "HOST_OFFLINE", "ONLINE"]
         :type initial_control_state: string
         """
-        super().__init__(address, port, active, session_id, name, custom_connection_handler)
+        super().__init__(connection)
 
         self.isHost = False
 
         self.initialControlStates = ["EQUIPMENT_OFFLINE", "ATTEMPT_ONLINE", "HOST_OFFLINE", "ONLINE"]
         self.initialControlState = initial_control_state
 
         self.onlineControlStates = ["LOCAL", "REMOTE"]
         self.onlineControlState = initial_online_control_state
 
         self._time_format = 1
 
-        self._data_values = {
+        self._data_values: typing.Dict[typing.Union[int, str], DataValue] = {
         }
 
-        self._status_variables = {
+        self._status_variables: typing.Dict[typing.Union[int, str], StatusVariable] = {
             SVID_CLOCK: StatusVariable(SVID_CLOCK, "Clock", "", secsgem.secs.variables.String),
             SVID_CONTROL_STATE: StatusVariable(SVID_CONTROL_STATE, "ControlState", "", secsgem.secs.variables.Binary),
             SVID_EVENTS_ENABLED: StatusVariable(SVID_EVENTS_ENABLED, "EventsEnabled", "", secsgem.secs.variables.Array),
             SVID_ALARMS_ENABLED: StatusVariable(SVID_ALARMS_ENABLED, "AlarmsEnabled", "", secsgem.secs.variables.Array),
             SVID_ALARMS_SET: StatusVariable(SVID_ALARMS_SET, "AlarmsSet", "", secsgem.secs.variables.Array),
         }
 
-        self._collection_events = {
+        self._collection_events: typing.Dict[typing.Union[int, str], CollectionEvent] = {
             CEID_EQUIPMENT_OFFLINE: CollectionEvent(CEID_EQUIPMENT_OFFLINE, "EquipmentOffline", []),
             CEID_CONTROL_STATE_LOCAL: CollectionEvent(CEID_CONTROL_STATE_LOCAL, "ControlStateLocal", []),
             CEID_CONTROL_STATE_REMOTE: CollectionEvent(CEID_CONTROL_STATE_REMOTE, "ControlStateRemote", []),
             CEID_CMD_START_DONE: CollectionEvent(CEID_CMD_START_DONE, "CmdStartDone", []),
             CEID_CMD_STOP_DONE: CollectionEvent(CEID_CMD_STOP_DONE, "CmdStopDone", []),
         }
 
-        self._equipment_constants = {
+        self._equipment_constants: typing.Dict[typing.Union[int, str], EquipmentConstant] = {
             ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT: EquipmentConstant(ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT,
                                                                      "EstablishCommunicationsTimeout", 10, 120, 10,
                                                                      "sec", secsgem.secs.variables.I2),
             ECID_TIME_FORMAT: EquipmentConstant(ECID_TIME_FORMAT, "TimeFormat", 0, 2, 1, "", secsgem.secs.variables.I4),
         }
 
-        self._alarms = {
+        self._alarms: typing.Dict[typing.Union[int, str], Alarm] = {
         }
 
-        self._remote_commands = {
+        self._remote_commands: typing.Dict[typing.Union[int, str], RemoteCommand] = {
             RCMD_START: RemoteCommand(RCMD_START, "Start", [], CEID_CMD_START_DONE),
             RCMD_STOP: RemoteCommand(RCMD_STOP, "Stop", [], CEID_CMD_STOP_DONE),
         }
 
-        self._registered_reports = {}
-        self._registered_collection_events = {}
+        self._registered_reports: typing.Dict[typing.Union[int, str], CollectionEventReport] = {}
+        self._registered_collection_events: typing.Dict[typing.Union[int, str], CollectionEventLink] = {}
 
         self.controlState = secsgem.common.Fysom({
             'initial': "INIT",
             'events': [
                 {'name': 'start', 'src': 'INIT', 'dst': 'CONTROL'},  # 1
                 {'name': 'initial_offline', 'src': 'CONTROL', 'dst': 'OFFLINE'},  # 1
                 {'name': 'initial_equipment_offline', 'src': 'OFFLINE', 'dst': 'EQUIPMENT_OFFLINE'},  # 2
@@ -162,15 +157,15 @@
             'autoforward': [
                 # {'src': 'OFFLINE', 'dst': 'EQUIPMENT_OFFLINE'},  # 2
                 # {'src': 'EQUIPMENT_INITIATED_CONNECT', 'dst': 'WAIT_CRA'},  # 5
                 # {'src': 'HOST_INITIATED_CONNECT', 'dst': 'WAIT_CR_FROM_HOST'},  # 10
             ]
         })
 
-        self.controlState.start()
+        self.controlState.start()  # type: ignore
 
     # control state model
 
     def _on_control_state_control(self, _):
         if self.initialControlState == "ONLINE":
             self.controlState.initial_online()
         else:
@@ -228,67 +223,73 @@
         self.onlineControlState = "LOCAL"
 
     def control_switch_online_remote(self):
         """Operator switches to the local online control state."""
         self.controlState.switch_online_remote()
         self.onlineControlState = "REMOTE"
 
-    def _on_s01f15(self, handler, packet):
+    def _on_s01f15(self, 
+                   handler: secsgem.secs.SecsHandler, 
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 15, Request offline.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
         """
         del handler, packet  # unused parameters
 
         OFLACK = 0
 
         if self.controlState.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
-            self.controlState.remote_offline()
+            self.controlState.remote_offline()  # type: ignore
             self.trigger_collection_events([CEID_EQUIPMENT_OFFLINE])
 
         return self.stream_function(1, 16)(OFLACK)
 
-    def _on_s01f17(self, handler, packet):
+    def _on_s01f17(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 17, Request online.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
         """
         del handler, packet  # unused parameters
 
         ONLACK = 1
 
         if self.controlState.isstate("HOST_OFFLINE"):
-            self.controlState.remote_online()
+            self.controlState.remote_online()  # type: ignore
             ONLACK = 0
         elif self.controlState.current in ["ONLINE", "ONLINE_LOCAL", "ONLINE_REMOTE"]:
             ONLACK = 2
 
         return self.stream_function(1, 18)(ONLACK)
 
     # data values
 
     @property
-    def data_values(self):
+    def data_values(self) -> typing.Dict[typing.Union[int, str], DataValue]:
         """
         Get list of the data values.
 
         :returns: Data value list
         :rtype: list of :class:`secsgem.gem.DataValue`
         """
         return self._data_values
 
-    def on_dv_value_request(self, dvid, dv):
+    def on_dv_value_request(self, 
+                            dvid: secsgem.secs.variables.Base, 
+                            dv: DataValue) -> secsgem.secs.variables.Base:
         """
         Get the data value depending on its configuation.
 
         Override in inherited class to provide custom data value request handling.
 
         :param dvid: Id of the data value encoded in the corresponding type
         :type dvid: :class:`secsgem.secs.variables.Base`
@@ -297,15 +298,15 @@
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
         del dvid  # unused variable
 
         return dv.value_type(dv.value)
 
-    def _get_dv_value(self, dv):
+    def _get_dv_value(self, dv: DataValue) -> secsgem.secs.variables.Base:
         """
         Get the data value depending on its configuation.
 
         :param dv: The data value requested
         :type dv: :class:`secsgem.gem.DataValue`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
@@ -314,24 +315,24 @@
             return self.on_dv_value_request(dv.id_type(dv.dvid), dv)
 
         return dv.value_type(dv.value)
 
     # status variables
 
     @property
-    def status_variables(self):
+    def status_variables(self) -> typing.Dict[typing.Union[int, str], StatusVariable]:
         """
         Get list of the status variables.
 
         :returns: Status variable list
         :rtype: list of :class:`secsgem.gem.StatusVariables`
         """
         return self._status_variables
 
-    def on_sv_value_request(self, svid, sv):
+    def on_sv_value_request(self, svid: secsgem.secs.variables.Base, sv: StatusVariable) -> secsgem.secs.variables.Base:
         """
         Get the status variable value depending on its configuation.
 
         Override in inherited class to provide custom status variable request handling.
 
         :param svid: Id of the status variable encoded in the corresponding type
         :type svid: :class:`secsgem.secs.variables.Base`
@@ -340,15 +341,15 @@
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
         del svid  # unused variable
 
         return sv.value_type(sv.value)
 
-    def _get_sv_value(self, sv):
+    def _get_sv_value(self, sv: StatusVariable) -> secsgem.secs.variables.Base:
         """
         Get the status variable value depending on its configuation.
 
         :param sv: The status variable requested
         :type sv: :class:`secsgem.gem.StatusVariable`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
@@ -368,15 +369,17 @@
             return sv.value_type(secsgem.secs.data_items.SV, alarms)
 
         if sv.use_callback:
             return self.on_sv_value_request(sv.id_type(sv.svid), sv)
 
         return sv.value_type(sv.value)
 
-    def _on_s01f03(self, handler, packet):
+    def _on_s01f03(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 3, Equipment status request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -396,15 +399,17 @@
                     responses.append(secsgem.secs.variables.Array(secsgem.secs.data_items.SV, []))
                 else:
                     sv = self._status_variables[svid]
                     responses.append(self._get_sv_value(sv))
 
         return self.stream_function(1, 4)(responses)
 
-    def _on_s01f11(self, handler, packet):
+    def _on_s01f11(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 11, SV namelist request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -427,45 +432,45 @@
                     responses.append({"SVID": sv.svid, "SVNAME": sv.name, "UNITS": sv.unit})
 
         return self.stream_function(1, 12)(responses)
 
     # collection events
 
     @property
-    def collection_events(self):
+    def collection_events(self) -> typing.Dict[typing.Union[int, str], CollectionEvent]:
         """
         Get list of the collection events.
 
         :returns: Collection event list
         :rtype: list of :class:`secsgem.gem.CollectionEvent`
         """
         return self._collection_events
 
     @property
-    def registered_reports(self):
+    def registered_reports(self) -> typing.Dict[typing.Union[int, str], CollectionEventReport]:
         """
         Get list of the subscribed reports.
 
         :returns: Collection event report list
         :rtype: dictionary of subscribed reports
         """
         return self._registered_reports
 
     @property
-    def registered_collection_events(self):
+    def registered_collection_events(self) -> typing.Dict[typing.Union[int, str], CollectionEventLink]:
         """
         Get list of the subscribed collection events.
 
         :returns: Collection event list
         :rtype: dictionary of :class:`secsgem.gem.CollectionEventLink`
 
         """
         return self._registered_collection_events
 
-    def trigger_collection_events(self, ceids):
+    def trigger_collection_events(self, ceids: typing.List[typing.Union[int, str]]):
         """
         Triggers the supplied collection events.
 
         :param ceids: List of collection events
         :type ceids: list of various
         """
         if not isinstance(ceids, list):
@@ -475,15 +480,17 @@
             if ceid in self._registered_collection_events:
                 if self._registered_collection_events[ceid].enabled:
                     reports = self._build_collection_event(ceid)
 
                     self.send_and_waitfor_response(self.stream_function(6, 11)(
                         {"DATAID": 1, "CEID": ceid, "RPT": reports}))
 
-    def _on_s02f33(self, handler, packet):
+    def _on_s02f33(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 33, Define Report.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -536,15 +543,17 @@
                     del self._registered_reports[report.RPTID]
             else:
                 # add report
                 self._registered_reports[report.RPTID] = CollectionEventReport(report.RPTID, report.VID)
 
         return result
 
-    def _on_s02f35(self, handler, packet):
+    def _on_s02f35(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 35, Link event report.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -588,15 +597,17 @@
                             ce.reports.append(rptid)
                     else:
                         self._registered_collection_events[event.CEID.get()] = \
                             CollectionEventLink(self._collection_events[event.CEID.get()], event.RPTID.get())
 
         return self.stream_function(2, 36)(LRACK)
 
-    def _on_s02f37(self, handler, packet):
+    def _on_s02f37(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Callback handler for Stream 2, Function 37, En-/Disable Event Report.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -610,15 +621,17 @@
         ERACK = 0
 
         if not self._set_ce_state(message.CEED.get(), message.CEID.get()):
             ERACK = 1
 
         return self.stream_function(2, 38)(ERACK)
 
-    def _on_s06f15(self, handler, packet):
+    def _on_s06f15(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Callback handler for Stream 6, Function 15, event report request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -633,15 +646,15 @@
 
         if ceid in self._registered_collection_events:
             if self._registered_collection_events[ceid].enabled:
                 reports = self._build_collection_event(ceid)
 
         return self.stream_function(6, 16)({"DATAID": 1, "CEID": ceid, "RPT": reports})
 
-    def _set_ce_state(self, ceed, ceids):
+    def _set_ce_state(self, ceed: bool, ceids: typing.List[typing.Union[int, str]]) -> bool:
         """
         En-/Disable event reports for the supplied ceids (or all, if ceid is an empty list).
 
         :param ceed: Enable (True) or disable (False) event reports
         :type ceed: bool
         :param ceids: List of collection events
         :type ceids: list of integer
@@ -657,15 +670,15 @@
                 if ceid in self._registered_collection_events:
                     self._registered_collection_events[ceid].enabled = ceed
                 else:
                     result = False
 
         return result
 
-    def _build_collection_event(self, ceid):
+    def _build_collection_event(self, ceid: typing.Union[int, str]):
         """
         Build reports for a collection event.
 
         :param ceid: collection event to build
         :type ceid: integer
         :returns: collection event data
         :rtype: array
@@ -686,24 +699,26 @@
             reports.append({"RPTID": rptid, "V": variables})
 
         return reports
 
     # equipment constants
 
     @property
-    def equipment_constants(self):
+    def equipment_constants(self) -> typing.Dict[typing.Union[int, str], EquipmentConstant]:
         """
         The list of the equipments contstants.
 
         :returns: Equipment constant list
         :rtype: list of :class:`secsgem.gem.EquipmentConstant`
         """
         return self._equipment_constants
 
-    def on_ec_value_request(self, ecid, ec):
+    def on_ec_value_request(self,
+                            ecid: secsgem.secs.variables.Base,
+                            ec: EquipmentConstant) -> secsgem.secs.variables.Base:
         """
         Get the equipment constant value depending on its configuation.
 
         Override in inherited class to provide custom equipment constant request handling.
 
         :param ecid: Id of the equipment constant encoded in the corresponding type
         :type ecid: :class:`secsgem.secs.variables.Base`
@@ -712,15 +727,18 @@
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
         """
         del ecid  # unused variable
 
         return ec.value_type(ec.value)
 
-    def on_ec_value_update(self, ecid, ec, value):
+    def on_ec_value_update(self,
+                           ecid: secsgem.secs.variables.Base,
+                           ec: EquipmentConstant, 
+                           value: typing.Union[int, float]):
         """
         Set the equipment constant value depending on its configuation.
 
         Override in inherited class to provide custom equipment constant update handling.
 
         :param ecid: Id of the equipment constant encoded in the corresponding type
         :type ecid: :class:`secsgem.secs.variables.Base`
@@ -729,15 +747,15 @@
         :param value: The value encoded in the corresponding type
         :type value: :class:`secsgem.secs.variables.Base`
         """
         del ecid  # unused variable
 
         ec.value = value
 
-    def _get_ec_value(self, ec):
+    def _get_ec_value(self, ec: EquipmentConstant) -> secsgem.secs.variables.Base:
         """
         Get the equipment constant value depending on its configuation.
 
         :param ec: The equipment requested
         :type ec: :class:`secsgem.gem.EquipmentConstant`
         :returns: The value encoded in the corresponding type
         :rtype: :class:`secsgem.secs.variables.Base`
@@ -747,34 +765,36 @@
         if ec.ecid == ECID_TIME_FORMAT:
             return ec.value_type(self._time_format)
 
         if ec.use_callback:
             return self.on_ec_value_request(ec.id_type(ec.ecid), ec)
         return ec.value_type(ec.value)
 
-    def _set_ec_value(self, ec, value):
+    def _set_ec_value(self, ec: EquipmentConstant, value: typing.Union[int, float]):
         """
         Get the equipment constant value depending on its configuation.
 
         :param ec: The equipment requested
         :type ec: :class:`secsgem.gem.EquipmentConstant`
         :param value: The value encoded in the corresponding type
         :type value: :class:`secsgem.secs.variables.Base`
         """
         if ec.ecid == ECID_ESTABLISH_COMMUNICATIONS_TIMEOUT:
-            self.establishCommunicationTimeout = value
+            self.establishCommunicationTimeout = int(value)
         if ec.ecid == ECID_TIME_FORMAT:
-            self._time_format = value
+            self._time_format = int(value)
 
         if ec.use_callback:
             self.on_ec_value_update(ec.id_type(ec.ecid), ec, value)
         else:
             ec.value = value
 
-    def _on_s02f13(self, handler, packet):
+    def _on_s02f13(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 13, Equipment constant request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -794,15 +814,17 @@
                     responses.append(secsgem.secs.variables.Array(secsgem.secs.data_items.ECV, []))
                 else:
                     ec = self._equipment_constants[ecid]
                     responses.append(self._get_ec_value(ec))
 
         return self.stream_function(2, 14)(responses)
 
-    def _on_s02f15(self, handler, packet):
+    def _on_s02f15(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 15, Equipment constant send.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -825,19 +847,21 @@
 
                 if constant.max_value is not None:
                     if ec.ECV.get() > constant.max_value:
                         eac = 3
 
         if eac == 0:
             for ec in message:
-                self._set_ec_value(self._equipment_constants[ec.ECID], ec.ECV)
+                self._set_ec_value(self._equipment_constants[ec.ECID], ec.ECV.get())
 
         return self.stream_function(2, 16)(eac)
 
-    def _on_s02f29(self, handler, packet):
+    def _on_s02f29(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 29, EC namelist request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -866,24 +890,24 @@
                                       "ECDEF": eq_constant.default_value, "UNITS": eq_constant.unit})
 
         return self.stream_function(2, 30)(responses)
 
     # alarms
 
     @property
-    def alarms(self):
+    def alarms(self) -> typing.Dict[typing.Union[int, str], Alarm]:
         """
         Get the list of the alarms.
 
         :returns: Alarms list
         :rtype: list of :class:`secsgem.gem.Alarm`
         """
         return self._alarms
 
-    def set_alarm(self, alid):
+    def set_alarm(self, alid: typing.Union[int, str]):
         """
         Set the list of the alarms.
 
         :param alid: Alarm id
         :type alid: str/int
         """
         if alid not in self.alarms:
@@ -900,15 +924,15 @@
                     "ALTX": self.alarms[alid].text
                 }))
 
         self.alarms[alid].set = True
 
         self.trigger_collection_events([self.alarms[alid].ce_on])
 
-    def clear_alarm(self, alid):
+    def clear_alarm(self, alid: typing.Union[int, str]):
         """
         Clear the list of the alarms.
 
         :param alid: Alarm id
         :type alid: str/int
         """
         if alid not in self.alarms:
@@ -921,15 +945,17 @@
             self.send_and_waitfor_response(self.stream_function(5, 1)({"ALCD": self.alarms[alid].code,
                                                                        "ALID": alid, "ALTX": self.alarms[alid].text}))
 
         self.alarms[alid].set = False
 
         self.trigger_collection_events([self.alarms[alid].ce_off])
 
-    def _on_s05f03(self, handler, packet):
+    def _on_s05f03(self,
+                   handler: secsgem.secs.SecsHandler, 
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 3, Alarm en-/disabled.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -946,15 +972,17 @@
         if alid not in self._alarms:
             result = secsgem.secs.data_items.ACKC5.ERROR
         else:
             self.alarms[alid].enabled = (message.ALED.get() == secsgem.secs.data_items.ALED.ENABLE)
 
         return self.stream_function(5, 4)(result)
 
-    def _on_s05f05(self, handler, packet):
+    def _on_s05f05(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 5, Alarm list.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -974,15 +1002,17 @@
             result.append({"ALCD": self.alarms[alid].code |
                            (secsgem.secs.data_items.ALCD.ALARM_SET if self.alarms[alid].set else 0),
                            "ALID": alid,
                            "ALTX": self.alarms[alid].text})
 
         return self.stream_function(5, 6)(result)
 
-    def _on_s05f07(self, handler, packet):
+    def _on_s05f07(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 7, Enabled alarm list.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -998,24 +1028,26 @@
                                "ALID": alid, "ALTX": self.alarms[alid].text})
 
         return self.stream_function(5, 8)(result)
 
     # remote commands
 
     @property
-    def remote_commands(self):
+    def remote_commands(self) -> typing.Dict[typing.Union[int, str], RemoteCommand]:
         """
         Get list of the remote commands.
 
         :returns: Remote command list
         :rtype: list of :class:`secsgem.gem.RemoteCommand`
         """
         return self._remote_commands
 
-    def _on_s02f41(self, handler, packet):
+    def _on_s02f41(self,
+                   handler: secsgem.secs.SecsHandler,
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 2, Function 41, host command send.
 
         The remote command handing differs from usual stream function handling, because we send the ack with later
         completion first.
         Then we run the actual remote command callback and signal success with the matching collection event.
 
@@ -1065,15 +1097,15 @@
         self.logger.warning("remote command START not implemented, this is required for GEM compliance")
 
     def _on_rcmd_STOP(self):
         self.logger.warning("remote command STOP not implemented, this is required for GEM compliance")
 
     # helpers
 
-    def _get_clock(self):
+    def _get_clock(self) -> str:
         """
         Get the clock depending on configured time format.
 
         :returns: time code
         :rtype: string
         """
         now = datetime.now(tzlocal())
@@ -1081,15 +1113,15 @@
             return now.strftime("%y%m%d%H%M%S")
 
         if self._time_format == 2:
             return now.isoformat()
 
         return now.strftime("%Y%m%d%H%M%S") + now.strftime("%f")[0:2]
 
-    def _get_control_state_id(self):
+    def _get_control_state_id(self) -> int:
         """
         Get id of the control state for the current control state.
 
         :returns: control state
         :rtype: integer
         """
         if self.controlState.isstate("EQUIPMENT_OFFLINE"):
@@ -1101,45 +1133,45 @@
         if self.controlState.isstate("ONLINE_LOCAL"):
             return 4
         if self.controlState.isstate("ONLINE_REMOTE"):
             return 5
 
         return -1
 
-    def _get_events_enabled(self):
+    def _get_events_enabled(self) -> typing.List[typing.Union[int, str]]:
         """
         List of the enabled collection events.
 
         :returns: collection event
         :rtype: list of various
         """
         enabled_ceid = []
 
         for ceid, collection_event in self._registered_collection_events.items():
             if collection_event.enabled:
                 enabled_ceid.append(ceid)
 
         return enabled_ceid
 
-    def _get_alarms_enabled(self):
+    def _get_alarms_enabled(self) -> typing.List[typing.Union[int, str]]:
         """
         List of the enabled alarms.
 
         :returns: alarms
         :rtype: list of various
         """
         enabled_alarms = []
 
         for alid, alarm in self._alarms.items():
             if alarm.enabled:
                 enabled_alarms.append(alid)
 
         return enabled_alarms
 
-    def _get_alarms_set(self):
+    def _get_alarms_set(self) -> typing.List[typing.Union[int, str]]:
         """
         List of the set alarms.
 
         :returns: alarms
         :rtype: list of various
         """
         set_alarms = []
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/handler.py` & `secsgem-0.2.0a3/secsgem/gem/handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,45 +10,36 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Handler for GEM commands. Used in combination with :class:`secsgem.HsmsHandler.HsmsConnectionManager`."""
-
 import logging
 import threading
+import typing
 
 import secsgem.common
+import secsgem.hsms
 import secsgem.secs
 
 
 class GemHandler(secsgem.secs.SecsHandler):
     """Baseclass for creating Host/Equipment models. This layer contains GEM functionality."""
 
-    def __init__(self, address, port, active, session_id, name, custom_connection_handler=None):
+    def __init__(self, connection: secsgem.hsms.HsmsHandler):
         """
         Initialize a gem handler.
 
         Inherit from this class and override required functions.
 
-        :param address: IP address of remote host
-        :type address: string
-        :param port: TCP port of remote host
-        :type port: integer
-        :param active: Is the connection active (*True*) or passive (*False*)
-        :type active: boolean
-        :param session_id: session / device ID to use for connection
-        :type session_id: integer
-        :param name: Name of the underlying configuration
-        :type name: string
-        :param custom_connection_handler: object for connection handling (ie multi server)
-        :type custom_connection_handler: :class:`secsgem.hsms.connections.HsmsMultiPassiveServer`
+        :param connection: connection to use
         """
-        super().__init__(address, port, active, session_id, name, custom_connection_handler)
+        super().__init__(connection)
+        self._connection.events.hsms_selected += self._on_hsms_select
 
         self.MDLN = "secsgem"  #: model number returned by S01E13/14
         self.SOFTREV = "0.1.0"  #: software version returned by S01E13/14
 
         self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
 
         self.isHost = True
@@ -90,76 +81,76 @@
 
         self.waitCRATimer = None
         self.commDelayTimer = None
         self.establishCommunicationTimeout = 10
 
         self.reportIDCounter = 1000
 
-        self.waitEventList = []
+        self.waitEventList: typing.List[threading.Event] = []
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Generate textual representation for an object of this class."""
         return f"{self.__class__.__name__} {str(self._serialize_data())}"
 
-    def _serialize_data(self):
+    def _serialize_data(self)-> typing.Dict[str, typing.Any]:
         """
         Get serialized data.
 
         :returns: data to serialize for this object
         :rtype: dict
         """
-        data = super()._serialize_data()
+        data = self.connection._serialize_data()  # pylint: disable=protected-access
         data.update({'communicationState': self.communicationState.current,
                      'commDelayTimeout': self.establishCommunicationTimeout,
                      'reportIDCounter': self.reportIDCounter})
         return data
 
-    def enable(self):
+    def enable(self) -> None:
         """Enable the connection."""
         self.connection.enable()
-        self.communicationState.enable()
+        self.communicationState.enable()  # type: ignore
 
         self.logger.info("Connection enabled")
 
-    def disable(self):
+    def disable(self) -> None:
         """Disable the connection."""
         self.connection.disable()
-        self.communicationState.disable()
+        self.communicationState.disable()  # type: ignore
 
         self.logger.info("Connection disabled")
 
-    def _on_hsms_packet_received(self, packet):
+    def _on_hsms_packet_received(self, data: typing.Dict[str, typing.Any]):
         """
         Packet received from hsms layer.
 
-        :param packet: received data packet
-        :type packet: :class:`secsgem.HsmsPacket`
+        :param data: received event data
         """
+        packet = data["packet"]
         if self.communicationState.isstate('WAIT_CRA'):
             if packet.header.stream == 1 and packet.header.function == 13:
                 if self.isHost:
                     self.send_response(self.stream_function(1, 14)({"COMMACK": self.on_commack_requested(),
                                                                     "MDLN": []}),
                                        packet.header.system)
                 else:
                     self.send_response(self.stream_function(1, 14)({"COMMACK": self.on_commack_requested(),
                                                                     "MDLN": [self.MDLN, self.SOFTREV]}),
                                        packet.header.system)
 
-                self.communicationState.s1f13received()
+                self.communicationState.s1f13received()  # type: ignore
             elif packet.header.stream == 1 and packet.header.function == 14:
-                self.communicationState.s1f14received()
+                self.communicationState.s1f14received()  # type: ignore
         elif self.communicationState.isstate('WAIT_DELAY'):
             pass
         elif self.communicationState.isstate('COMMUNICATING'):
             threading.Thread(target=self._handle_stream_function, args=(packet, ),
                              name=f"secsgem_gemHandler_callback_S{packet.header.stream}F{packet.header.function}"
                              ).start()
 
-    def _on_hsms_select(self):
+    def _on_hsms_select(self, _):
         """Selected received from hsms layer."""
         self.communicationState.select()
 
     def _on_wait_cra_timeout(self):
         """Linktest time timed out, so send linktest request."""
         self.communicationState.communicationreqfail()
 
@@ -172,15 +163,15 @@
         Connection state model changed to state WAIT_CRA.
 
         :param data: event attributes
         :type data: object
         """
         self.logger.debug("connectionState -> WAIT_CRA")
 
-        self.waitCRATimer = threading.Timer(self.connection.T3, self._on_wait_cra_timeout)
+        self.waitCRATimer = threading.Timer(self.connection.connection.T3, self._on_wait_cra_timeout)
         self.waitCRATimer.start()
 
         if self.isHost:
             self.send_stream_function(self.stream_function(1, 13)())
         else:
             self.send_stream_function(self.stream_function(1, 13)([self.MDLN, self.SOFTREV]))
 
@@ -237,54 +228,57 @@
         # call parent handlers
         super().on_connection_closed(connection)
 
         if self.communicationState.current == "COMMUNICATING":
             # update communication state
             self.communicationState.communicationfail()
 
-    def on_commack_requested(self):
+    def on_commack_requested(self) -> int:
         """
         Get the acknowledgement code for the connection request.
 
         override to accept or deny connection request
 
         :returns: 0 when connection is accepted, 1 when connection is denied
         :rtype: integer
         """
         return 0
 
-    def send_process_program(self, ppid, ppbody):
+    def send_process_program(self,
+                             ppid: typing.Union[int, str],
+                             ppbody: str):
         """
         Send a process program.
 
         :param ppid: Transferred process programs ID
         :type ppid: string
         :param ppbody: Content of process program
         :type ppbody: string
         """
         # send remote command
         self.logger.info("Send process program %s", ppid)
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 3)(
             {"PPID": ppid, "PPBODY": ppbody}))).get()
 
-    def request_process_program(self, ppid):
+    def request_process_program(self, 
+                                ppid: typing.Union[int, str]) -> typing.Tuple[typing.Union[int, str], str]:
         """
         Request a process program.
 
         :param ppid: Transferred process programs ID
         :type ppid: string
         """
         self.logger.info("Request process program %s", ppid)
 
         # send remote command
         s7f6 = self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 5)(ppid)))
         return s7f6.PPID.get(), s7f6.PPBODY.get()
 
-    def waitfor_communicating(self, timeout=None):
+    def waitfor_communicating(self, timeout: typing.Optional[float] = None) -> bool:
         """
         Wait until connection gets into communicating state. Returns immediately if state is communicating.
 
         :param timeout: seconds to wait before aborting
         :type timeout: float
         :returns: True if state is communicating, False if timed out
         :rtype: bool
@@ -298,15 +292,17 @@
 
         result = event.wait(timeout)
 
         self.waitEventList.remove(event)
 
         return result
 
-    def _on_s01f01(self, handler, packet):
+    def _on_s01f01(self, 
+                   handler: secsgem.secs.SecsHandler, 
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 1, Are You There.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -314,15 +310,17 @@
         del handler, packet  # unused parameters
 
         if self.isHost:
             return self.stream_function(1, 2)()
 
         return self.stream_function(1, 2)([self.MDLN, self.SOFTREV])
 
-    def _on_s01f13(self, handler, packet):
+    def _on_s01f13(self, 
+                   handler: secsgem.secs.SecsHandler, 
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 1, Function 13, Establish Communication Request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/hosthandler.py` & `secsgem-0.2.0a3/secsgem/gem/hosthandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,62 +10,55 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Handler for GEM host."""
-
 import collections
+import typing
 
+import secsgem.hsms
 import secsgem.secs
 
 from .handler import GemHandler
 
 
 class GemHostHandler(GemHandler):
     """Baseclass for creating host models. Inherit from this class and override required functions."""
 
-    def __init__(self, address, port, active, session_id, name, custom_connection_handler=None):
+    def __init__(self, connection: secsgem.hsms.HsmsHandler):
         """
         Initialize a gem host handler.
 
-        :param address: IP address of remote host
-        :type address: string
-        :param port: TCP port of remote host
-        :type port: integer
-        :param active: Is the connection active (*True*) or passive (*False*)
-        :type active: boolean
-        :param session_id: session / device ID to use for connection
-        :type session_id: integer
-        :param name: Name of the underlying configuration
-        :type name: string
-        :param custom_connection_handler: object for connection handling (ie multi server)
-        :type custom_connection_handler: :class:`secsgem.hsms.connections.HsmsMultiPassiveServer`
+        :param connection: Connection
         """
-        GemHandler.__init__(self, address, port, active, session_id, name, custom_connection_handler)
+        GemHandler.__init__(self, connection)
 
         self.isHost = True
 
-        self.reportSubscriptions = {}
+        self.reportSubscriptions: typing.Dict[typing.Union[int, str], typing.List[typing.Union[int, str]]] = {}
 
-    def clear_collection_events(self):
+    def clear_collection_events(self) -> None:
         """Clear all collection events."""
         self.logger.info("Clearing collection events")
 
         # clear subscribed reports
         self.reportSubscriptions = {}
 
         # disable all ceids
         self.disable_ceids()
 
         # delete all reports
         self.disable_ceid_reports()
 
-    def subscribe_collection_event(self, ceid, dvs, report_id=None):
+    def subscribe_collection_event(self,
+                                   ceid: typing.Union[int, str],
+                                   dvs: typing.List[typing.Union[int, str]],
+                                   report_id: typing.Optional[typing.Union[int, str]] = None):
         """
         Subscribe to a collection event.
 
         :param ceid: ID of the collection event
         :type ceid: integer
         :param dvs: DV IDs to add for collection event
         :type dvs: list of integers
@@ -88,15 +81,17 @@
         # link event report to collection event
         self.send_and_waitfor_response(self.stream_function(2, 35)(
             {"DATAID": 0, "DATA": [{"CEID": ceid, "RPTID": [report_id]}]}))
 
         # enable collection event
         self.send_and_waitfor_response(self.stream_function(2, 37)({"CEED": True, "CEID": [ceid]}))
 
-    def send_remote_command(self, rcmd, params):
+    def send_remote_command(self,
+                            rcmd: typing.Union[int, str],
+                            params: typing.List[str]):
         """
         Send a remote command.
 
         :param rcmd: Name of command
         :type rcmd: string
         :param params: DV IDs to add for collection event
         :type params: list of strings
@@ -111,72 +106,78 @@
         elif isinstance(params, collections.OrderedDict):
             for param in params:
                 s2f41.PARAMS.append({"CPNAME": param, "CPVAL": params[param]})
 
         # send remote command
         return self.secs_decode(self.send_and_waitfor_response(s2f41))
 
-    def delete_process_programs(self, ppids):
+    def delete_process_programs(self,
+                                ppids: typing.List[typing.Union[int, str]]):
         """
         Delete a list of process program.
 
         :param ppids: Process programs to delete
         :type ppids: list of strings
         """
         self.logger.info("Delete process programs %s", ppids)
 
         # send remote command
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 17)(ppids))).get()
 
-    def get_process_program_list(self):
+    def get_process_program_list(self) -> secsgem.secs.SecsStreamFunction:
         """Get process program list."""
         self.logger.info("Get process program list")
 
         # send remote command
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(7, 19)())).get()
 
-    def go_online(self):
+    def go_online(self) -> typing.Optional[str]:
         """Set control state to online."""
         self.logger.info("Go online")
 
         # send remote command
-        return self.secs_decode(self.send_and_waitfor_response(self.stream_function(1, 17)())).get()
+        resp = self.secs_decode(self.send_and_waitfor_response(self.stream_function(1, 17)()))
+        if resp is None:
+            return None
+
+        return resp.get()
 
-    def go_offline(self):
+    def go_offline(self) -> typing.Optional[str]:
         """Set control state to offline."""
         self.logger.info("Go offline")
 
         # send remote command
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(1, 15)())).get()
 
-    def enable_alarm(self, alid):
+    def enable_alarm(self, alid: typing.Union[int, str]):
         """
         Enable alarm.
 
         :param alid: alarm id to enable
         :type alid: :class:`secsgem.secs.dataitems.ALID`
         """
         self.logger.info("Enable alarm %d", alid)
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(5, 3)(
             {"ALED": secsgem.secs.data_items.ALED.ENABLE, "ALID": alid}))).get()
 
-    def disable_alarm(self, alid):
+    def disable_alarm(self, alid: typing.Union[int, str]):
         """
         Disable alarm.
 
         :param alid: alarm id to disable
         :type alid: :class:`secsgem.secs.dataitems.ALID`
         """
         self.logger.info("Disable alarm %d", alid)
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(5, 3)(
             {"ALED": secsgem.secs.data_items.ALED.DISABLE, "ALID": alid}))).get()
 
-    def list_alarms(self, alids=None):
+    def list_alarms(self, 
+                    alids: typing.Optional[typing.List[typing.Union[int, str]]] = None):
         """
         List alarms.
 
         :param alids: alarms to list details for
         :type alids: array of int/str
         """
         if alids is None:
@@ -193,15 +194,17 @@
 
         return self.secs_decode(self.send_and_waitfor_response(self.stream_function(5, 7)())).get()
 
     def _on_alarm_received(self, handler, ALID, ALCD, ALTX):
         del handler, ALID, ALCD, ALTX  # unused variables
         return secsgem.secs.data_items.ACKC5.ACCEPTED
 
-    def _on_s05f01(self, handler, packet):
+    def _on_s05f01(self, 
+                   handler: secsgem.secs.SecsHandler, 
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 5, Function 1, Alarm request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -211,15 +214,17 @@
         result = self._callback_handler.alarm_received(handler, s5f1.ALID, s5f1.ALCD, s5f1.ALTX)
 
         self.events.fire("alarm_received", {"code": s5f1.ALCD, "alid": s5f1.ALID, "text": s5f1.ALTX,
                                             "handler": self.connection, 'peer': self})
 
         return self.stream_function(5, 2)(result)
 
-    def _on_s06f11(self, handler, packet):
+    def _on_s06f11(self, 
+                   handler: secsgem.secs.SecsHandler, 
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 6, Function 11, Establish Communication Request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
@@ -243,15 +248,17 @@
 
         return self.stream_function(6, 12)(0)
 
     def _on_terminal_received(self, handler, TID, TEXT):
         del handler, TID, TEXT  # unused variables
         return secsgem.secs.data_items.ACKC10.ACCEPTED
 
-    def _on_s10f01(self, handler, packet):
+    def _on_s10f01(self, 
+                   handler: secsgem.secs.SecsHandler, 
+                   packet: secsgem.hsms.HsmsPacket) -> typing.Optional[secsgem.secs.SecsStreamFunction]:
         """
         Handle Stream 10, Function 1, Terminal Request.
 
         :param handler: handler the message was received on
         :type handler: :class:`secsgem.hsms.handler.HsmsHandler`
         :param packet: complete message received
         :type packet: :class:`secsgem.hsms.HsmsPacket`
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/remote_command.py` & `secsgem-0.2.0a3/secsgem/gem/remote_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,22 +10,28 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Wrapper for GEM remote command."""
+import typing
 
-import secsgem.secs
+from secsgem.secs.variables import U4, String, Base
 
 
 class RemoteCommand:
     """Remote command definition."""
 
-    def __init__(self, rcmd, name, params, ce_finished, **kwargs):
+    def __init__(self,
+                 rcmd: typing.Union[int, str],
+                 name: str,
+                 params: typing.List[str],
+                 ce_finished: typing.Union[int, str],
+                 **kwargs):
         """
         Initialize a remote command.
 
         You can manually set the secs-type of the id with the 'id_type' keyword argument.
 
         Custom parameters can be set with the keyword arguments,
         they will be passed to the GemEquipmentHandlers callback
@@ -41,14 +47,16 @@
         :type ce_finished: types supported by data item CEID
         """
         self.rcmd = rcmd
         self.name = name
         self.params = params
         self.ce_finished = ce_finished
 
+        self.id_type: typing.Type[Base]
+
         if isinstance(self.rcmd, int):
-            self.id_type = secsgem.secs.variables.U4
+            self.id_type = U4
         else:
-            self.id_type = secsgem.secs.variables.String
+            self.id_type = String
 
         for key, value in kwargs.items():
             setattr(self, key, value)
```

### Comparing `secsgem-0.2.0a2/secsgem/gem/status_variable.py` & `secsgem-0.2.0a3/secsgem/gem/status_variable.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/__init__.py` & `secsgem-0.2.0a3/secsgem/hsms/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/active_connection.py` & `secsgem-0.2.0a3/secsgem/hsms/active_connection.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/connection.py` & `secsgem-0.2.0a3/secsgem/hsms/connection.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/connectionmanager.py` & `secsgem-0.2.0a3/secsgem/hsms/connectionmanager.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/connectionstatemachine.py` & `secsgem-0.2.0a3/secsgem/hsms/connectionstatemachine.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/deselect_req_header.py` & `secsgem-0.2.0a3/secsgem/hsms/deselect_req_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/deselect_rsp_header.py` & `secsgem-0.2.0a3/secsgem/hsms/deselect_rsp_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/handler.py` & `secsgem-0.2.0a3/secsgem/hsms/handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Contains class to create model for hsms endpoints."""
-
-import random
-import threading
 import logging
 import queue
+import random
+import threading
+import typing
 
 import secsgem.common
 
 from .connection import HSMS_STYPES
 from .active_connection import HsmsActiveConnection
 from .passive_connection import HsmsPassiveConnection
 from .packet import HsmsPacket
@@ -79,28 +79,27 @@
 
             client.disable()
 
         """
         self._eventProducer = secsgem.common.EventProducer()
         self._eventProducer.targets += self
 
-        self._callback_handler = secsgem.common.CallbackHandler()
-        self._callback_handler.target = self
-
         self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
         self.communicationLogger = logging.getLogger("hsms_communication")
 
         self.address = address
         self.port = port
         self.active = active
         self.sessionID = session_id
         self.name = name
 
         self.connected = False
 
+        self._secs_decode = None
+
         # system id counter
         self.systemCounter = random.randint(0, (2 ** 32) - 1)
 
         # repeating linktest variables
         self.linktestTimer = None
         self.linktestTimeout = 30
 
@@ -131,17 +130,22 @@
 
     @property
     def events(self):
         """Property for event handling."""
         return self._eventProducer
 
     @property
-    def callbacks(self):
-        """Property for callback handling."""
-        return self._callback_handler
+    def secs_decode(self) -> typing.Optional[typing.Callable[[HsmsPacket], typing.Any]]:
+        """Get secs decode."""
+        return self._secs_decode
+
+    @secs_decode.setter
+    def secs_decode(self, value: typing.Optional[typing.Callable[[HsmsPacket], typing.Any]]):
+        """Get secs decode."""
+        self._secs_decode = value
 
     def get_next_system_counter(self):
         """
         Return the next System.
 
         :returns: System for the next command
         :rtype: integer
@@ -200,18 +204,14 @@
 
         :param data: event attributes
         :type data: object
         """
         # send event
         self.events.fire('hsms_selected', {'connection': self})
 
-        # notify hsms handler of selection
-        if hasattr(self, '_on_hsms_select') and callable(getattr(self, '_on_hsms_select')):
-            self._on_hsms_select()
-
     def _on_linktest_timer(self):
         """Linktest time timed out, so send linktest request."""
         # send linktest request and wait for response
         self.send_linktest_req()
 
         # restart the timer
         self._start_linktest_timer()
@@ -306,16 +306,16 @@
 
         :param packet: received data packet
         :type packet: :class:`secsgem.hsms.HsmsPacket`
         """
         if packet.header.sType > 0:
             self.__handle_hsms_requests(packet)
         else:
-            if hasattr(self, 'secs_decode') and callable(getattr(self, 'secs_decode')):
-                message = self.secs_decode(packet)
+            if callable(self._secs_decode):
+                message = self._secs_decode(packet)
                 self.communicationLogger.info("< %s\n%s", packet, message, extra=self._get_log_extra())
             else:
                 self.communicationLogger.info("< %s", packet, extra=self._get_log_extra())
 
             if not self.connectionState.is_CONNECTED_SELECTED():
                 self.logger.warning("received message when not selected")
 
@@ -326,20 +326,17 @@
 
                 return
 
             # someone is waiting for this message
             if packet.header.system in self._systemQueues:
                 # send packet to request sender
                 self._systemQueues[packet.header.system].put_nowait(packet)
-            # redirect packet to hsms handler
-            elif hasattr(self, '_on_hsms_packet_received') and callable(getattr(self, '_on_hsms_packet_received')):
-                self._on_hsms_packet_received(packet)
             # just log if nobody is interested
             else:
-                self.logger.warning("packet unhandled")
+                self.events.fire("hsms_packet_received", {'connection': self, 'packet': packet})
 
     def _get_queue_for_system(self, system_id):
         """
         Create a new queue to receive responses for a certain system.
 
         :param system_id: system id to watch
         :type system_id: int
```

### Comparing `secsgem-0.2.0a2/secsgem/hsms/header.py` & `secsgem-0.2.0a3/secsgem/hsms/header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/linktest_req_header.py` & `secsgem-0.2.0a3/secsgem/hsms/linktest_req_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/linktest_rsp_header.py` & `secsgem-0.2.0a3/secsgem/hsms/linktest_rsp_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/multi_passive_connection.py` & `secsgem-0.2.0a3/secsgem/hsms/multi_passive_connection.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/multi_passive_server.py` & `secsgem-0.2.0a3/secsgem/hsms/multi_passive_server.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/packet.py` & `secsgem-0.2.0a3/secsgem/hsms/packet.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/passive_connection.py` & `secsgem-0.2.0a3/secsgem/hsms/passive_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,12 +151,13 @@
 
             # make socket nonblocking
             self.sock.setblocking(0)
 
             # start the receiver thread
             self._start_receiver()
 
+            self.serverSock.shutdown(socket.SHUT_RDWR)
             self.serverSock.close()
 
             return
 
         self.stopServerThread = False
```

### Comparing `secsgem-0.2.0a2/secsgem/hsms/reject_req_header.py` & `secsgem-0.2.0a3/secsgem/hsms/reject_req_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/select_req_header.py` & `secsgem-0.2.0a3/secsgem/hsms/select_req_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/select_rsp_header.py` & `secsgem-0.2.0a3/secsgem/hsms/select_rsp_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/separate_req_header.py` & `secsgem-0.2.0a3/secsgem/hsms/separate_req_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/hsms/stream_function_header.py` & `secsgem-0.2.0a3/secsgem/hsms/stream_function_header.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/__init__.py` & `secsgem-0.2.0a3/secsgem/secs/__init__.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/acka.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/mid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 #####################################################################
-# acka.py
+# mid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ACKA data item."""
+"""MID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ACKA(DataItemBase):
+class MID(DataItemBase):
     """
-    Request success.
+    Material ID.
 
-       :Types: :class:`Boolean <secsgem.secs.variables.Boolean>`
-       :Length: 1
-
-    **Values**
-        +-------+---------+
-        | Value |         |
-        +=======+=========+
-        | True  | Success |
-        +-------+---------+
-        | False | Failed  |
-        +-------+---------+
+    :Types:
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 80
 
     **Used In Function**
-        - :class:`SecsS05F14 <secsgem.secs.functions.SecsS05F14>`
-        - :class:`SecsS05F15 <secsgem.secs.functions.SecsS05F15>`
-        - :class:`SecsS05F18 <secsgem.secs.functions.SecsS05F18>`
-        - :class:`SecsS16F02 <secsgem.secs.functions.SecsS16F02>`
-        - :class:`SecsS16F04 <secsgem.secs.functions.SecsS16F04>`
-        - :class:`SecsS16F06 <secsgem.secs.functions.SecsS16F06>`
-        - :class:`SecsS16F12 <secsgem.secs.functions.SecsS16F12>`
-        - :class:`SecsS16F14 <secsgem.secs.functions.SecsS16F14>`
-        - :class:`SecsS16F16 <secsgem.secs.functions.SecsS16F16>`
-        - :class:`SecsS16F18 <secsgem.secs.functions.SecsS16F18>`
-        - :class:`SecsS16F24 <secsgem.secs.functions.SecsS16F24>`
-        - :class:`SecsS16F26 <secsgem.secs.functions.SecsS16F26>`
-        - :class:`SecsS16F28 <secsgem.secs.functions.SecsS16F28>`
-        - :class:`SecsS16F30 <secsgem.secs.functions.SecsS16F30>`
-        - :class:`SecsS17F04 <secsgem.secs.functions.SecsS17F04>`
-        - :class:`SecsS17F08 <secsgem.secs.functions.SecsS17F08>`
-        - :class:`SecsS17F14 <secsgem.secs.functions.SecsS17F14>`
+        - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
+        - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
+        - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
+        - :class:`SecsS12F05 <secsgem.secs.functions.SecsS12F05>`
+        - :class:`SecsS12F07 <secsgem.secs.functions.SecsS12F07>`
+        - :class:`SecsS12F09 <secsgem.secs.functions.SecsS12F09>`
+        - :class:`SecsS12F11 <secsgem.secs.functions.SecsS12F11>`
+        - :class:`SecsS12F13 <secsgem.secs.functions.SecsS12F13>`
+        - :class:`SecsS12F14 <secsgem.secs.functions.SecsS12F14>`
+        - :class:`SecsS12F15 <secsgem.secs.functions.SecsS12F15>`
+        - :class:`SecsS12F16 <secsgem.secs.functions.SecsS12F16>`
+        - :class:`SecsS12F17 <secsgem.secs.functions.SecsS12F17>`
+        - :class:`SecsS12F18 <secsgem.secs.functions.SecsS12F18>`
 
     """
 
-    __type__ = variables.Boolean
-    __count__ = 1
+    __type__ = variables.Dynamic
+    __allowedtypes__ = [
+        variables.String,
+        variables.Binary
+    ]
+    __count__ = 80
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ackc10.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/orloc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,59 @@
 #####################################################################
-# ackc10.py
+# orloc.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ACKC10 data item."""
+"""ORLOC data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ACKC10(DataItemBase):
+class ORLOC(DataItemBase):
     """
-    Acknowledge code.
+    Origin location.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+------------------------+----------------------------------------------------------------+
-        | Value | Description            | Constant                                                       |
-        +=======+========================+================================================================+
-        | 0     | Accepted               | :const:`secsgem.secs.data_items.ACKC10.ACCEPTED`               |
-        +-------+------------------------+----------------------------------------------------------------+
-        | 1     | Will not be displayed  | :const:`secsgem.secs.data_items.ACKC10.NOT_DISPLAYED`          |
-        +-------+------------------------+----------------------------------------------------------------+
-        | 2     | Terminal not available | :const:`secsgem.secs.data_items.ACKC10.TERMINAL_NOT_AVAILABLE` |
-        +-------+------------------------+----------------------------------------------------------------+
-        | 3-63  | Other error            |                                                                |
-        +-------+------------------------+----------------------------------------------------------------+
+        +-------+---------------------+----------------------------------------------------+
+        | Value | Description         | Constant                                           |
+        +=======+=====================+====================================================+
+        | 0     | Center die of wafer | :const:`secsgem.secs.data_items.ORLOC.CENTER_DIE`  |
+        +-------+---------------------+----------------------------------------------------+
+        | 1     | Upper right         | :const:`secsgem.secs.data_items.ORLOC.UPPER_RIGHT` |
+        +-------+---------------------+----------------------------------------------------+
+        | 2     | Upper left          | :const:`secsgem.secs.data_items.ORLOC.UPPER_LEFT`  |
+        +-------+---------------------+----------------------------------------------------+
+        | 3     | Lower left          | :const:`secsgem.secs.data_items.ORLOC.LOWER_LEFT`  |
+        +-------+---------------------+----------------------------------------------------+
+        | 4     | Lower right         | :const:`secsgem.secs.data_items.ORLOC.LOWER_RIGHT` |
+        +-------+---------------------+----------------------------------------------------+
+        | 5-63  | Reserved, error     |                                                    |
+        +-------+---------------------+----------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS10F02 <secsgem.secs.functions.SecsS10F02>`
-        - :class:`SecsS10F04 <secsgem.secs.functions.SecsS10F04>`
-        - :class:`SecsS10F06 <secsgem.secs.functions.SecsS10F06>`
-        - :class:`SecsS10F10 <secsgem.secs.functions.SecsS10F10>`
+        - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
+        - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
+        - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ACCEPTED = 0
-    NOT_DISPLAYED = 1
-    TERMINAL_NOT_AVAILABLE = 2
+    CENTER_DIE = 0
+    UPPER_RIGHT = 1
+    UPPER_LEFT = 2
+    LOWER_LEFT = 3
+    LOWER_RIGHT = 4
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ackc5.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ackc5.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 """ACKC5 data item."""
 from .. import variables
 from .base import DataItemBase
 
 
 class ACKC5(DataItemBase):
     """
-    Acknowledge code.
+    Acknowledge code for stream 5.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+-------------------+-------------------------------------------------+
-        | Value | Description       | Constant                                        |
-        +=======+===================+=================================================+
-        | 0     | Accepted          | :const:`secsgem.secs.data_items.ACKC5.ACCEPTED` |
-        +-------+-------------------+-------------------------------------------------+
-        | 1-63  | Error             | :const:`secsgem.secs.data_items.ACKC5.ERROR`    |
-        +-------+-------------------+-------------------------------------------------+
+        +-------+-------------+-------------------------------------------------+
+        | Value | Description | Constant                                        |
+        +=======+=============+=================================================+
+        | 0     | Accepted    | :const:`secsgem.secs.data_items.ACKC5.ACCEPTED` |
+        +-------+-------------+-------------------------------------------------+
+        | 1-63  | Error       | :const:`secsgem.secs.data_items.ACKC5.ERROR`    |
+        +-------+-------------+-------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS05F02 <secsgem.secs.functions.SecsS05F02>`
         - :class:`SecsS05F04 <secsgem.secs.functions.SecsS05F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ackc6.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/commack.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 #####################################################################
-# ackc6.py
+# commack.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ACKC6 data item."""
+"""COMMACK data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ACKC6(DataItemBase):
+class COMMACK(DataItemBase):
     """
-    Acknowledge code.
+    Establish communications acknowledge.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+-------------------+-------------------------------------------------+
-        | Value | Description       | Constant                                        |
-        +=======+===================+============?====================================+
-        | 0     | Accepted          | :const:`secsgem.secs.data_items.ACKC6.ACCEPTED` |
-        +-------+-------------------+-------------------------------------------------+
-        | 1-63  | Error             | :const:`secsgem.secs.data_items.ACKC6.ERROR`    |
-        +-------+-------------------+-------------------------------------------------+
+        +-------+-------------------+---------------------------------------------------+
+        | Value | Description       | Constant                                          |
+        +=======+===================+===================================================+
+        | 0     | Accepted          | :const:`secsgem.secs.data_items.COMMACK.ACCEPTED` |
+        +-------+-------------------+---------------------------------------------------+
+        | 1     | Denied, Try Again | :const:`secsgem.secs.data_items.COMMACK.DENIED`   |
+        +-------+-------------------+---------------------------------------------------+
+        | 2-63  | Reserved          |                                                   |
+        +-------+-------------------+---------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS06F02 <secsgem.secs.functions.SecsS06F02>`
-        - :class:`SecsS06F04 <secsgem.secs.functions.SecsS06F04>`
-        - :class:`SecsS06F10 <secsgem.secs.functions.SecsS06F10>`
-        - :class:`SecsS06F12 <secsgem.secs.functions.SecsS06F12>`
-        - :class:`SecsS06F14 <secsgem.secs.functions.SecsS06F14>`
+        - :class:`SecsS01F14 <secsgem.secs.functions.SecsS01F14>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     ACCEPTED = 0
-    ERROR = 1
+    DENIED = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ackc7.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/limitack.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,66 @@
 #####################################################################
-# ackc7.py
+# limitack.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ACKC7 data item."""
+"""LIMITACK data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ACKC7(DataItemBase):
+class LIMITACK(DataItemBase):
     """
-    Acknowledge code.
+    Acknowledgement code for variable limit.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+------------------------+---------------------------------------------------------+
-        | Value | Description            | Constant                                                |
-        +=======+========================+=========================================================+
-        | 0     | Accepted               | :const:`secsgem.secs.data_items.ACKC7.ACCEPTED`         |
-        +-------+------------------------+---------------------------------------------------------+
-        | 1     | Permission not granted | :const:`secsgem.secs.data_items.ACKC7.NO_PERMISSION`    |
-        +-------+------------------------+---------------------------------------------------------+
-        | 2     | Length error           | :const:`secsgem.secs.data_items.ACKC7.LENGTH_ERROR`     |
-        +-------+------------------------+---------------------------------------------------------+
-        | 3     | Matrix overflow        | :const:`secsgem.secs.data_items.ACKC7.MATRIX_OVERFLOW`  |
-        +-------+------------------------+---------------------------------------------------------+
-        | 4     | PPID not found         | :const:`secsgem.secs.data_items.ACKC7.PPID_NOT_FOUND`   |
-        +-------+------------------------+---------------------------------------------------------+
-        | 5     | Mode unsupported       | :const:`secsgem.secs.data_items.ACKC7.MODE_UNSUPPORTED` |
-        +-------+------------------------+---------------------------------------------------------+
-        | 6     | Performed later        | :const:`secsgem.secs.data_items.ACKC7.PERFORMED_LATER`  |
-        +-------+------------------------+---------------------------------------------------------+
-        | 7-63  | Reserved               |                                                         |
-        +-------+------------------------+---------------------------------------------------------+
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | Value | Description                        | Constant                                                        |
+        +=======+====================================+=================================================================+
+        | 0     | OK                                 | :const:`secsgem.secs.data_items.LIMITACK.OK`                    |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 1     | LIMITID does not exist             | :const:`secsgem.secs.data_items.LIMITACK.LIMITID_UNKNOWN`       |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 2     | UPPERDB > LIMITMAX                 | :const:`secsgem.secs.data_items.LIMITACK.UPPERDB_MORE_LIMITMAX` |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 3     | LOWERDB < LIMITMIN                 | :const:`secsgem.secs.data_items.LIMITACK.LOWERDB_LESS_LIMITMIN` |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 4     | UPPERDB < LOWERDB                  | :const:`secsgem.secs.data_items.LIMITACK.UPPERDB_LESS_LOWERDB`  |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 5     | Illegal format UPPER-/LOWERDB      | :const:`secsgem.secs.data_items.LIMITACK.ILLEGAL_FORMAT`        |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 6     | Illegal ASCII value                | :const:`secsgem.secs.data_items.LIMITACK.ASCII_ILLEGAL`         |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 7     | Duplicate limit definition         | :const:`secsgem.secs.data_items.LIMITACK.DUPLICATE`             |
+        +-------+------------------------------------+-----------------------------------------------------------------+
+        | 8-63  | Reserved, equipment specific error |                                                                 |
+        +-------+------------------------------------+-----------------------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS07F04 <secsgem.secs.functions.SecsS07F04>`
-        - :class:`SecsS07F12 <secsgem.secs.functions.SecsS07F12>`
-        - :class:`SecsS07F14 <secsgem.secs.functions.SecsS07F14>`
-        - :class:`SecsS07F16 <secsgem.secs.functions.SecsS07F16>`
-        - :class:`SecsS07F18 <secsgem.secs.functions.SecsS07F18>`
-        - :class:`SecsS07F24 <secsgem.secs.functions.SecsS07F24>`
-        - :class:`SecsS07F32 <secsgem.secs.functions.SecsS07F32>`
-        - :class:`SecsS07F38 <secsgem.secs.functions.SecsS07F38>`
-        - :class:`SecsS07F40 <secsgem.secs.functions.SecsS07F40>`
-        - :class:`SecsS07F42 <secsgem.secs.functions.SecsS07F42>`
-        - :class:`SecsS07F44 <secsgem.secs.functions.SecsS07F44>`
+        - :class:`SecsS02F46 <secsgem.secs.functions.SecsS02F46>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ACCEPTED = 0
-    NO_PERMISSION = 1
-    LENGTH_ERROR = 2
-    MATRIX_OVERFLOW = 3
-    PPID_NOT_FOUND = 4
-    MODE_UNSUPPORTED = 5
-    PERFORMED_LATER = 6
+    OK = 0
+    LIMITID_UNKNOWN = 1
+    UPPERDB_MORE_LIMITMAX = 2
+    LOWERDB_LESS_LIMITMIN = 3
+    UPPERDB_LESS_LOWERDB = 4
+    ILLEGAL_FORMAT = 5
+    ASCII_ILLEGAL = 6
+    DUPLICATE = 7
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/alcd.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/alcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class ALCD(DataItemBase):
     """
     Alarm code byte.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+---------------------------+-----------------------------------------------------------------+
         | Value | Description               | Constant                                                        |
         +=======+===========================+=================================================================+
         | 0     | Not used                  |                                                                 |
         +-------+---------------------------+-----------------------------------------------------------------+
@@ -43,22 +43,23 @@
         +-------+---------------------------+-----------------------------------------------------------------+
         | 6     | Equipment status warning  | :const:`secsgem.secs.data_items.ALCD.EQUIPMENT_STATUS_WARNING`  |
         +-------+---------------------------+-----------------------------------------------------------------+
         | 7     | Attention flags           | :const:`secsgem.secs.data_items.ALCD.ATTENTION_FLAGS`           |
         +-------+---------------------------+-----------------------------------------------------------------+
         | 8     | Data integrity            | :const:`secsgem.secs.data_items.ALCD.DATA_INTEGRITY`            |
         +-------+---------------------------+-----------------------------------------------------------------+
-        | 9-63  | Other catogories          |                                                                 |
+        | 9-63  | Other catogeries          |                                                                 |
         +-------+---------------------------+-----------------------------------------------------------------+
         | 128   | Alarm set flag            | :const:`secsgem.secs.data_items.ALCD.ALARM_SET`                 |
         +-------+---------------------------+-----------------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS05F01 <secsgem.secs.functions.SecsS05F01>`
         - :class:`SecsS05F06 <secsgem.secs.functions.SecsS05F06>`
+        - :class:`SecsS05F08 <secsgem.secs.functions.SecsS05F08>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     PERSONAL_SAFETY = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/aled.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/aled.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class ALED(DataItemBase):
     """
     Alarm en-/disable code byte.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +---------+-------------+-----------------------------------------------+
         | Value   | Description | Constant                                      |
         +=========+=============+===============================================+
         | 0       | Disable     | :const:`secsgem.secs.data_items.ALED.DISABLE` |
         +---------+-------------+-----------------------------------------------+
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/alid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/rptid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 #####################################################################
-# alid.py
+# rptid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ALID data item."""
+"""RPTID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ALID(DataItemBase):
+class RPTID(DataItemBase):
     """
-    Alarm ID.
+    Report ID.
 
     :Types:
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS05F01 <secsgem.secs.functions.SecsS05F01>`
-        - :class:`SecsS05F03 <secsgem.secs.functions.SecsS05F03>`
-        - :class:`SecsS05F05 <secsgem.secs.functions.SecsS05F05>`
-        - :class:`SecsS05F06 <secsgem.secs.functions.SecsS05F06>`
+        - :class:`SecsS02F33 <secsgem.secs.functions.SecsS02F33>`
+        - :class:`SecsS02F35 <secsgem.secs.functions.SecsS02F35>`
+        - :class:`SecsS06F11 <secsgem.secs.functions.SecsS06F11>`
+        - :class:`SecsS06F16 <secsgem.secs.functions.SecsS06F16>`
+        - :class:`SecsS06F19 <secsgem.secs.functions.SecsS06F19>`
+        - :class:`SecsS06F21 <secsgem.secs.functions.SecsS06F21>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
         variables.U4,
         variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
-        variables.I8
+        variables.I8,
+        variables.String
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/altx.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/tid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #####################################################################
-# altx.py
+# tid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ALTX data item."""
+"""TID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ALTX(DataItemBase):
+class TID(DataItemBase):
     """
-    Alarm ID.
+    Terminal ID.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Used In Function**
-        - :class:`SecsS05F01 <secsgem.secs.functions.SecsS05F01>`
-        - :class:`SecsS05F06 <secsgem.secs.functions.SecsS05F06>`
+        - :class:`SecsS10F01 <secsgem.secs.functions.SecsS10F01>`
+        - :class:`SecsS10F03 <secsgem.secs.functions.SecsS10F03>`
 
     """
 
-    __type__ = variables.String
-    __count__ = 120
+    __type__ = variables.Binary
+    __count__ = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/attrdata.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/cmda.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,55 @@
 #####################################################################
-# attrdata.py
+# cmda.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ATTRDATA data item."""
+"""CMDA data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ATTRDATA(DataItemBase):
+class CMDA(DataItemBase):
     """
-    Object attribute value.
+    Command acknowledged code.
 
     :Types:
-       - :class:`Array <secsgem.secs.variables.Array>`
-       - :class:`Binary <secsgem.secs.variables.Binary>`
-       - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`F8 <secsgem.secs.variables.F8>`
-       - :class:`F4 <secsgem.secs.variables.F4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
-       - :class:`U2 <secsgem.secs.variables.U2>`
-       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+
+    **Values**
+        +-------+------------------------------------+-------------------------------------------------------+
+        | Value | Description                        | Constant                                              |
+        +=======+====================================+=======================================================+
+        | 0     | Completed or done                  | :const:`secsgem.secs.data_items.CMDA.DONE`            |
+        +-------+------------------------------------+-------------------------------------------------------+
+        | 1     | Command does not exist             | :const:`secsgem.secs.data_items.CMDA.COMMAND_UNKNOWN` |
+        +-------+------------------------------------+-------------------------------------------------------+
+        | 2     | Cannot perform now                 | :const:`secsgem.secs.data_items.CMDA.NOT_NOW`         |
+        +-------+------------------------------------+-------------------------------------------------------+
+        | 3-63  | Reserved, equipment specific error |                                                       |
+        +-------+------------------------------------+-------------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS01F20 <secsgem.secs.functions.SecsS01F20>`
-        - :class:`SecsS03F17 <secsgem.secs.functions.SecsS03F17>`
-        - :class:`SecsS03F18 <secsgem.secs.functions.SecsS03F18>`
-        - :class:`SecsS13F14 <secsgem.secs.functions.SecsS13F14>`
-        - :class:`SecsS13F16 <secsgem.secs.functions.SecsS13F16>`
-        - :class:`SecsS14F01 <secsgem.secs.functions.SecsS14F01>`
-        - :class:`SecsS14F02 <secsgem.secs.functions.SecsS14F02>`
-        - :class:`SecsS14F03 <secsgem.secs.functions.SecsS14F03>`
-        - :class:`SecsS14F04 <secsgem.secs.functions.SecsS14F04>`
-        - :class:`SecsS14F09 <secsgem.secs.functions.SecsS14F09>`
-        - :class:`SecsS14F10 <secsgem.secs.functions.SecsS14F10>`
-        - :class:`SecsS14F11 <secsgem.secs.functions.SecsS14F11>`
-        - :class:`SecsS14F12 <secsgem.secs.functions.SecsS14F12>`
-        - :class:`SecsS14F13 <secsgem.secs.functions.SecsS14F13>`
-        - :class:`SecsS14F14 <secsgem.secs.functions.SecsS14F14>`
-        - :class:`SecsS14F15 <secsgem.secs.functions.SecsS14F15>`
-        - :class:`SecsS14F16 <secsgem.secs.functions.SecsS14F16>`
-        - :class:`SecsS14F17 <secsgem.secs.functions.SecsS14F17>`
-        - :class:`SecsS14F18 <secsgem.secs.functions.SecsS14F18>`
-        - :class:`SecsS18F02 <secsgem.secs.functions.SecsS18F02>`
-        - :class:`SecsS18F03 <secsgem.secs.functions.SecsS18F03>`
+        - :class:`SecsS02F22 <secsgem.secs.functions.SecsS02F22>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
-        variables.Array,
-        variables.Boolean,
         variables.U1,
-        variables.U2,
-        variables.U4,
-        variables.U8,
-        variables.I1,
-        variables.I2,
-        variables.I4,
-        variables.I8,
-        variables.F4,
-        variables.F8,
-        variables.String,
-        variables.Binary
+        variables.I1
     ]
+
+    DONE = 0
+    COMMAND_UNKNOWN = 1
+    NOT_NOW = 2
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/attrreln.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/attrreln.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .base import DataItemBase
 
 
 class ATTRRELN(DataItemBase):
     """
     Attribute relation to attribute of object.
 
-       :Types: :class:`U1 <secsgem.secs.variables.U1>`
+    :Type: :class:`U1 <secsgem.secs.variables.U1>`
 
     **Values**
         +-------+-----------------------+------------------------------------------------------+
         | Value | Description           | Constant                                             |
         +=======+=======================+======================================================+
         | 0     | Equal to              | :const:`secsgem.secs.data_items.ATTRRELN.EQUAL`      |
         +-------+-----------------------+------------------------------------------------------+
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/base.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 # pylint: disable=non-parent-init-called
 """Data item base class."""
+import typing
 
 from .. import variables
 
 
 class DataItemMeta(type):
     """Meta class for data items."""
 
@@ -31,16 +32,16 @@
 class DataItemBase(metaclass=DataItemMeta):
     """
     Base class for data items.
 
     It provides type and output handling.
     """
 
-    __type__ = None
-    __allowedtypes__ = None
+    __type__: typing.Optional[typing.Type[variables.Base]] = None
+    __allowedtypes__: typing.Optional[typing.List[typing.Type[variables.Base]]] = None
     __count__ = -1
 
     def __init__(self, value=None):
         """
         Initialize a data item.
 
         :param value: Value of the data item
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/bcequ.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/nulbc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 #####################################################################
-# bcequ.py
+# nulbc.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""BCEQU data item."""
+"""NULBC data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class BCEQU(DataItemBase):
+class NULBC(DataItemBase):
     """
-    Bin code equivalents.
+    Column count in dies.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
        - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
+        - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
 
     __type__ = variables.Dynamic
-    __allowedtypes__ = [variables.U1, variables.String]
+    __allowedtypes__ = [
+        variables.U1,
+        variables.String
+    ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/binlt.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/binlt.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,22 +19,25 @@
 
 
 class BINLT(DataItemBase):
     """
     Bin list.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
        - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
         - :class:`SecsS12F07 <secsgem.secs.functions.SecsS12F07>`
         - :class:`SecsS12F09 <secsgem.secs.functions.SecsS12F09>`
         - :class:`SecsS12F11 <secsgem.secs.functions.SecsS12F11>`
         - :class:`SecsS12F14 <secsgem.secs.functions.SecsS12F14>`
         - :class:`SecsS12F16 <secsgem.secs.functions.SecsS12F16>`
         - :class:`SecsS12F18 <secsgem.secs.functions.SecsS12F18>`
 
     """
 
     __type__ = variables.Dynamic
-    __allowedtypes__ = [variables.U1, variables.String]
+    __allowedtypes__ = [
+        variables.U1,
+        variables.String
+    ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ceed.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ceed.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,26 @@
 from .base import DataItemBase
 
 
 class CEED(DataItemBase):
     """
     Collection event or trace enable/disable code.
 
-       :Types: :class:`Boolean <secsgem.secs.variables.Boolean>`
-       :Length: 1
+    :Type: :class:`Boolean <secsgem.secs.variables.Boolean>`
+    :Length: 1
 
     **Values**
         +-------+---------+
-        | Value | State   |
+        | Value |         |
         +=======+=========+
         | True  | Enable  |
         +-------+---------+
         | False | Disable |
         +-------+---------+
 
     **Used In Function**
         - :class:`SecsS02F37 <secsgem.secs.functions.SecsS02F37>`
-        - :class:`SecsS17F05 <secsgem.secs.functions.SecsS17F05>`
 
     """
 
     __type__ = variables.Boolean
     __count__ = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ceid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/dataid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 #####################################################################
-# ceid.py
+# dataid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""CEID data item."""
+"""DATAID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class CEID(DataItemBase):
+class DATAID(DataItemBase):
     """
-    Collection event ID.
+    Data ID.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
+        - :class:`SecsS02F33 <secsgem.secs.functions.SecsS02F33>`
         - :class:`SecsS02F35 <secsgem.secs.functions.SecsS02F35>`
-        - :class:`SecsS02F37 <secsgem.secs.functions.SecsS02F37>`
-        - :class:`SecsS06F03 <secsgem.secs.functions.SecsS06F03>`
+        - :class:`SecsS02F45 <secsgem.secs.functions.SecsS02F45>`
+        - :class:`SecsS02F49 <secsgem.secs.functions.SecsS02F49>`
+        - :class:`SecsS06F05 <secsgem.secs.functions.SecsS06F05>`
+        - :class:`SecsS06F07 <secsgem.secs.functions.SecsS06F07>`
         - :class:`SecsS06F08 <secsgem.secs.functions.SecsS06F08>`
-        - :class:`SecsS06F09 <secsgem.secs.functions.SecsS06F09>`
         - :class:`SecsS06F11 <secsgem.secs.functions.SecsS06F11>`
-        - :class:`SecsS06F13 <secsgem.secs.functions.SecsS06F13>`
-        - :class:`SecsS06F15 <secsgem.secs.functions.SecsS06F15>`
         - :class:`SecsS06F16 <secsgem.secs.functions.SecsS06F16>`
-        - :class:`SecsS06F17 <secsgem.secs.functions.SecsS06F17>`
-        - :class:`SecsS06F18 <secsgem.secs.functions.SecsS06F18>`
-        - :class:`SecsS17F05 <secsgem.secs.functions.SecsS17F05>`
-        - :class:`SecsS17F09 <secsgem.secs.functions.SecsS17F09>`
-        - :class:`SecsS17F10 <secsgem.secs.functions.SecsS17F10>`
-        - :class:`SecsS17F11 <secsgem.secs.functions.SecsS17F11>`
-        - :class:`SecsS17F12 <secsgem.secs.functions.SecsS17F12>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/colct.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/colct.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 
 class COLCT(DataItemBase):
     """
     Column count in dies.
 
     :Types:
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/commack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/rspack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #####################################################################
-# commack.py
+# rspack.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""COMMACK data item."""
+"""RSPACK data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class COMMACK(DataItemBase):
+class RSPACK(DataItemBase):
     """
-    Establish communications acknowledge.
+    Reset spooling acknowledge.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+-------------------+---------------------------------------------------+
-        | Value | Description       | Constant                                          |
-        +=======+===================+===================================================+
-        | 0     | Accepted          | :const:`secsgem.secs.data_items.COMMACK.ACCEPTED` |
-        +-------+-------------------+---------------------------------------------------+
-        | 1     | Denied, Try Again | :const:`secsgem.secs.data_items.COMMACK.DENIED`   |
-        +-------+-------------------+---------------------------------------------------+
-        | 2-63  | Reserved          |                                                   |
-        +-------+-------------------+---------------------------------------------------+
+        +-------+--------------------------------------+--------------------------------------------------+
+        | Value | Description                          | Constant                                         |
+        +=======+======================================+==================================================+
+        | 0     | Acknowledge, spooling setup accepted | :const:`secsgem.secs.data_items.RSPACK.ACK`      |
+        +-------+--------------------------------------+--------------------------------------------------+
+        | 1     | Spooling setup rejected              | :const:`secsgem.secs.data_items.RSPACK.REJECTED` |
+        +-------+--------------------------------------+--------------------------------------------------+
+        | 2-63  | Reserved                             |                                                  |
+        +-------+--------------------------------------+--------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS01F14 <secsgem.secs.functions.SecsS01F14>`
+        - :class:`SecsS02F44 <secsgem.secs.functions.SecsS02F44>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ACCEPTED = 0
-    DENIED = 1
+    ACK = 0
+    REJECTED = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/cpack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/cpack.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class CPACK(DataItemBase):
     """
     Command parameter acknowledge code.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+------------------------+-------------------------------------------------------------+
         | Value | Description            | Constant                                                    |
         +=======+========================+=============================================================+
         | 1     | Parameter name unknown | :const:`secsgem.secs.data_items.CPACK.PARAMETER_UNKNOWN`    |
         +-------+------------------------+-------------------------------------------------------------+
@@ -36,14 +36,16 @@
         | 3     | CPVAL format illegal   | :const:`secsgem.secs.data_items.CPACK.CPVAL_ILLEGAL_FORMAT` |
         +-------+------------------------+-------------------------------------------------------------+
         | 4-63  | Reserved               |                                                             |
         +-------+------------------------+-------------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS02F42 <secsgem.secs.functions.SecsS02F42>`
+        - :class:`SecsS02F50 <secsgem.secs.functions.SecsS02F50>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     PARAMETER_UNKNOWN = 1
     CPVAL_ILLEGAL_VALUE = 2
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/cpname.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/vid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 #####################################################################
-# cpname.py
+# vid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""CPNAME data item."""
+"""VID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class CPNAME(DataItemBase):
+class VID(DataItemBase):
     """
-    Command parameter name.
+    Variable ID.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS02F41 <secsgem.secs.functions.SecsS02F41>`
-        - :class:`SecsS02F42 <secsgem.secs.functions.SecsS02F42>`
-        - :class:`SecsS02F49 <secsgem.secs.functions.SecsS02F49>`
-        - :class:`SecsS02F50 <secsgem.secs.functions.SecsS02F50>`
-        - :class:`SecsS04F21 <secsgem.secs.functions.SecsS04F21>`
-        - :class:`SecsS04F29 <secsgem.secs.functions.SecsS04F29>`
-        - :class:`SecsS16F05 <secsgem.secs.functions.SecsS16F05>`
-        - :class:`SecsS16F27 <secsgem.secs.functions.SecsS16F27>`
+        - :class:`SecsS01F21 <secsgem.secs.functions.SecsS01F21>`
+        - :class:`SecsS01F22 <secsgem.secs.functions.SecsS01F22>`
+        - :class:`SecsS01F24 <secsgem.secs.functions.SecsS01F24>`
+        - :class:`SecsS02F33 <secsgem.secs.functions.SecsS02F33>`
+        - :class:`SecsS02F45 <secsgem.secs.functions.SecsS02F45>`
+        - :class:`SecsS02F46 <secsgem.secs.functions.SecsS02F46>`
+        - :class:`SecsS02F47 <secsgem.secs.functions.SecsS02F47>`
+        - :class:`SecsS02F48 <secsgem.secs.functions.SecsS02F48>`
+        - :class:`SecsS06F22 <secsgem.secs.functions.SecsS06F22>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/cpval.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ceid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,59 @@
 #####################################################################
-# cpval.py
+# ceid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""CPVAL data item."""
+"""CEID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class CPVAL(DataItemBase):
+class CEID(DataItemBase):
     """
-    Command parameter name.
+    Collection event ID.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
-       - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS02F41 <secsgem.secs.functions.SecsS02F41>`
-        - :class:`SecsS02F49 <secsgem.secs.functions.SecsS02F49>`
-        - :class:`SecsS04F21 <secsgem.secs.functions.SecsS04F21>`
-        - :class:`SecsS04F29 <secsgem.secs.functions.SecsS04F29>`
-        - :class:`SecsS16F05 <secsgem.secs.functions.SecsS16F05>`
-        - :class:`SecsS16F27 <secsgem.secs.functions.SecsS16F27>`
-        - :class:`SecsS18F13 <secsgem.secs.functions.SecsS18F13>`
+        - :class:`SecsS01F23 <secsgem.secs.functions.SecsS01F23>`
+        - :class:`SecsS01F24 <secsgem.secs.functions.SecsS01F24>`
+        - :class:`SecsS02F35 <secsgem.secs.functions.SecsS02F35>`
+        - :class:`SecsS02F37 <secsgem.secs.functions.SecsS02F37>`
+        - :class:`SecsS06F08 <secsgem.secs.functions.SecsS06F08>`
+        - :class:`SecsS06F11 <secsgem.secs.functions.SecsS06F11>`
+        - :class:`SecsS06F15 <secsgem.secs.functions.SecsS06F15>`
+        - :class:`SecsS06F16 <secsgem.secs.functions.SecsS06F16>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
-        variables.Boolean,
         variables.U1,
         variables.U2,
         variables.U4,
         variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
         variables.I8,
-        variables.String,
-        variables.Binary
+        variables.String
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/datalength.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/v.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 #####################################################################
-# datalength.py
+# v.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""DATALENGTH data item."""
+"""V data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class DATALENGTH(DataItemBase):
+class V(DataItemBase):
     """
-    Length of data to be sent.
+    Variable data.
 
     :Types:
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`Array <secsgem.secs.variables.Array>`
+       - :class:`Boolean <secsgem.secs.variables.Boolean>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`F4 <secsgem.secs.variables.F4>`
+       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
-        - :class:`SecsS02F39 <secsgem.secs.functions.SecsS02F39>`
-        - :class:`SecsS03F15 <secsgem.secs.functions.SecsS03F15>`
-        - :class:`SecsS03F29 <secsgem.secs.functions.SecsS03F29>`
-        - :class:`SecsS03F31 <secsgem.secs.functions.SecsS03F31>`
-        - :class:`SecsS04F25 <secsgem.secs.functions.SecsS04F25>`
-        - :class:`SecsS06F05 <secsgem.secs.functions.SecsS06F05>`
-        - :class:`SecsS13F11 <secsgem.secs.functions.SecsS13F11>`
-        - :class:`SecsS14F23 <secsgem.secs.functions.SecsS14F23>`
-        - :class:`SecsS16F01 <secsgem.secs.functions.SecsS16F01>`
-        - :class:`SecsS16F11 <secsgem.secs.functions.SecsS16F11>`
-        - :class:`SecsS18F05 <secsgem.secs.functions.SecsS18F05>`
-        - :class:`SecsS18F07 <secsgem.secs.functions.SecsS18F07>`
-        - :class:`SecsS19F19 <secsgem.secs.functions.SecsS19F19>`
+        - :class:`SecsS06F11 <secsgem.secs.functions.SecsS06F11>`
+        - :class:`SecsS06F16 <secsgem.secs.functions.SecsS06F16>`
+        - :class:`SecsS06F20 <secsgem.secs.functions.SecsS06F20>`
+        - :class:`SecsS06F22 <secsgem.secs.functions.SecsS06F22>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
+        variables.Array,
+        variables.Boolean,
         variables.U1,
         variables.U2,
         variables.U4,
         variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
-        variables.I8
+        variables.I8,
+        variables.F4,
+        variables.F8,
+        variables.String,
+        variables.Binary
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/datlc.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/datlc.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .base import DataItemBase
 
 
 class DATLC(DataItemBase):
     """
     Data location.
 
-       :Types: :class:`U1 <secsgem.secs.variables.U1>`
+    :Type: :class:`U1 <secsgem.secs.variables.U1>`
 
     **Used In Function**
         - :class:`SecsS12F19 <secsgem.secs.functions.SecsS12F19>`
 
     """
 
     __type__ = variables.U1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/drack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/drack.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class DRACK(DataItemBase):
     """
     Define report acknowledge code.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+-------------------------------+-----------------------------------------------------------+
         | Value | Description                   | Constant                                                  |
         +=======+===============================+===========================================================+
         | 0     | Acknowledge                   | :const:`secsgem.secs.data_items.DRACK.ACK`                |
         +-------+-------------------------------+-----------------------------------------------------------+
@@ -40,14 +40,15 @@
         | 4     | Denied, VID doesn't exist     | :const:`secsgem.secs.data_items.DRACK.VID_UNKNOWN`        |
         +-------+-------------------------------+-----------------------------------------------------------+
         | 5-63  | Reserved, other errors        |                                                           |
         +-------+-------------------------------+-----------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS02F34 <secsgem.secs.functions.SecsS02F34>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     ACK = 0
     INSUFFICIENT_SPACE = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/dsid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/dsid.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,38 +9,36 @@
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""DSIG data item."""
+"""DSID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
 class DSID(DataItemBase):
     """
     Data set ID.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS06F03 <secsgem.secs.functions.SecsS06F03>`
         - :class:`SecsS06F08 <secsgem.secs.functions.SecsS06F08>`
-        - :class:`SecsS06F09 <secsgem.secs.functions.SecsS06F09>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/dutms.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/dutms.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 from .base import DataItemBase
 
 
 class DUTMS(DataItemBase):
     """
     Die units of measure.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/dvname.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/dvname.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 
 
 class DVNAME(DataItemBase):
     """
     Data value name.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS06F03 <secsgem.secs.functions.SecsS06F03>`
         - :class:`SecsS06F08 <secsgem.secs.functions.SecsS06F08>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/dvval.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/attrdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 #####################################################################
-# dvval.py
+# attrdata.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""DVVAL data item."""
+"""ATTRDATA data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class DVVAL(DataItemBase):
+class ATTRDATA(DataItemBase):
     """
-    Data value.
+    Object attribute value.
 
     :Types:
        - :class:`Array <secsgem.secs.variables.Array>`
-       - :class:`Binary <secsgem.secs.variables.Binary>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`U2 <secsgem.secs.variables.U2>`
+       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`F4 <secsgem.secs.variables.F4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
-       - :class:`U1 <secsgem.secs.variables.U1>`
-       - :class:`U2 <secsgem.secs.variables.U2>`
-       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
-        - :class:`SecsS06F03 <secsgem.secs.functions.SecsS06F03>`
-        - :class:`SecsS06F08 <secsgem.secs.functions.SecsS06F08>`
-        - :class:`SecsS06F09 <secsgem.secs.functions.SecsS06F09>`
+        - :class:`SecsS14F01 <secsgem.secs.functions.SecsS14F01>`
+        - :class:`SecsS14F02 <secsgem.secs.functions.SecsS14F02>`
+        - :class:`SecsS14F03 <secsgem.secs.functions.SecsS14F03>`
+        - :class:`SecsS14F04 <secsgem.secs.functions.SecsS14F04>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.Array,
         variables.Boolean,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/eac.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/eac.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,35 @@
 from .base import DataItemBase
 
 
 class EAC(DataItemBase):
     """
     Equipment acknowledge code.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+---------------------------------+--------------------------------------------------------+
-        | Value | Description                     | Constant                                               |
-        +=======+=================================+========================================================+
-        | 0     | Acknowledge                     | :const:`secsgem.secs.data_items.EAC.ACK`               |
-        +-------+---------------------------------+--------------------------------------------------------+
-        | 1     | Denied, not all constants exist | :const:`secsgem.secs.data_items.EAC.INVALID_CONSTANT`  |
-        +-------+---------------------------------+--------------------------------------------------------+
-        | 2     | Denied, busy                    | :const:`secsgem.secs.data_items.EAC.BUSY`              |
-        +-------+---------------------------------+--------------------------------------------------------+
-        | 3     | Denied, constant out of range   | :const:`secsgem.secs.data_items.EAC.OUT_OF_RANGE`      |
-        +-------+---------------------------------+--------------------------------------------------------+
-        | 4-63  | Reserved, equipment specific    |                                                        |
-        +-------+---------------------------------+--------------------------------------------------------+
+        +-------+---------------------------------+-------------------------------------------------------+
+        | Value | Description                     | Constant                                              |
+        +=======+=================================+=======================================================+
+        | 0     | Acknowledge                     | :const:`secsgem.secs.data_items.EAC.ACK`              |
+        +-------+---------------------------------+-------------------------------------------------------+
+        | 1     | Denied, not all constants exist | :const:`secsgem.secs.data_items.EAC.INVALID_CONSTANT` |
+        +-------+---------------------------------+-------------------------------------------------------+
+        | 2     | Denied, busy                    | :const:`secsgem.secs.data_items.EAC.BUSY`             |
+        +-------+---------------------------------+-------------------------------------------------------+
+        | 3     | Denied, constant out of range   | :const:`secsgem.secs.data_items.EAC.OUT_OF_RANGE`     |
+        +-------+---------------------------------+-------------------------------------------------------+
+        | 4-63  | Reserved, equipment specific    |                                                       |
+        +-------+---------------------------------+-------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS02F16 <secsgem.secs.functions.SecsS02F16>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     ACK = 0
     INVALID_CONSTANT = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ecdef.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ecdef.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 
 
 class ECDEF(DataItemBase):
     """
     Equipment constant default value.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
        - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
        - :class:`F8 <secsgem.secs.variables.F8>`
        - :class:`F4 <secsgem.secs.variables.F4>`
        - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
         - :class:`SecsS02F30 <secsgem.secs.functions.SecsS02F30>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.Boolean,
         variables.I8,
         variables.I1,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ecid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ecid.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 
 
 class ECID(DataItemBase):
     """
     Equipment constant ID.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
         - :class:`SecsS02F13 <secsgem.secs.functions.SecsS02F13>`
         - :class:`SecsS02F15 <secsgem.secs.functions.SecsS02F15>`
         - :class:`SecsS02F29 <secsgem.secs.functions.SecsS02F29>`
         - :class:`SecsS02F30 <secsgem.secs.functions.SecsS02F30>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
         variables.U4,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ecmax.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ecmax.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 
 
 class ECMAX(DataItemBase):
     """
     Equipment constant maximum value.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
        - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
        - :class:`F8 <secsgem.secs.variables.F8>`
        - :class:`F4 <secsgem.secs.variables.F4>`
        - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
         - :class:`SecsS02F30 <secsgem.secs.functions.SecsS02F30>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.Boolean,
         variables.I8,
         variables.I1,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ecmin.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ecmin.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 
 
 class ECMIN(DataItemBase):
     """
     Equipment constant minimum value.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
        - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
        - :class:`F8 <secsgem.secs.variables.F8>`
        - :class:`F4 <secsgem.secs.variables.F4>`
        - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
         - :class:`SecsS02F30 <secsgem.secs.functions.SecsS02F30>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.Boolean,
         variables.I8,
         variables.I1,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ecname.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/cename.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #####################################################################
-# ecname.py
+# cename.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ECNAME data item."""
+"""CENAME data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ECNAME(DataItemBase):
+class CENAME(DataItemBase):
     """
-    Equipment constant name.
+    Collection event Name.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS02F30 <secsgem.secs.functions.SecsS02F30>`
+        - :class:`SecsS01F24 <secsgem.secs.functions.SecsS01F24>`
+
     """
 
     __type__ = variables.String
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ecv.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/cepval.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 #####################################################################
-# ecv.py
+# cepval.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ECV data item."""
+"""CEPVAL data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ECV(DataItemBase):
+class CEPVAL(DataItemBase):
     """
-    Equipment constant value.
+    Command enhanced parameter value.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
+       - :class:`Array <secsgem.secs.variables.Array>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`U2 <secsgem.secs.variables.U2>`
+       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`F4 <secsgem.secs.variables.F4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
-       - :class:`U1 <secsgem.secs.variables.U1>`
-       - :class:`U2 <secsgem.secs.variables.U2>`
-       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
-        - :class:`SecsS02F14 <secsgem.secs.functions.SecsS02F14>`
-        - :class:`SecsS02F15 <secsgem.secs.functions.SecsS02F15>`
+        - :class:`SecsS02F49 <secsgem.secs.functions.SecsS02F49>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.Array,
         variables.Boolean,
-        variables.I8,
+        variables.U1,
+        variables.U2,
+        variables.U4,
+        variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
-        variables.F8,
+        variables.I8,
         variables.F4,
-        variables.U8,
-        variables.U1,
-        variables.U2,
-        variables.U4,
+        variables.F8,
         variables.String,
         variables.Binary
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/edid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/trid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 #####################################################################
-# edid.py
+# trid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""EDID data item."""
+"""TRID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class EDID(DataItemBase):
+class TRID(DataItemBase):
     """
-    Expected data identification.
+    Trace request ID.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS09F13 <secsgem.secs.functions.SecsS09F13>`
+        - :class:`SecsS02F23 <secsgem.secs.functions.SecsS02F23>`
+        - :class:`SecsS06F01 <secsgem.secs.functions.SecsS06F01>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
-        variables.U1,
-        variables.U2,
-        variables.U4,
-        variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
         variables.I8,
-        variables.String,
-        variables.Binary
+        variables.U1,
+        variables.U2,
+        variables.U4,
+        variables.U8,
+        variables.String
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/erack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/maper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 #####################################################################
-# erack.py
+# maper.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ERACK data item."""
+"""MAPER data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ERACK(DataItemBase):
+class MAPER(DataItemBase):
     """
-    Enable/disable event report acknowledge.
+    Map error.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+----------------------------+-----------------------------------------------------+
-        | Value | Description                | Constant                                            |
-        +=======+============================+=====================================================+
-        | 0     | Accepted                   | :const:`secsgem.secs.data_items.ERACK.ACCEPTED`     |
-        +-------+----------------------------+-----------------------------------------------------+
-        | 1     | Denied, CEID doesn't exist | :const:`secsgem.secs.data_items.ERACK.CEID_UNKNOWN` |
-        +-------+----------------------------+-----------------------------------------------------+
-        | 2-63  | Reserved                   |                                                     |
-        +-------+----------------------------+-----------------------------------------------------+
+        +-------+---------------+-----------------------------------------------------+
+        | Value | Description   | Constant                                            |
+        +=======+===============+=====================================================+
+        | 0     | ID not found  | :const:`secsgem.secs.data_items.MAPER.ID_UNKNOWN`   |
+        +-------+---------------+-----------------------------------------------------+
+        | 1     | Invalid data  | :const:`secsgem.secs.data_items.MAPER.INVALID_DATA` |
+        +-------+---------------+-----------------------------------------------------+
+        | 2     | Format error  | :const:`secsgem.secs.data_items.MAPER.FORMAT_ERROR` |
+        +-------+---------------+-----------------------------------------------------+
+        | 3-63  | Invalid error |                                                     |
+        +-------+---------------+-----------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS02F38 <secsgem.secs.functions.SecsS02F38>`
+        - :class:`SecsS12F19 <secsgem.secs.functions.SecsS12F19>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ACCEPTED = 0
-    CEID_UNKNOWN = 1
+    ID_UNKNOWN = 0
+    INVALID_DATA = 1
+    FORMAT_ERROR = 2
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/exid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/exid.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 from .base import DataItemBase
 
 
 class EXID(DataItemBase):
     """
     Exception identifier.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
+    :Length: 20
 
     **Used In Function**
         - :class:`SecsS05F09 <secsgem.secs.functions.SecsS05F09>`
         - :class:`SecsS05F11 <secsgem.secs.functions.SecsS05F11>`
         - :class:`SecsS05F13 <secsgem.secs.functions.SecsS05F13>`
         - :class:`SecsS05F14 <secsgem.secs.functions.SecsS05F14>`
         - :class:`SecsS05F15 <secsgem.secs.functions.SecsS05F15>`
         - :class:`SecsS05F17 <secsgem.secs.functions.SecsS05F17>`
         - :class:`SecsS05F18 <secsgem.secs.functions.SecsS05F18>`
+
     """
 
     __type__ = variables.String
     __count__ = 20
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/exmessage.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/exrecvra.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 #####################################################################
-# exmessage.py
+# exrecvra.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""EXMESSAGE data item."""
+"""EXRECVRA data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class EXMESSAGE(DataItemBase):
+class EXRECVRA(DataItemBase):
     """
-    Exception message.
+    Exception recovery action.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
+    :Length: 40
 
     **Used In Function**
         - :class:`SecsS05F09 <secsgem.secs.functions.SecsS05F09>`
-        - :class:`SecsS05F11 <secsgem.secs.functions.SecsS05F11>`
+        - :class:`SecsS05F13 <secsgem.secs.functions.SecsS05F13>`
+
     """
 
     __type__ = variables.String
+    __count__ = 40
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/exrecvra.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/timestamp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #####################################################################
-# exrecvra.py
+# timestamp.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""EXRECVRA data item."""
+"""TIMESTAMP data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class EXRECVRA(DataItemBase):
+class TIMESTAMP(DataItemBase):
     """
-    Exception recovery action.
+    Timestamp.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
+    :Length: 32
 
     **Used In Function**
         - :class:`SecsS05F09 <secsgem.secs.functions.SecsS05F09>`
-        - :class:`SecsS05F13 <secsgem.secs.functions.SecsS05F13>`
+        - :class:`SecsS05F11 <secsgem.secs.functions.SecsS05F11>`
+        - :class:`SecsS05F15 <secsgem.secs.functions.SecsS05F15>`
+
     """
 
     __type__ = variables.String
-    __count__ = 40
+    __count__ = 32
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/extype.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/attrid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 #####################################################################
-# extype.py
+# attrid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""EXTYPE data item."""
+"""ATTRID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class EXTYPE(DataItemBase):
+class ATTRID(DataItemBase):
     """
-    Exception type.
+    Object attribute identifier.
 
     :Types:
+       - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`U2 <secsgem.secs.variables.U2>`
+       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS05F09 <secsgem.secs.functions.SecsS05F09>`
-        - :class:`SecsS05F11 <secsgem.secs.functions.SecsS05F11>`
         - :class:`SecsS14F01 <secsgem.secs.functions.SecsS14F01>`
         - :class:`SecsS14F02 <secsgem.secs.functions.SecsS14F02>`
-        - :class:`SecsS14F08 <secsgem.secs.functions.SecsS14F08>`
+        - :class:`SecsS14F03 <secsgem.secs.functions.SecsS14F03>`
+        - :class:`SecsS14F04 <secsgem.secs.functions.SecsS14F04>`
+
     """
 
-    __type__ = variables.String
+    __type__ = variables.Dynamic
+    __allowedtypes__ = [
+        variables.U1,
+        variables.U2,
+        variables.U4,
+        variables.U8,
+        variables.String
+    ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ffrot.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ffrot.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class FFROT(DataItemBase):
     """
     Film frame rotation.
 
     In degrees from the bottom CW. (Bottom equals zero degrees.) Zero length indicates not used.
 
-       :Types: :class:`U2 <secsgem.secs.variables.U2>`
+    :Type: :class:`U2 <secsgem.secs.variables.U2>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/fnloc.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/fnloc.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class FNLOC(DataItemBase):
     """
     Flat/notch location.
 
     In degrees from the bottom CW. (Bottom equals zero degrees.) Zero length indicates not used.
 
-       :Types: :class:`U2 <secsgem.secs.variables.U2>`
+    :Type: :class:`U2 <secsgem.secs.variables.U2>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/grant5.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/grant6.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #####################################################################
-# grant5.py
+# grant6.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""GRANT5 data item."""
+"""GRANT6 data item."""
 from .. import variables
 from .base import DataItemBase
 
 
 class GRANT6(DataItemBase):
     """
     Permission to send.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+----------------+--------------------------------------------------------+
         | Value | Description    | Constant                                               |
         +=======+================+========================================================+
         | 0     | Granted        | :const:`secsgem.secs.data_items.GRANT6.GRANTED`        |
         +-------+----------------+--------------------------------------------------------+
@@ -36,14 +36,15 @@
         | 2     | Not interested | :const:`secsgem.secs.data_items.GRANT6.NOT_INTERESTED` |
         +-------+----------------+--------------------------------------------------------+
         | 3-63  | Other error    |                                                        |
         +-------+----------------+--------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS06F06 <secsgem.secs.functions.SecsS06F06>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     GRANTED = 0
     BUSY = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/grnt1.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/grnt1.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class GRNT1(DataItemBase):
     """
     Grant code.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+-----------------------+-----------------------------------------------------------+
         | Value | Description           | Constant                                                  |
         +=======+=======================+===========================================================+
         | 0     | Acknowledge           | :const:`secsgem.secs.data_items.GRNT1.ACK`                |
         +-------+-----------------------+-----------------------------------------------------------+
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/hcack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/hcack.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class HCACK(DataItemBase):
     """
     Host command parameter acknowledge code.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+--------------------------------+-------------------------------------------------------------+
         | Value | Description                    | Constant                                                    |
         +=======+================================+=============================================================+
         | 0     | Acknowledge                    | :const:`secsgem.secs.data_items.HCACK.ACK`                  |
         +-------+--------------------------------+-------------------------------------------------------------+
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/idtyp.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/idtyp.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class IDTYP(DataItemBase):
     """
     ID type.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+-------------------+-------------------------------------------------------+
         | Value | Description       | Constant                                              |
         +=======+===================+=======================================================+
         | 0     | Wafer ID          | :const:`secsgem.secs.data_items.IDTYP.WAFER`          |
         +-------+-------------------+-------------------------------------------------------+
@@ -38,15 +38,15 @@
         | 3-63  | Reserved, error   |                                                       |
         +-------+-------------------+-------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
-        - :class:`SecsS12F05 <secsgem.secs.functions.SecsS12F06>`
+        - :class:`SecsS12F05 <secsgem.secs.functions.SecsS12F05>`
         - :class:`SecsS12F07 <secsgem.secs.functions.SecsS12F07>`
         - :class:`SecsS12F09 <secsgem.secs.functions.SecsS12F09>`
         - :class:`SecsS12F11 <secsgem.secs.functions.SecsS12F11>`
         - :class:`SecsS12F13 <secsgem.secs.functions.SecsS12F13>`
         - :class:`SecsS12F14 <secsgem.secs.functions.SecsS12F14>`
         - :class:`SecsS12F15 <secsgem.secs.functions.SecsS12F15>`
         - :class:`SecsS12F16 <secsgem.secs.functions.SecsS12F16>`
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/length.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/length.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,25 @@
 
 
 class LENGTH(DataItemBase):
     """
     Service/process program length.
 
     :Types:
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
 
     **Used In Function**
-        - :class:`SecsS02F01 <secsgem.secs.functions.SecsS02F01>`
         - :class:`SecsS07F01 <secsgem.secs.functions.SecsS07F01>`
-        - :class:`SecsS07F29 <secsgem.secs.functions.SecsS07F29>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/lrack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/lrack.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class LRACK(DataItemBase):
     """
     Link report acknowledge code.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+-----------------------------+-----------------------------------------------------------+
         | Value | Description                 | Constant                                                  |
         +=======+=============================+===========================================================+
         | 0     | Acknowledge                 | :const:`secsgem.secs.data_items.LRACK.ACK`                |
         +-------+-----------------------------+-----------------------------------------------------------+
@@ -42,14 +42,15 @@
         | 5     | Denied, RPTID doesn't exist | :const:`secsgem.secs.data_items.LRACK.RPTID_UNKNOWN`      |
         +-------+-----------------------------+-----------------------------------------------------------+
         | 6-63  | Reserved, other errors      |                                                           |
         +-------+-----------------------------+-----------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS02F36 <secsgem.secs.functions.SecsS02F36>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     ACK = 0
     INSUFFICIENT_SPACE = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/maper.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/mapft.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 #####################################################################
-# maper.py
+# mapft.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""MAPER data item."""
+"""MAPFT data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class MAPER(DataItemBase):
+class MAPFT(DataItemBase):
     """
-    Map error.
+    Map data format.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+---------------+-----------------------------------------------------+
-        | Value | Description   | Constant                                            |
-        +=======+===============+=====================================================+
-        | 0     | ID not found  | :const:`secsgem.secs.data_items.MAPER.ID_UNKNOWN`   |
-        +-------+---------------+-----------------------------------------------------+
-        | 1     | Invalid data  | :const:`secsgem.secs.data_items.MAPER.INVALID_DATA` |
-        +-------+---------------+-----------------------------------------------------+
-        | 2     | Format error  | :const:`secsgem.secs.data_items.MAPER.FORMAT_ERROR` |
-        +-------+---------------+-----------------------------------------------------+
-        | 3-63  | Invalid error |                                                     |
-        +-------+---------------+-----------------------------------------------------+
+        +-------+-------------------+---------------------------------------------------+
+        | Value | Description       | Constant                                          |
+        +=======+===================+===================================================+
+        | 0     | Row format        | :const:`secsgem.secs.data_items.MAPFT.ROW`        |
+        +-------+-------------------+---------------------------------------------------+
+        | 1     | Array format      | :const:`secsgem.secs.data_items.MAPFT.ARRAY`      |
+        +-------+-------------------+---------------------------------------------------+
+        | 2     | Coordinate format | :const:`secsgem.secs.data_items.MAPFT.COORDINATE` |
+        +-------+-------------------+---------------------------------------------------+
+        | 3-63  | Error             |                                                   |
+        +-------+-------------------+---------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS12F19 <secsgem.secs.functions.SecsS12F19>`
+        - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
+        - :class:`SecsS12F05 <secsgem.secs.functions.SecsS12F05>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ID_UNKNOWN = 0
-    INVALID_DATA = 1
-    FORMAT_ERROR = 2
+    ROW = 0
+    ARRAY = 1
+    COORDINATE = 2
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/mapft.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/mdack.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #####################################################################
-# mapft.py
+# mdack.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""MAPFT data item."""
+"""MDACK data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class MAPFT(DataItemBase):
+class MDACK(DataItemBase):
     """
-    Map data format.
+    Map data acknowledge.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+-------------------+---------------------------------------------------+
-        | Value | Description       | Constant                                          |
-        +=======+===================+===================================================+
-        | 0     | Row format        | :const:`secsgem.secs.data_items.MAPFT.ROW`        |
-        +-------+-------------------+---------------------------------------------------+
-        | 1     | Array format      | :const:`secsgem.secs.data_items.MAPFT.ARRAY`      |
-        +-------+-------------------+---------------------------------------------------+
-        | 2     | Coordinate format | :const:`secsgem.secs.data_items.MAPFT.COORDINATE` |
-        +-------+-------------------+---------------------------------------------------+
-        | 3-63  | Error             |                                                   |
-        +-------+-------------------+---------------------------------------------------+
+        +-------+-------------------+-----------------------------------------------------+
+        | Value | Description       | Constant                                            |
+        +=======+===================+=====================================================+
+        | 0     | Map received      | :const:`secsgem.secs.data_items.MDACK.ACK`          |
+        +-------+-------------------+-----------------------------------------------------+
+        | 1     | Format error      | :const:`secsgem.secs.data_items.MDACK.FORMAT_ERROR` |
+        +-------+-------------------+-----------------------------------------------------+
+        | 2     | No ID match       | :const:`secsgem.secs.data_items.MDACK.UNKNOWN_ID`   |
+        +-------+-------------------+-----------------------------------------------------+
+        | 3     | Abort/discard map | :const:`secsgem.secs.data_items.MDACK.ABORT_MAP`    |
+        +-------+-------------------+-----------------------------------------------------+
+        | 4-63  | Reserved, error   |                                                     |
+        +-------+-------------------+-----------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
-        - :class:`SecsS12F05 <secsgem.secs.functions.SecsS12F05>`
+        - :class:`SecsS12F08 <secsgem.secs.functions.SecsS12F08>`
+        - :class:`SecsS12F10 <secsgem.secs.functions.SecsS12F10>`
+        - :class:`SecsS12F12 <secsgem.secs.functions.SecsS12F12>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ROW = 0
-    ARRAY = 1
-    COORDINATE = 2
+    ACK = 0
+    FORMAT_ERROR = 1
+    UNKNOWN_ID = 2
+    ABORT_MAP = 3
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/mdack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/strack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,52 @@
 #####################################################################
-# mdack.py
+# strack.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""MDACK data item."""
+"""STRACK data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class MDACK(DataItemBase):
+class STRACK(DataItemBase):
     """
-    Map data acknowledge.
+    Spool stream acknowledge.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+-------------------+-----------------------------------------------------+
-        | Value | Description       | Constant                                            |
-        +=======+===================+=====================================================+
-        | 0     | Map received      | :const:`secsgem.secs.data_items.MDACK.ACK`          |
-        +-------+-------------------+-----------------------------------------------------+
-        | 1     | Format error      | :const:`secsgem.secs.data_items.MDACK.FORMAT_ERROR` |
-        +-------+-------------------+-----------------------------------------------------+
-        | 2     | No ID match       | :const:`secsgem.secs.data_items.MDACK.UNKNOWN_ID`   |
-        +-------+-------------------+-----------------------------------------------------+
-        | 3     | Abort/discard map | :const:`secsgem.secs.data_items.MDACK.ABORT_MAP`    |
-        +-------+-------------------+-----------------------------------------------------+
-        | 4-63  | Reserved, error   |                                                     |
-        +-------+-------------------+-----------------------------------------------------+
+        +-------+------------------------------------+----------------------------------------------------------+
+        | Value | Description                        | Constant                                                 |
+        +=======+====================================+==========================================================+
+        | 1     | Spooling not allowed for stream    | :const:`secsgem.secs.data_items.STRACK.NOT_ALLOWED`      |
+        +-------+------------------------------------+----------------------------------------------------------+
+        | 2     | Stream unknown                     | :const:`secsgem.secs.data_items.STRACK.STREAM_UNKNOWN`   |
+        +-------+------------------------------------+----------------------------------------------------------+
+        | 3     | Unknown function for stream        | :const:`secsgem.secs.data_items.STRACK.FUNCTION_UNKNOWN` |
+        +-------+------------------------------------+----------------------------------------------------------+
+        | 4     | Secondary function for this stream | :const:`secsgem.secs.data_items.STRACK.SECONDARY`        |
+        +-------+------------------------------------+----------------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS12F08 <secsgem.secs.functions.SecsS12F08>`
-        - :class:`SecsS12F10 <secsgem.secs.functions.SecsS12F10>`
-        - :class:`SecsS12F12 <secsgem.secs.functions.SecsS12F12>`
+        - :class:`SecsS02F44 <secsgem.secs.functions.SecsS02F44>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ACK = 0
-    FORMAT_ERROR = 1
-    UNKNOWN_ID = 2
-    ABORT_MAP = 3
+    NOT_ALLOWED = 1
+    STREAM_UNKNOWN = 2
+    FUNCTION_UNKNOWN = 3
+    SECONDARY = 4
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/mdln.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ppid.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 #####################################################################
-# mdln.py
+# ppid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""MDLN data item."""
+"""PPID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class MDLN(DataItemBase):
+class PPID(DataItemBase):
     """
-    Equipment model type.
+    Process program ID.
 
     :Types:
        - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 120
 
     **Used In Function**
-        - :class:`SecsS01F02 <secsgem.secs.functions.SecsS01F02>`
-        - :class:`SecsS01F13 <secsgem.secs.functions.SecsS01F13>`
-        - :class:`SecsS01F14 <secsgem.secs.functions.SecsS01F14>`
-        - :class:`SecsS07F22 <secsgem.secs.functions.SecsS07F22>`
-        - :class:`SecsS07F23 <secsgem.secs.functions.SecsS07F23>`
-        - :class:`SecsS07F26 <secsgem.secs.functions.SecsS07F26>`
-        - :class:`SecsS07F31 <secsgem.secs.functions.SecsS07F31>`
-        - :class:`SecsS07F39 <secsgem.secs.functions.SecsS07F39>`
-        - :class:`SecsS07F43 <secsgem.secs.functions.SecsS07F43>`
+        - :class:`SecsS07F01 <secsgem.secs.functions.SecsS07F01>`
+        - :class:`SecsS07F03 <secsgem.secs.functions.SecsS07F03>`
+        - :class:`SecsS07F05 <secsgem.secs.functions.SecsS07F05>`
+        - :class:`SecsS07F06 <secsgem.secs.functions.SecsS07F06>`
+        - :class:`SecsS07F17 <secsgem.secs.functions.SecsS07F17>`
+        - :class:`SecsS07F20 <secsgem.secs.functions.SecsS07F20>`
 
     """
 
-    __type__ = variables.String
-    __count__ = 20
+    __type__ = variables.Dynamic
+    __allowedtypes__ = [
+        variables.String,
+        variables.Binary
+    ]
+    __count__ = 120
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/mexp.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/mexp.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 from .base import DataItemBase
 
 
 class MEXP(DataItemBase):
     """
     Message expected.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
+    :Length: 6
 
     **Used In Function**
         - :class:`SecsS09F13 <secsgem.secs.functions.SecsS09F13>`
+
     """
 
     __type__ = variables.String
     __count__ = 6
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/mhead.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/mhead.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class MHEAD(DataItemBase):
     """
     SECS message header.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 10
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 10
 
     **Used In Function**
         - :class:`SecsS09F01 <secsgem.secs.functions.SecsS09F01>`
         - :class:`SecsS09F03 <secsgem.secs.functions.SecsS09F03>`
         - :class:`SecsS09F05 <secsgem.secs.functions.SecsS09F05>`
         - :class:`SecsS09F07 <secsgem.secs.functions.SecsS09F07>`
         - :class:`SecsS09F11 <secsgem.secs.functions.SecsS09F11>`
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/mlcl.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/mlcl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 
 class MLCL(DataItemBase):
     """
     Message length.
 
     :Types:
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
 
     **Used In Function**
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
         - :class:`SecsS12F05 <secsgem.secs.functions.SecsS12F05>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/nulbc.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/units.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 #####################################################################
-# nulbc.py
+# units.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""NULBC data item."""
+"""UNITS data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class NULBC(DataItemBase):
+class UNITS(DataItemBase):
     """
-    Column count in dies.
+    Units identifier.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`U1 <secsgem.secs.variables.U1>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
-        - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
-        - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
+        - :class:`SecsS01F12 <secsgem.secs.functions.SecsS01F12>`
+        - :class:`SecsS01F22 <secsgem.secs.functions.SecsS01F22>`
+        - :class:`SecsS02F30 <secsgem.secs.functions.SecsS02F30>`
+        - :class:`SecsS02F48 <secsgem.secs.functions.SecsS02F48>`
 
     """
 
-    __type__ = variables.Dynamic
-    __allowedtypes__ = [variables.U1, variables.String]
+    __type__ = variables.String
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/objack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/objack.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class OBJACK(DataItemBase):
     """
     Object acknowledgement code.
 
-       :Types: :class:`U1 <secsgem.secs.variables.U1>`
-       :Length: 1
+    :Type: :class:`U1 <secsgem.secs.variables.U1>`
+    :Length: 1
 
     **Values**
         +-------+-------------+----------------------------------------------------+
         | Value | Description | Constant                                           |
         +=======+=============+====================================================+
         | 0     | Successful  | :const:`secsgem.secs.data_items.OBJACK.SUCCESSFUL` |
         +-------+-------------+----------------------------------------------------+
@@ -35,23 +35,14 @@
         +-------+-------------+----------------------------------------------------+
         | 2-63  | Reserved    |                                                    |
         +-------+-------------+----------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS14F02 <secsgem.secs.functions.SecsS14F02>`
         - :class:`SecsS14F04 <secsgem.secs.functions.SecsS14F04>`
-        - :class:`SecsS14F06 <secsgem.secs.functions.SecsS14F06>`
-        - :class:`SecsS14F08 <secsgem.secs.functions.SecsS14F08>`
-        - :class:`SecsS14F10 <secsgem.secs.functions.SecsS14F10>`
-        - :class:`SecsS14F12 <secsgem.secs.functions.SecsS14F12>`
-        - :class:`SecsS14F14 <secsgem.secs.functions.SecsS14F14>`
-        - :class:`SecsS14F16 <secsgem.secs.functions.SecsS14F16>`
-        - :class:`SecsS14F18 <secsgem.secs.functions.SecsS14F18>`
-        - :class:`SecsS14F26 <secsgem.secs.functions.SecsS14F26>`
-        - :class:`SecsS14F28 <secsgem.secs.functions.SecsS14F28>`
 
     """
 
     __type__ = variables.U1
     __count__ = 1
 
     SUCCESSFUL = 0
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/objid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/objid.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,21 @@
 
 
 class OBJID(DataItemBase):
     """
     Object identifier.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS01F19 <secsgem.secs.functions.SecsS01F19>`
         - :class:`SecsS14F01 <secsgem.secs.functions.SecsS14F01>`
         - :class:`SecsS14F02 <secsgem.secs.functions.SecsS14F02>`
         - :class:`SecsS14F03 <secsgem.secs.functions.SecsS14F03>`
         - :class:`SecsS14F04 <secsgem.secs.functions.SecsS14F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/objspec.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/cpval.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 #####################################################################
-# objspec.py
+# cpval.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""OBJSPEC data item."""
+"""CPVAL data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class OBJSPEC(DataItemBase):
+class CPVAL(DataItemBase):
     """
-    Specific object instance.
+    Command parameter value.
 
     :Types:
+       - :class:`Boolean <secsgem.secs.variables.Boolean>`
+       - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`U2 <secsgem.secs.variables.U2>`
+       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
-        - :class:`SecsS02F49 <secsgem.secs.functions.SecsS02F49>`
-        - :class:`SecsS13F11 <secsgem.secs.functions.SecsS13F11>`
-        - :class:`SecsS13F13 <secsgem.secs.functions.SecsS13F13>`
-        - :class:`SecsS13F15 <secsgem.secs.functions.SecsS13F15>`
-        - :class:`SecsS14F01 <secsgem.secs.functions.SecsS14F01>`
-        - :class:`SecsS14F03 <secsgem.secs.functions.SecsS14F03>`
-        - :class:`SecsS14F05 <secsgem.secs.functions.SecsS14F05>`
-        - :class:`SecsS14F07 <secsgem.secs.functions.SecsS14F07>`
-        - :class:`SecsS14F09 <secsgem.secs.functions.SecsS14F09>`
-        - :class:`SecsS14F10 <secsgem.secs.functions.SecsS14F10>`
-        - :class:`SecsS14F11 <secsgem.secs.functions.SecsS14F11>`
-        - :class:`SecsS14F13 <secsgem.secs.functions.SecsS14F13>`
-        - :class:`SecsS14F15 <secsgem.secs.functions.SecsS14F15>`
-        - :class:`SecsS14F16 <secsgem.secs.functions.SecsS14F16>`
-        - :class:`SecsS14F17 <secsgem.secs.functions.SecsS14F17>`
-        - :class:`SecsS14F19 <secsgem.secs.functions.SecsS14F19>`
-        - :class:`SecsS14F25 <secsgem.secs.functions.SecsS14F25>`
-        - :class:`SecsS14F27 <secsgem.secs.functions.SecsS14F27>`
-        - :class:`SecsS15F43 <secsgem.secs.functions.SecsS15F43>`
-        - :class:`SecsS15F47 <secsgem.secs.functions.SecsS15F47>`
+        - :class:`SecsS02F41 <secsgem.secs.functions.SecsS02F41>`
 
     """
 
-    __type__ = variables.String
+    __type__ = variables.Dynamic
+    __allowedtypes__ = [
+        variables.Boolean,
+        variables.U1,
+        variables.U2,
+        variables.U4,
+        variables.U8,
+        variables.I1,
+        variables.I2,
+        variables.I4,
+        variables.I8,
+        variables.String,
+        variables.Binary
+    ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/objtype.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/svid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 #####################################################################
-# objtype.py
+# svid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""OBJTYPE data item."""
+"""SVID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class OBJTYPE(DataItemBase):
+class SVID(DataItemBase):
     """
-    Class of object identifier.
+    Status variable ID.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS01F19 <secsgem.secs.functions.SecsS01F19>`
-        - :class:`SecsS14F01 <secsgem.secs.functions.SecsS14F01>`
-        - :class:`SecsS14F03 <secsgem.secs.functions.SecsS14F03>`
-        - :class:`SecsS14F06 <secsgem.secs.functions.SecsS14F06>`
-        - :class:`SecsS14F07 <secsgem.secs.functions.SecsS14F07>`
-        - :class:`SecsS14F08 <secsgem.secs.functions.SecsS14F08>`
-        - :class:`SecsS14F25 <secsgem.secs.functions.SecsS14F25>`
-        - :class:`SecsS14F26 <secsgem.secs.functions.SecsS14F26>`
-        - :class:`SecsS14F27 <secsgem.secs.functions.SecsS14F27>`
+        - :class:`SecsS01F03 <secsgem.secs.functions.SecsS01F03>`
+        - :class:`SecsS01F11 <secsgem.secs.functions.SecsS01F11>`
+        - :class:`SecsS01F12 <secsgem.secs.functions.SecsS01F12>`
+        - :class:`SecsS02F23 <secsgem.secs.functions.SecsS02F23>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
         variables.U4,
         variables.U8,
+        variables.I1,
+        variables.I2,
+        variables.I4,
+        variables.I8,
         variables.String
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/oflack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/sdack.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #####################################################################
-# oflack.py
+# sdack.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""OFLACK data item."""
+"""SDACK data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class OFLACK(DataItemBase):
+class SDACK(DataItemBase):
     """
-    Acknowledge code for OFFLINE request.
+    Map setup acknowledge.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+---------------------+---------------------------------------------+
-        | Value | Description         | Constant                                    |
-        +=======+=====================+=============================================+
-        | 0     | OFFLINE Acknowledge | :const:`secsgem.secs.data_items.OFLACK.ACK` |
-        +-------+---------------------+---------------------------------------------+
-        | 1-63  | Reserved            |                                             |
-        +-------+---------------------+---------------------------------------------+
+        +-------+---------------+--------------------------------------------+
+        | Value | Description   | Constant                                   |
+        +=======+===============+============================================+
+        | 0     | Received Data | :const:`secsgem.secs.data_items.SDACK.ACK` |
+        +-------+---------------+--------------------------------------------+
+        | 1-63  | Error         |                                            |
+        +-------+---------------+--------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS01F16 <secsgem.secs.functions.SecsS01F16>`
+        - :class:`SecsS12F02 <secsgem.secs.functions.SecsS12F02>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     ACK = 0
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/onlack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/onlack.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class ONLACK(DataItemBase):
     """
     Acknowledge code for ONLINE request.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+--------------------+-----------------------------------------------------+
         | Value | Description        | Constant                                            |
         +=======+====================+=====================================================+
         | 0     | ONLINE Accepted    | :const:`secsgem.secs.data_items.ONLACK.ACCEPTED`    |
         +-------+--------------------+-----------------------------------------------------+
@@ -36,14 +36,15 @@
         | 2     | Already ONLINE     | :const:`secsgem.secs.data_items.ONLACK.ALREADY_ON`  |
         +-------+--------------------+-----------------------------------------------------+
         | 3-63  | Reserved           |                                                     |
         +-------+--------------------+-----------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS01F18 <secsgem.secs.functions.SecsS01F18>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     ACCEPTED = 0
     NOT_ALLOWED = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/orloc.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ackc7.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 #####################################################################
-# orloc.py
+# ackc7.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""ORLOC data item."""
+"""ACKC7 data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class ORLOC(DataItemBase):
+class ACKC7(DataItemBase):
     """
-    Origin location.
+    Acknowledge code for stream 7.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+---------------------+----------------------------------------------------+
-        | Value | Description         | Constant                                           |
-        +=======+=====================+====================================================+
-        | 0     | Center die of wafer | :const:`secsgem.secs.data_items.ORLOC.CENTER_DIE`  |
-        +-------+---------------------+----------------------------------------------------+
-        | 1     | Upper right         | :const:`secsgem.secs.data_items.ORLOC.UPPER_RIGHT` |
-        +-------+---------------------+----------------------------------------------------+
-        | 2     | Upper left          | :const:`secsgem.secs.data_items.ORLOC.UPPER_LEFT`  |
-        +-------+---------------------+----------------------------------------------------+
-        | 3     | Lower left          | :const:`secsgem.secs.data_items.ORLOC.LOWER_LEFT`  |
-        +-------+---------------------+----------------------------------------------------+
-        | 4     | Lower right         | :const:`secsgem.secs.data_items.ORLOC.LOWER_RIGHT` |
-        +-------+---------------------+----------------------------------------------------+
-        | 5-63  | Reserved, error     |                                                    |
-        +-------+---------------------+----------------------------------------------------+
+        +-------+------------------------+---------------------------------------------------------+
+        | Value | Description            | Constant                                                |
+        +=======+========================+=========================================================+
+        | 0     | Accepted               | :const:`secsgem.secs.data_items.ACKC7.ACCEPTED`         |
+        +-------+------------------------+---------------------------------------------------------+
+        | 1     | Permission not granted | :const:`secsgem.secs.data_items.ACKC7.NO_PERMISSION`    |
+        +-------+------------------------+---------------------------------------------------------+
+        | 2     | Length error           | :const:`secsgem.secs.data_items.ACKC7.LENGTH_ERROR`     |
+        +-------+------------------------+---------------------------------------------------------+
+        | 3     | Matrix overflow        | :const:`secsgem.secs.data_items.ACKC7.MATRIX_OVERFLOW`  |
+        +-------+------------------------+---------------------------------------------------------+
+        | 4     | PPID not found         | :const:`secsgem.secs.data_items.ACKC7.PPID_NOT_FOUND`   |
+        +-------+------------------------+---------------------------------------------------------+
+        | 5     | Mode unsupported       | :const:`secsgem.secs.data_items.ACKC7.MODE_UNSUPPORTED` |
+        +-------+------------------------+---------------------------------------------------------+
+        | 6     | Performed later        | :const:`secsgem.secs.data_items.ACKC7.PERFORMED_LATER`  |
+        +-------+------------------------+---------------------------------------------------------+
+        | 7-63  | Reserved               |                                                         |
+        +-------+------------------------+---------------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
-        - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
-        - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
+        - :class:`SecsS07F04 <secsgem.secs.functions.SecsS07F04>`
+        - :class:`SecsS07F18 <secsgem.secs.functions.SecsS07F18>`
 
     """
 
     __type__ = variables.Binary
+    __count__ = 1
 
-    CENTER_DIE = 0
-    UPPER_RIGHT = 1
-    UPPER_LEFT = 2
-    LOWER_LEFT = 3
-    LOWER_RIGHT = 3
+    ACCEPTED = 0
+    NO_PERMISSION = 1
+    LENGTH_ERROR = 2
+    MATRIX_OVERFLOW = 3
+    PPID_NOT_FOUND = 4
+    MODE_UNSUPPORTED = 5
+    PERFORMED_LATER = 6
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ppbody.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/cpname.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 #####################################################################
-# ppbody.py
+# cpname.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""PPBODY data item."""
+"""CPNAME data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class PPBODY(DataItemBase):
+class CPNAME(DataItemBase):
     """
-    Status variable ID.
+    Command parameter name.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS07F03 <secsgem.secs.functions.SecsS07F03>`
-        - :class:`SecsS07F06 <secsgem.secs.functions.SecsS07F06>`
-        - :class:`SecsS07F36 <secsgem.secs.functions.SecsS07F36>`
-        - :class:`SecsS07F37 <secsgem.secs.functions.SecsS07F37>`
-        - :class:`SecsS07F41 <secsgem.secs.functions.SecsS07F41>`
+        - :class:`SecsS02F41 <secsgem.secs.functions.SecsS02F41>`
+        - :class:`SecsS02F42 <secsgem.secs.functions.SecsS02F42>`
+        - :class:`SecsS02F49 <secsgem.secs.functions.SecsS02F49>`
+        - :class:`SecsS02F50 <secsgem.secs.functions.SecsS02F50>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
         variables.U4,
         variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
         variables.I8,
-        variables.String,
-        variables.Binary
+        variables.String
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ppgnt.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ppgnt.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class PPGNT(DataItemBase):
     """
     Process program grant status.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+------------------------+--------------------------------------------------------+
         | Value | Description            | Constant                                               |
         +=======+========================+========================================================+
         | 0     | OK                     | :const:`secsgem.secs.data_items.PPGNT.OK`              |
         +-------+------------------------+--------------------------------------------------------+
@@ -42,15 +42,14 @@
         | 5     | Will not accept        | :const:`secsgem.secs.data_items.PPGNT.WILL_NOT_ACCEPT` |
         +-------+------------------------+--------------------------------------------------------+
         | 6-63  | Reserved, other errors |                                                        |
         +-------+------------------------+--------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS07F02 <secsgem.secs.functions.SecsS07F02>`
-        - :class:`SecsS07F30 <secsgem.secs.functions.SecsS07F30>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     OK = 0
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/praxi.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/praxi.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class PRAXI(DataItemBase):
     """
     Process axis.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+----------------------------+--------------------------------------------------------+
         | Value | Description                | Constant                                               |
         +=======+============================+========================================================+
         | 0     | Rows, top, increasing      | :const:`secsgem.secs.data_items.PRAXI.ROWS_TOP_INCR`   |
         +-------+----------------------------+--------------------------------------------------------+
@@ -46,15 +46,15 @@
         | 7     | Columns, right, decreasing | :const:`secsgem.secs.data_items.PRAXI.COLS_RIGHT_DECR` |
         +-------+----------------------------+--------------------------------------------------------+
         | 8-63  | Error                      |                                                        |
         +-------+----------------------------+--------------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
-        - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
+        - :class:`SecsS12F03 <secsgem.secs.functions.SecsS12F03>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     ROWS_TOP_INCR = 0
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/prdct.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/prdct.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 
 class PRDCT(DataItemBase):
     """
     Process die count.
 
     :Types:
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/rcmd.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/rcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 
 
 class RCMD(DataItemBase):
     """
     Remote command.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
         - :class:`SecsS02F21 <secsgem.secs.functions.SecsS02F21>`
         - :class:`SecsS02F41 <secsgem.secs.functions.SecsS02F41>`
         - :class:`SecsS02F49 <secsgem.secs.functions.SecsS02F49>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.I1,
         variables.String
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/refp.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/extype.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,33 @@
 #####################################################################
-# refp.py
+# extype.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""REFP data item."""
+"""EXTYPE data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class REFP(DataItemBase):
+class EXTYPE(DataItemBase):
     """
-    Reference point.
+    Exception type.
 
-    :Types:
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
-        - :class:`SecsS01F03 <secsgem.secs.functions.SecsS01F03>`
-        - :class:`SecsS01F11 <secsgem.secs.functions.SecsS01F11>`
-        - :class:`SecsS01F12 <secsgem.secs.functions.SecsS01F12>`
-        - :class:`SecsS02F23 <secsgem.secs.functions.SecsS02F23>`
+        - :class:`SecsS05F09 <secsgem.secs.functions.SecsS05F09>`
+        - :class:`SecsS05F11 <secsgem.secs.functions.SecsS05F11>`
+
     """
 
-    __type__ = variables.Dynamic
-    __allowedtypes__ = [
-        variables.I1,
-        variables.I2,
-        variables.I4,
-        variables.I8
-    ]
+    __type__ = variables.String
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/rowct.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/rowct.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 
 class ROWCT(DataItemBase):
     """
     Row count in dies.
 
     :Types:
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/rpsel.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/rpsel.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .base import DataItemBase
 
 
 class RPSEL(DataItemBase):
     """
     Reference point select.
 
-       :Types: :class:`U1 <secsgem.secs.variables.U1>`
+    :Type: :class:`U1 <secsgem.secs.variables.U1>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/rptid.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f41.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,93 @@
 #####################################################################
-# rptid.py
+# s02f41.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""RPTID data item."""
-from .. import variables
-from .base import DataItemBase
+"""Class for stream 02 function 41."""
 
+from secsgem.secs.functions.base import SecsStreamFunction
+from secsgem.secs.data_items import RCMD
+from secsgem.secs.data_items import CPNAME
+from secsgem.secs.data_items import CPVAL
 
-class RPTID(DataItemBase):
+
+class SecsS02F41(SecsStreamFunction):
     """
-    Report ID.
+    host command - send.
+
+    **Data Items**
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
-       - :class:`U1 <secsgem.secs.variables.U1>`
-       - :class:`U2 <secsgem.secs.variables.U2>`
-       - :class:`U4 <secsgem.secs.variables.U4>`
-
-    **Used In Function**
-        - :class:`SecsS02F33 <secsgem.secs.functions.SecsS02F33>`
-        - :class:`SecsS02F35 <secsgem.secs.functions.SecsS02F35>`
-        - :class:`SecsS06F11 <secsgem.secs.functions.SecsS06F11>`
-        - :class:`SecsS06F13 <secsgem.secs.functions.SecsS06F13>`
-        - :class:`SecsS06F16 <secsgem.secs.functions.SecsS06F16>`
-        - :class:`SecsS06F18 <secsgem.secs.functions.SecsS06F18>`
-        - :class:`SecsS06F19 <secsgem.secs.functions.SecsS06F19>`
-        - :class:`SecsS06F21 <secsgem.secs.functions.SecsS06F21>`
-        - :class:`SecsS06F27 <secsgem.secs.functions.SecsS06F27>`
-        - :class:`SecsS06F30 <secsgem.secs.functions.SecsS06F30>`
-        - :class:`SecsS17F01 <secsgem.secs.functions.SecsS17F01>`
-        - :class:`SecsS17F02 <secsgem.secs.functions.SecsS17F02>`
-        - :class:`SecsS17F03 <secsgem.secs.functions.SecsS17F03>`
-        - :class:`SecsS17F04 <secsgem.secs.functions.SecsS17F04>`
-        - :class:`SecsS17F05 <secsgem.secs.functions.SecsS17F05>`
-        - :class:`SecsS17F09 <secsgem.secs.functions.SecsS17F09>`
-        - :class:`SecsS17F11 <secsgem.secs.functions.SecsS17F11>`
-        - :class:`SecsS17F12 <secsgem.secs.functions.SecsS17F12>`
+    - :class:`RCMD <secsgem.secs.data_items.RCMD>`
+    - :class:`CPNAME <secsgem.secs.data_items.CPNAME>`
+    - :class:`CPVAL <secsgem.secs.data_items.CPVAL>`
+
+    **Structure**::
+
+        >>> import secsgem.secs
+        >>> secsgem.secs.functions.SecsS02F41
+        {
+            RCMD: U1/I1/A
+            PARAMS: [
+                {
+                    CPNAME: U1/U2/U4/U8/I1/I2/I4/I8/A
+                    CPVAL: BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/A/B
+                }
+                ...
+            ]
+        }
+
+    **Example**::
+
+        >>> import secsgem.secs
+        >>> secsgem.secs.functions.SecsS02F41({"RCMD": "COMMAND", "PARAMS": [{"CPNAME": "PARAM1", "CPVAL": "VAL1"},
+        ...     {"CPNAME": "PARAM2", "CPVAL": "VAL2"}]})
+        S2F41 W
+          <L [2]
+            <A "COMMAND">
+            <L [2]
+              <L [2]
+                <A "PARAM1">
+                <A "VAL1">
+              >
+              <L [2]
+                <A "PARAM2">
+                <A "VAL2">
+              >
+            >
+          > .
 
+    :param value: parameters for this function (see example)
+    :type value: dict
     """
 
-    __type__ = variables.Dynamic
-    __allowedtypes__ = [
-        variables.U1,
-        variables.U2,
-        variables.U4,
-        variables.U8,
-        variables.I1,
-        variables.I2,
-        variables.I4,
-        variables.I8,
-        variables.String
+    _stream = 2
+    _function = 41
+
+    _data_format = [
+        RCMD,
+        [
+            [
+                "PARAMS",
+                CPNAME,
+                CPVAL
+            ]
+        ]
     ]
+
+    _to_host = False
+    _to_equipment = True
+
+    _has_reply = True
+    _is_reply_required = True
+
+    _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/rsinf.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/rsinf.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 
 
 class RSINF(DataItemBase):
     """
     Starting location.
 
     :Types:
-       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+    :Length: 3
 
     **Used In Function**
         - :class:`SecsS12F07 <secsgem.secs.functions.SecsS12F07>`
         - :class:`SecsS12F14 <secsgem.secs.functions.SecsS12F14>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/sdack.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ackc6.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #####################################################################
-# sdack.py
+# ackc6.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""SDACK data item."""
+"""ACKC6 data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class SDACK(DataItemBase):
+class ACKC6(DataItemBase):
     """
-    Map setup acknowledge.
+    Acknowledge code for stream 6.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
-        +-------+---------------+--------------------------------------------+
-        | Value | Description   | Constant                                   |
-        +=======+===============+============================================+
-        | 0     | Received Data | :const:`secsgem.secs.data_items.SDACK.ACK` |
-        +-------+---------------+--------------------------------------------+
-        | 1-63  | Error         |                                            |
-        +-------+---------------+--------------------------------------------+
+        +-------+-------------+-------------------------------------------------+
+        | Value | Description | Constant                                        |
+        +=======+=============+=================================================+
+        | 0     | Accepted    | :const:`secsgem.secs.data_items.ACKC6.ACCEPTED` |
+        +-------+-------------+-------------------------------------------------+
+        | 1-63  | Error       | :const:`secsgem.secs.data_items.ACKC6.ERROR`    |
+        +-------+-------------+-------------------------------------------------+
 
     **Used In Function**
-        - :class:`SecsS12F02 <secsgem.secs.functions.SecsS12F02>`
+        - :class:`SecsS06F02 <secsgem.secs.functions.SecsS06F02>`
+        - :class:`SecsS06F12 <secsgem.secs.functions.SecsS06F12>`
 
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
-    ACK = 0
+    ACCEPTED = 0
+    ERROR = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/sdbin.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/sdbin.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 from .base import DataItemBase
 
 
 class SDBIN(DataItemBase):
     """
     Send bin information.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Values**
         +-------+---------------------------+--------------------------------------------------+
         | Value | Description               | Constant                                         |
         +=======+===========================+==================================================+
         | 0     | Send bin information      | :const:`secsgem.secs.data_items.SDBIN.SEND`      |
         +-------+---------------------------+--------------------------------------------------+
         | 1     | Don't send bin infomation | :const:`secsgem.secs.data_items.SDBIN.DONT_SEND` |
         +-------+---------------------------+--------------------------------------------------+
         | 2-63  | Reserved                  |                                                  |
         +-------+---------------------------+--------------------------------------------------+
 
     **Used In Function**
         - :class:`SecsS12F17 <secsgem.secs.functions.SecsS12F17>`
+
     """
 
     __type__ = variables.Binary
     __count__ = 1
 
     SEND = 0
     DONT_SEND = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/shead.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/shead.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from .base import DataItemBase
 
 
 class SHEAD(DataItemBase):
     """
     SECS message header.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 10
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 10
 
     **Used In Function**
         - :class:`SecsS09F09 <secsgem.secs.functions.SecsS09F09>`
 
     """
 
     __type__ = variables.Binary
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/softrev.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f14.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 #####################################################################
-# softrev.py
+# s02f14.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""SOFTREV data item."""
-from .. import variables
-from .base import DataItemBase
+"""Class for stream 02 function 14."""
 
+from secsgem.secs.functions.base import SecsStreamFunction
+from secsgem.secs.data_items import ECV
 
-class SOFTREV(DataItemBase):
+
+class SecsS02F14(SecsStreamFunction):
     """
-    Software revision.
+    equipment constant - data.
+
+    **Data Items**
+
+    - :class:`ECV <secsgem.secs.data_items.ECV>`
+
+    **Structure**::
+
+        >>> import secsgem.secs
+        >>> secsgem.secs.functions.SecsS02F14
+        [
+            ECV: L/BOOLEAN/I8/I1/I2/I4/F8/F4/U8/U1/U2/U4/A/B
+            ...
+        ]
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    **Example**::
 
-    **Used In Function**
-        - :class:`SecsS01F02 <secsgem.secs.functions.SecsS01F02>`
-        - :class:`SecsS01F13 <secsgem.secs.functions.SecsS01F13>`
-        - :class:`SecsS01F14 <secsgem.secs.functions.SecsS01F14>`
-        - :class:`SecsS07F22 <secsgem.secs.functions.SecsS07F22>`
-        - :class:`SecsS07F23 <secsgem.secs.functions.SecsS07F23>`
-        - :class:`SecsS07F26 <secsgem.secs.functions.SecsS07F26>`
-        - :class:`SecsS07F31 <secsgem.secs.functions.SecsS07F31>`
-        - :class:`SecsS07F39 <secsgem.secs.functions.SecsS07F39>`
-        - :class:`SecsS07F43 <secsgem.secs.functions.SecsS07F43>`
+        >>> import secsgem.secs
+        >>> secsgem.secs.functions.SecsS02F14([secsgem.secs.variables.U1(1), "text"])
+        S2F14
+          <L [2]
+            <U1 1 >
+            <A "text">
+          > .
 
+    :param value: parameters for this function (see example)
+    :type value: list
     """
 
-    __type__ = variables.String
-    __count__ = 20
+    _stream = 2
+    _function = 14
+
+    _data_format = [ECV]
+
+    _to_host = True
+    _to_equipment = False
+
+    _has_reply = False
+    _is_reply_required = False
+
+    _is_multi_block = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/strp.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/strp.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 
 
 class STRP(DataItemBase):
     """
     Starting position.
 
     :Types:
-       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+    :Length: 2
 
     **Used In Function**
         - :class:`SecsS12F09 <secsgem.secs.functions.SecsS12F09>`
         - :class:`SecsS12F16 <secsgem.secs.functions.SecsS12F16>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.I1,
         variables.I2,
         variables.I4,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/sv.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/sv.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,31 +20,32 @@
 
 class SV(DataItemBase):
     """
     Status variable value.
 
     :Types:
        - :class:`Array <secsgem.secs.variables.Array>`
-       - :class:`Binary <secsgem.secs.variables.Binary>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`U1 <secsgem.secs.variables.U1>`
+       - :class:`U2 <secsgem.secs.variables.U2>`
+       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`F4 <secsgem.secs.variables.F4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
-       - :class:`U1 <secsgem.secs.variables.U1>`
-       - :class:`U2 <secsgem.secs.variables.U2>`
-       - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`F8 <secsgem.secs.variables.F8>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
         - :class:`SecsS01F04 <secsgem.secs.functions.SecsS01F04>`
         - :class:`SecsS06F01 <secsgem.secs.functions.SecsS06F01>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.Array,
         variables.Boolean,
         variables.U1,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/svid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/smpln.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 #####################################################################
-# svid.py
+# smpln.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""SVID data item."""
+"""SMPLN data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class SVID(DataItemBase):
+class SMPLN(DataItemBase):
     """
-    Status variable ID.
+    Sample number.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
 
     **Used In Function**
-        - :class:`SecsS01F03 <secsgem.secs.functions.SecsS01F03>`
-        - :class:`SecsS01F11 <secsgem.secs.functions.SecsS01F11>`
-        - :class:`SecsS01F12 <secsgem.secs.functions.SecsS01F12>`
-        - :class:`SecsS02F23 <secsgem.secs.functions.SecsS02F23>`
+        - :class:`SecsS06F01 <secsgem.secs.functions.SecsS06F01>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
-        variables.U1,
-        variables.U2,
-        variables.U4,
-        variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
         variables.I8,
-        variables.String
+        variables.U1,
+        variables.U2,
+        variables.U4,
+        variables.U8
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/svname.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/svname.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .base import DataItemBase
 
 
 class SVNAME(DataItemBase):
     """
     Status variable name.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
 
     **Used In Function**
         - :class:`SecsS01F12 <secsgem.secs.functions.SecsS01F12>`
+
     """
 
     __type__ = variables.String
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/text.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/text.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,30 +19,28 @@
 
 
 class TEXT(DataItemBase):
     """
     Line of characters.
 
     :Types:
-       - :class:`Binary <secsgem.secs.variables.Binary>`
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
         - :class:`SecsS10F01 <secsgem.secs.functions.SecsS10F01>`
         - :class:`SecsS10F03 <secsgem.secs.functions.SecsS10F03>`
-        - :class:`SecsS10F05 <secsgem.secs.functions.SecsS10F05>`
-        - :class:`SecsS10F09 <secsgem.secs.functions.SecsS10F09>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/tid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/errtext.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #####################################################################
-# tid.py
+# errtext.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""TID data item."""
+"""ERRTEXT data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class TID(DataItemBase):
+class ERRTEXT(DataItemBase):
     """
-    Terminal ID.
+    Error description for error code.
 
-       :Types: :class:`Binary <secsgem.secs.variables.Binary>`
-       :Length: 1
+    :Type: :class:`String <secsgem.secs.variables.String>`
+    :Length: 120
 
     **Used In Function**
-        - :class:`SecsS10F01 <secsgem.secs.functions.SecsS10F01>`
-        - :class:`SecsS10F03 <secsgem.secs.functions.SecsS10F03>`
-        - :class:`SecsS10F05 <secsgem.secs.functions.SecsS10F05>`
-        - :class:`SecsS10F07 <secsgem.secs.functions.SecsS10F07>`
+        - :class:`SecsS05F14 <secsgem.secs.functions.SecsS05F14>`
+        - :class:`SecsS05F15 <secsgem.secs.functions.SecsS05F15>`
+        - :class:`SecsS05F18 <secsgem.secs.functions.SecsS05F18>`
+        - :class:`SecsS14F02 <secsgem.secs.functions.SecsS14F02>`
+        - :class:`SecsS14F04 <secsgem.secs.functions.SecsS14F04>`
 
     """
 
-    __type__ = variables.Binary
-    __count__ = 1
+    __type__ = variables.String
+    __count__ = 120
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/time.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/fcnid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #####################################################################
-# time.py
+# fcnid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""TIME data item."""
+"""FCNID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class TIME(DataItemBase):
+class FCNID(DataItemBase):
     """
-    Time of day.
+    Function ID.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`U1 <secsgem.secs.variables.U1>`
+    :Length: 1
 
     **Used In Function**
-        - :class:`SecsS02F18 <secsgem.secs.functions.SecsS02F18>`
-        - :class:`SecsS02F31 <secsgem.secs.functions.SecsS02F31>`
+        - :class:`SecsS02F43 <secsgem.secs.functions.SecsS02F43>`
+        - :class:`SecsS02F44 <secsgem.secs.functions.SecsS02F44>`
+
     """
 
-    __type__ = variables.String
-    __count__ = 32
+    __type__ = variables.U1
+    __count__ = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/timestamp.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/altx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 #####################################################################
-# timestamp.py
+# altx.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""TIMESTAMP data item."""
+"""ALTX data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class TIMESTAMP(DataItemBase):
+class ALTX(DataItemBase):
     """
-    Timestamp.
+    Alarm text.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`String <secsgem.secs.variables.String>`
+    :Length: 120
 
     **Used In Function**
-        - :class:`SecsS05F09 <secsgem.secs.functions.SecsS05F09>`
-        - :class:`SecsS05F11 <secsgem.secs.functions.SecsS05F11>`
-        - :class:`SecsS05F15 <secsgem.secs.functions.SecsS05F15>`
-        - :class:`SecsS15F41 <secsgem.secs.functions.SecsS15F41>`
-        - :class:`SecsS15F44 <secsgem.secs.functions.SecsS15F44>`
-        - :class:`SecsS16F05 <secsgem.secs.functions.SecsS16F05>`
-        - :class:`SecsS16F07 <secsgem.secs.functions.SecsS16F07>`
-        - :class:`SecsS16F09 <secsgem.secs.functions.SecsS16F09>`
+        - :class:`SecsS05F01 <secsgem.secs.functions.SecsS05F01>`
+        - :class:`SecsS05F06 <secsgem.secs.functions.SecsS05F06>`
+        - :class:`SecsS05F08 <secsgem.secs.functions.SecsS05F08>`
+
     """
 
     __type__ = variables.String
-    __count__ = 32
+    __count__ = 120
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/units.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/limitid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 #####################################################################
-# units.py
+# limitid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""UNITS data item."""
+"""LIMITID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class UNITS(DataItemBase):
+class LIMITID(DataItemBase):
     """
-    Units identifier.
+    Limit ID.
 
-    :Types:
-       - :class:`String <secsgem.secs.variables.String>`
+    :Type: :class:`Binary <secsgem.secs.variables.Binary>`
+    :Length: 1
 
     **Used In Function**
-        - :class:`SecsS01F12 <secsgem.secs.functions.SecsS01F12>`
-        - :class:`SecsS02F30 <secsgem.secs.functions.SecsS02F30>`
+        - :class:`SecsS02F45 <secsgem.secs.functions.SecsS02F45>`
+        - :class:`SecsS02F46 <secsgem.secs.functions.SecsS02F46>`
         - :class:`SecsS02F48 <secsgem.secs.functions.SecsS02F48>`
-        - :class:`SecsS07F22 <secsgem.secs.functions.SecsS07F22>`
+
     """
 
-    __type__ = variables.String
+    __type__ = variables.Binary
+    __count__ = 1
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/v.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ecv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 #####################################################################
-# v.py
+# ecv.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""V data item."""
+"""ECV data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class V(DataItemBase):
+class ECV(DataItemBase):
     """
-    Variable data.
+    Equipment constant value.
 
     :Types:
        - :class:`Array <secsgem.secs.variables.Array>`
-       - :class:`Binary <secsgem.secs.variables.Binary>`
        - :class:`Boolean <secsgem.secs.variables.Boolean>`
-       - :class:`String <secsgem.secs.variables.String>`
        - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
        - :class:`F8 <secsgem.secs.variables.F8>`
        - :class:`F4 <secsgem.secs.variables.F4>`
        - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`String <secsgem.secs.variables.String>`
+       - :class:`Binary <secsgem.secs.variables.Binary>`
 
     **Used In Function**
-        - :class:`SecsS06F11 <secsgem.secs.functions.SecsS06F11>`
-        - :class:`SecsS06F13 <secsgem.secs.functions.SecsS06F13>`
-        - :class:`SecsS06F16 <secsgem.secs.functions.SecsS06F16>`
-        - :class:`SecsS06F20 <secsgem.secs.functions.SecsS06F20>`
-        - :class:`SecsS06F22 <secsgem.secs.functions.SecsS06F22>`
+        - :class:`SecsS02F14 <secsgem.secs.functions.SecsS02F14>`
+        - :class:`SecsS02F15 <secsgem.secs.functions.SecsS02F15>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.Array,
         variables.Boolean,
-        variables.U1,
-        variables.U2,
-        variables.U4,
-        variables.U8,
+        variables.I8,
         variables.I1,
         variables.I2,
         variables.I4,
-        variables.I8,
-        variables.F4,
         variables.F8,
+        variables.F4,
+        variables.U8,
+        variables.U1,
+        variables.U2,
+        variables.U4,
         variables.String,
         variables.Binary
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/vid.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/alid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 #####################################################################
-# vid.py
+# alid.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""VID data item."""
+"""ALID data item."""
 from .. import variables
 from .base import DataItemBase
 
 
-class VID(DataItemBase):
+class ALID(DataItemBase):
     """
-    Variable ID.
+    Alarm ID.
 
     :Types:
-       - :class:`String <secsgem.secs.variables.String>`
-       - :class:`I8 <secsgem.secs.variables.I8>`
-       - :class:`I1 <secsgem.secs.variables.I1>`
-       - :class:`I2 <secsgem.secs.variables.I2>`
-       - :class:`I4 <secsgem.secs.variables.I4>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`I1 <secsgem.secs.variables.I1>`
+       - :class:`I2 <secsgem.secs.variables.I2>`
+       - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
 
     **Used In Function**
-        - :class:`SecsS02F33 <secsgem.secs.functions.SecsS02F33>`
-        - :class:`SecsS02F45 <secsgem.secs.functions.SecsS02F45>`
-        - :class:`SecsS02F46 <secsgem.secs.functions.SecsS02F46>`
-        - :class:`SecsS02F47 <secsgem.secs.functions.SecsS02F47>`
-        - :class:`SecsS02F48 <secsgem.secs.functions.SecsS02F48>`
-        - :class:`SecsS06F13 <secsgem.secs.functions.SecsS06F13>`
-        - :class:`SecsS06F18 <secsgem.secs.functions.SecsS06F18>`
-        - :class:`SecsS06F22 <secsgem.secs.functions.SecsS06F22>`
-        - :class:`SecsS17F01 <secsgem.secs.functions.SecsS17F01>`
+        - :class:`SecsS05F01 <secsgem.secs.functions.SecsS05F01>`
+        - :class:`SecsS05F03 <secsgem.secs.functions.SecsS05F03>`
+        - :class:`SecsS05F05 <secsgem.secs.functions.SecsS05F05>`
+        - :class:`SecsS05F06 <secsgem.secs.functions.SecsS05F06>`
+        - :class:`SecsS05F08 <secsgem.secs.functions.SecsS05F08>`
 
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.U1,
         variables.U2,
         variables.U4,
         variables.U8,
         variables.I1,
         variables.I2,
         variables.I4,
-        variables.I8,
-        variables.String
+        variables.I8
     ]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/xdies.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/xdies.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
 
 class XDIES(DataItemBase):
     """
     Die size/index X-axis.
 
     :Types:
-       - :class:`F4 <secsgem.secs.variables.F4>`
-       - :class:`F8 <secsgem.secs.variables.F8>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`F4 <secsgem.secs.variables.F4>`
+       - :class:`F8 <secsgem.secs.variables.F8>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/xypos.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/xypos.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 
 
 class XYPOS(DataItemBase):
     """
     X/Y coordinate position.
 
     :Types:
-       - :class:`I8 <secsgem.secs.variables.I8>`
        - :class:`I1 <secsgem.secs.variables.I1>`
        - :class:`I2 <secsgem.secs.variables.I2>`
        - :class:`I4 <secsgem.secs.variables.I4>`
+       - :class:`I8 <secsgem.secs.variables.I8>`
+    :Length: 2
 
     **Used In Function**
         - :class:`SecsS12F11 <secsgem.secs.functions.SecsS12F11>`
         - :class:`SecsS12F18 <secsgem.secs.functions.SecsS12F18>`
+
     """
 
     __type__ = variables.Dynamic
     __allowedtypes__ = [
         variables.I1,
         variables.I2,
         variables.I4,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/data_items/ydies.py` & `secsgem-0.2.0a3/secsgem/secs/data_items/ydies.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
 
 class YDIES(DataItemBase):
     """
     Die size/index Y-axis.
 
     :Types:
-       - :class:`F4 <secsgem.secs.variables.F4>`
-       - :class:`F8 <secsgem.secs.variables.F8>`
-       - :class:`U8 <secsgem.secs.variables.U8>`
        - :class:`U1 <secsgem.secs.variables.U1>`
        - :class:`U2 <secsgem.secs.variables.U2>`
        - :class:`U4 <secsgem.secs.variables.U4>`
+       - :class:`U8 <secsgem.secs.variables.U8>`
+       - :class:`F4 <secsgem.secs.variables.F4>`
+       - :class:`F8 <secsgem.secs.variables.F8>`
 
     **Used In Function**
         - :class:`SecsS12F01 <secsgem.secs.functions.SecsS12F01>`
         - :class:`SecsS12F04 <secsgem.secs.functions.SecsS12F04>`
 
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/base.py` & `secsgem-0.2.0a3/secsgem/secs/functions/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Base class for for SECS stream and functions."""
+import typing
 
 import secsgem.common
+from ..data_items import DataItemBase
 from ..variables import functions
 
+DataItemRecursive = typing.Union[typing.Type[DataItemBase], typing.Iterable["DataItemRecursive"]]
+
 
 class StructureDisplayingMeta(type):
     """Meta class overriding the default __repr__ of a class."""
 
     def __repr__(cls):
         """Generate textual representation for an object of this class."""
         return cls.get_format()
@@ -35,15 +39,15 @@
     To create a function specific content the class variables :attr:`_stream`, :attr:`_function`
     and :attr:`_data_format` must be overridden.
     """
 
     _stream = 0
     _function = 0
 
-    _data_format = None
+    _data_format: typing.Optional[DataItemRecursive] = None
 
     _to_host = True
     _to_equipment = True
 
     _has_reply = False
     _is_reply_required = False
 
@@ -183,14 +187,17 @@
     def get(self):
         """
         Get the current value of the stream/function parameter.
 
         :returns: current parameter value
         :rtype: various
         """
+        if self.data is None:
+            return None
+        
         return self.data.get()
 
     @classmethod
     def get_format(cls):
         """
         Get the format of the function.
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s00f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s00f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f01.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f01.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f02.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f02.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,24 +33,37 @@
     **Structure E->H**::
 
         {
             MDLN: A[20]
             SOFTREV: A[20]
         }
 
+    **Data Items**
+
+    - :class:`MDLN <secsgem.secs.data_items.MDLN>`
+
+    **Structure**::
+
+        >>> import secsgem.secs
+        >>> secsgem.secs.functions.SecsS01F02
+        [
+            MDLN: A[20]
+            ...
+        ]
+
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS01F02(['secsgem', '0.0.6']) # E->H
+        >>> secsgem.secs.functions.SecsS01F02(["secsgem", "0.0.6"]) # E->H
         S1F2
           <L [2]
             <A "secsgem">
             <A "0.0.6">
           > .
-        >>> secsgem.secs.functions.SecsS01F02() #H->E
+        >>> secsgem.secs.functions.SecsS01F02() # H->E
         S1F2
           <L> .
 
     :param value: parameters for this function (see example)
     :type value: list
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f03.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f03.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f04.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f04.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f11.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f11.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from secsgem.secs.data_items import SVID
 
 
 class SecsS01F11(SecsStreamFunction):
     """
     status variable namelist - request.
 
+    An empty list will return all available status variables.
+
     **Data Items**
 
     - :class:`SVID <secsgem.secs.data_items.SVID>`
 
     **Structure**::
 
         >>> import secsgem.secs
@@ -42,16 +44,14 @@
         >>> secsgem.secs.functions.SecsS01F11([1, 1337])
         S1F11 W
           <L [2]
             <U1 1 >
             <U2 1337 >
           > .
 
-    An empty list will return all available status variables.
-
     :param value: parameters for this function (see example)
     :type value: list
     """
 
     _stream = 1
     _function = 11
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f12.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f12.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 01 function 12."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import SVID, SVNAME, UNITS
+from secsgem.secs.data_items import SVID
+from secsgem.secs.data_items import SVNAME
+from secsgem.secs.data_items import UNITS
 
 
 class SecsS01F12(SecsStreamFunction):
     """
     status variable namelist - reply.
 
     **Data Items**
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f13.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f13.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,35 +22,48 @@
 class SecsS01F13(SecsStreamFunction):
     """
     establish communication - request.
 
     .. caution::
 
         This Stream/function has different structures depending on the source.
-        If it is sent from the eqipment side it has the structure below,
-        if it is sent from the host it is an empty list.
+        If it is sent from the eqipment side it has the structure below, if it
+        is sent from the host it is an empty list.
         Be sure to fill the array accordingly.
 
     **Structure E->H**::
 
         {
             MDLN: A[20]
             SOFTREV: A[20]
         }
 
+    **Data Items**
+
+    - :class:`MDLN <secsgem.secs.data_items.MDLN>`
+
+    **Structure**::
+
+        >>> import secsgem.secs
+        >>> secsgem.secs.functions.SecsS01F13
+        [
+            MDLN: A[20]
+            ...
+        ]
+
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS01F13(['secsgem', '0.0.6']) # E->H
+        >>> secsgem.secs.functions.SecsS01F13(["secsgem", "0.0.6"]) # E->H
         S1F13 W
           <L [2]
             <A "secsgem">
             <A "0.0.6">
           > .
-        >>> secsgem.secs.functions.SecsS01F13() #H->E
+        >>> secsgem.secs.functions.SecsS01F13() # H->E
         S1F13 W
           <L> .
 
     :param value: parameters for this function (see example)
     :type value: list
     """
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f14.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f14.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,31 +12,28 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 01 function 14."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import COMMACK, MDLN
+from secsgem.secs.data_items import COMMACK
+from secsgem.secs.data_items import MDLN
 
 
 class SecsS01F14(SecsStreamFunction):
     """
     establish communication - acknowledge.
 
     .. caution::
 
         This Stream/function has different structures depending on the source.
         See structure definition below for details.
         Be sure to fill the array accordingly.
 
-    **Data Items**
-
-    - :class:`COMMACK <secsgem.secs.data_items.COMMACK>`
-
     **Structure E->H**::
 
         {
             COMMACK: B[1]
             DATA: {
                 MDLN: A[20]
                 SOFTREV: A[20]
@@ -46,19 +43,36 @@
     **Structure H->E**::
 
         {
             COMMACK: B[1]
             DATA: []
         }
 
+    **Data Items**
+
+    - :class:`COMMACK <secsgem.secs.data_items.COMMACK>`
+    - :class:`MDLN <secsgem.secs.data_items.MDLN>`
+
+    **Structure**::
+
+        >>> import secsgem.secs
+        >>> secsgem.secs.functions.SecsS01F14
+        {
+            COMMACK: B[1]
+            MDLN: [
+                DATA: A[20]
+                ...
+            ]
+        }
+
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS01F14({"COMMACK": secsgem.secs.data_items.COMMACK.ACCEPTED, \
-                                               "MDLN": ["secsgem", "0.0.6"]})
+        >>> secsgem.secs.functions.SecsS01F14({"COMMACK": secsgem.secs.data_items.COMMACK.ACCEPTED,
+        ...     "MDLN": ["secsgem", "0.0.6"]})
         S1F14
           <L [2]
             <B 0x0>
             <L [2]
               <A "secsgem">
               <A "0.0.6">
             >
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f15.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f15.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f16.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f16.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS01F16(secsgem.secs.data_items.OFLACK.ACK)
         S1F16
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 1
     _function = 16
 
     _data_format = OFLACK
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f17.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f17.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s01f18.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f18.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS01F18(secsgem.secs.data_items.ONLACK.ALREADY_ON)
         S1F18
           <B 0x2> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 1
     _function = 18
 
     _data_format = ONLACK
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f13.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f13.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from secsgem.secs.data_items import ECID
 
 
 class SecsS02F13(SecsStreamFunction):
     """
     equipment constant - request.
 
+    An empty list will return all available equipment constants.
+
     **Data Items**
 
     - :class:`ECID <secsgem.secs.data_items.ECID>`
 
     **Structure**::
 
         >>> import secsgem.secs
@@ -42,16 +44,14 @@
         >>> secsgem.secs.functions.SecsS02F13([1, 1337])
         S2F13 W
           <L [2]
             <U1 1 >
             <U2 1337 >
           > .
 
-    An empty list will return all available equipment constants.
-
     :param value: parameters for this function (see example)
     :type value: list
     """
 
     _stream = 2
     _function = 13
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f14.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f02.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 #####################################################################
-# s02f14.py
+# s06f02.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 02 function 14."""
+"""Class for stream 06 function 02."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import ECV
+from secsgem.secs.data_items import ACKC6
 
 
-class SecsS02F14(SecsStreamFunction):
+class SecsS06F02(SecsStreamFunction):
     """
-    equipment constant - data.
+    Trace data - acknowledge.
 
     **Data Items**
 
-    - :class:`ECV <secsgem.secs.data_items.ECV>`
+    - :class:`ACKC6 <secsgem.secs.data_items.ACKC6>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F14
-        [
-            ECV: L/BOOLEAN/I8/I1/I2/I4/F8/F4/U8/U1/U2/U4/A/B
-            ...
-        ]
+        >>> secsgem.secs.functions.SecsS06F02
+        ACKC6: B[1]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F14([secsgem.secs.variables.U1(1), "text"])
-        S2F14
-          <L [2]
-            <U1 1 >
-            <A "text">
-          > .
+        >>> secsgem.secs.functions.SecsS06F02(secsgem.secs.data_items.ACKC6.ACCEPTED)
+        S6F2
+          <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: bytes
     """
 
-    _stream = 2
-    _function = 14
+    _stream = 6
+    _function = 2
 
-    _data_format = [ECV]
+    _data_format = ACKC6
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
     _has_reply = False
     _is_reply_required = False
 
-    _is_multi_block = True
+    _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f15.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f15.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 02 function 15."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import ECID, ECV
+from secsgem.secs.data_items import ECID
+from secsgem.secs.data_items import ECV
 
 
 class SecsS02F15(SecsStreamFunction):
     """
     new equipment constant - send.
 
     **Data Items**
@@ -39,17 +40,17 @@
             }
             ...
         ]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F15([ \
-                {"ECID": 1, "ECV": secsgem.secs.variables.U4(10)}, \
-                {"ECID": "1337", "ECV": "text"}])
+        >>> secsgem.secs.functions.SecsS02F15([
+        ...     {"ECID": 1, "ECV": secsgem.secs.variables.U4(10)},
+        ...     {"ECID": "1337", "ECV": "text"}])
         S2F15 W
           <L [2]
             <L [2]
               <U1 1 >
               <U4 10 >
             >
             <L [2]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f16.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f16.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS02F16(secsgem.secs.data_items.EAC.BUSY)
         S2F16
           <B 0x2> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 2
     _function = 16
 
     _data_format = EAC
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f17.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f17.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f18.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f18.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS02F18("160816205942")
         S2F18
           <A "160816205942"> .
 
     :param value: parameters for this function (see example)
-    :type value: ASCII string
+    :type value: bytes
     """
 
     _stream = 2
     _function = 18
 
     _data_format = TIME
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f29.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f29.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from secsgem.secs.data_items import ECID
 
 
 class SecsS02F29(SecsStreamFunction):
     """
     equipment constant namelist - request.
 
+    An empty list will return all available equipment constants.
+
     **Data Items**
 
     - :class:`ECID <secsgem.secs.data_items.ECID>`
 
     **Structure**::
 
         >>> import secsgem.secs
@@ -42,16 +44,14 @@
         >>> secsgem.secs.functions.SecsS02F29([1, 1337])
         S2F29 W
           <L [2]
             <U1 1 >
             <U2 1337 >
           > .
 
-    An empty list will return all available equipment constants.
-
     :param value: parameters for this function (see example)
     :type value: list
     """
 
     _stream = 2
     _function = 29
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f30.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f35.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,93 @@
 #####################################################################
-# s02f30.py
+# s02f35.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 02 function 30."""
+"""Class for stream 02 function 35."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import ECID, ECNAME, ECMIN, ECMAX, ECDEF, UNITS
+from secsgem.secs.data_items import DATAID
+from secsgem.secs.data_items import CEID
+from secsgem.secs.data_items import RPTID
 
 
-class SecsS02F30(SecsStreamFunction):
+class SecsS02F35(SecsStreamFunction):
     """
-    equipment constant namelist.
+    link event report.
 
     **Data Items**
 
-    - :class:`ECID <secsgem.secs.data_items.ECID>`
-    - :class:`ECNAME <secsgem.secs.data_items.ECNAME>`
-    - :class:`ECMIN <secsgem.secs.data_items.ECMIN>`
-    - :class:`ECMAX <secsgem.secs.data_items.ECMAX>`
-    - :class:`ECDEF <secsgem.secs.data_items.ECDEF>`
-    - :class:`UNITS <secsgem.secs.data_items.UNITS>`
+    - :class:`DATAID <secsgem.secs.data_items.DATAID>`
+    - :class:`CEID <secsgem.secs.data_items.CEID>`
+    - :class:`RPTID <secsgem.secs.data_items.RPTID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F30
-        [
-            {
-                ECID: U1/U2/U4/U8/I1/I2/I4/I8/A
-                ECNAME: A
-                ECMIN: BOOLEAN/I8/I1/I2/I4/F8/F4/U8/U1/U2/U4/A/B
-                ECMAX: BOOLEAN/I8/I1/I2/I4/F8/F4/U8/U1/U2/U4/A/B
-                ECDEF: BOOLEAN/I8/I1/I2/I4/F8/F4/U8/U1/U2/U4/A/B
-                UNITS: A
-            }
-            ...
-        ]
+        >>> secsgem.secs.functions.SecsS02F35
+        {
+            DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
+            DATA: [
+                {
+                    CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
+                    RPTID: [
+                        DATA: U1/U2/U4/U8/I1/I2/I4/I8/A
+                        ...
+                    ]
+                }
+                ...
+            ]
+        }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F30([ \
-            {"ECID": 1, \
-             "ECNAME": "EC1", \
-             "ECMIN": secsgem.secs.variables.U1(0), \
-             "ECMAX": secsgem.secs.variables.U1(100), \
-             "ECDEF": secsgem.secs.variables.U1(50), \
-             "UNITS": "mm"}, \
-            {"ECID": 1337, \
-             "ECNAME": "EC2", \
-             "ECMIN": "", \
-             "ECMAX": "", \
-             "ECDEF": "", \
-             "UNITS": ""}])
-        S2F30
+        >>> secsgem.secs.functions.SecsS02F35({"DATAID": 1, "DATA": [{"CEID": 1337, "RPTID": [1000, 1001]}]})
+        S2F35 W
           <L [2]
-            <L [6]
-              <U1 1 >
-              <A "EC1">
-              <U1 0 >
-              <U1 100 >
-              <U1 50 >
-              <A "mm">
-            >
-            <L [6]
-              <U2 1337 >
-              <A "EC2">
-              <A>
-              <A>
-              <A>
-              <A>
+            <U1 1 >
+            <L [1]
+              <L [2]
+                <U2 1337 >
+                <L [2]
+                  <U2 1000 >
+                  <U2 1001 >
+                >
+              >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 2
-    _function = 30
+    _function = 35
 
     _data_format = [
+        DATAID,
         [
-            ECID,
-            ECNAME,
-            ECMIN,
-            ECMAX,
-            ECDEF,
-            UNITS
+            [
+                CEID,
+                [RPTID]
+            ]
         ]
     ]
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
-    _has_reply = False
-    _is_reply_required = False
+    _has_reply = True
+    _is_reply_required = True
 
     _is_multi_block = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f33.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f33.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 02 function 33."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import DATAID, RPTID, VID
+from secsgem.secs.data_items import DATAID
+from secsgem.secs.data_items import RPTID
+from secsgem.secs.data_items import VID
 
 
 class SecsS02F33(SecsStreamFunction):
     """
     define report.
 
     **Data Items**
@@ -46,16 +48,16 @@
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F33({"DATAID": 1, "DATA": [{"RPTID": 1000, "VID": [12, 1337]}, \
-{"RPTID": 1001, "VID": [1, 2355]}]})
+        >>> secsgem.secs.functions.SecsS02F33({"DATAID": 1, "DATA": [{"RPTID": 1000, "VID": [12, 1337]},
+        ...     {"RPTID": 1001, "VID": [1, 2355]}]})
         S2F33 W
           <L [2]
             <U1 1 >
             <L [2]
               <L [2]
                 <U2 1000 >
                 <L [2]
@@ -70,15 +72,15 @@
                   <U2 2355 >
                 >
               >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 2
     _function = 33
 
     _data_format = [
         DATAID,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f34.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f34.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS02F34(secsgem.secs.data_items.DRACK.INVALID_FORMAT)
         S2F34
           <B 0x2> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 2
     _function = 34
 
     _data_format = DRACK
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f35.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f01.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,89 @@
 #####################################################################
-# s02f35.py
+# s06f01.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 02 function 35."""
+"""Class for stream 06 function 01."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import DATAID, CEID, RPTID
+from secsgem.secs.data_items import TRID
+from secsgem.secs.data_items import SMPLN
+from secsgem.secs.data_items import STIME
+from secsgem.secs.data_items import SV
 
 
-class SecsS02F35(SecsStreamFunction):
+class SecsS06F01(SecsStreamFunction):
     """
-    link event report.
+    Trace data send.
 
     **Data Items**
 
-    - :class:`DATAID <secsgem.secs.data_items.DATAID>`
-    - :class:`CEID <secsgem.secs.data_items.CEID>`
-    - :class:`RPTID <secsgem.secs.data_items.RPTID>`
+    - :class:`TRID <secsgem.secs.data_items.TRID>`
+    - :class:`SMPLN <secsgem.secs.data_items.SMPLN>`
+    - :class:`STIME <secsgem.secs.data_items.STIME>`
+    - :class:`SV <secsgem.secs.data_items.SV>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F35
+        >>> secsgem.secs.functions.SecsS06F01
         {
-            DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
-            DATA: [
-                {
-                    CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
-                    RPTID: [
-                        DATA: U1/U2/U4/U8/I1/I2/I4/I8/A
-                        ...
-                    ]
-                }
+            TRID: I1/I2/I4/I8/U1/U2/U4/U8/A
+            SMPLN: I1/I2/I4/I8/U1/U2/U4/U8
+            STIME: A
+            SV: [
+                DATA: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F35({"DATAID": 1, "DATA": [{"CEID": 1337, "RPTID": [1000, 1001]}]})
-        S2F35 W
-          <L [2]
-            <U1 1 >
-            <L [1]
-              <L [2]
-                <U2 1337 >
-                <L [2]
-                  <U2 1000 >
-                  <U2 1001 >
-                >
-              >
+        >>> secsgem.secs.functions.SecsS06F01({
+        ...     "TRID": 1,
+        ...     "SMPLN": 3,
+        ...     "STIME": "TIME",
+        ...     "SV": [1, 4]})
+        S6F1
+          <L [4]
+            <I1 1 >
+            <I1 3 >
+            <A "TIME">
+            <L [2]
+              <U1 1 >
+              <U1 4 >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
-    _stream = 2
-    _function = 35
+    _stream = 6
+    _function = 1
 
     _data_format = [
-        DATAID,
-        [
-            [
-                CEID,
-                [RPTID]
-            ]
-        ]
+        TRID,
+        SMPLN,
+        STIME,
+        [SV]
     ]
 
-    _to_host = False
-    _to_equipment = True
+    _to_host = True
+    _to_equipment = False
 
     _has_reply = True
-    _is_reply_required = True
+    _is_reply_required = False
 
     _is_multi_block = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f36.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f36.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,22 +37,22 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS02F36(secsgem.secs.data_items.LRACK.CEID_UNKNOWN)
         S2F36
           <B 0x4> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 2
     _function = 36
 
     _data_format = LRACK
 
-    _to_host = False
-    _to_equipment = True
+    _to_host = True
+    _to_equipment = False
 
     _has_reply = False
     _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f37.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f37.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 02 function 37."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import CEED, CEID
+from secsgem.secs.data_items import CEED
+from secsgem.secs.data_items import CEID
 
 
 class SecsS02F37(SecsStreamFunction):
     """
     en-/disable event report.
 
     **Data Items**
@@ -49,15 +50,15 @@
             <BOOLEAN True >
             <L [1]
               <U2 1337 >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 2
     _function = 37
 
     _data_format = [
         CEED,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f38.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f38.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS02F38(secsgem.secs.data_items.ERACK.CEID_UNKNOWN)
         S2F38
           <B 0x1> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 2
     _function = 38
 
     _data_format = ERACK
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f41.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f19.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,69 @@
 #####################################################################
-# s02f41.py
+# s12f19.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 02 function 41."""
+"""Class for stream 12 function 19."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import RCMD, CPNAME, CPVAL
+from secsgem.secs.data_items import MAPER
+from secsgem.secs.data_items import DATLC
 
 
-class SecsS02F41(SecsStreamFunction):
+class SecsS12F19(SecsStreamFunction):
     """
-    host command - send.
+    map error report - send.
 
     **Data Items**
 
-    - :class:`RCMD <secsgem.secs.data_items.RCMD>`
-    - :class:`CPNAME <secsgem.secs.data_items.CPNAME>`
-    - :class:`CPVAL <secsgem.secs.data_items.CPVAL>`
+    - :class:`MAPER <secsgem.secs.data_items.MAPER>`
+    - :class:`DATLC <secsgem.secs.data_items.DATLC>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F41
+        >>> secsgem.secs.functions.SecsS12F19
         {
-            RCMD: U1/I1/A
-            PARAMS: [
-                {
-                    CPNAME: U1/U2/U4/U8/I1/I2/I4/I8/A
-                    CPVAL: BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/A/B
-                }
-                ...
-            ]
+            MAPER: B[1]
+            DATLC: U1
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F41({"RCMD": "COMMAND", "PARAMS": [{"CPNAME": "PARAM1", "CPVAL": "VAL1"}, \
-{"CPNAME": "PARAM2", "CPVAL": "VAL2"}]})
-        S2F41 W
+        >>> secsgem.secs.functions.SecsS12F19({"MAPER": secsgem.secs.data_items.MAPER.INVALID_DATA, "DATLC": 0})
+        S12F19
           <L [2]
-            <A "COMMAND">
-            <L [2]
-              <L [2]
-                <A "PARAM1">
-                <A "VAL1">
-              >
-              <L [2]
-                <A "PARAM2">
-                <A "VAL2">
-              >
-            >
+            <B 0x1>
+            <U1 0 >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
-    _stream = 2
-    _function = 41
+    _stream = 12
+    _function = 19
 
     _data_format = [
-        RCMD,
-        [
-            [
-                "PARAMS",   # name of the list
-                CPNAME,
-                CPVAL
-            ]
-        ]
+        MAPER,
+        DATLC
     ]
 
-    _to_host = False
+    _to_host = True
     _to_equipment = True
 
-    _has_reply = True
-    _is_reply_required = True
+    _has_reply = False
+    _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s02f42.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f42.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 02 function 42."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import HCACK, CPNAME, CPACK
+from secsgem.secs.data_items import HCACK
+from secsgem.secs.data_items import CPNAME
+from secsgem.secs.data_items import CPACK
 
 
 class SecsS02F42(SecsStreamFunction):
     """
     host command - acknowledge.
 
     **Data Items**
@@ -43,19 +45,19 @@
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS02F42({ \
-            "HCACK": secsgem.secs.data_items.HCACK.INVALID_COMMAND, \
-            "PARAMS": [ \
-                {"CPNAME": "PARAM1", "CPACK": secsgem.secs.data_items.CPACK.CPVAL_ILLEGAL_VALUE}, \
-                {"CPNAME": "PARAM2", "CPACK": secsgem.secs.data_items.CPACK.CPVAL_ILLEGAL_FORMAT}]})
+        >>> secsgem.secs.functions.SecsS02F42({
+        ...     "HCACK": secsgem.secs.data_items.HCACK.INVALID_COMMAND,
+        ...     "PARAMS": [
+        ...         {"CPNAME": "PARAM1", "CPACK": secsgem.secs.data_items.CPACK.CPVAL_ILLEGAL_VALUE},
+        ...         {"CPNAME": "PARAM2", "CPACK": secsgem.secs.data_items.CPACK.CPVAL_ILLEGAL_FORMAT}]})
         S2F42
           <L [2]
             <B 0x1>
             <L [2]
               <L [2]
                 <A "PARAM1">
                 <B 0x2>
@@ -64,25 +66,25 @@
                 <A "PARAM2">
                 <B 0x3>
               >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 2
     _function = 42
 
     _data_format = [
         HCACK,
         [
             [
-                "PARAMS",   # name of the list
+                "PARAMS",
                 CPNAME,
                 CPACK
             ]
         ]
     ]
 
     _to_host = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f01.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f21.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,58 @@
 #####################################################################
-# s05f01.py
+# s02f21.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 01."""
+"""Class for stream 02 function 21."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import ALCD, ALID, ALTX
+from secsgem.secs.data_items import RCMD
 
 
-class SecsS05F01(SecsStreamFunction):
+class SecsS02F21(SecsStreamFunction):
     """
-    alarm report - send.
+    Remote command send.
 
     **Data Items**
 
-    - :class:`ALCD <secsgem.secs.data_items.ALCD>`
-    - :class:`ALID <secsgem.secs.data_items.ALID>`
-    - :class:`ALTX <secsgem.secs.data_items.ALTX>`
+    - :class:`RCMD <secsgem.secs.data_items.RCMD>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F01
-        {
-            ALCD: B[1]
-            ALID: U1/U2/U4/U8/I1/I2/I4/I8
-            ALTX: A[120]
-        }
+        >>> secsgem.secs.functions.SecsS02F21
+        RCMD: U1/I1/A
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F01({"ALCD": secsgem.secs.data_items.ALCD.PERSONAL_SAFETY | \
-                                                       secsgem.secs.data_items.ALCD.ALARM_SET, \
-                                               "ALID": 100, \
-                                               "ALTX": "text"})
-        S5F1
-          <L [3]
-            <B 0x81>
-            <U1 100 >
-            <A "text">
-          > .
+        >>> secsgem.secs.functions.SecsS02F21("COMMMAND1")
+        S2F21
+          <A "COMMMAND1"> .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: int
     """
 
-    _stream = 5
-    _function = 1
+    _stream = 2
+    _function = 21
 
-    _data_format = [
-        ALCD,
-        ALID,
-        ALTX
-    ]
+    _data_format = RCMD
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
     _has_reply = True
     _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f02.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f02.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS05F02(secsgem.secs.data_items.ACKC5.ACCEPTED)
         S5F2
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 5
     _function = 2
 
     _data_format = ACKC5
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f03.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f07.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,58 @@
 #####################################################################
-# s05f03.py
+# s06f07.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 03."""
+"""Class for stream 06 function 07."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import ALED, ALID
+from secsgem.secs.data_items import DATAID
 
 
-class SecsS05F03(SecsStreamFunction):
+class SecsS06F07(SecsStreamFunction):
     """
-    en-/disable alarm - send.
+    data transfer request.
 
     **Data Items**
 
-    - :class:`ALED <secsgem.secs.data_items.ALED>`
-    - :class:`ALID <secsgem.secs.data_items.ALID>`
+    - :class:`DATAID <secsgem.secs.data_items.DATAID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F03
-        {
-            ALED: B[1]
-            ALID: U1/U2/U4/U8/I1/I2/I4/I8
-        }
+        >>> secsgem.secs.functions.SecsS06F07
+        DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F03({"ALED": secsgem.secs.data_items.ALED.ENABLE, "ALID": 100})
-        S5F3
-          <L [2]
-            <B 0x80>
-            <U1 100 >
-          > .
+        >>> secsgem.secs.functions.SecsS06F07(1)
+        S6F7 W
+          <U1 1 > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: int
     """
 
-    _stream = 5
-    _function = 3
+    _stream = 6
+    _function = 7
 
-    _data_format = [
-        ALED,
-        ALID
-    ]
+    _data_format = DATAID
 
     _to_host = False
     _to_equipment = True
 
     _has_reply = True
-    _is_reply_required = False
+    _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f04.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f04.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS05F04(secsgem.secs.data_items.ACKC5.ACCEPTED)
         S5F4
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 5
     _function = 4
 
     _data_format = ACKC5
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f05.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f05.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f06.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f24.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 #####################################################################
-# s05f06.py
+# s01f24.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 06."""
+"""Class for stream 01 function 24."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import ALCD, ALID, ALTX
+from secsgem.secs.data_items import CEID
+from secsgem.secs.data_items import CENAME
+from secsgem.secs.data_items import VID
 
 
-class SecsS05F06(SecsStreamFunction):
+class SecsS01F24(SecsStreamFunction):
     """
-    list alarms - data.
+    Collection event namelist.
 
     **Data Items**
 
-    - :class:`ALCD <secsgem.secs.data_items.ALCD>`
-    - :class:`ALID <secsgem.secs.data_items.ALID>`
-    - :class:`ALTX <secsgem.secs.data_items.ALTX>`
+    - :class:`CEID <secsgem.secs.data_items.CEID>`
+    - :class:`CENAME <secsgem.secs.data_items.CENAME>`
+    - :class:`VID <secsgem.secs.data_items.VID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F06
+        >>> secsgem.secs.functions.SecsS01F24
         [
             {
-                ALCD: B[1]
-                ALID: U1/U2/U4/U8/I1/I2/I4/I8
-                ALTX: A[120]
+                CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
+                CENAME: A
+                VID: [
+                    DATA: U1/U2/U4/U8/I1/I2/I4/I8/A
+                    ...
+                ]
             }
             ...
         ]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F06([{"ALCD": secsgem.secs.data_items.ALCD.PERSONAL_SAFETY | \
-                                                        secsgem.secs.data_items.ALCD.ALARM_SET, \
-                                                "ALID": 100, \
-                                                "ALTX": "text"}])
-        S5F6
+        >>> secsgem.secs.functions.SecsS01F24([{"CEID": 1, "CENAME": "CE1", "VID": [1, "VARIABLEID"]}])
+        S1F24
           <L [1]
             <L [3]
-              <B 0x81>
-              <U1 100 >
-              <A "text">
+              <U1 1 >
+              <A "CE1">
+              <L [2]
+                <U1 1 >
+                <A "VARIABLEID">
+              >
             >
           > .
 
     :param value: parameters for this function (see example)
     :type value: list
     """
 
-    _stream = 5
-    _function = 6
+    _stream = 1
+    _function = 24
 
-    _data_format = [[
-        ALCD,
-        ALID,
-        ALTX
-    ]]
+    _data_format = [
+        [
+            CEID,
+            CENAME,
+            [VID]
+        ]
+    ]
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
     _is_reply_required = False
 
-    _is_multi_block = True
+    _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f07.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f26.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 #####################################################################
-# s05f07.py
+# s02f26.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 07."""
+"""Class for stream 02 function 26."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
+from secsgem.secs.data_items import ABS
 
 
-class SecsS05F07(SecsStreamFunction):
+class SecsS02F26(SecsStreamFunction):
     """
-    list enabled alarms - request.
+    Loopback diagnostic data.
+
+    **Data Items**
+
+    - :class:`ABS <secsgem.secs.data_items.ABS>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F07
-        Header only
+        >>> secsgem.secs.functions.SecsS02F26
+        ABS: B
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F07()
-        S5F7 W .
+        >>> secsgem.secs.functions.SecsS02F26("Text")
+        S2F26
+          <B 0x54 0x65 0x78 0x74> .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: bytes
     """
 
-    _stream = 5
-    _function = 7
+    _stream = 2
+    _function = 26
 
-    _data_format = None
+    _data_format = ABS
 
-    _to_host = False
+    _to_host = True
     _to_equipment = True
 
-    _has_reply = True
-    _is_reply_required = True
+    _has_reply = False
+    _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f08.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f22.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 #####################################################################
-# s05f08.py
+# s06f22.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 08."""
+"""Class for stream 06 function 22."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import ALCD, ALID, ALTX
+from secsgem.secs.data_items import VID
+from secsgem.secs.data_items import V
 
 
-class SecsS05F08(SecsStreamFunction):
+class SecsS06F22(SecsStreamFunction):
     """
-    list enabled alarms - data.
+    annotated individual report data.
 
     **Data Items**
 
-    - :class:`ALCD <secsgem.secs.data_items.ALCD>`
-    - :class:`ALID <secsgem.secs.data_items.ALID>`
-    - :class:`ALTX <secsgem.secs.data_items.ALTX>`
+    - :class:`VID <secsgem.secs.data_items.VID>`
+    - :class:`V <secsgem.secs.data_items.V>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F08
+        >>> secsgem.secs.functions.SecsS06F22
         [
             {
-                ALCD: B[1]
-                ALID: U1/U2/U4/U8/I1/I2/I4/I8
-                ALTX: A[120]
+                VID: U1/U2/U4/U8/I1/I2/I4/I8/A
+                V: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
             }
             ...
         ]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F08([{"ALCD": secsgem.secs.data_items.ALCD.PERSONAL_SAFETY | \
-                                                        secsgem.secs.data_items.ALCD.ALARM_SET, \
-                                                "ALID": 100, \
-                                                "ALTX": "text"}])
-        S5F8
-          <L [1]
-            <L [3]
-              <B 0x81>
-              <U1 100 >
-              <A "text">
+        >>> secsgem.secs.functions.SecsS06F22([{"VID": "VID1", "V": "ASD"}, {"VID": 2, "V": 1337}])
+        S6F22
+          <L [2]
+            <L [2]
+              <A "VID1">
+              <A "ASD">
+            >
+            <L [2]
+              <U1 2 >
+              <U2 1337 >
             >
           > .
 
     :param value: parameters for this function (see example)
     :type value: list
     """
 
-    _stream = 5
-    _function = 8
+    _stream = 6
+    _function = 22
 
-    _data_format = [[
-        ALCD,
-        ALID,
-        ALTX
-    ]]
+    _data_format = [
+        [
+            VID,
+            V
+        ]
+    ]
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
     _is_reply_required = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f09.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f09.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 05 function 09."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import TIMESTAMP, EXID, EXTYPE, EXMESSAGE, EXRECVRA
+from secsgem.secs.data_items import TIMESTAMP
+from secsgem.secs.data_items import EXID
+from secsgem.secs.data_items import EXTYPE
+from secsgem.secs.data_items import EXMESSAGE
+from secsgem.secs.data_items import EXRECVRA
 
 
 class SecsS05F09(SecsStreamFunction):
     """
     exception post - notify.
 
     **Data Items**
@@ -45,34 +49,34 @@
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F09({ \
-            "TIMESTAMP": "161006221500", \
-            "EXID": "EX123", \
-            "EXTYPE": "ALARM", \
-            "EXMESSAGE": "Exception", \
-            "EXRECVRA": ["EXRECVRA1", "EXRECVRA2"] })
+        >>> secsgem.secs.functions.SecsS05F09({
+        ...     "TIMESTAMP": "161006221500",
+        ...     "EXID": "EX123",
+        ...     "EXTYPE": "ALARM",
+        ...     "EXMESSAGE": "Exception",
+        ...     "EXRECVRA": ["EXRECVRA1", "EXRECVRA2"] })
         S5F9
           <L [5]
             <A "161006221500">
             <A "EX123">
             <A "ALARM">
             <A "Exception">
             <L [2]
               <A "EXRECVRA1">
               <A "EXRECVRA2">
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 5
     _function = 9
 
     _data_format = [
         TIMESTAMP,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f10.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f10.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f11.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f15.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,58 @@
 #####################################################################
-# s05f11.py
+# s06f15.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 11."""
+"""Class for stream 06 function 15."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import TIMESTAMP, EXID, EXTYPE, EXMESSAGE
+from secsgem.secs.data_items import CEID
 
 
-class SecsS05F11(SecsStreamFunction):
+class SecsS06F15(SecsStreamFunction):
     """
-    exception clear - notify.
+    event report request.
 
     **Data Items**
 
-    - :class:`TIMESTAMP <secsgem.secs.data_items.TIMESTAMP>`
-    - :class:`EXID <secsgem.secs.data_items.EXID>`
-    - :class:`EXTYPE <secsgem.secs.data_items.EXTYPE>`
-    - :class:`EXMESSAGE <secsgem.secs.data_items.EXMESSAGE>`
+    - :class:`CEID <secsgem.secs.data_items.CEID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F11
-        {
-            TIMESTAMP: A[32]
-            EXID: A[20]
-            EXTYPE: A
-            EXMESSAGE: A
-        }
+        >>> secsgem.secs.functions.SecsS06F15
+        CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F11({"TIMESTAMP": "161006221500", "EXID": "EX123", "EXTYPE": "ALARM", \
-"EXMESSAGE": "Exception"})
-        S5F11
-          <L [4]
-            <A "161006221500">
-            <A "EX123">
-            <A "ALARM">
-            <A "Exception">
-          > .
+        >>> secsgem.secs.functions.SecsS06F15(1337)
+        S6F15 W
+          <U2 1337 > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: int
     """
 
-    _stream = 5
-    _function = 11
+    _stream = 6
+    _function = 15
 
-    _data_format = [
-        TIMESTAMP,
-        EXID,
-        EXTYPE,
-        EXMESSAGE,
-    ]
+    _data_format = CEID
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
     _has_reply = True
-    _is_reply_required = False
+    _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f12.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f12.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f13.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f13.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 05 function 13."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import EXID, EXRECVRA
+from secsgem.secs.data_items import EXID
+from secsgem.secs.data_items import EXRECVRA
 
 
 class SecsS05F13(SecsStreamFunction):
     """
     exception recover - request.
 
     **Data Items**
@@ -44,15 +45,15 @@
         S5F13 W
           <L [2]
             <A "EX123">
             <A "EXRECVRA2">
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 5
     _function = 13
 
     _data_format = [
         EXID,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f14.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f05.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,69 @@
 #####################################################################
-# s05f14.py
+# s06f05.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 14."""
+"""Class for stream 06 function 05."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import EXID, ACKA, ERRCODE, ERRTEXT
+from secsgem.secs.data_items import DATAID
+from secsgem.secs.data_items import DATALENGTH
 
 
-class SecsS05F14(SecsStreamFunction):
+class SecsS06F05(SecsStreamFunction):
     """
-    exception recover - acknowledge.
+    multi block data inquiry.
 
     **Data Items**
 
-    - :class:`EXID <secsgem.secs.data_items.EXID>`
-    - :class:`ACKA <secsgem.secs.data_items.ACKA>`
-    - :class:`ERRCODE <secsgem.secs.data_items.ERRCODE>`
-    - :class:`ERRTEXT <secsgem.secs.data_items.ERRTEXT>`
+    - :class:`DATAID <secsgem.secs.data_items.DATAID>`
+    - :class:`DATALENGTH <secsgem.secs.data_items.DATALENGTH>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F14
+        >>> secsgem.secs.functions.SecsS06F05
         {
-            EXID: A[20]
-            DATA: {
-                ACKA: BOOLEAN[1]
-                DATA: {
-                    ERRCODE: I1/I2/I4/I8
-                    ERRTEXT: A[120]
-                }
-            }
+            DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
+            DATALENGTH: U1/U2/U4/U8/I1/I2/I4/I8
         }
 
     **Example**::
+
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F14({"EXID": "EX123", \
-                                               "DATA": {"ACKA": False, \
-                                                        "DATA": {"ERRCODE": 10, \
-                                                                 "ERRTEXT": "Error"}}})
-        S5F14
+        >>> secsgem.secs.functions.SecsS06F05({"DATAID": 1, "DATALENGTH": 1337})
+        S6F5 W
           <L [2]
-            <A "EX123">
-            <L [2]
-              <BOOLEAN False >
-              <L [2]
-                <I1 10 >
-                <A "Error">
-              >
-            >
+            <U1 1 >
+            <U2 1337 >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
-    _stream = 5
-    _function = 14
+    _stream = 6
+    _function = 5
 
     _data_format = [
-        EXID,
-        [
-            ACKA,
-            [
-                ERRCODE,
-                ERRTEXT
-            ]
-        ]
+        DATAID,
+        DATALENGTH
     ]
 
     _to_host = True
     _to_equipment = False
 
-    _has_reply = False
-    _is_reply_required = False
+    _has_reply = True
+    _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f15.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f43.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,92 +1,89 @@
 #####################################################################
-# s05f15.py
+# s02f43.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 05 function 15."""
+"""Class for stream 02 function 43."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import TIMESTAMP, EXID, ACKA, ERRCODE, ERRTEXT
+from secsgem.secs.data_items import STRID
+from secsgem.secs.data_items import FCNID
 
 
-class SecsS05F15(SecsStreamFunction):
+class SecsS02F43(SecsStreamFunction):
     """
-    exception recover complete - notify.
+    reset spooling streams and functions - send.
 
     **Data Items**
 
-    - :class:`TIMESTAMP <secsgem.secs.data_items.TIMESTAMP>`
-    - :class:`EXID <secsgem.secs.data_items.EXID>`
-    - :class:`ACKA <secsgem.secs.data_items.ACKA>`
-    - :class:`ERRCODE <secsgem.secs.data_items.ERRCODE>`
-    - :class:`ERRTEXT <secsgem.secs.data_items.ERRTEXT>`
+    - :class:`STRID <secsgem.secs.data_items.STRID>`
+    - :class:`FCNID <secsgem.secs.data_items.FCNID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F15
-        {
-            TIMESTAMP: A[32]
-            EXID: A[20]
-            DATA: {
-                ACKA: BOOLEAN[1]
-                DATA: {
-                    ERRCODE: I1/I2/I4/I8
-                    ERRTEXT: A[120]
-                }
+        >>> secsgem.secs.functions.SecsS02F43
+        [
+            {
+                STRID: U1[1]
+                FCNID: [
+                    DATA: U1[1]
+                    ...
+                ]
             }
-        }
+            ...
+        ]
 
     **Example**::
+
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F15({"TIMESTAMP": "161006221500", "EXID": "EX123", "DATA": \
-{"ACKA": False, "DATA": {"ERRCODE": 10, "ERRTEXT": "Error"}}})
-        S5F15
-          <L [3]
-            <A "161006221500">
-            <A "EX123">
+        >>> secsgem.secs.functions.SecsS02F43([{"STRID": 1, "FCNID": [10, 20]}, {"STRID": 2, "FCNID": [30, 40]}])
+        S2F43 W
+          <L [2]
+            <L [2]
+              <U1 1 >
+              <L [2]
+                <U1 10 >
+                <U1 20 >
+              >
+            >
             <L [2]
-              <BOOLEAN False >
+              <U1 2 >
               <L [2]
-                <I1 10 >
-                <A "Error">
+                <U1 30 >
+                <U1 40 >
               >
             >
           > .
 
     :param value: parameters for this function (see example)
     :type value: list
     """
 
-    _stream = 5
-    _function = 15
+    _stream = 2
+    _function = 43
 
     _data_format = [
-        TIMESTAMP,
-        EXID,
         [
-            ACKA,
-            [
-                ERRCODE,
-                ERRTEXT
-            ]
+            STRID,
+            [FCNID]
         ]
     ]
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
     _has_reply = True
-    _is_reply_required = False
+    _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f16.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f16.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f17.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f17.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS05F17("EX123")
         S5F17 W
           <A "EX123"> .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: bytes
     """
 
     _stream = 5
     _function = 17
 
     _data_format = EXID
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s05f18.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f18.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 05 function 18."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import EXID, ACKA, ERRCODE, ERRTEXT
+from secsgem.secs.data_items import EXID
+from secsgem.secs.data_items import ACKA
+from secsgem.secs.data_items import ERRCODE
+from secsgem.secs.data_items import ERRTEXT
 
 
 class SecsS05F18(SecsStreamFunction):
     """
     exception recover abort - acknowledge.
 
     **Data Items**
@@ -42,33 +45,37 @@
                     ERRCODE: I1/I2/I4/I8
                     ERRTEXT: A[120]
                 }
             }
         }
 
     **Example**::
+
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS05F18({"EXID": "EX123", \
-                                               "DATA": {"ACKA": False, \
-                                                        "DATA": {"ERRCODE": 10, \
-                                                                 "ERRTEXT": "Error"}}})
+        >>> secsgem.secs.functions.SecsS05F18({
+        ...     "EXID": "EX123",
+        ...     "DATA": {
+        ...         "ACKA": False,
+        ...         "DATA": {
+        ...             "ERRCODE": 10,
+        ...             "ERRTEXT": "Error"}}})
         S5F18
           <L [2]
             <A "EX123">
             <L [2]
               <BOOLEAN False >
               <L [2]
                 <I1 10 >
                 <A "Error">
               >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 5
     _function = 18
 
     _data_format = [
         EXID,
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f05.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f24.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,58 @@
 #####################################################################
-# s06f05.py
+# s02f24.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 05."""
+"""Class for stream 02 function 24."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import DATAID, DATALENGTH
+from secsgem.secs.data_items import TIAACK
 
 
-class SecsS06F05(SecsStreamFunction):
+class SecsS02F24(SecsStreamFunction):
     """
-    multi block data inquiry.
+    Trace initialize - acknowledge.
 
     **Data Items**
 
-    - :class:`DATAID <secsgem.secs.data_items.DATAID>`
-    - :class:`DATALENGTH <secsgem.secs.data_items.DATALENGTH>`
+    - :class:`TIAACK <secsgem.secs.data_items.TIAACK>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F05
-        {
-            DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
-            DATALENGTH: U1/U2/U4/U8/I1/I2/I4/I8
-        }
+        >>> secsgem.secs.functions.SecsS02F24
+        TIAACK: B[1]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F05({"DATAID": 1, "DATALENGTH": 1337})
-        S6F5 W
-          <L [2]
-            <U1 1 >
-            <U2 1337 >
-          > .
+        >>> secsgem.secs.functions.SecsS02F24(secsgem.secs.data_items.TIAACK.SVID_EXCEEDED)
+        S2F24
+          <B 0x1> .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: bytes
     """
 
-    _stream = 6
-    _function = 5
+    _stream = 2
+    _function = 24
 
-    _data_format = [
-        DATAID,
-        DATALENGTH
-    ]
+    _data_format = TIAACK
 
     _to_host = True
     _to_equipment = False
 
-    _has_reply = True
-    _is_reply_required = True
+    _has_reply = False
+    _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f06.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f06.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS06F06(secsgem.secs.data_items.GRANT6.BUSY)
         S6F6
           <B 0x1> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 6
     _function = 6
 
     _data_format = GRANT6
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f07.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f06.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 #####################################################################
-# s06f07.py
+# s12f06.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 07."""
+"""Class for stream 12 function 06."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import DATAID
+from secsgem.secs.data_items import GRNT1
 
 
-class SecsS06F07(SecsStreamFunction):
+class SecsS12F06(SecsStreamFunction):
     """
-    data transfer request.
+    map transmit - grant.
 
     **Data Items**
 
-    - :class:`DATAID <secsgem.secs.data_items.DATAID>`
+    - :class:`GRNT1 <secsgem.secs.data_items.GRNT1>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F07
-        DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
+        >>> secsgem.secs.functions.SecsS12F06
+        GRNT1: B[1]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F07(1)
-        S6F7 W
-          <U1 1 > .
+        >>> secsgem.secs.functions.SecsS12F06(secsgem.secs.data_items.GRNT1.MATERIALID_UNKNOWN)
+        S12F6
+          <B 0x5> .
 
     :param value: parameters for this function (see example)
-    :type value: integer
+    :type value: bytes
     """
 
-    _stream = 6
-    _function = 7
+    _stream = 12
+    _function = 6
 
-    _data_format = DATAID
+    _data_format = GRNT1
 
     _to_host = False
     _to_equipment = True
 
-    _has_reply = True
-    _is_reply_required = True
+    _has_reply = False
+    _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f08.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f16.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,100 @@
 #####################################################################
-# s06f08.py
+# s06f16.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 08."""
+"""Class for stream 06 function 16."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import DATAID, CEID, DSID, DVNAME, DVVAL
+from secsgem.secs.data_items import DATAID
+from secsgem.secs.data_items import CEID
+from secsgem.secs.data_items import RPTID
+from secsgem.secs.data_items import V
 
 
-class SecsS06F08(SecsStreamFunction):
+class SecsS06F16(SecsStreamFunction):
     """
-    data transfer data.
+    event report data.
 
     **Data Items**
 
     - :class:`DATAID <secsgem.secs.data_items.DATAID>`
     - :class:`CEID <secsgem.secs.data_items.CEID>`
-    - :class:`DSID <secsgem.secs.data_items.DSID>`
-    - :class:`DVNAME <secsgem.secs.data_items.DVNAME>`
+    - :class:`RPTID <secsgem.secs.data_items.RPTID>`
+    - :class:`V <secsgem.secs.data_items.V>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F08
+        >>> secsgem.secs.functions.SecsS06F16
         {
             DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
             CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
-            DS: [
+            RPT: [
                 {
-                    DSID: U1/U2/U4/U8/I1/I2/I4/I8/A
-                    DV: [
-                        {
-                            DVNAME: U1/U2/U4/U8/I1/I2/I4/I8/A
-                            DVVAL: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
-                        }
+                    RPTID: U1/U2/U4/U8/I1/I2/I4/I8/A
+                    V: [
+                        DATA: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
                         ...
                     ]
                 }
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F08({ \
-            "DATAID": 1, \
-            "CEID": 1337, \
-            "DS": [{ \
-                "DSID": 1000, \
-                "DV": [ \
-                    {"DVNAME": "VAR1", "DVVAL": "VAR"}, \
-                    {"DVNAME": "VAR2", "DVVAL": secsgem.secs.variables.U4(100)}]}]})
-        S6F8
+        >>> secsgem.secs.functions.SecsS06F16({
+        ...     "DATAID": 1,
+        ...     "CEID": 1337,
+        ...     "RPT": [{
+        ...         "RPTID": 1000,
+        ...         "V": ["VAR", secsgem.secs.variables.U4(100)]}]})
+        S6F16
           <L [3]
             <U1 1 >
             <U2 1337 >
             <L [1]
               <L [2]
                 <U2 1000 >
                 <L [2]
-                  <L [2]
-                    <A "VAR1">
-                    <A "VAR">
-                  >
-                  <L [2]
-                    <A "VAR2">
-                    <U4 100 >
-                  >
+                  <A "VAR">
+                  <U4 100 >
                 >
               >
             >
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
     _stream = 6
-    _function = 8
+    _function = 16
 
     _data_format = [
         DATAID,
         CEID,
         [
             [
-                "DS",   # name of the list
-                DSID,
-                [
-                    [
-                        "DV",   # name of the list
-                        DVNAME,
-                        DVVAL
-                    ]
-                ]
+                "RPT",
+                RPTID,
+                [V]
             ]
         ]
     ]
 
     _to_host = True
     _to_equipment = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f11.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f11.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 06 function 11."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import DATAID, CEID, RPTID, V
+from secsgem.secs.data_items import DATAID
+from secsgem.secs.data_items import CEID
+from secsgem.secs.data_items import RPTID
+from secsgem.secs.data_items import V
 
 
 class SecsS06F11(SecsStreamFunction):
     """
     event report.
 
     **Data Items**
@@ -48,16 +51,20 @@
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F11({"DATAID": 1, "CEID": 1337, "RPT": [{"RPTID": 1000, "V": \
-["VAR", secsgem.secs.variables.U4(100)]}]})
+        >>> secsgem.secs.functions.SecsS06F11({
+        ...     "DATAID": 1,
+        ...     "CEID": 1337,
+        ...     "RPT": [{
+        ...         "RPTID": 1000,
+        ...         "V": ["VAR", secsgem.secs.variables.U4(100)]}]})
         S6F11 W
           <L [3]
             <U1 1 >
             <U2 1337 >
             <L [1]
               <L [2]
                 <U2 1000 >
@@ -66,26 +73,26 @@
                   <U4 100 >
                 >
               >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
     _stream = 6
     _function = 11
 
     _data_format = [
         DATAID,
         CEID,
         [
             [
-                "RPT",   # name of the list
+                "RPT",
                 RPTID,
                 [V]
             ]
         ]
     ]
 
     _to_host = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f12.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f12.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS06F12(secsgem.secs.data_items.ACKC6.ACCEPTED)
         S6F12
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 6
     _function = 12
 
     _data_format = ACKC6
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f15.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f23.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 #####################################################################
-# s06f15.py
+# s01f23.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 15."""
+"""Class for stream 01 function 23."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
 from secsgem.secs.data_items import CEID
 
 
-class SecsS06F15(SecsStreamFunction):
+class SecsS01F23(SecsStreamFunction):
     """
-    event report request.
+    Collection event namelist request.
 
     **Data Items**
 
     - :class:`CEID <secsgem.secs.data_items.CEID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F15
-        CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
+        >>> secsgem.secs.functions.SecsS01F23
+        [
+            CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
+            ...
+        ]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F15(1337)
-        S6F15 W
-          <U2 1337 > .
+        >>> secsgem.secs.functions.SecsS01F23([1, "COLLEVTID"])
+        S1F23 W
+          <L [2]
+            <U1 1 >
+            <A "COLLEVTID">
+          > .
 
     :param value: parameters for this function (see example)
     :type value: list
     """
 
-    _stream = 6
-    _function = 15
+    _stream = 1
+    _function = 23
 
-    _data_format = CEID
+    _data_format = [CEID]
 
     _to_host = False
     _to_equipment = True
 
     _has_reply = True
     _is_reply_required = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f16.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f50.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,96 @@
 #####################################################################
-# s06f16.py
+# s02f50.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 16."""
+"""Class for stream 02 function 50."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import DATAID, CEID, RPTID, V
+from secsgem.secs.data_items import HCACK
+from secsgem.secs.data_items import CPNAME
+from secsgem.secs.data_items import CPACK
 
 
-class SecsS06F16(SecsStreamFunction):
+class SecsS02F50(SecsStreamFunction):
     """
-    event report data.
+    Enhanced remote command - acknowledge.
 
     **Data Items**
 
-    - :class:`DATAID <secsgem.secs.data_items.DATAID>`
-    - :class:`CEID <secsgem.secs.data_items.CEID>`
-    - :class:`RPTID <secsgem.secs.data_items.RPTID>`
-    - :class:`V <secsgem.secs.data_items.V>`
+    - :class:`HCACK <secsgem.secs.data_items.HCACK>`
+    - :class:`CPNAME <secsgem.secs.data_items.CPNAME>`
+    - :class:`CPACK <secsgem.secs.data_items.CPACK>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F16
+        >>> secsgem.secs.functions.SecsS02F50
         {
-            DATAID: U1/U2/U4/U8/I1/I2/I4/I8/A
-            CEID: U1/U2/U4/U8/I1/I2/I4/I8/A
-            RPT: [
+            HCACK: B[1]
+            PARAMS: [
                 {
-                    RPTID: U1/U2/U4/U8/I1/I2/I4/I8/A
-                    V: [
-                        DATA: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
-                        ...
-                    ]
+                    CPNAME: U1/U2/U4/U8/I1/I2/I4/I8/A
+                    CPACK: B[1]
                 }
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F16({"DATAID": 1, "CEID": 1337, "RPT": [{"RPTID": 1000, "V": \
-["VAR", secsgem.secs.variables.U4(100)]}]})
-        S6F16
-          <L [3]
-            <U1 1 >
-            <U2 1337 >
-            <L [1]
+        >>> secsgem.secs.functions.SecsS02F50({
+        ...     "HCACK": secsgem.secs.data_items.HCACK.INVALID_COMMAND,
+        ...     "PARAMS": [
+        ...         {"CPNAME": "PARAM1", "CPACK": secsgem.secs.data_items.CPACK.CPVAL_ILLEGAL_VALUE},
+        ...         {"CPNAME": "PARAM2", "CPACK": secsgem.secs.data_items.CPACK.CPVAL_ILLEGAL_FORMAT}]})
+        S2F50
+          <L [2]
+            <B 0x1>
+            <L [2]
               <L [2]
-                <U2 1000 >
-                <L [2]
-                  <A "VAR">
-                  <U4 100 >
-                >
+                <A "PARAM1">
+                <B 0x2>
+              >
+              <L [2]
+                <A "PARAM2">
+                <B 0x3>
               >
             >
           > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: dict
     """
 
-    _stream = 6
-    _function = 16
+    _stream = 2
+    _function = 50
 
     _data_format = [
-        DATAID,
-        CEID,
+        HCACK,
         [
             [
-                "RPT",   # name of the list
-                RPTID,
-                [V]
+                "PARAMS",
+                CPNAME,
+                CPACK
             ]
         ]
     ]
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
     _is_reply_required = False
 
-    _is_multi_block = True
+    _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f19.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f21.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #####################################################################
-# s06f19.py
+# s06f21.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 19."""
+"""Class for stream 06 function 21."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
 from secsgem.secs.data_items import RPTID
 
 
-class SecsS06F19(SecsStreamFunction):
+class SecsS06F21(SecsStreamFunction):
     """
-    individual report request.
+    annotated individual report request.
 
     **Data Items**
 
     - :class:`RPTID <secsgem.secs.data_items.RPTID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F19
+        >>> secsgem.secs.functions.SecsS06F21
         RPTID: U1/U2/U4/U8/I1/I2/I4/I8/A
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F19(secsgem.secs.variables.U4(1337))
-        S6F19 W
+        >>> secsgem.secs.functions.SecsS06F21(secsgem.secs.variables.U4(1337))
+        S6F21 W
           <U4 1337 > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: int
     """
 
     _stream = 6
-    _function = 19
+    _function = 21
 
     _data_format = RPTID
 
     _to_host = False
     _to_equipment = True
 
     _has_reply = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f20.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f20.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f21.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s06f19.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #####################################################################
-# s06f21.py
+# s06f19.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 21."""
+"""Class for stream 06 function 19."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
 from secsgem.secs.data_items import RPTID
 
 
-class SecsS06F21(SecsStreamFunction):
+class SecsS06F19(SecsStreamFunction):
     """
-    annotated individual report request.
+    individual report request.
 
     **Data Items**
 
     - :class:`RPTID <secsgem.secs.data_items.RPTID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F21
+        >>> secsgem.secs.functions.SecsS06F19
         RPTID: U1/U2/U4/U8/I1/I2/I4/I8/A
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F21(secsgem.secs.variables.U4(1337))
-        S6F21 W
+        >>> secsgem.secs.functions.SecsS06F19(secsgem.secs.variables.U4(1337))
+        S6F19 W
           <U4 1337 > .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: int
     """
 
     _stream = 6
-    _function = 21
+    _function = 19
 
     _data_format = RPTID
 
     _to_host = False
     _to_equipment = True
 
     _has_reply = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s06f22.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f09.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,58 @@
 #####################################################################
-# s06f22.py
+# s09f09.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 06 function 22."""
+"""Class for stream 09 function 09."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import VID, V
+from secsgem.secs.data_items import SHEAD
 
 
-class SecsS06F22(SecsStreamFunction):
+class SecsS09F09(SecsStreamFunction):
     """
-    annotated individual report data.
+    transaction timer timeout.
 
     **Data Items**
 
-    - :class:`VID <secsgem.secs.data_items.VID>`
-    - :class:`V <secsgem.secs.data_items.V>`
+    - :class:`SHEAD <secsgem.secs.data_items.SHEAD>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F22
-        [
-            {
-                VID: U1/U2/U4/U8/I1/I2/I4/I8/A
-                V: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
-            }
-            ...
-        ]
+        >>> secsgem.secs.functions.SecsS09F09
+        SHEAD: B[10]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS06F22([{"VID": "VID1", "V": "ASD"}, {"VID": 2, "V": 1337}])
-        S6F22
-          <L [2]
-            <L [2]
-              <A "VID1">
-              <A "ASD">
-            >
-            <L [2]
-              <U1 2 >
-              <U2 1337 >
-            >
-          > .
+        >>> secsgem.secs.functions.SecsS09F09("HEADERDATA")
+        S9F9
+          <B 0x48 0x45 0x41 0x44 0x45 0x52 0x44 0x41 0x54 0x41> .
 
     :param value: parameters for this function (see example)
-    :type value: list
+    :type value: bytes
     """
 
-    _stream = 6
-    _function = 22
+    _stream = 9
+    _function = 9
 
-    _data_format = [
-        [
-            VID,
-            V
-        ]
-    ]
+    _data_format = SHEAD
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
     _is_reply_required = False
 
-    _is_multi_block = True
+    _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f01.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f01.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 07 function 01."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import PPID, LENGTH
+from secsgem.secs.data_items import PPID
+from secsgem.secs.data_items import LENGTH
 
 
 class SecsS07F01(SecsStreamFunction):
     """
     process program load - inquire.
 
     **Data Items**
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f02.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f02.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS07F02(secsgem.secs.data_items.PPGNT.OK)
         S7F2
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 7
     _function = 2
 
     _data_format = PPGNT
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f03.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f03.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 07 function 03."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import PPID, PPBODY
+from secsgem.secs.data_items import PPID
+from secsgem.secs.data_items import PPBODY
 
 
 class SecsS07F03(SecsStreamFunction):
     """
     process program - send.
 
     **Data Items**
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f04.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f04.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS07F04(secsgem.secs.data_items.ACKC7.MATRIX_OVERFLOW)
         S7F4
           <B 0x3> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 7
     _function = 4
 
     _data_format = ACKC7
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f05.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f05.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS07F05("program")
         S7F5 W
           <A "program"> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 7
     _function = 5
 
     _data_format = PPID
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f06.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f06.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 07 function 06."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import PPID, PPBODY
+from secsgem.secs.data_items import PPID
+from secsgem.secs.data_items import PPBODY
 
 
 class SecsS07F06(SecsStreamFunction):
     """
     process program - data.
 
     **Data Items**
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f17.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f17.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         S7F17 W
           <L [2]
             <A "program1">
             <A "program2">
           > .
 
     :param value: parameters for this function (see example)
-    :type value: dict
+    :type value: list
     """
 
     _stream = 7
     _function = 17
 
     _data_format = [PPID]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f18.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f18.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS07F18(secsgem.secs.data_items.ACKC7.MODE_UNSUPPORTED)
         S7F18
           <B 0x5> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 7
     _function = 18
 
     _data_format = ACKC7
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f19.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f19.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
     **Example**::
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS07F19()
         S7F19 W .
 
-    :param value: parameters for this function (see example)
-    :type value: dict
+    :param value: function has no parameters
+    :type value: None
     """
 
     _stream = 7
     _function = 19
 
     _data_format = None
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s07f20.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s07f20.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         S7F20
           <L [2]
             <A "program1">
             <A "program2">
           > .
 
     :param value: parameters for this function (see example)
-    :type value: dict
+    :type value: list
     """
 
     _stream = 7
     _function = 20
 
     _data_format = [PPID]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f01.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f01.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS09F01("HEADERDATA")
         S9F1
           <B 0x48 0x45 0x41 0x44 0x45 0x52 0x44 0x41 0x54 0x41> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 9
     _function = 1
 
     _data_format = MHEAD
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f03.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f05.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #####################################################################
-# s09f03.py
+# s09f05.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 09 function 03."""
+"""Class for stream 09 function 05."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
 from secsgem.secs.data_items import MHEAD
 
 
-class SecsS09F03(SecsStreamFunction):
+class SecsS09F05(SecsStreamFunction):
     """
-    unrecognized stream type.
+    unrecognized function type.
 
     **Data Items**
 
     - :class:`MHEAD <secsgem.secs.data_items.MHEAD>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F03
+        >>> secsgem.secs.functions.SecsS09F05
         MHEAD: B[10]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F03("HEADERDATA")
-        S9F3
+        >>> secsgem.secs.functions.SecsS09F05("HEADERDATA")
+        S9F5
           <B 0x48 0x45 0x41 0x44 0x45 0x52 0x44 0x41 0x54 0x41> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 9
-    _function = 3
+    _function = 5
 
     _data_format = MHEAD
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f05.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f07.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #####################################################################
-# s09f05.py
+# s09f07.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 09 function 05."""
+"""Class for stream 09 function 07."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
 from secsgem.secs.data_items import MHEAD
 
 
-class SecsS09F05(SecsStreamFunction):
+class SecsS09F07(SecsStreamFunction):
     """
-    unrecognized function type.
+    illegal data.
 
     **Data Items**
 
     - :class:`MHEAD <secsgem.secs.data_items.MHEAD>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F05
+        >>> secsgem.secs.functions.SecsS09F07
         MHEAD: B[10]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F05("HEADERDATA")
-        S9F5
+        >>> secsgem.secs.functions.SecsS09F07("HEADERDATA")
+        S9F7
           <B 0x48 0x45 0x41 0x44 0x45 0x52 0x44 0x41 0x54 0x41> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 9
-    _function = 5
+    _function = 7
 
     _data_format = MHEAD
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f07.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f11.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #####################################################################
-# s09f07.py
+# s09f11.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 09 function 07."""
+"""Class for stream 09 function 11."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
 from secsgem.secs.data_items import MHEAD
 
 
-class SecsS09F07(SecsStreamFunction):
+class SecsS09F11(SecsStreamFunction):
     """
-    illegal data.
+    data too long.
 
     **Data Items**
 
     - :class:`MHEAD <secsgem.secs.data_items.MHEAD>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F07
+        >>> secsgem.secs.functions.SecsS09F11
         MHEAD: B[10]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F07("HEADERDATA")
-        S9F7
+        >>> secsgem.secs.functions.SecsS09F11("HEADERDATA")
+        S9F11
           <B 0x48 0x45 0x41 0x44 0x45 0x52 0x44 0x41 0x54 0x41> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 9
-    _function = 7
+    _function = 11
 
     _data_format = MHEAD
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f09.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s10f01.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,69 @@
 #####################################################################
-# s09f09.py
+# s10f01.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 09 function 09."""
+"""Class for stream 10 function 01."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import SHEAD
+from secsgem.secs.data_items import TID
+from secsgem.secs.data_items import TEXT
 
 
-class SecsS09F09(SecsStreamFunction):
+class SecsS10F01(SecsStreamFunction):
     """
-    transaction timer timeout.
+    terminal - request.
 
     **Data Items**
 
-    - :class:`SHEAD <secsgem.secs.data_items.SHEAD>`
+    - :class:`TID <secsgem.secs.data_items.TID>`
+    - :class:`TEXT <secsgem.secs.data_items.TEXT>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F09
-        SHEAD: B[10]
+        >>> secsgem.secs.functions.SecsS10F01
+        {
+            TID: B[1]
+            TEXT: U1/U2/U4/U8/I1/I2/I4/I8/A/B
+        }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F09("HEADERDATA")
-        S9F9
-          <B 0x48 0x45 0x41 0x44 0x45 0x52 0x44 0x41 0x54 0x41> .
+        >>> secsgem.secs.functions.SecsS10F01({"TID": 0, "TEXT": "hello?"})
+        S10F1
+          <L [2]
+            <B 0x0>
+            <A "hello?">
+          > .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: dict
     """
 
-    _stream = 9
-    _function = 9
+    _stream = 10
+    _function = 1
 
-    _data_format = SHEAD
+    _data_format = [
+        TID,
+        TEXT
+    ]
 
     _to_host = True
     _to_equipment = False
 
-    _has_reply = False
+    _has_reply = True
     _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f11.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f03.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #####################################################################
-# s09f11.py
+# s09f03.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 09 function 11."""
+"""Class for stream 09 function 03."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
 from secsgem.secs.data_items import MHEAD
 
 
-class SecsS09F11(SecsStreamFunction):
+class SecsS09F03(SecsStreamFunction):
     """
-    data too long.
+    unrecognized stream type.
 
     **Data Items**
 
     - :class:`MHEAD <secsgem.secs.data_items.MHEAD>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F11
+        >>> secsgem.secs.functions.SecsS09F03
         MHEAD: B[10]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F11("HEADERDATA")
-        S9F11
+        >>> secsgem.secs.functions.SecsS09F03("HEADERDATA")
+        S9F3
           <B 0x48 0x45 0x41 0x44 0x45 0x52 0x44 0x41 0x54 0x41> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 9
-    _function = 11
+    _function = 3
 
     _data_format = MHEAD
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s09f13.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f07.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,52 @@
 #####################################################################
-# s09f13.py
+# s05f07.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 09 function 13."""
+"""Class for stream 05 function 07."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MEXP, EDID
 
 
-class SecsS09F13(SecsStreamFunction):
+class SecsS05F07(SecsStreamFunction):
     """
-    conversation timeout.
-
-    **Data Items**
-
-    - :class:`MEXP <secsgem.secs.data_items.MEXP>`
-    - :class:`EDID <secsgem.secs.data_items.EDID>`
+    list enabled alarms - request.
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F13
-        {
-            MEXP: A[6]
-            EDID: U1/U2/U4/U8/I1/I2/I4/I8/A/B
-        }
+        >>> secsgem.secs.functions.SecsS05F07
+        Header only
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS09F13({"MEXP": "S01E01", "EDID": "data"})
-        S9F13
-          <L [2]
-            <A "S01E01">
-            <A "data">
-          > .
+        >>> secsgem.secs.functions.SecsS05F07()
+        S5F7 W .
 
-    :param value: parameters for this function (see example)
-    :type value: dict
+    :param value: function has no parameters
+    :type value: None
     """
 
-    _stream = 9
-    _function = 13
+    _stream = 5
+    _function = 7
 
-    _data_format = [
-        MEXP,
-        EDID
-    ]
+    _data_format = None
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
-    _has_reply = False
-    _is_reply_required = False
+    _has_reply = True
+    _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s10f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s10f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s10f01.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s10f03.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 #####################################################################
-# s10f01.py
+# s10f03.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 10 function 01."""
+"""Class for stream 10 function 03."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import TID, TEXT
+from secsgem.secs.data_items import TID
+from secsgem.secs.data_items import TEXT
 
 
-class SecsS10F01(SecsStreamFunction):
+class SecsS10F03(SecsStreamFunction):
     """
-    terminal - request.
+    terminal single - display.
 
     **Data Items**
 
     - :class:`TID <secsgem.secs.data_items.TID>`
     - :class:`TEXT <secsgem.secs.data_items.TEXT>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS10F01
+        >>> secsgem.secs.functions.SecsS10F03
         {
             TID: B[1]
             TEXT: U1/U2/U4/U8/I1/I2/I4/I8/A/B
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS10F01({"TID": 0, "TEXT": "hello?"})
-        S10F1
+        >>> secsgem.secs.functions.SecsS10F03({"TID": 0, "TEXT": "hello!"})
+        S10F3
           <L [2]
             <B 0x0>
-            <A "hello?">
+            <A "hello!">
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
     _stream = 10
-    _function = 1
+    _function = 3
 
     _data_format = [
         TID,
         TEXT
     ]
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
     _has_reply = True
     _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s10f02.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s10f02.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS10F02(secsgem.secs.data_items.ACKC10.ACCEPTED)
         S10F2
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 10
     _function = 2
 
     _data_format = ACKC10
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s10f03.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f03.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 #####################################################################
-# s10f03.py
+# s05f03.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 10 function 03."""
+"""Class for stream 05 function 03."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import TID, TEXT
+from secsgem.secs.data_items import ALED
+from secsgem.secs.data_items import ALID
 
 
-class SecsS10F03(SecsStreamFunction):
+class SecsS05F03(SecsStreamFunction):
     """
-    terminal single - display.
+    en-/disable alarm - send.
 
     **Data Items**
 
-    - :class:`TID <secsgem.secs.data_items.TID>`
-    - :class:`TEXT <secsgem.secs.data_items.TEXT>`
+    - :class:`ALED <secsgem.secs.data_items.ALED>`
+    - :class:`ALID <secsgem.secs.data_items.ALID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS10F03
+        >>> secsgem.secs.functions.SecsS05F03
         {
-            TID: B[1]
-            TEXT: U1/U2/U4/U8/I1/I2/I4/I8/A/B
+            ALED: B[1]
+            ALID: U1/U2/U4/U8/I1/I2/I4/I8
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS10F03({"TID": 0, "TEXT": "hello!"})
-        S10F3
+        >>> secsgem.secs.functions.SecsS05F03({"ALED": secsgem.secs.data_items.ALED.ENABLE, "ALID": 100})
+        S5F3
           <L [2]
-            <B 0x0>
-            <A "hello!">
+            <B 0x80>
+            <U1 100 >
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
-    _stream = 10
+    _stream = 5
     _function = 3
 
     _data_format = [
-        TID,
-        TEXT
+        ALED,
+        ALID
     ]
 
     _to_host = False
     _to_equipment = True
 
     _has_reply = True
     _is_reply_required = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s10f04.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s10f04.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS10F04(secsgem.secs.data_items.ACKC10.TERMINAL_NOT_AVAILABLE)
         S10F4
           <B 0x2> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 10
     _function = 4
 
     _data_format = ACKC10
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f01.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s14f04.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,157 @@
 #####################################################################
-# s12f01.py
+# s14f04.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 01."""
+"""Class for stream 14 function 04."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, FNLOC, FFROT, ORLOC, RPSEL, REFP, DUTMS, XDIES, YDIES, ROWCT, COLCT, \
-    NULBC, PRDCT, PRAXI
+from secsgem.secs.data_items import OBJID
+from secsgem.secs.data_items import ATTRID
+from secsgem.secs.data_items import ATTRDATA
+from secsgem.secs.data_items import OBJACK
+from secsgem.secs.data_items import ERRCODE
+from secsgem.secs.data_items import ERRTEXT
 
 
-class SecsS12F01(SecsStreamFunction):
+class SecsS14F04(SecsStreamFunction):
     """
-    map setup data - send.
+    SetAttr data.
 
     **Data Items**
 
-    - :class:`MID <secsgem.secs.data_items.MID>`
-    - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
-    - :class:`FNLOC <secsgem.secs.data_items.FNLOC>`
-    - :class:`FFROT <secsgem.secs.data_items.FFROT>`
-    - :class:`ORLOC <secsgem.secs.data_items.ORLOC>`
-    - :class:`RPSEL <secsgem.secs.data_items.RPSEL>`
-    - :class:`REFP <secsgem.secs.data_items.REFP>`
-    - :class:`DUTMS <secsgem.secs.data_items.DUTMS>`
-    - :class:`XDIES <secsgem.secs.data_items.XDIES>`
-    - :class:`YDIES <secsgem.secs.data_items.YDIES>`
-    - :class:`ROWCT <secsgem.secs.data_items.ROWCT>`
-    - :class:`COLCT <secsgem.secs.data_items.COLCT>`
-    - :class:`NULBC <secsgem.secs.data_items.NULBC>`
-    - :class:`PRDCT <secsgem.secs.data_items.PRDCT>`
-    - :class:`PRAXI <secsgem.secs.data_items.PRAXI>`
+    - :class:`OBJID <secsgem.secs.data_items.OBJID>`
+    - :class:`ATTRID <secsgem.secs.data_items.ATTRID>`
+    - :class:`ATTRDATA <secsgem.secs.data_items.ATTRDATA>`
+    - :class:`OBJACK <secsgem.secs.data_items.OBJACK>`
+    - :class:`ERRCODE <secsgem.secs.data_items.ERRCODE>`
+    - :class:`ERRTEXT <secsgem.secs.data_items.ERRTEXT>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F01
+        >>> secsgem.secs.functions.SecsS14F04
         {
-            MID: A/B[80]
-            IDTYP: B[1]
-            FNLOC: U2
-            FFROT: U2
-            ORLOC: B
-            RPSEL: U1
-            REFP: [
-                DATA: I1/I2/I4/I8
+            DATA: [
+                {
+                    OBJID: U1/U2/U4/U8/A
+                    ATTRIBS: [
+                        {
+                            ATTRID: U1/U2/U4/U8/A
+                            ATTRDATA: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
+                        }
+                        ...
+                    ]
+                }
                 ...
             ]
-            DUTMS: A
-            XDIES: U1/U2/U4/U8/F4/F8
-            YDIES: U1/U2/U4/U8/F4/F8
-            ROWCT: U1/U2/U4/U8
-            COLCT: U1/U2/U4/U8
-            NULBC: U1/A
-            PRDCT: U1/U2/U4/U8
-            PRAXI: B[1]
+            ERRORS: {
+                OBJACK: U1[1]
+                ERROR: [
+                    {
+                        ERRCODE: I1/I2/I4/I8
+                        ERRTEXT: A[120]
+                    }
+                    ...
+                ]
+            }
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F01({"MID": "materialID", \
-                "IDTYP": secsgem.secs.data_items.IDTYP.WAFER, \
-                "FNLOC": 0, \
-                "FFROT": 0, \
-                "ORLOC": secsgem.secs.data_items.ORLOC.UPPER_LEFT, \
-                "RPSEL": 0, \
-                "REFP": [[1,2], [2,3]], \
-                "DUTMS": "unit", \
-                "XDIES": 100, \
-                "YDIES": 100, \
-                "ROWCT": 10, \
-                "COLCT": 10, \
-                "NULBC": "{x}", \
-                "PRDCT": 100, \
-                "PRAXI": secsgem.secs.data_items.PRAXI.ROWS_TOP_INCR, \
-                })
-        S12F1 W
-          <L [15]
-            <A "materialID">
-            <B 0x0>
-            <U2 0 >
-            <U2 0 >
-            <B 0x2>
-            <U1 0 >
+        >>> secsgem.secs.functions.SecsS14F04({
+        ...     "DATA": [{
+        ...         "OBJID": "MAP001",
+        ...         "ATTRIBS": [
+        ...             {"ATTRID": "OriginLocation", "ATTRDATA": "0"},
+        ...             {"ATTRID": "Rows", "ATTRDATA": 4},
+        ...             {"ATTRID": "Columns", "ATTRDATA": 4},
+        ...             {"ATTRID": "CellStatus", "ATTRDATA": 6},
+        ...             {"ATTRID": "LotID", "ATTRDATA":"LOT001"}]}],
+        ...         "ERRORS": {"OBJACK": 0}})
+        S14F4
+          <L [2]
+            <L [1]
+              <L [2]
+                <A "MAP001">
+                <L [5]
+                  <L [2]
+                    <A "OriginLocation">
+                    <A "0">
+                  >
+                  <L [2]
+                    <A "Rows">
+                    <U1 4 >
+                  >
+                  <L [2]
+                    <A "Columns">
+                    <U1 4 >
+                  >
+                  <L [2]
+                    <A "CellStatus">
+                    <U1 6 >
+                  >
+                  <L [2]
+                    <A "LotID">
+                    <A "LOT001">
+                  >
+                >
+              >
+            >
             <L [2]
-              <I1 1 2 >
-              <I1 2 3 >
+              <U1 0 >
+              <L>
             >
-            <A "unit">
-            <U1 100 >
-            <U1 100 >
-            <U1 10 >
-            <U1 10 >
-            <A "{x}">
-            <U1 100 >
-            <B 0x0>
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
-    _stream = 12
-    _function = 1
+    _stream = 14
+    _function = 4
 
     _data_format = [
-        MID,
-        IDTYP,
-        FNLOC,
-        FFROT,
-        ORLOC,
-        RPSEL,
-        [REFP],
-        DUTMS,
-        XDIES,
-        YDIES,
-        ROWCT,
-        COLCT,
-        NULBC,
-        PRDCT,
-        PRAXI
+        [
+            [
+                OBJID,
+                [
+                    [
+                        "ATTRIBS",
+                        ATTRID,
+                        ATTRDATA
+                    ]
+                ]
+            ]
+        ],
+        [
+            "ERRORS",
+            OBJACK,
+            [
+                [
+                    "ERROR",
+                    ERRCODE,
+                    ERRTEXT
+                ]
+            ]
+        ]
     ]
 
     _to_host = True
-    _to_equipment = False
+    _to_equipment = True
 
-    _has_reply = True
-    _is_reply_required = True
+    _has_reply = False
+    _is_reply_required = False
 
-    _is_multi_block = False
+    _is_multi_block = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f02.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f02.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS12F02(secsgem.secs.data_items.SDACK.ACK)
         S12F2
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 12
     _function = 2
 
     _data_format = SDACK
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f03.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f15.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,104 @@
 #####################################################################
-# s12f03.py
+# s05f15.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 03."""
+"""Class for stream 05 function 15."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, MAPFT, FNLOC, FFROT, ORLOC, PRAXI, BCEQU, NULBC
+from secsgem.secs.data_items import TIMESTAMP
+from secsgem.secs.data_items import EXID
+from secsgem.secs.data_items import ACKA
+from secsgem.secs.data_items import ERRCODE
+from secsgem.secs.data_items import ERRTEXT
 
 
-class SecsS12F03(SecsStreamFunction):
+class SecsS05F15(SecsStreamFunction):
     """
-    map setup data - request.
+    exception recover complete - notify.
 
     **Data Items**
 
-    - :class:`MID <secsgem.secs.data_items.MID>`
-    - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
-    - :class:`MAPFT <secsgem.secs.data_items.MAPFT>`
-    - :class:`FNLOC <secsgem.secs.data_items.FNLOC>`
-    - :class:`FFROT <secsgem.secs.data_items.FFROT>`
-    - :class:`ORLOC <secsgem.secs.data_items.ORLOC>`
-    - :class:`PRAXI <secsgem.secs.data_items.PRAXI>`
-    - :class:`BCEQU <secsgem.secs.data_items.BCEQU>`
-    - :class:`NULBC <secsgem.secs.data_items.NULBC>`
+    - :class:`TIMESTAMP <secsgem.secs.data_items.TIMESTAMP>`
+    - :class:`EXID <secsgem.secs.data_items.EXID>`
+    - :class:`ACKA <secsgem.secs.data_items.ACKA>`
+    - :class:`ERRCODE <secsgem.secs.data_items.ERRCODE>`
+    - :class:`ERRTEXT <secsgem.secs.data_items.ERRTEXT>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F03
+        >>> secsgem.secs.functions.SecsS05F15
         {
-            MID: A/B[80]
-            IDTYP: B[1]
-            MAPFT: B[1]
-            FNLOC: U2
-            FFROT: U2
-            ORLOC: B
-            PRAXI: B[1]
-            BCEQU: U1/A
-            NULBC: U1/A
+            TIMESTAMP: A[32]
+            EXID: A[20]
+            DATA: {
+                ACKA: BOOLEAN[1]
+                DATA: {
+                    ERRCODE: I1/I2/I4/I8
+                    ERRTEXT: A[120]
+                }
+            }
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F03({"MID": "materialID", \
-                "IDTYP": secsgem.secs.data_items.IDTYP.WAFER_CASSETTE, \
-                "MAPFT": secsgem.secs.data_items.MAPFT.ROW, \
-                "FNLOC": 0, \
-                "FFROT": 0, \
-                "ORLOC": secsgem.secs.data_items.ORLOC.LOWER_LEFT, \
-                "PRAXI": secsgem.secs.data_items.PRAXI.COLS_LEFT_INCR, \
-                "BCEQU": [1, 3, 5, 7], \
-                "NULBC": "{x}", \
-                })
-        S12F3 W
-          <L [9]
-            <A "materialID">
-            <B 0x1>
-            <B 0x0>
-            <U2 0 >
-            <U2 0 >
-            <B 0x3>
-            <B 0x4>
-            <U1 1 3 5 7 >
-            <A "{x}">
+        >>> secsgem.secs.functions.SecsS05F15({
+        ...     "TIMESTAMP": "161006221500",
+        ...     "EXID": "EX123",
+        ...     "DATA": {
+        ...         "ACKA": False,
+        ...         "DATA": {
+        ...             "ERRCODE": 10,
+        ...             "ERRTEXT": "Error"
+        ...         }}})
+        S5F15
+          <L [3]
+            <A "161006221500">
+            <A "EX123">
+            <L [2]
+              <BOOLEAN False >
+              <L [2]
+                <I1 10 >
+                <A "Error">
+              >
+            >
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
-    _stream = 12
-    _function = 3
+    _stream = 5
+    _function = 15
 
     _data_format = [
-        MID,
-        IDTYP,
-        MAPFT,
-        FNLOC,
-        FFROT,
-        ORLOC,
-        PRAXI,
-        BCEQU,
-        NULBC
+        TIMESTAMP,
+        EXID,
+        [
+            ACKA,
+            [
+                ERRCODE,
+                ERRTEXT
+            ]
+        ]
     ]
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = True
-    _is_reply_required = True
+    _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f04.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s14f02.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,157 @@
 #####################################################################
-# s12f04.py
+# s14f02.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 04."""
+"""Class for stream 14 function 02."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, FNLOC, ORLOC, RPSEL, REFP, DUTMS, XDIES, YDIES, ROWCT, COLCT, PRDCT, \
-    BCEQU, NULBC, MLCL
+from secsgem.secs.data_items import OBJID
+from secsgem.secs.data_items import ATTRID
+from secsgem.secs.data_items import ATTRDATA
+from secsgem.secs.data_items import OBJACK
+from secsgem.secs.data_items import ERRCODE
+from secsgem.secs.data_items import ERRTEXT
 
 
-class SecsS12F04(SecsStreamFunction):
+class SecsS14F02(SecsStreamFunction):
     """
-    map setup data.
+    GetAttr data.
 
     **Data Items**
 
-    - :class:`MID <secsgem.secs.data_items.MID>`
-    - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
-    - :class:`FNLOC <secsgem.secs.data_items.FNLOC>`
-    - :class:`ORLOC <secsgem.secs.data_items.ORLOC>`
-    - :class:`RPSEL <secsgem.secs.data_items.RPSEL>`
-    - :class:`REFP <secsgem.secs.data_items.REFP>`
-    - :class:`DUTMS <secsgem.secs.data_items.DUTMS>`
-    - :class:`XDIES <secsgem.secs.data_items.XDIES>`
-    - :class:`YDIES <secsgem.secs.data_items.YDIES>`
-    - :class:`ROWCT <secsgem.secs.data_items.ROWCT>`
-    - :class:`COLCT <secsgem.secs.data_items.COLCT>`
-    - :class:`PRDCT <secsgem.secs.data_items.PRDCT>`
-    - :class:`BCEQU <secsgem.secs.data_items.BCEQU>`
-    - :class:`NULBC <secsgem.secs.data_items.NULBC>`
-    - :class:`MLCL <secsgem.secs.data_items.MLCL>`
+    - :class:`OBJID <secsgem.secs.data_items.OBJID>`
+    - :class:`ATTRID <secsgem.secs.data_items.ATTRID>`
+    - :class:`ATTRDATA <secsgem.secs.data_items.ATTRDATA>`
+    - :class:`OBJACK <secsgem.secs.data_items.OBJACK>`
+    - :class:`ERRCODE <secsgem.secs.data_items.ERRCODE>`
+    - :class:`ERRTEXT <secsgem.secs.data_items.ERRTEXT>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F04
+        >>> secsgem.secs.functions.SecsS14F02
         {
-            MID: A/B[80]
-            IDTYP: B[1]
-            FNLOC: U2
-            ORLOC: B
-            RPSEL: U1
-            REFP: [
-                DATA: I1/I2/I4/I8
+            DATA: [
+                {
+                    OBJID: U1/U2/U4/U8/A
+                    ATTRIBS: [
+                        {
+                            ATTRID: U1/U2/U4/U8/A
+                            ATTRDATA: L/BOOLEAN/U1/U2/U4/U8/I1/I2/I4/I8/F4/F8/A/B
+                        }
+                        ...
+                    ]
+                }
                 ...
             ]
-            DUTMS: A
-            XDIES: U1/U2/U4/U8/F4/F8
-            YDIES: U1/U2/U4/U8/F4/F8
-            ROWCT: U1/U2/U4/U8
-            COLCT: U1/U2/U4/U8
-            PRDCT: U1/U2/U4/U8
-            BCEQU: U1/A
-            NULBC: U1/A
-            MLCL: U1/U2/U4/U8
+            ERRORS: {
+                OBJACK: U1[1]
+                ERROR: [
+                    {
+                        ERRCODE: I1/I2/I4/I8
+                        ERRTEXT: A[120]
+                    }
+                    ...
+                ]
+            }
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F04({"MID": "materialID", \
-                "IDTYP": secsgem.secs.data_items.IDTYP.FILM_FRAME, \
-                "FNLOC": 0, \
-                "ORLOC": secsgem.secs.data_items.ORLOC.CENTER_DIE, \
-                "RPSEL": 0, \
-                "REFP": [[1,2], [2,3]], \
-                "DUTMS": "unit", \
-                "XDIES": 100, \
-                "YDIES": 100, \
-                "ROWCT": 10, \
-                "COLCT": 10, \
-                "PRDCT": 100, \
-                "BCEQU": [1, 3, 5, 7], \
-                "NULBC": "{x}", \
-                "MLCL": 0, \
-                })
-        S12F4
-          <L [15]
-            <A "materialID">
-            <B 0x2>
-            <U2 0 >
-            <B 0x0>
-            <U1 0 >
+        >>> secsgem.secs.functions.SecsS14F02({
+        ...     "DATA": [{
+        ...         "OBJID": "MAP001",
+        ...         "ATTRIBS": [
+        ...             {"ATTRID": "OriginLocation", "ATTRDATA": "0"},
+        ...             {"ATTRID": "Rows", "ATTRDATA": 4},
+        ...             {"ATTRID": "Columns", "ATTRDATA": 4},
+        ...             {"ATTRID": "CellStatus", "ATTRDATA": 6},
+        ...             {"ATTRID": "LotID", "ATTRDATA":"LOT001"}]}],
+        ...         "ERRORS": {"OBJACK": 0}})
+        S14F2
+          <L [2]
+            <L [1]
+              <L [2]
+                <A "MAP001">
+                <L [5]
+                  <L [2]
+                    <A "OriginLocation">
+                    <A "0">
+                  >
+                  <L [2]
+                    <A "Rows">
+                    <U1 4 >
+                  >
+                  <L [2]
+                    <A "Columns">
+                    <U1 4 >
+                  >
+                  <L [2]
+                    <A "CellStatus">
+                    <U1 6 >
+                  >
+                  <L [2]
+                    <A "LotID">
+                    <A "LOT001">
+                  >
+                >
+              >
+            >
             <L [2]
-              <I1 1 2 >
-              <I1 2 3 >
+              <U1 0 >
+              <L>
             >
-            <A "unit">
-            <U1 100 >
-            <U1 100 >
-            <U1 10 >
-            <U1 10 >
-            <U1 100 >
-            <U1 1 3 5 7 >
-            <A "{x}">
-            <U1 0 >
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
-    _stream = 12
-    _function = 4
+    _stream = 14
+    _function = 2
 
     _data_format = [
-        MID,
-        IDTYP,
-        FNLOC,
-        ORLOC,
-        RPSEL,
-        [REFP],
-        DUTMS,
-        XDIES,
-        YDIES,
-        ROWCT,
-        COLCT,
-        PRDCT,
-        BCEQU,
-        NULBC,
-        MLCL
+        [
+            [
+                OBJID,
+                [
+                    [
+                        "ATTRIBS",
+                        ATTRID,
+                        ATTRDATA
+                    ]
+                ]
+            ]
+        ],
+        [
+            "ERRORS",
+            OBJACK,
+            [
+                [
+                    "ERROR",
+                    ERRCODE,
+                    ERRTEXT
+                ]
+            ]
+        ]
     ]
 
-    _to_host = False
+    _to_host = True
     _to_equipment = True
 
     _has_reply = False
     _is_reply_required = False
 
-    _is_multi_block = False
+    _is_multi_block = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f05.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f25.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,58 @@
 #####################################################################
-# s12f05.py
+# s02f25.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 05."""
+"""Class for stream 02 function 25."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, MAPFT, MLCL
+from secsgem.secs.data_items import ABS
 
 
-class SecsS12F05(SecsStreamFunction):
+class SecsS02F25(SecsStreamFunction):
     """
-    map transmit inquire.
+    Loopback diagnostic request.
 
     **Data Items**
 
-    - :class:`MID <secsgem.secs.data_items.MID>`
-    - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
-    - :class:`MAPFT <secsgem.secs.data_items.MAPFT>`
-    - :class:`MLCL <secsgem.secs.data_items.MLCL>`
+    - :class:`ABS <secsgem.secs.data_items.ABS>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F05
-        {
-            MID: A/B[80]
-            IDTYP: B[1]
-            MAPFT: B[1]
-            MLCL: U1/U2/U4/U8
-        }
+        >>> secsgem.secs.functions.SecsS02F25
+        ABS: B
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F05({"MID": "materialID", \
-                                               "IDTYP": secsgem.secs.data_items.IDTYP.WAFER, \
-                                               "MAPFT": secsgem.secs.data_items.MAPFT.ARRAY, \
-                                               "MLCL": 0})
-        S12F5 W
-          <L [4]
-            <A "materialID">
-            <B 0x0>
-            <B 0x1>
-            <U1 0 >
-          > .
+        >>> secsgem.secs.functions.SecsS02F25("Text")
+        S2F25 W
+          <B 0x54 0x65 0x78 0x74> .
 
     :param value: parameters for this function (see example)
-    :type value: dict
+    :type value: bytes
     """
 
-    _stream = 12
-    _function = 5
+    _stream = 2
+    _function = 25
 
-    _data_format = [
-        MID,
-        IDTYP,
-        MAPFT,
-        MLCL
-    ]
+    _data_format = ABS
 
     _to_host = True
-    _to_equipment = False
+    _to_equipment = True
 
     _has_reply = True
     _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f06.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f12.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 #####################################################################
-# s12f06.py
+# s12f12.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 06."""
+"""Class for stream 12 function 12."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import GRNT1
+from secsgem.secs.data_items import MDACK
 
 
-class SecsS12F06(SecsStreamFunction):
+class SecsS12F12(SecsStreamFunction):
     """
-    map transmit - grant.
+    map data type 3 - acknowledge.
 
     **Data Items**
 
-    - :class:`GRNT1 <secsgem.secs.data_items.GRNT1>`
+    - :class:`MDACK <secsgem.secs.data_items.MDACK>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F06
-        GRNT1: B[1]
+        >>> secsgem.secs.functions.SecsS12F12
+        MDACK: B[1]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F06(secsgem.secs.data_items.GRNT1.MATERIALID_UNKNOWN)
-        S12F6
-          <B 0x5> .
+        >>> secsgem.secs.functions.SecsS12F12(secsgem.secs.data_items.MDACK.FORMAT_ERROR)
+        S12F12
+          <B 0x1> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 12
-    _function = 6
+    _function = 12
 
-    _data_format = GRNT1
+    _data_format = MDACK
 
     _to_host = False
     _to_equipment = True
 
     _has_reply = False
     _is_reply_required = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f08.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f08.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS12F08(secsgem.secs.data_items.MDACK.ABORT_MAP)
         S12F8
           <B 0x3> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 12
     _function = 8
 
     _data_format = MDACK
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f09.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f09.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 12 function 09."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, STRP, BINLT
+from secsgem.secs.data_items import MID
+from secsgem.secs.data_items import IDTYP
+from secsgem.secs.data_items import STRP
+from secsgem.secs.data_items import BINLT
 
 
 class SecsS12F09(SecsStreamFunction):
     """
     map data type 2 - send.
 
     **Data Items**
@@ -40,18 +43,19 @@
             STRP: I1/I2/I4/I8[2]
             BINLT: U1/A
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F09({"MID": "materialID", \
-                                               "IDTYP": secsgem.secs.data_items.IDTYP.WAFER, \
-                                               "STRP": [0, 1], \
-                                               "BINLT": [1, 2, 3, 4, 5, 6]})
+        >>> secsgem.secs.functions.SecsS12F09({
+        ...     "MID": "materialID",
+        ...     "IDTYP": secsgem.secs.data_items.IDTYP.WAFER,
+        ...     "STRP": [0, 1],
+        ...     "BINLT": [1, 2, 3, 4, 5, 6]})
         S12F9 W
           <L [4]
             <A "materialID">
             <B 0x0>
             <I1 0 1 >
             <U1 1 2 3 4 5 6 >
           > .
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f10.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f10.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
         >>> import secsgem.secs
         >>> secsgem.secs.functions.SecsS12F10(secsgem.secs.data_items.MDACK.ACK)
         S12F10
           <B 0x0> .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: bytes
     """
 
     _stream = 12
     _function = 10
 
     _data_format = MDACK
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f11.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s05f01.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,78 @@
 #####################################################################
-# s12f11.py
+# s05f01.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 11."""
+"""Class for stream 05 function 01."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, XYPOS, BINLT
+from secsgem.secs.data_items import ALCD
+from secsgem.secs.data_items import ALID
+from secsgem.secs.data_items import ALTX
 
 
-class SecsS12F11(SecsStreamFunction):
+class SecsS05F01(SecsStreamFunction):
     """
-    map data type 3 - send.
+    alarm report - send.
 
     **Data Items**
 
-    - :class:`MID <secsgem.secs.data_items.MID>`
-    - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
-    - :class:`XYPOS <secsgem.secs.data_items.XYPOS>`
-    - :class:`BINLT <secsgem.secs.data_items.BINLT>`
+    - :class:`ALCD <secsgem.secs.data_items.ALCD>`
+    - :class:`ALID <secsgem.secs.data_items.ALID>`
+    - :class:`ALTX <secsgem.secs.data_items.ALTX>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F11
+        >>> secsgem.secs.functions.SecsS05F01
         {
-            MID: A/B[80]
-            IDTYP: B[1]
-            DATA: [
-                {
-                    XYPOS: I1/I2/I4/I8[2]
-                    BINLT: U1/A
-                }
-                ...
-            ]
+            ALCD: B[1]
+            ALID: U1/U2/U4/U8/I1/I2/I4/I8
+            ALTX: A[120]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F11({ \
-            "MID": "materialID", \
-            "IDTYP": secsgem.secs.data_items.IDTYP.WAFER, \
-            "DATA": [ \
-                {"XYPOS": [1, 2], "BINLT": [1, 2, 3, 4]}, \
-                {"XYPOS": [3, 4], "BINLT": [5, 6, 7, 8]}]})
-        S12F11 W
+        >>> secsgem.secs.functions.SecsS05F01({
+        ...     "ALCD": secsgem.secs.data_items.ALCD.PERSONAL_SAFETY |
+        ...             secsgem.secs.data_items.ALCD.ALARM_SET,
+        ...     "ALID": 100,
+        ...     "ALTX": "text"})
+        S5F1
           <L [3]
-            <A "materialID">
-            <B 0x0>
-            <L [2]
-              <L [2]
-                <I1 1 2 >
-                <U1 1 2 3 4 >
-              >
-              <L [2]
-                <I1 3 4 >
-                <U1 5 6 7 8 >
-              >
-            >
+            <B 0x81>
+            <U1 100 >
+            <A "text">
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
-    _stream = 12
-    _function = 11
+    _stream = 5
+    _function = 1
 
     _data_format = [
-        MID,
-        IDTYP,
-        [
-            [
-                XYPOS,
-                BINLT
-            ]
-        ]
+        ALCD,
+        ALID,
+        ALTX
     ]
 
     _to_host = True
     _to_equipment = False
 
     _has_reply = True
-    _is_reply_required = True
+    _is_reply_required = False
 
-    _is_multi_block = True
+    _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f12.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f47.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 #####################################################################
-# s12f12.py
+# s02f47.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 12."""
+"""Class for stream 02 function 47."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MDACK
+from secsgem.secs.data_items import VID
 
 
-class SecsS12F12(SecsStreamFunction):
+class SecsS02F47(SecsStreamFunction):
     """
-    map data type 3 - acknowledge.
+    Variable limit attribute request.
 
     **Data Items**
 
-    - :class:`MDACK <secsgem.secs.data_items.MDACK>`
+    - :class:`VID <secsgem.secs.data_items.VID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F12
-        MDACK: B[1]
+        >>> secsgem.secs.functions.SecsS02F47
+        [
+            VID: U1/U2/U4/U8/I1/I2/I4/I8/A
+            ...
+        ]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F12(secsgem.secs.data_items.MDACK.FORMAT_ERROR)
-        S12F12
-          <B 0x1> .
+        >>> secsgem.secs.functions.SecsS02F47([1, "VARIABLEID"])
+        S2F47 W
+          <L [2]
+            <U1 1 >
+            <A "VARIABLEID">
+          > .
 
     :param value: parameters for this function (see example)
-    :type value: byte
+    :type value: list
     """
 
-    _stream = 12
-    _function = 12
+    _stream = 2
+    _function = 47
 
-    _data_format = MDACK
+    _data_format = [VID]
 
     _to_host = False
     _to_equipment = True
 
-    _has_reply = False
-    _is_reply_required = False
+    _has_reply = True
+    _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f13.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s09f13.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 #####################################################################
-# s12f13.py
+# s09f13.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 13."""
+"""Class for stream 09 function 13."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP
+from secsgem.secs.data_items import MEXP
+from secsgem.secs.data_items import EDID
 
 
-class SecsS12F13(SecsStreamFunction):
+class SecsS09F13(SecsStreamFunction):
     """
-    map data type 1 - request.
+    conversation timeout.
 
     **Data Items**
 
-    - :class:`MID <secsgem.secs.data_items.MID>`
-    - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
+    - :class:`MEXP <secsgem.secs.data_items.MEXP>`
+    - :class:`EDID <secsgem.secs.data_items.EDID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F13
+        >>> secsgem.secs.functions.SecsS09F13
         {
-            MID: A/B[80]
-            IDTYP: B[1]
+            MEXP: A[6]
+            EDID: U1/U2/U4/U8/I1/I2/I4/I8/A/B
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F13({"MID": "materialID", "IDTYP": secsgem.secs.data_items.IDTYP.WAFER})
-        S12F13 W
+        >>> secsgem.secs.functions.SecsS09F13({"MEXP": "S01E01", "EDID": "data"})
+        S9F13
           <L [2]
-            <A "materialID">
-            <B 0x0>
+            <A "S01E01">
+            <A "data">
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
-    _stream = 12
+    _stream = 9
     _function = 13
 
     _data_format = [
-        MID,
-        IDTYP
+        MEXP,
+        EDID
     ]
 
     _to_host = True
     _to_equipment = False
 
-    _has_reply = True
-    _is_reply_required = True
+    _has_reply = False
+    _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f14.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f14.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 12 function 14."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, RSINF, BINLT
+from secsgem.secs.data_items import MID
+from secsgem.secs.data_items import IDTYP
+from secsgem.secs.data_items import RSINF
+from secsgem.secs.data_items import BINLT
 
 
 class SecsS12F14(SecsStreamFunction):
     """
     map data type 1.
 
     **Data Items**
@@ -45,20 +48,20 @@
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F14({ \
-            "MID": "materialID", \
-            "IDTYP": secsgem.secs.data_items.IDTYP.WAFER, \
-            "DATA": [ \
-                {"RSINF": [1, 2, 3], "BINLT": [1, 2, 3, 4]}, \
-                {"RSINF": [4, 5, 6], "BINLT": [5, 6, 7, 8]}]})
+        >>> secsgem.secs.functions.SecsS12F14({
+        ...     "MID": "materialID",
+        ...     "IDTYP": secsgem.secs.data_items.IDTYP.WAFER,
+        ...     "DATA": [
+        ...         {"RSINF": [1, 2, 3], "BINLT": [1, 2, 3, 4]},
+        ...         {"RSINF": [4, 5, 6], "BINLT": [5, 6, 7, 8]}]})
         S12F14
           <L [3]
             <A "materialID">
             <B 0x0>
             <L [2]
               <L [2]
                 <I1 1 2 3 >
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f15.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f13.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 #####################################################################
-# s12f15.py
+# s12f13.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 15."""
+"""Class for stream 12 function 13."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP
+from secsgem.secs.data_items import MID
+from secsgem.secs.data_items import IDTYP
 
 
-class SecsS12F15(SecsStreamFunction):
+class SecsS12F13(SecsStreamFunction):
     """
-    map data type 2 - request.
+    map data type 1 - request.
 
     **Data Items**
 
     - :class:`MID <secsgem.secs.data_items.MID>`
     - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F15
+        >>> secsgem.secs.functions.SecsS12F13
         {
             MID: A/B[80]
             IDTYP: B[1]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F15({"MID": "materialID", "IDTYP": secsgem.secs.data_items.IDTYP.WAFER})
-        S12F15 W
+        >>> secsgem.secs.functions.SecsS12F13({"MID": "materialID", "IDTYP": secsgem.secs.data_items.IDTYP.WAFER})
+        S12F13 W
           <L [2]
             <A "materialID">
             <B 0x0>
           > .
 
     :param value: parameters for this function (see example)
     :type value: dict
     """
 
     _stream = 12
-    _function = 15
+    _function = 13
 
     _data_format = [
         MID,
         IDTYP
     ]
 
     _to_host = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f16.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s12f16.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 12 function 16."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, STRP, BINLT
+from secsgem.secs.data_items import MID
+from secsgem.secs.data_items import IDTYP
+from secsgem.secs.data_items import STRP
+from secsgem.secs.data_items import BINLT
 
 
 class SecsS12F16(SecsStreamFunction):
     """
     map data type 2.
 
     **Data Items**
@@ -40,18 +43,19 @@
             STRP: I1/I2/I4/I8[2]
             BINLT: U1/A
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F16({"MID": "materialID", \
-                                               "IDTYP": secsgem.secs.data_items.IDTYP.WAFER, \
-                                               "STRP": [0, 1], \
-                                               "BINLT": [1, 2, 3, 4, 5, 6]})
+        >>> secsgem.secs.functions.SecsS12F16({
+        ...     "MID": "materialID",
+        ...     "IDTYP": secsgem.secs.data_items.IDTYP.WAFER,
+        ...     "STRP": [0, 1],
+        ...     "BINLT": [1, 2, 3, 4, 5, 6]})
         S12F16
           <L [4]
             <A "materialID">
             <B 0x0>
             <I1 0 1 >
             <U1 1 2 3 4 5 6 >
           > .
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f17.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s01f21.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,64 @@
 #####################################################################
-# s12f17.py
+# s01f21.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 17."""
+"""Class for stream 01 function 21."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MID, IDTYP, SDBIN
+from secsgem.secs.data_items import VID
 
 
-class SecsS12F17(SecsStreamFunction):
+class SecsS01F21(SecsStreamFunction):
     """
-    map data type 3 - request.
+    Data variable namelist request.
 
     **Data Items**
 
-    - :class:`MID <secsgem.secs.data_items.MID>`
-    - :class:`IDTYP <secsgem.secs.data_items.IDTYP>`
-    - :class:`SDBIN <secsgem.secs.data_items.SDBIN>`
+    - :class:`VID <secsgem.secs.data_items.VID>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F17
-        {
-            MID: A/B[80]
-            IDTYP: B[1]
-            SDBIN: B[1]
-        }
+        >>> secsgem.secs.functions.SecsS01F21
+        [
+            VID: U1/U2/U4/U8/I1/I2/I4/I8/A
+            ...
+        ]
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F17({"MID": "materialID", \
-                                               "IDTYP": secsgem.secs.data_items.IDTYP.WAFER, \
-                                               "SDBIN": secsgem.secs.data_items.SDBIN.DONT_SEND})
-        S12F17 W
-          <L [3]
-            <A "materialID">
-            <B 0x0>
-            <B 0x1>
+        >>> secsgem.secs.functions.SecsS01F21([1, "VARIABLEID"])
+        S1F21 W
+          <L [2]
+            <U1 1 >
+            <A "VARIABLEID">
           > .
 
     :param value: parameters for this function (see example)
-    :type value: dict
+    :type value: list
     """
 
-    _stream = 12
-    _function = 17
+    _stream = 1
+    _function = 21
 
-    _data_format = [
-        MID,
-        IDTYP,
-        SDBIN
-    ]
+    _data_format = [VID]
 
-    _to_host = True
-    _to_equipment = False
+    _to_host = False
+    _to_equipment = True
 
     _has_reply = True
     _is_reply_required = True
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s12f19.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s02f22.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,58 @@
 #####################################################################
-# s12f19.py
+# s02f22.py
 #
 # (c) Copyright 2021, Benjamin Parzella. All rights reserved.
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
-"""Class for stream 12 function 19."""
+"""Class for stream 02 function 22."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import MAPER, DATLC
+from secsgem.secs.data_items import CMDA
 
 
-class SecsS12F19(SecsStreamFunction):
+class SecsS02F22(SecsStreamFunction):
     """
-    map error report - send.
+    Remote command - acknowledge.
 
     **Data Items**
 
-    - :class:`MAPER <secsgem.secs.data_items.MAPER>`
-    - :class:`DATLC <secsgem.secs.data_items.DATLC>`
+    - :class:`CMDA <secsgem.secs.data_items.CMDA>`
 
     **Structure**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F19
-        {
-            MAPER: B[1]
-            DATLC: U1
-        }
+        >>> secsgem.secs.functions.SecsS02F22
+        CMDA: U1/I1
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS12F19({"MAPER": secsgem.secs.data_items.MAPER.INVALID_DATA, "DATLC": 0})
-        S12F19
-          <L [2]
-            <B 0x1>
-            <U1 0 >
-          > .
+        >>> secsgem.secs.functions.SecsS02F22(secsgem.secs.data_items.CMDA.DONE)
+        S2F22
+          <U1 0 > .
 
     :param value: parameters for this function (see example)
-    :type value: dict
+    :type value: int
     """
 
-    _stream = 12
-    _function = 19
+    _stream = 2
+    _function = 22
 
-    _data_format = [
-        MAPER,
-        DATLC
-    ]
+    _data_format = CMDA
 
     _to_host = True
-    _to_equipment = True
+    _to_equipment = False
 
     _has_reply = False
     _is_reply_required = False
 
     _is_multi_block = False
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s14f00.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s14f00.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s14f01.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s14f01.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 14 function 01."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import OBJSPEC, OBJTYPE, OBJID, ATTRID, ATTRDATA, ATTRRELN
+from secsgem.secs.data_items import OBJSPEC
+from secsgem.secs.data_items import OBJTYPE
+from secsgem.secs.data_items import OBJID
+from secsgem.secs.data_items import ATTRID
+from secsgem.secs.data_items import ATTRDATA
+from secsgem.secs.data_items import ATTRRELN
 
 
 class SecsS14F01(SecsStreamFunction):
     """
     GetAttr request.
 
     **Data Items**
@@ -56,20 +61,20 @@
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS14F01({ \
-            "OBJSPEC": '', \
-            "OBJTYPE": 'StripMap', \
-            "OBJID": ['MAP001'], \
-            "FILTER": [], \
-            "ATTRID": ['OriginLocation', 'Rows', 'Columns', 'CellStatus', 'LotID']})
+        >>> secsgem.secs.functions.SecsS14F01({
+        ...     "OBJSPEC": '',
+        ...     "OBJTYPE": 'StripMap',
+        ...     "OBJID": ['MAP001'],
+        ...     "FILTER": [],
+        ...     "ATTRID": ['OriginLocation', 'Rows', 'Columns', 'CellStatus', 'LotID']})
         S14F1 W
           <L [5]
             <A>
             <A "StripMap">
             <L [1]
               <A "MAP001">
             >
@@ -92,15 +97,15 @@
 
     _data_format = [
         OBJSPEC,
         OBJTYPE,
         [OBJID],
         [
             [
-                "FILTER",   # name of the list
+                "FILTER",
                 ATTRID,
                 ATTRDATA,
                 ATTRRELN
             ]
         ],
         [ATTRID]
     ]
@@ -108,18 +113,7 @@
     _to_host = True
     _to_equipment = True
 
     _has_reply = True
     _is_reply_required = True
 
     _is_multi_block = False
-
-    RELATION = {
-        "EQUAL": 0,
-        "NOTEQUAL": 1,
-        "LESS": 2,
-        "LESSEQUAL": 3,
-        "GREATER": 4,
-        "GREATEREQUAL": 5,
-        "PRESENT": 6,
-        "NOTPRESENT": 7,
-    }
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/functions/s14f03.py` & `secsgem-0.2.0a3/secsgem/secs/functions/s14f03.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Class for stream 14 function 03."""
 
 from secsgem.secs.functions.base import SecsStreamFunction
-from secsgem.secs.data_items import OBJSPEC, OBJTYPE, OBJID, ATTRID, ATTRDATA
+from secsgem.secs.data_items import OBJSPEC
+from secsgem.secs.data_items import OBJTYPE
+from secsgem.secs.data_items import OBJID
+from secsgem.secs.data_items import ATTRID
+from secsgem.secs.data_items import ATTRDATA
 
 
 class SecsS14F03(SecsStreamFunction):
     """
     SetAttr request.
 
     **Data Items**
@@ -50,16 +54,21 @@
                 ...
             ]
         }
 
     **Example**::
 
         >>> import secsgem.secs
-        >>> secsgem.secs.functions.SecsS14F03({"OBJSPEC": '', "OBJTYPE": 'StripMap', "OBJID": ['MAP001'], \
-"ATTRIBS": [ {"ATTRID": "CellStatus", "ATTRDATA": "3"} ] })
+        >>> secsgem.secs.functions.SecsS14F03({
+        ...       "OBJSPEC": '',
+        ...       "OBJTYPE": 'StripMap',
+        ...       "OBJID": ['MAP001'],
+        ...       "ATTRIBS": [{
+        ...           "ATTRID": "CellStatus", 
+        ...           "ATTRDATA": "3"}]})
         S14F3 W
           <L [4]
             <A>
             <A "StripMap">
             <L [1]
               <A "MAP001">
             >
@@ -80,15 +89,15 @@
 
     _data_format = [
         OBJSPEC,
         OBJTYPE,
         [OBJID],
         [
             [
-                "ATTRIBS",   # name of the list
+                "ATTRIBS",
                 ATTRID,
                 ATTRDATA
             ]
         ]
     ]
 
     _to_host = True
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/handler.py` & `secsgem-0.2.0a3/secsgem/secs/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,64 +10,110 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """Handler for SECS commands. Used in combination with :class:`secsgem.HsmsHandler.HsmsConnectionManager`."""
-
+import copy
 import logging
 import threading
-import copy
+import typing
 
 import secsgem.hsms
 
 from . import functions
 
+if typing.TYPE_CHECKING:
+    from ..gem.collection_event import CollectionEvent
+    from ..gem.data_value import DataValue
+    from ..gem.alarm import Alarm
+    from ..gem.remote_command import RemoteCommand
+
 
-class SecsHandler(secsgem.hsms.HsmsHandler):
+class SecsHandler:
     """
     Baseclass for creating Host/Equipment models. This layer contains the SECS functionality.
 
     Inherit from this class and override required functions.
     """
 
-    def __init__(self, address, port, active, session_id, name, custom_connection_handler=None):
+    def __init__(self, connection: secsgem.hsms.HsmsHandler):
         """
         Initialize a secs handler.
 
-        :param address: IP address of remote host
-        :type address: string
-        :param port: TCP port of remote host
-        :type port: integer
-        :param active: Is the connection active (*True*) or passive (*False*)
-        :type active: boolean
-        :param session_id: session / device ID to use for connection
-        :type session_id: integer
-        :param name: Name of the underlying configuration
-        :type name: string
-        :param custom_connection_handler: object for connection handling (ie multi server)
-        :type custom_connection_handler: :class:`secsgem.hsms.connections.HsmsMultiPassiveServer`
+        :param connection: connection to use
         """
-        super().__init__(address, port, active, session_id, name, custom_connection_handler)
+        self._connection = connection
+        self._connection.events.hsms_packet_received += self._on_hsms_packet_received
+        self._connection.secs_decode = self.secs_decode
 
         self.logger = logging.getLogger(self.__module__ + "." + self.__class__.__name__)
 
-        self._collectionEvents = {}
-        self._dataValues = {}
-        self._alarms = {}
-        self._remoteCommands = {}
+        self._collectionEvents: typing.Dict[typing.Union[int, str], CollectionEvent] = {}
+        self._dataValues: typing.Dict[typing.Union[int, str], DataValue] = {}
+        self._alarms: typing.Dict[typing.Union[int, str], Alarm] = {}
+        self._remoteCommands: typing.Dict[typing.Union[int, str], RemoteCommand] = {}
+
+        self._callback_handler = secsgem.common.CallbackHandler()
+        self._callback_handler.target = self
 
         self.secs_streams_functions = copy.deepcopy(functions.secs_streams_functions)
 
+    @classmethod
+    def hsms(cls, address, port, active, session_id, name, custom_connection_handler=None, **kwargs) -> "SecsHandler":
+        """
+        Initialize a secs handler using a hsms connection.
+
+        All arguments will be passed to the HSMS handler.
+        """
+        return cls(
+            secsgem.hsms.HsmsHandler(address, port, active, session_id, name, custom_connection_handler),
+            **kwargs)
+
     @staticmethod
-    def _generate_sf_callback_name(stream, function):
+    def _generate_sf_callback_name(stream: int, function: int) -> str:
         return f"s{stream:02d}f{function:02d}"
 
-    def register_stream_function(self, stream, function, callback):
+    @property
+    def connection(self) -> secsgem.hsms.HsmsHandler:
+        """Get the connection for the handler."""
+        return self._connection
+
+    def enable(self):
+        """Enable the connection."""
+        self.connection.enable()
+
+    def disable(self):
+        """Disable the connection."""
+        self.connection.disable()
+
+    def send_response(self, *args, **kwargs):
+        """Wrapper for connections send_response function."""
+        return self.connection.send_response(*args, **kwargs)
+
+    def send_and_waitfor_response(self, *args, **kwargs):
+        """Wrapper for connections send_and_waitfor_response function."""
+        return self.connection.send_and_waitfor_response(*args, **kwargs)
+
+    def send_stream_function(self, *args, **kwargs):
+        """Wrapper for connections send_stream_function function."""
+        return self.connection.send_stream_function(*args, **kwargs)
+
+    @property
+    def events(self):
+        """Wrapper for connections events."""
+        return self.connection.events
+
+    @property
+    def callbacks(self):
+        """Property for callback handling."""
+        return self._callback_handler
+
+    def register_stream_function(self, stream: int, function: int, callback):
         """
         Register the function callback for stream and function.
 
         :param stream: stream to register callback for
         :type stream: integer
         :param function: function to register callback for
         :type function: integer
@@ -92,15 +138,15 @@
     @property
     def collection_events(self):
         """
         Get available collection events.
 
         *Example*::
 
-            >>> handler = SecsHandler("127.0.0.1", 5000, False, 0, "test")
+            >>> handler = SecsHandler.hsms("127.0.0.1", 5000, False, 0, "test")
             >>> handler.collection_events[123] = {'name': 'collectionEventName', 'dvids': [1, 5] }
 
         **Key**
 
         Id of the collection event (integer)
 
         **Data**
@@ -119,15 +165,15 @@
     @property
     def data_values(self):
         """
         Get available data values.
 
         *Example*::
 
-            >>> handler = SecsHandler("127.0.0.1", 5000, False, 0, "test")
+            >>> handler = SecsHandler.hsms("127.0.0.1", 5000, False, 0, "test")
             >>> handler.data_values[5] = {'name': 'dataValueName', 'ceid': 123 }
 
         **Key**
 
         Id of the data value (integer)
 
         **Data**
@@ -146,15 +192,15 @@
     @property
     def alarms(self):
         """
         Get available alarms.
 
         *Example*::
 
-            >>> handler = SecsHandler("127.0.0.1", 5000, True, 0, "test")
+            >>> handler = SecsHandler.hsms("127.0.0.1", 5000, False, 0, "test")
             >>> handler.alarms[137] = {'ceidon': 1371, 'ceidoff': 1372}
 
         **Key**
 
         Id of the alarm (integer)
 
         **Data**
@@ -173,15 +219,15 @@
     @property
     def remote_commands(self):
         """
         Get available remote commands.
 
         *Example*::
 
-            >>> handler = SecsHandler("127.0.0.1", 5000, True, 0, "test")
+            >>> handler = SecsHandler.hsms("127.0.0.1", 5000, False, 0, "test")
             >>> handler.remote_commands["PP_SELECT"] = {'params': [{'name': 'PROGRAM', 'format': 'A'}], \
 'ceids': [200, 343]}
 
         **Key**
 
         Name of the remote command (string)
 
@@ -224,21 +270,23 @@
             result = callback(self, packet)
             if result is not None:
                 self.send_response(result, packet.header.system)
         except Exception:  # pylint: disable=broad-except
             self.logger.exception('Callback aborted because of exception, abort sent')
             self.send_response(self.stream_function(packet.header.stream, 0)(), packet.header.system)
 
-    def _on_hsms_packet_received(self, packet):
+    def _on_hsms_packet_received(self, data):
         """
         Packet received from hsms layer.
 
-        :param packet: received data packet
-        :type packet: :class:`secsgem.hsms.HsmsPacket`
+        :param data: received data
+        :type data: :class:`secsgem.hsms.HsmsPacket`
         """
+        packet = data["packet"]
+
         # check if callbacks available for this stream and function
         threading.Thread(
             target=self._handle_stream_function, args=(packet, ),
             name=f"secsgem_secsHandler_callback_S{packet.header.stream}F{packet.header.function}").start()
 
     def disable_ceids(self):
         """Disable all Collection Events."""
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/array.py` & `secsgem-0.2.0a3/secsgem/secs/variables/array.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/base.py` & `secsgem-0.2.0a3/secsgem/secs/variables/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,29 +10,31 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """SECS variable base type."""
+import typing
 
 
 class Base:
     """
     Base class for SECS variables.
 
     Due to the python types, wrapper classes for variables are required.
     If constructor is called with Base or subclass only the value is copied.
     """
 
     format_code = -1
+    preferred_types: typing.Optional[typing.List[typing.Type]]
 
-    def __init__(self):
+    def __init__(self, value=None):
         """Initialize a secs variable."""
-        self.value = None
+        self.value = value
 
     def set(self, value):
         """
         Set the internal value to the provided value.
 
         :param value: new value
         :type value: various
@@ -103,7 +105,12 @@
 
         return text_pos, format_code, length
 
     @property
     def is_dynamic(self) -> bool:
         """Check if this instance is Dynamic or derived."""
         return False
+
+    @property
+    def preferred_type(self):
+        """Get the preferred type for this variable."""
+        return self.preferred_types[0]
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/base_number.py` & `secsgem-0.2.0a3/secsgem/secs/variables/base_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 #
 # This software is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #####################################################################
 """SECS numeric variable base type."""
-
 import struct
+import typing
 
 from .base import Base
 
 
 class BaseNumber(Base):
     """Secs base type for numeric data."""
 
     format_code = 0
     text_code = ""
-    _base_type = int
-    _min = 0
-    _max = 0
+    _base_type: typing.Union[typing.Type[int], typing.Type[float]] = int
+    _min: typing.Union[int, float] = 0
+    _max: typing.Union[int, float] = 0
     _bytes = 0
     _struct_code = ""
 
     def __init__(self, value=None, count=-1):
         """
         Initialize a numeric secs variable.
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/base_text.py` & `secsgem-0.2.0a3/secsgem/secs/variables/base_text.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/binary.py` & `secsgem-0.2.0a3/secsgem/secs/variables/binary.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/boolean.py` & `secsgem-0.2.0a3/secsgem/secs/variables/boolean.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/dynamic.py` & `secsgem-0.2.0a3/secsgem/secs/variables/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,23 @@
             return True
 
         if typ in self.types:
             return True
 
         return False
 
+    @property
+    def preferred_type(self):
+        """Get the preferred type."""
+        types = []
+        for typ in self.__allowedtypes__:
+            types += typ.preferred_types
+        
+        return types[0]
+
     def set(self, value):
         """
         Set the internal value to the provided value.
 
         In doubt provide the variable wrapped in the matching :class:`secsgem.secs.variables.Base` class,
         to avoid confusion.
```

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/f4.py` & `secsgem-0.2.0a3/secsgem/secs/variables/f4.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/f8.py` & `secsgem-0.2.0a3/secsgem/secs/variables/f8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/functions.py` & `secsgem-0.2.0a3/secsgem/secs/variables/functions.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/i1.py` & `secsgem-0.2.0a3/secsgem/secs/variables/i1.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/i2.py` & `secsgem-0.2.0a3/secsgem/secs/variables/i2.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/i4.py` & `secsgem-0.2.0a3/secsgem/secs/variables/i4.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/i8.py` & `secsgem-0.2.0a3/secsgem/secs/variables/i8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/jis8.py` & `secsgem-0.2.0a3/secsgem/secs/variables/jis8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/list_type.py` & `secsgem-0.2.0a3/secsgem/secs/variables/list_type.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/string.py` & `secsgem-0.2.0a3/secsgem/secs/variables/string.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/u1.py` & `secsgem-0.2.0a3/secsgem/secs/variables/u1.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/u2.py` & `secsgem-0.2.0a3/secsgem/secs/variables/u2.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/u4.py` & `secsgem-0.2.0a3/secsgem/secs/variables/u4.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/secsgem/secs/variables/u8.py` & `secsgem-0.2.0a3/secsgem/secs/variables/u8.py`

 * *Files identical despite different names*

### Comparing `secsgem-0.2.0a2/PKG-INFO` & `secsgem-0.2.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secsgem
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: Python SECS/GEM implementation
 Home-page: https://github.com/bparzella/secsgem
 License: LGPL-2.1-or-later
 Keywords: development,hsms,secs,gem
 Author: Benjamin Parzella
 Author-email: bparzella@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
```

