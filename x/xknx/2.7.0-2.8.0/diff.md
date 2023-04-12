# Comparing `tmp/xknx-2.7.0.tar.gz` & `tmp/xknx-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xknx-2.7.0.tar", last modified: Wed Mar 15 21:46:32 2023, max compression
+gzip compressed data, was "xknx-2.8.0.tar", last modified: Wed Apr 12 14:06:25 2023, max compression
```

## Comparing `xknx-2.7.0.tar` & `xknx-2.8.0.tar`

### file list

```diff
@@ -1,181 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.396461 xknx-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-03-15 21:46:17.000000 xknx-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-15 21:46:17.000000 xknx-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-15 21:46:32.396461 xknx-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-15 21:46:17.000000 xknx-2.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-15 21:46:17.000000 xknx-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-15 21:46:32.396461 xknx-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-15 21:46:17.000000 xknx-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.364461 xknx-2.7.0/xknx/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.368461 xknx-2.7.0/xknx/cemi/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/cemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21651 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/cemi/cemi_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/cemi/cemi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/cemi/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.368461 xknx-2.7.0/xknx/core/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/core/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/core/connection_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/core/state_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/core/task_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/core/telegram_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/core/value_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.372461 xknx-2.7.0/xknx/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/climate_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16477 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/expose_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/fan.py
--rw-r--r--   0 runner    (1001) docker     (123)    25755 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/numeric_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/raw_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/travelcalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/devices/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.380461 xknx-2.7.0/xknx/dpt/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_1byte_signed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_1byte_uint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_2byte_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_2byte_signed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_2byte_uint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_4bit_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_4byte_float.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_4byte_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_hvac_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/dpt/dpt_time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.380461 xknx-2.7.0/xknx/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/exceptions/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.380461 xknx-2.7.0/xknx/io/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/gateway_scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30669 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/ip_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/knxip_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.384461 xknx-2.7.0/xknx/io/request_response/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/connectionstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/device_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/request_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/request_response/tunnelling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/self_description.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.384461 xknx-2.7.0/xknx/io/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/transport/ip_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/transport/tcp_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/transport/udp_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    23229 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/io/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.392461 xknx-2.7.0/xknx/knxip/
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/connect_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/connect_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/connectionstate_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/connectionstate_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/description_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/description_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/device_configuration_ack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/device_configuration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/dib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/disconnect_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/hpai.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/knxip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/knxip_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/routing_busy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/routing_indication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/routing_lost_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/search_request_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/search_response_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/secure_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/session_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/session_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/session_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/srp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/timer_notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/tunnelling_ack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/knxip/tunnelling_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.392461 xknx-2.7.0/xknx/management/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/management/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/management/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.392461 xknx-2.7.0/xknx/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/profile/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.392461 xknx-2.7.0/xknx/remote_value/
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_1count.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_climate_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_color_rgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_color_rgbw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_color_xyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_dpt_2_byte_unsigned.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_dpt_value_1_ucount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_scene_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_setpoint_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_temp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/remote_value/remote_value_updown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.392461 xknx-2.7.0/xknx/secure/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/secure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/secure/data_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/secure/data_secure_asdu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/secure/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/secure/security_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/secure/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.396461 xknx-2.7.0/xknx/telegram/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/telegram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/telegram/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/telegram/address_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    52109 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/telegram/apci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/telegram/telegram.py
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/telegram/tpci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.396461 xknx-2.7.0/xknx/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/tools/group_communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-03-15 21:46:17.000000 xknx-2.7.0/xknx/xknx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 21:46:32.364461 xknx-2.7.0/xknx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-03-15 21:46:32.000000 xknx-2.7.0/xknx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-03-15 21:46:32.000000 xknx-2.7.0/xknx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:46:32.000000 xknx-2.7.0/xknx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 21:46:32.000000 xknx-2.7.0/xknx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-15 21:46:32.000000 xknx-2.7.0/xknx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-15 21:46:32.000000 xknx-2.7.0/xknx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.318770 xknx-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 14:06:12.000000 xknx-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-12 14:06:12.000000 xknx-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-12 14:06:25.318770 xknx-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-12 14:06:12.000000 xknx-2.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-12 14:06:12.000000 xknx-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-12 14:06:25.318770 xknx-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-12 14:06:12.000000 xknx-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.302769 xknx-2.8.0/xknx/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.302769 xknx-2.8.0/xknx/cemi/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/cemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21651 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/cemi/cemi_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/cemi/cemi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/cemi/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.302769 xknx-2.8.0/xknx/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/core/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/core/connection_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/core/state_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/core/task_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/core/telegram_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/core/value_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.306769 xknx-2.8.0/xknx/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/climate_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/expose_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/fan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25740 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/numeric_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/raw_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/travelcalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/devices/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.306769 xknx-2.8.0/xknx/dpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_1byte_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_1byte_uint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_2byte_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_2byte_signed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_2byte_uint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_4bit_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_4byte_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_4byte_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_hvac_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/dpt_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/dpt/payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.306769 xknx-2.8.0/xknx/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/exceptions/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.310769 xknx-2.8.0/xknx/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/gateway_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30669 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/ip_secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22261 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/knxip_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.310769 xknx-2.8.0/xknx/io/request_response/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/connectionstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/device_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/request_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/request_response/tunnelling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/self_description.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.310769 xknx-2.8.0/xknx/io/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/transport/ip_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/transport/tcp_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/transport/udp_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23229 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/io/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.314769 xknx-2.8.0/xknx/knxip/
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5498 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/connect_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/connect_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/connectionstate_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/connectionstate_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/description_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/description_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/device_configuration_ack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/device_configuration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/dib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/disconnect_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/hpai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/knxip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/knxip_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/routing_busy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/routing_indication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/routing_lost_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/search_request_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/search_response_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/secure_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/session_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/session_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/session_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/srp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/timer_notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/tunnelling_ack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/knxip/tunnelling_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.314769 xknx-2.8.0/xknx/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/management/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/management/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.314769 xknx-2.8.0/xknx/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13385 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/profile/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.318770 xknx-2.8.0/xknx/remote_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_1count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_climate_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_color_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_color_rgbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_color_xyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_dpt_2_byte_unsigned.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_dpt_value_1_ucount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_scene_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_setpoint_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/remote_value/remote_value_updown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.318770 xknx-2.8.0/xknx/secure/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/secure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/secure/data_secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/secure/data_secure_asdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/secure/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/secure/security_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/secure/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.318770 xknx-2.8.0/xknx/telegram/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/telegram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11226 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/telegram/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/telegram/address_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52109 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/telegram/apci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/telegram/telegram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/telegram/tpci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.318770 xknx-2.8.0/xknx/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/tools/group_communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-12 14:06:12.000000 xknx-2.8.0/xknx/xknx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:06:25.302769 xknx-2.8.0/xknx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-12 14:06:25.000000 xknx-2.8.0/xknx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-12 14:06:25.000000 xknx-2.8.0/xknx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:06:25.000000 xknx-2.8.0/xknx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:06:25.000000 xknx-2.8.0/xknx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-12 14:06:25.000000 xknx-2.8.0/xknx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-12 14:06:25.000000 xknx-2.8.0/xknx.egg-info/top_level.txt
```

### Comparing `xknx-2.7.0/LICENSE` & `xknx-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/PKG-INFO` & `xknx-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xknx
-Version: 2.7.0
+Version: 2.8.0
 Summary: An Asynchronous Library for the KNX protocol. Documentation: https://xknx.io/
 Home-page: https://xknx.io/
-Download-URL: https://github.com/XKNX/xknx/archive/2.7.0.zip
+Download-URL: https://github.com/XKNX/xknx/archive/2.8.0.zip
 Author: Julius Mittenzwei
 Author-email: julius@mittenzwei.com
 License: MIT
 Keywords: knx ip knxip eib home automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `xknx-2.7.0/README.md` & `xknx-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/pyproject.toml` & `xknx-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/setup.py` & `xknx-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/cemi/cemi_frame.py` & `xknx-2.8.0/xknx/cemi/cemi_frame.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/cemi/cemi_handler.py` & `xknx-2.8.0/xknx/cemi/cemi_handler.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/cemi/const.py` & `xknx-2.8.0/xknx/cemi/const.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/core/connection_manager.py` & `xknx-2.8.0/xknx/core/connection_manager.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/core/state_updater.py` & `xknx-2.8.0/xknx/core/state_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             except IndexError:
                 pass  # No time given (no _options[1])
 
         return TrackerOptions(tracker_type, update_interval)
 
     def register_remote_value(
         self,
-        remote_value: RemoteValue[Any, Any],
+        remote_value: RemoteValue[Any],
         tracker_options: TrackerOptionType = True,
     ) -> None:
         """Register a RemoteValue to initialize its state and/or track for expiration."""
 
         async def read_state_mutex() -> None:
             """Schedule to read the state from the KNX bus - one at a time."""
             async with self._semaphore:
@@ -158,19 +158,19 @@
             tracker_options.tracker_type,
             tracker_options.update_interval_min,
             remote_value,
         )
         if self.started:
             tracker.start()
 
-    def unregister_remote_value(self, remote_value: RemoteValue[Any, Any]) -> None:
+    def unregister_remote_value(self, remote_value: RemoteValue[Any]) -> None:
         """Unregister a RemoteValue from StateUpdater."""
         self._workers.pop(id(remote_value)).stop()
 
-    def update_received(self, remote_value: RemoteValue[Any, Any]) -> None:
+    def update_received(self, remote_value: RemoteValue[Any]) -> None:
         """Reset the timer when a state update was received."""
         if self.started and id(remote_value) in self._workers:
             self._workers[id(remote_value)].update_received()
 
     def _start(self) -> None:
         """Start internal StateUpdater. Initialize states."""
         logger.debug("StateUpdater initializing values")
```

### Comparing `xknx-2.7.0/xknx/core/task_registry.py` & `xknx-2.8.0/xknx/core/task_registry.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/core/telegram_queue.py` & `xknx-2.8.0/xknx/core/telegram_queue.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/core/value_reader.py` & `xknx-2.8.0/xknx/core/value_reader.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/__init__.py` & `xknx-2.8.0/xknx/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/binary_sensor.py` & `xknx-2.8.0/xknx/devices/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/climate.py` & `xknx-2.8.0/xknx/devices/climate.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             device_name=self.name,
             feature_name="Command value",
             after_update_cb=self.after_update,
         )
 
         self.mode = mode
 
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes."""
         yield self.temperature
         yield self.target_temperature
         yield self._setpoint_shift
         yield self.on
         yield self.active
         yield self.command_value
```

### Comparing `xknx-2.7.0/xknx/devices/climate_mode.py` & `xknx-2.8.0/xknx/devices/climate_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,52 +170,52 @@
         self._use_binary_operation_modes = any(
             operation_mode.initialized
             for operation_mode in self._iter_binary_operation_modes()
         )
 
     def _iter_remote_values(
         self,
-    ) -> Iterator[RemoteValue[Any, Any]]:
+    ) -> Iterator[RemoteValue[Any]]:
         """Iterate climate mode RemoteValue classes."""
         return chain(
             self._iter_operation_remote_values(),
             self._iter_controller_remote_values(),
         )
 
     def _iter_operation_remote_values(
         self,
-    ) -> Iterator[RemoteValueClimateModeBase[Any, HVACOperationMode]]:
+    ) -> Iterator[RemoteValueClimateModeBase[HVACOperationMode]]:
         return chain(
             self._iter_binary_operation_modes(),
             self._iter_byte_operation_modes(),
         )
 
     def _iter_binary_operation_modes(
         self,
-    ) -> Iterator[RemoteValueClimateModeBase[Any, HVACOperationMode]]:
+    ) -> Iterator[RemoteValueClimateModeBase[HVACOperationMode]]:
         """Iterate DPT 1 binary operation modes."""
         yield from (
             self.remote_value_operation_mode_comfort,
             self.remote_value_operation_mode_night,
             self.remote_value_operation_mode_protection,
             self.remote_value_operation_mode_standby,
         )
 
     def _iter_byte_operation_modes(
         self,
-    ) -> Iterator[RemoteValueClimateModeBase[Any, HVACOperationMode]]:
+    ) -> Iterator[RemoteValueClimateModeBase[HVACOperationMode]]:
         """Iterate normal DPT 20.102 operation mode remote values."""
         yield from (
             self.remote_value_operation_mode,
             self.remote_value_controller_status,
         )
 
     def _iter_controller_remote_values(
         self,
-    ) -> Iterator[RemoteValueClimateModeBase[Any, HVACControllerMode]]:
+    ) -> Iterator[RemoteValueClimateModeBase[HVACControllerMode]]:
         """Iterate DPT 20.105 controller remote values."""
         yield self.remote_value_controller_mode
         yield self.remote_value_heat_cool
 
     async def _set_internal_operation_mode(
         self, operation_mode: HVACOperationMode
     ) -> None:
@@ -238,15 +238,15 @@
             not self.supports_operation_mode
             or operation_mode not in self._operation_modes
         ):
             raise DeviceIllegalValue(
                 "operation (preset) mode not supported", str(operation_mode)
             )
 
-        rv_operation: RemoteValueClimateModeBase[Any, HVACOperationMode]
+        rv_operation: RemoteValueClimateModeBase[HVACOperationMode]
         for rv_operation in self._iter_operation_remote_values():
             if (
                 rv_operation.writable
                 and operation_mode in rv_operation.supported_operation_modes()
             ):
                 await rv_operation.set(operation_mode)
 
@@ -258,15 +258,15 @@
             not self.supports_controller_mode
             or controller_mode not in self._controller_modes
         ):
             raise DeviceIllegalValue(
                 "controller (HVAC) mode not supported", str(controller_mode)
             )
 
-        rv_controller: RemoteValueClimateModeBase[Any, HVACControllerMode]
+        rv_controller: RemoteValueClimateModeBase[HVACControllerMode]
         for rv_controller in self._iter_controller_remote_values():
             if (
                 rv_controller.writable
                 and controller_mode in rv_controller.supported_operation_modes()
             ):
                 await rv_controller.set(controller_mode)
```

### Comparing `xknx-2.7.0/xknx/devices/cover.py` & `xknx-2.8.0/xknx/devices/cover.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         self.travel_time_up = travel_time_up
         self.travelcalculator = TravelCalculator(travel_time_down, travel_time_up)
 
         self._auto_stop_task: Task | None = None
         self._periodic_update_task: Task | None = None
         self._travel_direction_tilt: TravelStatus | None = None
 
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes."""
         yield self.updown
         yield self.step
         yield self.stop_
         yield self.position_current
         yield self.position_target
         yield self.angle
```

### Comparing `xknx-2.7.0/xknx/devices/datetime.py` & `xknx-2.8.0/xknx/devices/datetime.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/device.py` & `xknx-2.8.0/xknx/devices/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         for remote_value in self._iter_remote_values():
             remote_value.__del__()  # pylint: disable=unnecessary-dunder-call
         for task in self._iter_tasks():
             if task:
                 self.xknx.task_registry.unregister(task.name)
 
     @abstractmethod
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes."""
         # yield self.remote_value
         # yield from (<list all used RemoteValue instances>)
         yield from ()
 
     def _iter_tasks(self) -> Iterator[Task | None]:
         """Iterate the device tasks."""
```

### Comparing `xknx-2.7.0/xknx/devices/devices.py` & `xknx-2.8.0/xknx/devices/devices.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/expose_sensor.py` & `xknx-2.8.0/xknx/devices/expose_sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._cooldown_task_name = f"expose_sensor.cooldown_{id(self)}"
 
     async def after_update(self) -> None:
         """Call after state was updated."""
         self._cooldown_latest_value = self.sensor_value.value
         await super().after_update()
 
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes."""
         yield self.sensor_value
 
     def _iter_tasks(self) -> Iterator[Task | None]:
         """Iterate the device tasks."""
         yield self._cooldown_task
```

### Comparing `xknx-2.7.0/xknx/devices/fan.py` & `xknx-2.8.0/xknx/devices/fan.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             group_address_oscillation_state,
             sync_state=sync_state,
             device_name=self.name,
             feature_name="Oscillation",
             after_update_cb=self.after_update,
         )
 
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes."""
         yield from (self.switch, self.speed, self.oscillation)
 
     @property
     def supports_oscillation(self) -> bool:
         """Return if fan supports oscillation."""
         return self.oscillation.initialized
```

### Comparing `xknx-2.7.0/xknx/devices/light.py` & `xknx-2.8.0/xknx/devices/light.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,34 +313,34 @@
         self.max_kelvin = max_kelvin
         self._individual_color_debounce_task_name = (
             f"{id(self)}_individual_color_debounce"
         )
         self._individual_color_debounce_telegram_counter: int
         self._reset_individual_color_debounce_telegrams()
 
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes."""
         return chain(
             self._iter_instant_remote_values(),
             self._iter_debounce_remote_values(),
         )
 
-    def _iter_instant_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_instant_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes calling after_update_cb immediately."""
         yield self.switch
         yield self.brightness
         yield self.color
         yield self.rgbw
         yield self.hue
         yield self.saturation
         yield self.xyy_color
         yield self.tunable_white
         yield self.color_temperature
 
-    def _iter_debounce_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_debounce_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes debouncing after_update_cb."""
         for color in self._iter_individual_colors():
             yield color.switch
             yield color.brightness
 
     def _iter_individual_colors(self) -> Iterator[_SwitchAndBrightness]:
         """Iterate the devices individual colors."""
```

### Comparing `xknx-2.7.0/xknx/devices/notification.py` & `xknx-2.8.0/xknx/devices/notification.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/numeric_value.py` & `xknx-2.8.0/xknx/devices/numeric_value.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/raw_value.py` & `xknx-2.8.0/xknx/devices/raw_value.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/scene.py` & `xknx-2.8.0/xknx/devices/scene.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/sensor.py` & `xknx-2.8.0/xknx/devices/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 sync_state=sync_state,
                 value_type=value_type,
                 device_name=self.name,
                 after_update_cb=self.after_update,
             )
         self.always_callback = always_callback
 
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices RemoteValue classes."""
         yield self.sensor_value
 
     @property
     def last_telegram(self) -> Telegram | None:
         """Return the last telegram received from the RemoteValue."""
         return self.sensor_value.telegram
```

### Comparing `xknx-2.7.0/xknx/devices/switch.py` & `xknx-2.8.0/xknx/devices/switch.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/travelcalculator.py` & `xknx-2.8.0/xknx/devices/travelcalculator.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/devices/weather.py` & `xknx-2.8.0/xknx/devices/weather.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             sync_state=sync_state,
             value_type="humidity",
             device_name=self.name,
             feature_name="Humidity",
             after_update_cb=self.after_update,
         )
 
-    def _iter_remote_values(self) -> Iterator[RemoteValue[Any, Any]]:
+    def _iter_remote_values(self) -> Iterator[RemoteValue[Any]]:
         """Iterate the devices remote values."""
         yield self._temperature
         yield self._brightness_south
         yield self._brightness_north
         yield self._brightness_east
         yield self._brightness_west
         yield self._wind_speed
```

### Comparing `xknx-2.7.0/xknx/dpt/__init__.py` & `xknx-2.8.0/xknx/dpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Module for encoding and decoding KNX datatypes.
 
 * KNX Values like Int, Float, String, Time
 * Derived KNX Values like Scaling, Temperature
 """
 # flake8: noqa
-from .dpt import DPTArray, DPTBase, DPTBinary, DPTNumeric
+from .dpt import DPTBase, DPTNumeric
 from .dpt_1byte_signed import DPTPercentV8, DPTSignedRelativeValue, DPTValue1Count
 from .dpt_1byte_uint import (
     DPTDecimalFactor,
     DPTPercentU8,
     DPTSceneNumber,
     DPTTariff,
     DPTValue1ByteUnsigned,
@@ -185,7 +185,8 @@
 from .dpt_color import DPTColorXYY
 from .dpt_date import DPTDate
 from .dpt_datetime import DPTDateTime
 from .dpt_hvac_mode import DPTControllerStatus, DPTHVACContrMode, DPTHVACMode
 from .dpt_scaling import DPTAngle, DPTScaling
 from .dpt_string import DPTLatin1, DPTString
 from .dpt_time import DPTTime
+from .payload import DPTArray, DPTBinary
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt.py` & `xknx-2.8.0/xknx/dpt/dpt.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from inspect import isabstract
 from typing import Any, TypeVar, cast
 
-from xknx.exceptions import ConversionError
+from xknx.exceptions import CouldNotParseTelegram
+
+from .payload import DPTArray, DPTBinary
 
 T = TypeVar("T", bound=type["DPTBase"])  # pylint: disable=invalid-name
 
 
 class DPTBase(ABC):
     """
     Base class for KNX data point type transcoder.
@@ -44,44 +46,69 @@
     20.yyy 8-bit enumeration, e.g. HVAC mode ('auto', 'comfort', 'standby', 'economy', 'protection')
     28.yyy UTF-8
     29.yyy V64, 64-bit signed value
     232.yyy RGB [0,0,0]...[255,255,255]
 
     """
 
-    payload_length: int = cast(int, None)
+    payload_type: type[DPTArray | DPTBinary]
+    payload_length: int = cast(int, None)  # only used for DPTArray
     dpt_main_number: int | None = None
     dpt_sub_number: int | None = None
     value_type: str | None = None
     unit: str | None = None
     ha_device_class: str | None = None
 
     @classmethod
     @abstractmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> Any:
-        """Parse/deserialize from KNX/IP raw data (big endian)."""
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> Any:
+        """
+        Parse/deserialize from KNX/IP payload data.
+
+        Raise `CouldNotParseTelegram` for wrong payload
+        or `ConversionError` for unparsable value.
+        """
+        # raw = cls.validate_payload(payload)
+
+    @classmethod
+    def validate_payload(cls, payload: DPTArray | DPTBinary) -> tuple[int, ...]:
+        """
+        Test if payload has the correct length and type for given DPT.
+
+        Return tuple of raw values.
+        Raise CouldNotParseTelegram if payload type or length is invalid for DPT.
+        """
+        if cls.payload_type is DPTArray and isinstance(payload, DPTArray):
+            if cls.payload_length == len(payload.value):
+                return payload.value
+
+            raise CouldNotParseTelegram(
+                f"Invalid payload length for {cls.__name__}",
+                payload=payload,
+                expected_length=cls.payload_length,
+            )
+
+        if cls.payload_type is DPTBinary and isinstance(payload, DPTBinary):
+            # wrap in tuple for consistent return signature
+            return (payload.value,)
+
+        raise CouldNotParseTelegram(
+            f"Invalid payload type for {cls.__name__}",
+            payload=payload,
+            expected_type=cls.payload_type,
+        )
 
     @classmethod
     @abstractmethod
-    def to_knx(cls, value: Any) -> bytes | tuple[int, ...]:
-        """Serialize to KNX/IP raw data."""
+    def to_knx(cls, value: Any) -> DPTArray | DPTBinary:
+        """
+        Serialize to KNX/IP raw data.
 
-    @classmethod
-    def test_bytesarray(cls, raw: tuple[int, ...]) -> None:
-        """Test if array of raw bytes has the correct length and values of correct type."""
-        if cls.payload_length is None:
-            raise NotImplementedError(f"payload_length has to be defined for: {cls}")
-        if (
-            not isinstance(raw, (tuple, list))
-            or len(raw) != cls.payload_length
-            or any(not isinstance(byte, int) for byte in raw)
-            or any(byte < 0 for byte in raw)
-            or any(byte > 255 for byte in raw)
-        ):
-            raise ConversionError("Invalid raw bytes", raw=raw)
+        Raise `ConversionError` for unparsable value.
+        """
 
     @classmethod
     def __recursive_subclasses__(cls: T) -> Iterator[T]:
         """Yield all subclasses and their subclasses."""
         for subclass in cls.__subclasses__():
             yield from subclass.__recursive_subclasses__()
             if not isabstract(subclass):
@@ -146,81 +173,21 @@
                         pass
             return transcoder
 
 
 class DPTNumeric(DPTBase):
     """Base class for KNX data point types decoding numeric values."""
 
+    payload_type = DPTArray
     value_min: int | float
     value_max: int | float
     resolution: int | float
 
     @classmethod
     @abstractmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int | float:
-        """Parse/deserialize from KNX/IP raw data (big endian)."""
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int | float:
+        """Parse/deserialize from KNX/IP payload data."""
 
     @classmethod
     @abstractmethod
-    def to_knx(cls, value: int | float) -> bytes | tuple[int, ...]:
+    def to_knx(cls, value: int | float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
-
-
-class DPTBinary:
-    """The DPTBinary is a base class for all datatypes encoded directly into the last 6 bit of the APCI/data octet."""
-
-    APCI_BITMASK = 0x3F  # APCI uses first 2 bits
-
-    def __init__(self, value: int | tuple[int]) -> None:
-        """Initialize DPTBinary class."""
-        if isinstance(value, tuple):
-            value = value[0]
-        if not isinstance(value, int):
-            raise TypeError()
-        if not 0 <= value <= DPTBinary.APCI_BITMASK:
-            raise ConversionError("Could not init DPTBinary", value=str(value))
-
-        self.value = value
-
-    def __eq__(self, other: object) -> bool:
-        """Equal operator."""
-        if isinstance(other, DPTBinary):
-            return self.value == other.value
-        return False
-
-    def __repr__(self) -> str:
-        """Return object representation."""
-        return f"DPTBinary({hex(self.value)})"
-
-    def __str__(self) -> str:
-        """Return object as readable string."""
-        return f'<DPTBinary value="{self.value}" />'
-
-
-class DPTArray:
-    """The DPTArray is a base class for all datatypes appended to the KNX telegram."""
-
-    def __init__(self, value: int | bytes | tuple[int, ...] | list[int]) -> None:
-        """Initialize DPTArray class."""
-        self.value: tuple[int, ...]
-        if isinstance(value, int):
-            self.value = (value,)
-        elif isinstance(value, (list, bytes)):
-            self.value = tuple(value)
-        elif isinstance(value, tuple):
-            self.value = value
-        else:
-            raise TypeError()
-
-    def __eq__(self, other: object) -> bool:
-        """Equal operator."""
-        if isinstance(other, DPTArray):
-            return self.value == other.value
-        return False
-
-    def __repr__(self) -> str:
-        """Return object representation."""
-        return f"DPTArray(({', '.join(hex(b) for b in self.value)}))"
-
-    def __str__(self) -> str:
-        """Return object as readable string."""
-        return f'<DPTArray value="[{",".join(hex(b) for b in self.value)}]" />'
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_1byte_signed.py` & `xknx-2.8.0/xknx/dpt/dpt_1byte_signed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation of Basic KNX 1-Byte signed integer values."""
 from __future__ import annotations
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPTSignedRelativeValue(DPTNumeric):
     """
     Abstraction for KNX 1 Byte "1-octet Signed Relative Value".
 
     DPT 6.***
@@ -19,31 +20,31 @@
     payload_length = 1
 
     value_min = -128
     value_max = 127
     resolution = 1
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
         if raw[0] > cls.value_max:
             return raw[0] - 0x100
         return raw[0]
 
     @classmethod
-    def to_knx(cls, value: int | float) -> tuple[int]:
+    def to_knx(cls, value: int | float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = int(value)
             if not cls._test_boundaries(knx_value):
                 raise ValueError
             if knx_value < 0:
                 knx_value += 0x100
-            return (knx_value & 0xFF,)
+            return DPTArray(knx_value & 0xFF)
         except ValueError:
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
     @classmethod
     def _test_boundaries(cls, value: int) -> bool:
         """Test if value is within defined range for this object."""
         return cls.value_min <= value <= cls.value_max
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_1byte_uint.py` & `xknx-2.8.0/xknx/dpt/dpt_1byte_uint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation of Basic KNX DPT_1_Ucount Values."""
 from __future__ import annotations
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPTValue1ByteUnsigned(DPTNumeric):
     """
     Abstraction for KNX 1 Octet.
 
     DPT 5.***
@@ -19,35 +20,33 @@
     payload_length = 1
 
     value_min = 0
     value_max = 255
     resolution = 1
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
-
-        value = raw[0]
+        value = cls.validate_payload(payload)[0]
 
         if not cls._test_boundaries(value):
             raise ConversionError(
-                f"Could not parse {cls.__name__}", value=value, raw=raw
+                f"Could not parse {cls.__name__}", value=value, payload=payload
             )
 
         return value
 
     @classmethod
-    def to_knx(cls, value: int | float) -> tuple[int]:
+    def to_knx(cls, value: int | float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = int(value)
             if not cls._test_boundaries(knx_value):
                 raise ValueError
-            return (knx_value,)
+            return DPTArray(knx_value)
         except ValueError:
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
     @classmethod
     def _test_boundaries(cls, value: int) -> bool:
         """Test if value is within defined range for this object."""
         return cls.value_min <= value <= cls.value_max
@@ -115,30 +114,28 @@
     dpt_sub_number = 1
     value_type = "scene_number"
 
     value_min = 1
     value_max = 64
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
-
-        value = raw[0] + 1
+        value = cls.validate_payload(payload)[0] + 1
 
         if not cls._test_boundaries(value):
             raise ConversionError(
-                f"Could not parse {cls.__name__}", value=value, raw=raw
+                f"Could not parse {cls.__name__}", value=value, payload=payload
             )
 
         return value
 
     @classmethod
-    def to_knx(cls, value: int | float) -> tuple[int]:
+    def to_knx(cls, value: int | float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = int(value) - 1
             if not cls._test_boundaries(knx_value + 1):
                 raise ValueError
-            return (knx_value,)
+            return DPTArray(knx_value)
         except ValueError:
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_2byte_float.py` & `xknx-2.8.0/xknx/dpt/dpt_2byte_float.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 They correspond to the the following KDN DPT 9 class.
 """
 from __future__ import annotations
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPT2ByteFloat(DPTNumeric):
     """
     Abstraction for KNX 2 Octet Floating Point Numbers.
 
     DPT 9.***
@@ -23,17 +24,17 @@
     payload_length = 2
 
     value_min = -671088.64
     value_max = 670760.96
     resolution = 0.01
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> float:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> float:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
         data = (raw[0] * 256) + raw[1]
         exponent = (data >> 11) & 0x0F
         significand = data & 0x7FF
         sign = data >> 15
 
         if sign == 1:
             significand = significand - 2048
@@ -42,15 +43,15 @@
 
         if not cls._test_boundaries(value):
             raise ConversionError(f"Could not parse {cls.__name__}", value=value)
 
         return value
 
     @classmethod
-    def to_knx(cls, value: float) -> tuple[int, int]:
+    def to_knx(cls, value: float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = float(value)
             if not cls._test_boundaries(knx_value):
                 raise ValueError
 
             value = knx_value * 100
@@ -60,15 +61,15 @@
                 value /= 2
 
             mantisse = int(round(value)) & 0x7FF
             msb = exponent << 3 | mantisse >> 8
             if value < 0:
                 msb |= 0x80
 
-            return msb, mantisse & 0xFF
+            return DPTArray((msb, mantisse & 0xFF))
         except ValueError:
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
     @classmethod
     def _test_boundaries(cls, value: float) -> bool:
         """Test if value is within defined range for this object."""
         return cls.value_min <= value <= cls.value_max
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_2byte_signed.py` & `xknx-2.8.0/xknx/dpt/dpt_2byte_signed.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import annotations
 
 import struct
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPT2ByteSigned(DPTNumeric):
     """
     Abstraction for KNX 2 Byte signed values.
 
     DPT 8.***
@@ -28,31 +29,31 @@
     value_min = -32768
     value_max = 32767
     resolution = 1
 
     _struct_format = ">h"
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
 
         try:
-            return struct.unpack(cls._struct_format, bytes(raw))[0]  # type: ignore
+            return struct.unpack(cls._struct_format, bytes(raw))[0]  # type: ignore[no-any-return]
         except struct.error:
             raise ConversionError(f"Could not parse {cls.__name__}", raw=raw)
 
     @classmethod
-    def to_knx(cls, value: int | float) -> tuple[int, ...]:
+    def to_knx(cls, value: int | float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = int(value)
             if not cls._test_boundaries(knx_value):
                 raise ValueError
-            return tuple(struct.pack(cls._struct_format, knx_value))
+            return DPTArray(struct.pack(cls._struct_format, knx_value))
         except (ValueError, struct.error):
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
     @classmethod
     def _test_boundaries(cls, value: int) -> bool:
         """Test if value is within defined range for this object."""
         return cls.value_min <= value <= cls.value_max
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_2byte_uint.py` & `xknx-2.8.0/xknx/dpt/dpt_2byte_uint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation of Basic KNX 2-Byte/octet values."""
 from __future__ import annotations
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPT2ByteUnsigned(DPTNumeric):
     """
     Abstraction for KNX 2 Byte "2-octet unsigned value".
 
     Contains smaller counters, timers  etc.
@@ -21,27 +22,27 @@
     payload_length = 2
 
     value_min = 0
     value_max = 65535
     resolution = 1
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
         return (raw[0] * 256) + raw[1]
 
     @classmethod
-    def to_knx(cls, value: int | float) -> tuple[int, int]:
+    def to_knx(cls, value: int | float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = int(value)
             if not cls._test_boundaries(knx_value):
                 raise ValueError
-            return knx_value >> 8, knx_value & 0xFF
+            return DPTArray((knx_value >> 8, knx_value & 0xFF))
         except ValueError:
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
     @classmethod
     def _test_boundaries(cls, value: int) -> bool:
         """Test if value is within defined range for this object."""
         return cls.value_min <= value <= cls.value_max
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_4bit_control.py` & `xknx-2.8.0/xknx/dpt/dpt_4bit_control.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 from abc import ABC
 from enum import Enum
 from typing import Any
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTBase
+from .payload import DPTArray, DPTBinary
 
 
 class DPTControlStepCode(DPTBase, ABC):
     """Abstraction for KNX B1U3 values (DPT 3.007/3.008)."""
 
     # APCI (application layer control information)
     APCI_CONTROLMASK = 0x08
     APCI_STEPCODEMASK = 0x07
     APCI_MAX_VALUE = APCI_CONTROLMASK | APCI_STEPCODEMASK
 
+    payload_type = DPTBinary
     payload_length = 1
 
     @classmethod
     def _encode(cls, control: bool, step_code: int) -> int:
         """Encode control-bit with step-code."""
         value = 1 if control > 0 else 0
         return (value << 3) | (step_code & cls.APCI_STEPCODEMASK)
@@ -42,28 +44,22 @@
     def _decode(cls, value: int) -> tuple[bool, int]:
         """Decode value into control-bit and step-code."""
         control = bool(value & cls.APCI_CONTROLMASK)
         step_code = value & cls.APCI_STEPCODEMASK
         return control, step_code
 
     @classmethod
-    def _test_boundaries(cls, raw: int) -> bool:
-        """Test if raw KNX data is within defined range for this object."""
-        if isinstance(raw, int):
-            return 0 <= raw <= cls.APCI_MAX_VALUE
-
-    @classmethod
     def _test_values(cls, step_code: int) -> bool:
         """Test if input values are valid."""
         if isinstance(step_code, int) and 0 <= step_code <= cls.APCI_STEPCODEMASK:
             return True
         return False
 
     @classmethod
-    def to_knx(cls, value: Any) -> tuple[int]:
+    def to_knx(cls, value: Any) -> DPTBinary:
         """Serialize to KNX/IP raw data."""
         # TODO: use Tuple or Named Tuple instead of Dict[str, int] to account for bool control
         if not isinstance(value, dict):
             raise ConversionError(
                 f"Can't serialize {cls.__name__}; invalid value type", value=value
             )
 
@@ -76,24 +72,24 @@
             )
 
         if not cls._test_values(step_code):
             raise ConversionError(
                 f"Can't serialize {cls.__name__}; invalid values", value=value
             )
 
-        return (cls._encode(control, step_code),)
+        return DPTBinary(cls._encode(control, step_code))
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> Any:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> Any:
         """Parse/deserialize from KNX/IP raw data."""
-        if not isinstance(raw, tuple) or not cls._test_boundaries(raw[0]):
+        raw = cls.validate_payload(payload)[0]
+        if raw > cls.APCI_MAX_VALUE:
             raise ConversionError(f"Can't parse {cls.__name__}", raw=raw)
 
-        control, step_code = cls._decode(raw[0])
-
+        control, step_code = cls._decode(raw)
         return {"control": control, "step_code": step_code}
 
 
 class DPTControlStepwise(DPTControlStepCode):
     """Abstraction for KNX DPT 3.xxx in stepwise mode with conversion to an increment value."""
 
     dpt_main_number = 3
@@ -132,25 +128,25 @@
     def _to_increment(value: dict[str, int]) -> int:
         """Calculate the increment value from the stepcode and control bit as defined in the KNX standard section 3.3.1."""
         # calculated using floor(100/2^((value&0x07)-1))
         inc = [0, 100, 50, 25, 12, 6, 3, 1][value["step_code"] & 0x07]
         return inc if value["control"] == 1 else -inc
 
     @classmethod
-    def to_knx(cls, value: int | dict[str, int]) -> tuple[int]:
+    def to_knx(cls, value: int | dict[str, int]) -> DPTBinary:
         """Serialize to KNX/IP raw data."""
         if not isinstance(value, int):
             raise ConversionError(f"Can't serialize {cls.__name__}", value=value)
 
         return super().to_knx(cls._from_increment(value))
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        return cls._to_increment(super().from_knx(raw))
+        return cls._to_increment(super().from_knx(payload))
 
 
 class DPTControlStepwiseDimming(DPTControlStepwise):
     """Abstraction for KNX DPT 3.007 / DPT_Control_Dimming in stepwise mode."""
 
     dpt_main_number = 3
     dpt_sub_number = 7
@@ -185,15 +181,15 @@
         """Enum for indicating the direction."""
 
         DECREASE = 0
         INCREASE = 1
         STOP = 2
 
     @classmethod
-    def to_knx(cls, value: Direction) -> tuple[int]:
+    def to_knx(cls, value: Direction) -> DPTBinary:
         """Convert value to payload."""
         control = 0
         step_code = 0
         if value == cls.Direction(1):  # INCREASE/DOWN
             control = 1
             step_code = 1
         elif value == cls.Direction(0):  # DECREASE/UP
@@ -205,17 +201,17 @@
         else:
             raise ConversionError(f"Can't serialize {cls.__name__}", value=value)
 
         values = {"control": control, "step_code": step_code}
         return super().to_knx(values)
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> Direction:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> Direction:
         """Convert current payload to value."""
-        values = super().from_knx(raw)
+        values = super().from_knx(payload)
         if values["step_code"] == 0:
             return cls.Direction(2)  # STOP
         if values["control"] == 0:
             return cls.Direction(0)  # DECREASE/UP
         return cls.Direction(1)  # INCREASE/DOWN
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_4byte_float.py` & `xknx-2.8.0/xknx/dpt/dpt_4byte_float.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from math import ceil, log10
 import struct
 from typing import cast
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPT4ByteFloat(DPTNumeric):
     """
     Abstraction for KNX 4 Octet Floating Point Numbers, with a maximum usable range as specified in IEEE 754.
 
     The largest positive finite float literal is 3.40282347e+38f.
@@ -32,36 +33,36 @@
     payload_length = 4
 
     value_min = float("-inf")
     value_max = float("inf")
     resolution = 0.0000001
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> float:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> float:
         """Parse/deserialize from KNX/IP raw data (big endian)."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
         try:
             raw_float = cast(float, struct.unpack(">f", bytes(raw))[0])
         except struct.error:
             raise ConversionError(f"Could not parse {cls.__name__}", raw=raw)
         try:
             # round to 7 digit precision independent of exponent - same value as ETS 5.7 group monitor
             return round(raw_float, 7 - ceil(log10(abs(raw_float))))
         except (ValueError, OverflowError):
             # account for 0 and special values
             # ValueError: log10(0.0); ceil(float('nan'))
             # OverflowError: ceil(float('inf'))
             return raw_float
 
     @classmethod
-    def to_knx(cls, value: float) -> tuple[int, ...]:
+    def to_knx(cls, value: float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = float(value)
-            return tuple(struct.pack(">f", knx_value))
+            return DPTArray(struct.pack(">f", knx_value))
         except (ValueError, struct.error):
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
 
 class DPTAcceleration(DPT4ByteFloat):
     """DPT 14.000 DPT_Value_Acceleration (ms-2)."""
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_4byte_int.py` & `xknx-2.8.0/xknx/dpt/dpt_4byte_int.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from __future__ import annotations
 
 import struct
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPT4ByteUnsigned(DPTNumeric):
     """
     Abstraction for KNX 4 Byte "32-bit unsigned".
 
     DPT 12.***
@@ -29,31 +30,31 @@
     value_min = 0
     value_max = 4294967295
     resolution = 1
 
     _struct_format = ">I"
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
 
         try:
-            return struct.unpack(cls._struct_format, bytes(raw))[0]  # type: ignore
+            return struct.unpack(cls._struct_format, bytes(raw))[0]  # type: ignore[no-any-return]
         except struct.error:
             raise ConversionError(f"Could not parse {cls.__name__}", raw=raw)
 
     @classmethod
-    def to_knx(cls, value: int | float) -> tuple[int, ...]:
+    def to_knx(cls, value: int | float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = int(value)
             if not cls._test_boundaries(knx_value):
                 raise ValueError
-            return tuple(struct.pack(cls._struct_format, knx_value))
+            return DPTArray(struct.pack(cls._struct_format, knx_value))
         except (ValueError, struct.error):
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
     @classmethod
     def _test_boundaries(cls, value: int) -> bool:
         """Test if value is within defined range for this object."""
         return cls.value_min <= value <= cls.value_max
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_color.py` & `xknx-2.8.0/xknx/dpt/dpt_color.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 from typing import NamedTuple
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTBase
+from .payload import DPTArray, DPTBinary
 
 
 class XYYColor(NamedTuple):
     """
     Representation of XY color with brightness.
 
     `color`: tuple(x-axis, y-axis) each 0..1; None if invalid.
@@ -20,20 +21,21 @@
     color: tuple[float, float] | None = None
     brightness: int | None = None
 
 
 class DPTColorXYY(DPTBase):
     """Abstraction for KNX 6 octet color xyY (DPT 242.600)."""
 
+    payload_type = DPTArray
     payload_length = 6
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> XYYColor:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> XYYColor:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
 
         x_axis_int = raw[0] << 8 | raw[1]
         y_axis_int = raw[2] << 8 | raw[3]
         brightness = raw[4]
 
         color_valid = raw[5] >> 1 & 0b1
         brightness_valid = raw[5] & 0b1
@@ -48,15 +50,15 @@
             else None,
             brightness=brightness if brightness_valid else None,
         )
 
     @classmethod
     def to_knx(
         cls, value: XYYColor | tuple[tuple[float, float] | None, int | None]
-    ) -> tuple[int, int, int, int, int, int]:
+    ) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             if not isinstance(value, XYYColor):
                 value = XYYColor(*value)
             color_valid = False
             brightness_valid = False
             x_axis, y_axis, brightness = 0, 0, 0
@@ -69,17 +71,19 @@
 
             if value.brightness is not None:
                 if not 0 <= value.brightness <= 255:
                     raise ValueError
                 brightness_valid = True
                 brightness = int(value.brightness)
 
-            return (
-                x_axis >> 8,
-                x_axis & 0xFF,
-                y_axis >> 8,
-                y_axis & 0xFF,
-                brightness,
-                color_valid << 1 | brightness_valid,
+            return DPTArray(
+                (
+                    x_axis >> 8,
+                    x_axis & 0xFF,
+                    y_axis >> 8,
+                    y_axis & 0xFF,
+                    brightness,
+                    color_valid << 1 | brightness_valid,
+                )
             )
         except (ValueError, TypeError):
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_date.py` & `xknx-2.8.0/xknx/dpt/dpt_date.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from __future__ import annotations
 
 import time
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTBase
+from .payload import DPTArray, DPTBinary
 
 
 class DPTDate(DPTBase):
     """Abstraction for KNX 3 octet date (DPT 11.001)."""
 
+    payload_type = DPTArray
     payload_length = 3
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> time.struct_time:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> time.struct_time:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
 
         day = raw[0] & 0x1F
         month = raw[1] & 0x0F
         year = raw[2] & 0x7F
 
         if not DPTDate._test_range(day, month, year):
             raise ConversionError("Could not parse DPTDate", raw=raw)
@@ -33,28 +35,34 @@
         try:
             # strptime conversion used for catching exceptions; filled with default values
             return time.strptime(f"{year} {month} {day}", "%Y %m %d")
         except ValueError:
             raise ConversionError("Could not parse DPTDate", raw=raw)
 
     @classmethod
-    def to_knx(cls, value: time.struct_time) -> tuple[int, int, int]:
+    def to_knx(cls, value: time.struct_time) -> DPTArray:
         """Serialize to KNX/IP raw data from time.struct_time."""
 
         def _knx_year(year: int) -> int:
             if 2000 <= year < 2090:
                 return year - 2000
             if 1990 <= year < 2000:
                 return year - 1900
             raise ConversionError("Could not serialize DPTDate", year=year)
 
         if not isinstance(value, time.struct_time):
             raise ConversionError("Could not serialize DPTDate", value=value)
 
-        return (value.tm_mday, value.tm_mon, _knx_year(value.tm_year))
+        return DPTArray(
+            (
+                value.tm_mday,
+                value.tm_mon,
+                _knx_year(value.tm_year),
+            )
+        )
 
     @staticmethod
     def _test_range(day: int, month: int, year: int) -> bool:
         """Test if the values are in the correct range."""
         if not 1 <= day <= 31:
             return False
         if not 1 <= month <= 12:
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_datetime.py` & `xknx-2.8.0/xknx/dpt/dpt_datetime.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from __future__ import annotations
 
 import time
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTBase
+from .payload import DPTArray, DPTBinary
 
 
 class DPTDateTime(DPTBase):
     """Abstraction for KNX 8 octet datetime (DPT 19.001)."""
 
+    payload_type = DPTArray
     payload_length = 8
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> time.struct_time:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> time.struct_time:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
 
         year = raw[0] + 1900
         month = raw[1] & 0x0F
         day = raw[2] & 0x3F
         weekday = (raw[3] & 0xE0) >> 5
         hours = raw[3] & 0x1F
         minutes = raw[4] & 0x3F
@@ -63,31 +65,33 @@
 
             return time.strptime(time_string, time_format)
 
         except ValueError:
             raise ConversionError("Could not parse DPTDateTime", raw=raw)
 
     @classmethod
-    def to_knx(cls, value: time.struct_time) -> tuple[int, ...]:
+    def to_knx(cls, value: time.struct_time) -> DPTArray:
         """Serialize to KNX/IP raw data from time.struct_time."""
         if not isinstance(value, time.struct_time):
             raise ConversionError("Could not serialize DPTDateTime", value=value)
 
         knx_year = (value.tm_year - 1900) & 0xFF
         month = value.tm_mon
         day = value.tm_mday
         weekday = value.tm_wday + 1
         hours = value.tm_hour
         minutes = value.tm_min
         seconds = value.tm_sec
         dst = value.tm_isdst == 1  # tm_isdst can be -1
 
-        return (
-            knx_year,
-            month,
-            day,
-            weekday << 5 | hours,
-            minutes,
-            seconds,
-            0x20 | dst,  # 0x20 working day not valid
-            0x80,  # assume clock with ext. sync signal
+        return DPTArray(
+            (
+                knx_year,
+                month,
+                day,
+                weekday << 5 | hours,
+                minutes,
+                seconds,
+                0x20 | dst,  # 0x20 working day not valid
+                0x80,  # assume clock with ext. sync signal
+            )
         )
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_hvac_mode.py` & `xknx-2.8.0/xknx/dpt/dpt_hvac_mode.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from enum import Enum
 from typing import Generic, TypeVar
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTBase
+from .payload import DPTArray, DPTBinary
 
 HVACModeT = TypeVar("HVACModeT", "HVACControllerMode", "HVACOperationMode")
 
 
 class HVACOperationMode(Enum):
     """Enum for the different KNX HVAC operation modes."""
 
@@ -41,31 +42,32 @@
 
 
 class _DPTClimateMode(DPTBase, Generic[HVACModeT]):
     """Base class for KNX Climate modes."""
 
     SUPPORTED_MODES: dict[int, HVACModeT] = {}
 
+    payload_type = DPTArray
     payload_length = 1
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> HVACModeT:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> HVACModeT:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
         try:
             return cls.SUPPORTED_MODES[raw[0]]
         except KeyError:
             raise ConversionError(f"Payload not supported for {cls.__name__}", raw=raw)
 
     @classmethod
-    def to_knx(cls, value: HVACModeT) -> tuple[int]:
+    def to_knx(cls, value: HVACModeT) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         for knx_value, mode in cls.SUPPORTED_MODES.items():
             if mode == value:
-                return (knx_value,)
+                return DPTArray(knx_value)
         raise ConversionError(f"Value not supported for {cls.__name__}", value=value)
 
 
 class DPTHVACContrMode(_DPTClimateMode[HVACControllerMode]):
     """
     Abstraction for KNX HVAC controller mode.
 
@@ -121,17 +123,17 @@
         0x21: HVACOperationMode.COMFORT,
         0x22: HVACOperationMode.STANDBY,
         0x24: HVACOperationMode.NIGHT,
         0x28: HVACOperationMode.FROST_PROTECTION,
     }
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> HVACOperationMode:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> HVACOperationMode:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
         if raw[0] & 8 > 0:
             return HVACOperationMode.FROST_PROTECTION
         if raw[0] & 4 > 0:
             return HVACOperationMode.NIGHT
         if raw[0] & 2 > 0:
             return HVACOperationMode.STANDBY
         if raw[0] & 1 > 0:
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_scaling.py` & `xknx-2.8.0/xknx/dpt/dpt_scaling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Implementation of scaled KNX DPT_1_Ucount Values."""
 from __future__ import annotations
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTNumeric
+from .payload import DPTArray, DPTBinary
 
 
 class DPTScaling(DPTNumeric):
     """
     Abstraction for KNX 1 Octet Percent.
 
     DPT 5.001
@@ -20,40 +21,37 @@
     payload_length = 1
 
     value_min = 0
     value_max = 100
     resolution = 1
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> int:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> int:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
-
-        knx_value = raw[0]
+        knx_value = cls.validate_payload(payload)[0]
         delta = cls.value_max - cls.value_min
         value = round((knx_value / 255) * delta) + cls.value_min
 
         if not cls._test_boundaries(value):
             raise ConversionError(
-                f"Could not parse {cls.__name__}", value=value, raw=raw
+                f"Could not parse {cls.__name__}", value=value, payload=payload
             )
-
         return value
 
     @classmethod
-    def to_knx(cls, value: float) -> tuple[int]:
+    def to_knx(cls, value: float) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             percent_value = float(value)
             if not cls._test_boundaries(percent_value):
                 raise ValueError
             delta = cls.value_max - cls.value_min
             knx_value = round((percent_value - cls.value_min) / delta * 255)
 
-            return (knx_value,)
+            return DPTArray(knx_value)
         except ValueError:
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
 
     @classmethod
     def _test_boundaries(cls, value: float) -> bool:
         """Test if value is within defined range for this object."""
         return cls.value_min <= value <= cls.value_max
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_string.py` & `xknx-2.8.0/xknx/dpt/dpt_string.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 """Implementation of 3.17 Datapoint Types String."""
 from __future__ import annotations
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTBase
+from .payload import DPTArray, DPTBinary
 
 
 class DPTString(DPTBase):
     """
     Abstraction for KNX 14 Octet ASCII string.
 
     DPT 16.000
     """
 
+    payload_type = DPTArray
     payload_length = 14
     dpt_main_number = 16
     dpt_sub_number = 0
     value_type = "string"
     unit = None
 
     _encoding = "ascii"
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> str:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> str:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
         return bytes(byte for byte in raw if byte != 0x00).decode(
             cls._encoding, errors="replace"
         )
 
     @classmethod
-    def to_knx(cls, value: str) -> tuple[int, ...]:
+    def to_knx(cls, value: str) -> DPTArray:
         """Serialize to KNX/IP raw data."""
         try:
             knx_value = str(value)
             if not cls._test_boundaries(knx_value):
                 raise ValueError
         except ValueError:
             raise ConversionError(f"Could not serialize {cls.__name__}", value=value)
         # replace invalid characters with question marks
         raw_bytes = knx_value.encode(cls._encoding, errors="replace")
         padding = bytes(cls.payload_length - len(raw_bytes))
-        return tuple(raw_bytes + padding)
+        return DPTArray(raw_bytes + padding)
 
     @classmethod
     def _test_boundaries(cls, value: str) -> bool:
         """Test if value is within defined range for this object."""
         return len(value) <= cls.payload_length
```

### Comparing `xknx-2.7.0/xknx/dpt/dpt_time.py` & `xknx-2.8.0/xknx/dpt/dpt_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 from __future__ import annotations
 
 import time
 
 from xknx.exceptions import ConversionError
 
 from .dpt import DPTBase
+from .payload import DPTArray, DPTBinary
 
 
 class DPTTime(DPTBase):
     """
     Abstraction for KNX 3 Octet Time.
 
     DPT 10.001
     """
 
+    payload_type = DPTArray
     payload_length = 3
 
     @classmethod
-    def from_knx(cls, raw: tuple[int, ...]) -> time.struct_time:
+    def from_knx(cls, payload: DPTArray | DPTBinary) -> time.struct_time:
         """Parse/deserialize from KNX/IP raw data."""
-        cls.test_bytesarray(raw)
+        raw = cls.validate_payload(payload)
 
         weekday = (raw[0] & 0xE0) >> 5
         hours = raw[0] & 0x1F
         minutes = raw[1] & 0x3F
         seconds = raw[2] & 0x3F
 
         if not DPTTime._test_range(weekday, hours, minutes, seconds):
@@ -41,30 +43,36 @@
             return time.strptime(
                 f"{hours} {minutes} {seconds} {weekday}", "%H %M %S %w"
             )
         except ValueError:
             raise ConversionError("Could not parse DPTTime", raw=raw)
 
     @classmethod
-    def to_knx(cls, value: time.struct_time) -> tuple[int, int, int]:
+    def to_knx(cls, value: time.struct_time) -> DPTArray:
         """Serialize to KNX/IP raw data from dict with elements weekday,hours,minutes,seconds."""
         if not isinstance(value, time.struct_time):
             raise ConversionError(
                 "Could not serialize DPTTime - time.struct_time expected", value=value
             )
 
         _default_time = time.strptime("", "")
         weekday = 0
         # if 0 year, 1 month, 2 day, 6 weekday, 7 yearday, 8 dst are equal to default assume "any weekday" (0)
         for index in [0, 1, 2, 6, 7, 8]:
             if value[index] is not _default_time[index]:
                 weekday = value.tm_wday + 1
                 break
 
-        return (weekday << 5 | value.tm_hour, value.tm_min, value.tm_sec)
+        return DPTArray(
+            (
+                weekday << 5 | value.tm_hour,
+                value.tm_min,
+                value.tm_sec,
+            )
+        )
 
     @staticmethod
     def _test_range(weekday: int, hours: int, minutes: int, seconds: int) -> bool:
         """Test if values are in the correct value range."""
         if not 0 <= weekday <= 7:
             return False
         if not 0 <= hours <= 23:
```

### Comparing `xknx-2.7.0/xknx/exceptions/__init__.py` & `xknx-2.8.0/xknx/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/exceptions/exception.py` & `xknx-2.8.0/xknx/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/__init__.py` & `xknx-2.8.0/xknx/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/connection.py` & `xknx-2.8.0/xknx/io/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         * TUNNELING connect to a specific KNX/IP tunneling device via UDP.
         * TUNNELING_TCP connect to a specific KNX/IP tunneling v2 device via TCP.
     * individual address:
         * AUTOMATIC use a specific tunnel endpoint from a given knxkeys file
         * ROUTING the individual address used as source address for routing
         * TCP TUNNELING request a specific tunnel endpoint
         * SECURE TUNNELING use a specific tunnel endpoint from the knxkeys file
-    * local_ip: Local ip of the interface though which KNXIPInterface should connect.
-    * gateway_ip: IP of KNX/IP tunneling device.
+    * local_ip: Local ip or interface name though which xknx should connect.
+    * gateway_ip: IP or hostname of KNX/IP tunneling device.
     * gateway_port: Port of KNX/IP tunneling device.
     * route_back: For UDP TUNNELING connection.
         The KNXnet/IP Server shall use the IP address and port in the received IP package
         as the target IP address or port number for the response to the KNXnet/IP Client.
     * multicast_group: Multicast group for KNXnet/IP routing.
     * multicast_port: Multicast port for KNXnet/IP routing.
     * auto_reconnect: Auto reconnect to KNX/IP tunneling device if connection cannot be established.
```

### Comparing `xknx-2.7.0/xknx/io/const.py` & `xknx-2.8.0/xknx/io/const.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/gateway_scanner.py` & `xknx-2.8.0/xknx/io/gateway_scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,21 +238,22 @@
                 scan_task.cancel()
             await scan_task  # to bubble up exceptions
 
     async def _scan(
         self, queue: asyncio.Queue[GatewayDescriptor | None] | None = None
     ) -> None:
         """Scan for gateways."""
-        local_ip = self.local_ip or await util.get_default_local_ip(
+        _local_ip = self.local_ip or await util.get_default_local_ip(
             remote_ip=self.xknx.multicast_group
         )
-        if local_ip is None:
+        if _local_ip is None:
             if queue is not None:
                 queue.put_nowait(None)
             raise XKNXException("No usable network interface found.")
+        local_ip = await util.validate_ip(_local_ip)
         interface_name = util.get_local_interface_name(local_ip=local_ip)
         logger.debug("Searching on %s / %s", interface_name, local_ip)
 
         udp_transport = UDPTransport(
             local_addr=(local_ip, 0),
             remote_addr=(self.xknx.multicast_group, self.xknx.multicast_port),
         )
```

### Comparing `xknx-2.7.0/xknx/io/interface.py` & `xknx-2.8.0/xknx/io/interface.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/ip_secure.py` & `xknx-2.8.0/xknx/io/ip_secure.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/knxip_interface.py` & `xknx-2.8.0/xknx/io/knxip_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,60 +69,69 @@
 
     async def start(self) -> None:
         """Start KNX/IP interface. Raise `CommunicationError` if connection fails."""
         await self._start()
 
     async def _start(self) -> None:
         """Start interface. Connecting KNX/IP device with the selected method."""
+        if gateway_ip := self.connection_config.gateway_ip:
+            gateway_ip = await util.validate_ip(gateway_ip, address_name="Gateway IP")
+        if local_ip := self.connection_config.local_ip:
+            local_ip = await util.validate_ip(local_ip, address_name="Local IP")
         keyring: Keyring | None = None
         if secure_config := self.connection_config.secure_config:
             if (
                 secure_config.knxkeys_file_path is not None
                 and secure_config.knxkeys_password is not None
             ):
                 keyring = await load_keyring(
                     secure_config.knxkeys_file_path,
                     secure_config.knxkeys_password,
                 )
         self.xknx.cemi_handler.data_secure_init(keyring=keyring)
 
         if self.connection_config.connection_type == ConnectionType.ROUTING:
-            await self._start_routing()
+            await self._start_routing(local_ip=local_ip)
         elif self.connection_config.connection_type == ConnectionType.ROUTING_SECURE:
-            await self._start_secure_routing(keyring=keyring)
+            await self._start_secure_routing(local_ip=local_ip, keyring=keyring)
         elif (
             self.connection_config.connection_type == ConnectionType.TUNNELING
-            and self.connection_config.gateway_ip is not None
+            and gateway_ip is not None
         ):
             await self._start_tunnelling_udp(
-                gateway_ip=self.connection_config.gateway_ip,
+                gateway_ip=gateway_ip,
                 gateway_port=self.connection_config.gateway_port,
+                local_ip=local_ip,
             )
         elif (
             self.connection_config.connection_type == ConnectionType.TUNNELING_TCP
-            and self.connection_config.gateway_ip is not None
+            and gateway_ip is not None
         ):
             await self._start_tunnelling_tcp(
-                gateway_ip=self.connection_config.gateway_ip,
+                gateway_ip=gateway_ip,
                 gateway_port=self.connection_config.gateway_port,
             )
         elif (
             self.connection_config.connection_type
             == ConnectionType.TUNNELING_TCP_SECURE
-            and self.connection_config.gateway_ip is not None
+            and gateway_ip is not None
         ):
             await self._start_secure_tunnelling_tcp(
-                gateway_ip=self.connection_config.gateway_ip,
+                gateway_ip=gateway_ip,
                 gateway_port=self.connection_config.gateway_port,
                 keyring=keyring,
             )
         else:
-            await self._start_automatic(keyring=keyring)
+            await self._start_automatic(local_ip=local_ip, keyring=keyring)
 
-    async def _start_automatic(self, keyring: Keyring | None) -> None:
+    async def _start_automatic(
+        self,
+        local_ip: str | None,
+        keyring: Keyring | None,
+    ) -> None:
         """Start GatewayScanner and connect to the found device."""
         keyring_host_filter: set[IndividualAddress] = set()
         if keyring:
             if required_addr := self.connection_config.individual_address:
                 _host_ia = keyring.get_tunnel_host_by_interface(
                     tunnelling_slot=required_addr
                 )
@@ -134,18 +143,17 @@
             else:
                 keyring_host_filter.update(
                     interface.host
                     for interface in keyring.interfaces
                     if interface.host is not None
                     and interface.type is InterfaceType.TUNNELING
                 )
-
         async for gateway in GatewayScanner(
             self.xknx,
-            local_ip=self.connection_config.local_ip,
+            local_ip=local_ip,
             scan_filter=self.connection_config.scan_filter,
         ).async_scan():
             if (
                 keyring_host_filter
                 and gateway.individual_address not in keyring_host_filter
             ):
                 logger.debug("Skipping %s. No match in keyring file", gateway)
@@ -167,17 +175,18 @@
                 elif (
                     gateway.supports_tunnelling
                     and not gateway.tunnelling_requires_secure
                 ):
                     await self._start_tunnelling_udp(
                         gateway_ip=gateway.ip_addr,
                         gateway_port=gateway.port,
+                        local_ip=local_ip,
                     )
                 elif gateway.supports_routing and not gateway.routing_requires_secure:
-                    await self._start_routing()
+                    await self._start_routing(local_ip=local_ip)
             except CommunicationError as ex:
                 logger.debug("Skipping %s. Could not connect: %s", gateway, ex)
                 continue
             except InvalidSecureConfiguration as ex:
                 logger.debug(
                     "Skipping %s. Invalid secure configuration: %s", gateway, ex
                 )
@@ -192,15 +201,14 @@
 
     async def _start_tunnelling_tcp(
         self,
         gateway_ip: str,
         gateway_port: int,
     ) -> None:
         """Start KNX/IP TCP tunnel."""
-        util.validate_ip(gateway_ip, address_name="Gateway IP address")
         tunnel_address = self.connection_config.individual_address
 
         logger.debug(
             "Starting tunnel to %s:%s over TCP%s",
             gateway_ip,
             gateway_port,
             f" requesting individual address {tunnel_address}"
@@ -259,15 +267,14 @@
             user_password = xml_interface.decrypted_password
             device_authentication_password = xml_interface.decrypted_authentication
         else:
             raise InvalidSecureConfiguration(
                 "No `user_id` or `knxkeys_file_path` and password found in secure configuration"
             )
 
-        util.validate_ip(gateway_ip, address_name="Gateway IP address")
         logger.debug(
             "Starting secure tunnel to %s:%s over TCP",
             gateway_ip,
             gateway_port,
         )
         self._interface = SecureTunnel(
             self.xknx,
@@ -335,29 +342,27 @@
             "No credentials for any free tunnelling slot found in keyfile"
         )
 
     async def _start_tunnelling_udp(
         self,
         gateway_ip: str,
         gateway_port: int,
+        local_ip: str | None,
     ) -> None:
         """Start KNX/IP UDP tunnel."""
-        util.validate_ip(gateway_ip, address_name="Gateway IP address")
-        local_ip = self.connection_config.local_ip or util.find_local_ip(
-            gateway_ip=gateway_ip
-        )
         local_port = self.connection_config.local_port
         route_back = self.connection_config.route_back
+
+        local_ip = local_ip or util.find_local_ip(gateway_ip=gateway_ip)
         if local_ip is None:
             local_ip = await util.get_default_local_ip(gateway_ip)
             if local_ip is None:
                 raise XKNXException("No network interface found.")
             route_back = True
             logger.debug("Falling back to default interface and enabling route back.")
-        util.validate_ip(local_ip, address_name="Local IP address")
 
         logger.debug(
             "Starting tunnel from %s:%s to %s:%s",
             local_ip,
             local_port,
             gateway_ip,
             gateway_port,
@@ -371,22 +376,23 @@
             route_back=route_back,
             cemi_received_callback=self.cemi_received,
             auto_reconnect=self.connection_config.auto_reconnect,
             auto_reconnect_wait=self.connection_config.auto_reconnect_wait,
         )
         await self._interface.connect()
 
-    async def _start_routing(self) -> None:
+    async def _start_routing(self, local_ip: str | None) -> None:
         """Start KNX/IP Routing."""
         multicast_group = self.connection_config.multicast_group
         multicast_port = self.connection_config.multicast_port
-        local_ip = self.connection_config.local_ip or await util.get_default_local_ip()
+
+        local_ip = local_ip or await util.get_default_local_ip()
         if local_ip is None:
             raise XKNXException("No network interface found.")
-        util.validate_ip(local_ip, address_name="Local IP address")
+
         individual_address = (
             self.connection_config.individual_address or DEFAULT_INDIVIDUAL_ADDRESS
         )
 
         logger.debug(
             "Starting Routing from %s as %s via %s:%s",
             local_ip,
@@ -402,14 +408,15 @@
             multicast_group=multicast_group,
             multicast_port=multicast_port,
         )
         await self._interface.connect()
 
     async def _start_secure_routing(
         self,
+        local_ip: str | None,
         keyring: Keyring | None = None,
     ) -> None:
         """Start KNX/IP Routing."""
         if self.connection_config.secure_config is None:
             raise InvalidSecureConfiguration("SecureConfig missing in ConnectionConfig")
         backbone_key = self.connection_config.secure_config.backbone_key
         latency_ms = self.connection_config.secure_config.latency_ms
@@ -423,18 +430,18 @@
             if keyring.backbone.multicast_address:
                 multicast_group = keyring.backbone.multicast_address
         if not backbone_key:
             raise InvalidSecureConfiguration(
                 "No backbone key found in secure configuration"
             )
 
-        local_ip = self.connection_config.local_ip or await util.get_default_local_ip()
+        local_ip = local_ip or await util.get_default_local_ip()
         if local_ip is None:
             raise XKNXException("No network interface found.")
-        util.validate_ip(local_ip, address_name="Local IP address")
+
         individual_address = (
             self.connection_config.individual_address or DEFAULT_INDIVIDUAL_ADDRESS
         )
 
         logger.debug(
             "Starting Secure Routing from %s as %s via %s:%s",
             local_ip,
```

### Comparing `xknx-2.7.0/xknx/io/request_response/authenticate.py` & `xknx-2.8.0/xknx/io/request_response/authenticate.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/request_response/connect.py` & `xknx-2.8.0/xknx/io/request_response/connect.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/request_response/connectionstate.py` & `xknx-2.8.0/xknx/io/request_response/connectionstate.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/request_response/device_configuration.py` & `xknx-2.8.0/xknx/io/request_response/device_configuration.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/request_response/disconnect.py` & `xknx-2.8.0/xknx/io/request_response/disconnect.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/request_response/request_response.py` & `xknx-2.8.0/xknx/io/request_response/request_response.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/request_response/session.py` & `xknx-2.8.0/xknx/io/request_response/session.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/request_response/tunnelling.py` & `xknx-2.8.0/xknx/io/request_response/tunnelling.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/routing.py` & `xknx-2.8.0/xknx/io/routing.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/self_description.py` & `xknx-2.8.0/xknx/io/self_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 import asyncio
 import logging
 from typing import TYPE_CHECKING, Final
 
-from xknx.exceptions import CommunicationError
+from xknx.exceptions import CommunicationError, XKNXException
 from xknx.io import util
 from xknx.io.gateway_scanner import GatewayDescriptor
 from xknx.knxip import (
     HPAI,
     SRP,
     DescriptionRequest,
     DescriptionResponse,
@@ -44,14 +44,19 @@
         # Fall back to default interface and use route back
         local_ip = await util.get_default_local_ip(gateway_ip)
         if local_ip is None:
             raise CommunicationError(
                 f"No network interface found to request gateway info from {gateway_ip}:{gateway_port}"
             )
         route_back = True
+    try:
+        local_ip = await util.validate_ip(local_ip, address_name="Local IP")
+        gateway_ip = await util.validate_ip(gateway_ip, address_name="Gateway IP")
+    except XKNXException as err:
+        raise CommunicationError("Invalid address") from err
 
     transport = UDPTransport(
         local_addr=(local_ip, local_port),
         remote_addr=(gateway_ip, gateway_port),
         multicast=False,
     )
     try:
```

### Comparing `xknx-2.7.0/xknx/io/transport/ip_transport.py` & `xknx-2.8.0/xknx/io/transport/ip_transport.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/transport/tcp_transport.py` & `xknx-2.8.0/xknx/io/transport/tcp_transport.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/transport/udp_transport.py` & `xknx-2.8.0/xknx/io/transport/udp_transport.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/tunnel.py` & `xknx-2.8.0/xknx/io/tunnel.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/io/util.py` & `xknx-2.8.0/xknx/io/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
         sock.setblocking(False)  # must be non-blocking for async
         loop = asyncio.get_running_loop()
         try:
             await loop.sock_connect(sock, (remote_ip, DEFAULT_MCAST_PORT))
             local_ip = sock.getsockname()[0]
             logger.debug("Using local ip: %s", local_ip)
-            return cast(str, local_ip)
+            return local_ip  # type: ignore[no-any-return]
         except Exception:  # pylint: disable=broad-except
             logger.warning(
                 "The system could not auto detect the source ip for %s on your operating system",
                 remote_ip,
             )
             return None
 
@@ -40,25 +40,55 @@
 
 
 def get_local_interface_name(local_ip: str) -> str:
     """Return the name of the interface with the given ip."""
     return next((link.nice_name for link in get_local_ips() if link.ip == local_ip), "")
 
 
+def get_ip_for_adapter_name(name: str) -> str | None:
+    """Return the ip for the given interface name."""
+    return next(
+        (
+            ip.ip  # type: ignore[misc] # IPv6 would return tuple
+            for iface in ifaddr.get_adapters()
+            if name in (iface.name, iface.nice_name)
+            for ip in iface.ips
+            if ip.is_IPv4
+        ),
+        None,
+    )
+
+
 def find_local_ip(gateway_ip: str) -> str | None:
     """Find local IP address on same subnet as gateway."""
     gateway = ipaddress.IPv4Address(gateway_ip)
     for link in get_local_ips():
         network = ipaddress.IPv4Network((link.ip, link.network_prefix), strict=False)
         if gateway in network:
             logger.debug("Using interface: %s", link.nice_name)
             return cast(str, link.ip)
     logger.debug("No interface on same subnet as gateway found.")
     return None
 
 
-def validate_ip(address: str, address_name: str = "IP address") -> None:
-    """Raise an exception if address cannot be parsed as IPv4 address."""
+async def validate_ip(address: str, address_name: str = "IP address") -> str:
+    """
+    Return IPv4 address parsed or resolved as a string.
+
+    Valid addresses are IPv4 strings, adapter names or hostnames.
+    Raises XKNXException if address is not a valid IPv4 address or cannot be resolved.
+    """
     try:
         ipaddress.IPv4Address(address)
+        return address
     except ipaddress.AddressValueError as ex:
-        raise XKNXException(f"{address_name} is not a valid IPv4 address.") from ex
+        logger.debug(
+            "%s is not a valid IPv4 address: %s. Trying to resolve...",
+            address_name,
+            ex,
+        )
+    if adapter_ip := get_ip_for_adapter_name(address):
+        return adapter_ip
+    try:
+        return await asyncio.to_thread(socket.gethostbyname, address)
+    except socket.gaierror as ex:
+        raise XKNXException(f"Could not resolve {address_name}: {address}") from ex
```

### Comparing `xknx-2.7.0/xknx/knxip/__init__.py` & `xknx-2.8.0/xknx/knxip/__init__.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/body.py` & `xknx-2.8.0/xknx/knxip/body.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/connect_request.py` & `xknx-2.8.0/xknx/knxip/connect_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/connect_response.py` & `xknx-2.8.0/xknx/knxip/connect_response.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/connectionstate_request.py` & `xknx-2.8.0/xknx/knxip/connectionstate_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/connectionstate_response.py` & `xknx-2.8.0/xknx/knxip/connectionstate_response.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/description_request.py` & `xknx-2.8.0/xknx/knxip/description_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/description_response.py` & `xknx-2.8.0/xknx/knxip/description_response.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/device_configuration_ack.py` & `xknx-2.8.0/xknx/knxip/device_configuration_ack.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/device_configuration_request.py` & `xknx-2.8.0/xknx/knxip/device_configuration_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/dib.py` & `xknx-2.8.0/xknx/knxip/dib.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/disconnect_request.py` & `xknx-2.8.0/xknx/knxip/disconnect_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/disconnect_response.py` & `xknx-2.8.0/xknx/knxip/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/error_code.py` & `xknx-2.8.0/xknx/knxip/error_code.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/header.py` & `xknx-2.8.0/xknx/knxip/header.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/hpai.py` & `xknx-2.8.0/xknx/knxip/hpai.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/knxip.py` & `xknx-2.8.0/xknx/knxip/knxip.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/knxip_enum.py` & `xknx-2.8.0/xknx/knxip/knxip_enum.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/routing_busy.py` & `xknx-2.8.0/xknx/knxip/routing_busy.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/routing_indication.py` & `xknx-2.8.0/xknx/knxip/routing_indication.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/routing_lost_message.py` & `xknx-2.8.0/xknx/knxip/routing_lost_message.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/search_request.py` & `xknx-2.8.0/xknx/knxip/search_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/search_request_extended.py` & `xknx-2.8.0/xknx/knxip/search_request_extended.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/search_response.py` & `xknx-2.8.0/xknx/knxip/search_response.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/search_response_extended.py` & `xknx-2.8.0/xknx/knxip/search_response_extended.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/secure_wrapper.py` & `xknx-2.8.0/xknx/knxip/secure_wrapper.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/session_authenticate.py` & `xknx-2.8.0/xknx/knxip/session_authenticate.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/session_request.py` & `xknx-2.8.0/xknx/knxip/session_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/session_response.py` & `xknx-2.8.0/xknx/knxip/session_response.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/session_status.py` & `xknx-2.8.0/xknx/knxip/session_status.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/srp.py` & `xknx-2.8.0/xknx/knxip/srp.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/timer_notify.py` & `xknx-2.8.0/xknx/knxip/timer_notify.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/tunnelling_ack.py` & `xknx-2.8.0/xknx/knxip/tunnelling_ack.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/knxip/tunnelling_request.py` & `xknx-2.8.0/xknx/knxip/tunnelling_request.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/management/management.py` & `xknx-2.8.0/xknx/management/management.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/management/procedures.py` & `xknx-2.8.0/xknx/management/procedures.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/profile/__init__.py` & `xknx-2.8.0/xknx/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/profile/const.py` & `xknx-2.8.0/xknx/profile/const.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/remote_value/__init__.py` & `xknx-2.8.0/xknx/remote_value/__init__.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value.py` & `xknx-2.8.0/xknx/remote_value/remote_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections.abc import Awaitable, Iterator
 import logging
 from typing import TYPE_CHECKING, Callable, Generic, TypeVar, Union
 
-from xknx.dpt.dpt import DPTArray, DPTBinary
+from xknx.dpt import DPTArray, DPTBinary
 from xknx.exceptions import ConversionError, CouldNotParseTelegram
 from xknx.telegram import GroupAddress, Telegram
 from xknx.telegram.address import (
     DeviceGroupAddress,
     InternalGroupAddress,
     parse_device_group_address,
 )
@@ -26,20 +26,19 @@
 if TYPE_CHECKING:
     from xknx.telegram.address import DeviceAddressableType
     from xknx.xknx import XKNX
 
 logger = logging.getLogger("xknx.log")
 
 AsyncCallbackType = Callable[[], Awaitable[None]]
-DPTPayloadT = TypeVar("DPTPayloadT", DPTArray, DPTBinary, Union[DPTArray, DPTBinary])
 GroupAddressesType = Union["DeviceAddressableType", list["DeviceAddressableType"]]
 ValueT = TypeVar("ValueT")
 
 
-class RemoteValue(ABC, Generic[DPTPayloadT, ValueT]):
+class RemoteValue(ABC, Generic[ValueT]):
     """Class for managing remote knx value."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -52,20 +51,20 @@
         self.xknx: XKNX = xknx
         self.passive_group_addresses: list[DeviceGroupAddress] = []
 
         def unpack_group_addresses(
             addresses: GroupAddressesType | None,
         ) -> DeviceGroupAddress | None:
             """Parse group addresses and assign passive addresses when given."""
-            if addresses is None:
+            if not addresses:  # None or empty list
                 return None
             if not isinstance(addresses, list):
                 return parse_device_group_address(addresses)
             active, *passive = map(parse_device_group_address, addresses)
-            self.passive_group_addresses.extend(passive)  # type: ignore
+            self.passive_group_addresses.extend(passive)
             return active
 
         self.group_address = unpack_group_addresses(group_address)
         self.group_address_state = unpack_group_addresses(group_address_state)
 
         self.device_name: str = "Unknown" if device_name is None else device_name
         self.feature_name: str = "Unknown" if feature_name is None else feature_name
@@ -135,24 +134,19 @@
             yield self.group_address
             yield self.group_address_state
             yield from self.passive_group_addresses
 
         return group_address in remote_value_addresses()
 
     @abstractmethod
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTPayloadT:
-        """Return payload if telegram payload may be parsed - to be implemented in derived class."""
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
-    @abstractmethod
-    def from_knx(self, payload: DPTPayloadT) -> ValueT:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> ValueT:
         """Convert current payload to value - to be implemented in derived class."""
 
     @abstractmethod
-    def to_knx(self, value: ValueT) -> DPTPayloadT:
+    def to_knx(self, value: ValueT) -> DPTArray | DPTBinary:
         """Convert value to payload - to be implemented in derived class."""
 
     async def process(self, telegram: Telegram, always_callback: bool = False) -> bool:
         """Process incoming or outgoing telegram."""
         if not isinstance(
             telegram.destination_address, (GroupAddress, InternalGroupAddress)
         ) or not self.has_group_address(telegram.destination_address):
@@ -170,16 +164,15 @@
                 destination_address=str(telegram.destination_address),
                 source_address=str(telegram.source_address),
                 device_name=self.device_name,
                 feature_name=self.feature_name,
             )
 
         try:
-            _new_payload = self.payload_valid(telegram.payload.value)
-            decoded_payload = self.from_knx(_new_payload)
+            decoded_payload = self.from_knx(telegram.payload.value)
         except (ConversionError, CouldNotParseTelegram) as err:
             logger.warning(
                 "Can not process %s for %s - %s: %s",
                 telegram,
                 self.device_name,
                 self.feature_name,
                 err,
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_climate_mode.py` & `xknx-2.8.0/xknx/remote_value/remote_value_climate_mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,36 +15,31 @@
     DPTControllerStatus,
     DPTHVACContrMode,
     DPTHVACMode,
 )
 from xknx.dpt.dpt_hvac_mode import HVACControllerMode, HVACModeT, HVACOperationMode
 from xknx.exceptions import ConversionError, CouldNotParseTelegram
 
-from .remote_value import (
-    AsyncCallbackType,
-    DPTPayloadT,
-    GroupAddressesType,
-    RemoteValue,
-)
+from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueClimateModeBase(RemoteValue[DPTPayloadT, Optional[HVACModeT]]):
+class RemoteValueClimateModeBase(RemoteValue[Optional[HVACModeT]]):
     """Base class for binary climate mode remote values."""
 
     @abstractmethod
     def supported_operation_modes(
         self,
     ) -> list[HVACModeT]:
         """Return a list of all supported operation modes."""
 
 
-class RemoteValueOperationMode(RemoteValueClimateModeBase[DPTArray, HVACOperationMode]):
+class RemoteValueOperationMode(RemoteValueClimateModeBase[HVACOperationMode]):
     """Abstraction for remote value of KNX climate operation modes."""
 
     class ClimateModeType(Enum):
         """Implemented climate mode types."""
 
         CONTROLLER_STATUS = DPTControllerStatus
         HVAC_MODE = DPTHVACMode
@@ -81,32 +76,24 @@
             DPTControllerStatus | DPTHVACMode
         ) = climate_mode_type.value
 
     def supported_operation_modes(self) -> list[HVACOperationMode]:
         """Return a list of all supported operation modes."""
         return list(self._climate_mode_transcoder.SUPPORTED_MODES.values())
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == 1:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: Any) -> DPTArray:
         """Convert value to payload."""
-        return DPTArray(self._climate_mode_transcoder.to_knx(value))
+        return self._climate_mode_transcoder.to_knx(value)
 
-    def from_knx(self, payload: DPTArray) -> HVACOperationMode | None:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> HVACOperationMode | None:
         """Convert current payload to value."""
-        return self._climate_mode_transcoder.from_knx(payload.value)
+        return self._climate_mode_transcoder.from_knx(payload)
 
 
-class RemoteValueControllerMode(
-    RemoteValueClimateModeBase[DPTArray, HVACControllerMode]
-):
+class RemoteValueControllerMode(RemoteValueClimateModeBase[HVACControllerMode]):
     """Abstraction for remote value of KNX climate controller modes."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -126,32 +113,24 @@
             after_update_cb=after_update_cb,
         )
 
     def supported_operation_modes(self) -> list[HVACControllerMode]:
         """Return a list of all supported operation modes."""
         return list(DPTHVACContrMode.SUPPORTED_MODES.values())
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == 1:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: Any) -> DPTArray:
         """Convert value to payload."""
-        return DPTArray(DPTHVACContrMode.to_knx(value))
+        return DPTHVACContrMode.to_knx(value)
 
-    def from_knx(self, payload: DPTArray) -> HVACControllerMode | None:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> HVACControllerMode | None:
         """Convert current payload to value."""
-        return DPTHVACContrMode.from_knx(payload.value)
+        return DPTHVACContrMode.from_knx(payload)
 
 
-class RemoteValueBinaryOperationMode(
-    RemoteValueClimateModeBase[DPTBinary, HVACOperationMode]
-):
+class RemoteValueBinaryOperationMode(RemoteValueClimateModeBase[HVACOperationMode]):
     """Abstraction for remote value of split up KNX climate modes."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -183,20 +162,14 @@
             group_address_state=group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTBinary:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTBinary):
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: Any) -> DPTBinary:
         """Convert value to payload."""
         if isinstance(value, HVACOperationMode):
             # foreign operation modes will set the RemoteValue to False
             return DPTBinary(value == self.operation_mode)
         raise ConversionError(
             "value invalid",
@@ -210,31 +183,29 @@
         return [
             HVACOperationMode.COMFORT,
             HVACOperationMode.FROST_PROTECTION,
             HVACOperationMode.NIGHT,
             HVACOperationMode.STANDBY,
         ]
 
-    def from_knx(self, payload: DPTPayloadT) -> HVACOperationMode | None:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> HVACOperationMode | None:
         """Convert current payload to value."""
-        if payload == DPTBinary(1):
+        if payload.value == 1:
             return self.operation_mode
-        if payload == DPTBinary(0):
+        if payload.value == 0:
             return None
         raise CouldNotParseTelegram(
-            "payload invalid",
+            "Payload invalid",
             payload=str(payload),
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
 
-class RemoteValueBinaryHeatCool(
-    RemoteValueClimateModeBase[DPTBinary, HVACControllerMode]
-):
+class RemoteValueBinaryHeatCool(RemoteValueClimateModeBase[HVACControllerMode]):
     """Abstraction for remote value of heat/cool controller mode."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -266,20 +237,14 @@
             group_address_state=group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTBinary:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTBinary):
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def supported_operation_modes(self) -> list[HVACControllerMode]:
         """Return a list of the configured operation mode."""
         return [HVACControllerMode.HEAT, HVACControllerMode.COOL]
 
     def to_knx(self, value: Any) -> DPTBinary:
         """Convert value to payload."""
         if isinstance(value, HVACControllerMode):
@@ -288,27 +253,27 @@
         raise ConversionError(
             "value invalid",
             value=value,
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
-    def from_knx(self, payload: DPTPayloadT) -> HVACControllerMode | None:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> HVACControllerMode | None:
         """Convert current payload to value."""
-        if payload == DPTBinary(1):
+        if payload.value == 1:
             return self.controller_mode
-        if payload == DPTBinary(0):
+        if payload.value == 0:
             # return the other operation mode
             return next(
                 (
                     _op
                     for _op in self.supported_operation_modes()
                     if _op is not self.controller_mode
                 ),
                 None,
             )
         raise CouldNotParseTelegram(
-            "payload invalid",
+            "Payload invalid",
             payload=str(payload),
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_color_rgb.py` & `xknx-2.8.0/xknx/remote_value/remote_value_color_rgb.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueColorRGB(RemoteValue[DPTArray, tuple[int, int, int]]):
+class RemoteValueColorRGB(RemoteValue[tuple[int, int, int]]):
     """Abstraction for remote value of KNX DPT 232.600 (DPT_Color_RGB)."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -37,20 +37,14 @@
             group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == 3:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: Sequence[int]) -> DPTArray:
         """Convert value to payload."""
         if not isinstance(value, (list, tuple)):
             raise ConversionError(
                 "Could not serialize RemoteValueColorRGB (wrong type)",
                 value=value,
                 type=type(value),
@@ -68,10 +62,13 @@
         ):
             raise ConversionError(
                 "Could not serialize DPT 232.600 (wrong bytes)", value=value
             )
 
         return DPTArray(list(value))
 
-    def from_knx(self, payload: DPTArray) -> tuple[int, int, int]:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> tuple[int, int, int]:
         """Convert current payload to value."""
+        if not (isinstance(payload, DPTArray) and len(payload.value) == 3):
+            raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
+
         return payload.value[0], payload.value[1], payload.value[2]
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_color_rgbw.py` & `xknx-2.8.0/xknx/remote_value/remote_value_color_rgbw.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueColorRGBW(RemoteValue[DPTArray, tuple[int, int, int, int]]):
+class RemoteValueColorRGBW(RemoteValue[tuple[int, int, int, int]]):
     """Abstraction for remote value of KNX DPT 251.600 (DPT_Color_RGBW)."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -38,20 +38,14 @@
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
         self.previous_value: tuple[int, int, int, int] = (0, 0, 0, 0)
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == 6:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: Sequence[int]) -> DPTArray:
         """
         Convert value (4-6 bytes) to payload (6 bytes).
 
         * Structure of DPT 251.600
         ** Byte 0: R value
         ** Byte 1: G value
@@ -95,21 +89,24 @@
             )
         if len(value) < 5:
             return DPTArray(list(rgbw) + [0x00, 0x0F])
         if len(value) < 6:
             return DPTArray(list(rgbw) + [0x00] + list(value[4:]))
         return DPTArray(value)
 
-    def from_knx(self, payload: DPTArray) -> tuple[int, int, int, int]:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> tuple[int, int, int, int]:
         """
         Convert current payload to value. Always 4 byte (RGBW).
 
         If one element is invalid, use the previous value. All previous element
         values are initialized to 0.
         """
+        if not (isinstance(payload, DPTArray) and len(payload.value) == 6):
+            raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
+
         _result = list(self.previous_value)
         for i in range(len(payload.value) - 2):
             if payload.value[5] & (0x08 >> i):  # R,G,B,W value valid?
                 _result[i] = payload.value[i]
         result = (_result[0], _result[1], _result[2], _result[3])
         self.previous_value = result
         return result
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_color_xyy.py` & `xknx-2.8.0/xknx/remote_value/remote_value_color_xyy.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,24 @@
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from xknx.dpt import DPTArray, DPTBinary
 from xknx.dpt.dpt_color import DPTColorXYY, XYYColor
-from xknx.exceptions import CouldNotParseTelegram
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueColorXYY(RemoteValue[DPTArray, XYYColor]):
+class RemoteValueColorXYY(RemoteValue[XYYColor]):
     """Abstraction for remote value of KNX DPT 242.600 (DPT_Colour_xyY)."""
 
-    PAYLOAD_LENGTH = 6
-
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
         sync_state: bool | int | float | str = True,
         device_name: str | None = None,
@@ -39,20 +36,14 @@
             group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == self.PAYLOAD_LENGTH:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: XYYColor) -> DPTArray:
         """Convert value to payload."""
-        return DPTArray(DPTColorXYY.to_knx(value))
+        return DPTColorXYY.to_knx(value)
 
-    def from_knx(self, payload: DPTArray) -> XYYColor:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> XYYColor:
         """Convert current payload to value."""
-        return DPTColorXYY.from_knx(payload.value)
+        return DPTColorXYY.from_knx(payload)
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_control.py` & `xknx-2.8.0/xknx/remote_value/remote_value_control.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 DPT 2.yyy and DPT 3.yyy
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 from xknx.dpt import DPTArray, DPTBinary, DPTControlStepCode
-from xknx.exceptions import ConversionError, CouldNotParseTelegram
+from xknx.exceptions import ConversionError
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueControl(RemoteValue[DPTBinary, Any]):
+class RemoteValueControl(RemoteValue[Any]):
     """Abstraction for remote value used for controlling."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -46,28 +46,21 @@
             group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTBinary:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTBinary):
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: Any) -> DPTBinary:
         """Convert value to payload."""
-        return DPTBinary(self.dpt_class.to_knx(value))
+        return self.dpt_class.to_knx(value)
 
-    def from_knx(self, payload: DPTBinary) -> Any:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> Any:
         """Convert current payload to value."""
-        # TODO: DPTBinary.value is int - DPTBase.from_knx requires Tuple[int, ...] - maybe use bytes
-        return self.dpt_class.from_knx((payload.value,))
+        return self.dpt_class.from_knx(payload)
 
     @property
     def unit_of_measurement(self) -> str | None:
         """Return the unit of measurement."""
         return self.dpt_class.unit
 
     @property
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_datetime.py` & `xknx-2.8.0/xknx/remote_value/remote_value_datetime.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import annotations
 
 from enum import Enum
 import time
 from typing import TYPE_CHECKING
 
 from xknx.dpt import DPTArray, DPTBinary, DPTDate, DPTDateTime, DPTTime
-from xknx.exceptions import ConversionError, CouldNotParseTelegram
+from xknx.exceptions import ConversionError
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
@@ -22,15 +22,15 @@
     """Enum class for the date or time value type."""
 
     DATETIME = DPTDateTime
     DATE = DPTDate
     TIME = DPTTime
 
 
-class RemoteValueDateTime(RemoteValue[DPTArray, time.struct_time]):
+class RemoteValueDateTime(RemoteValue[time.struct_time]):
     """Abstraction for remote value of KNX 10.001, 11.001 and 19.001 time and date objects."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -58,23 +58,14 @@
             group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if (
-            isinstance(payload, DPTArray)
-            and len(payload.value) == self.dpt_class.payload_length
-        ):
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: time.struct_time) -> DPTArray:
         """Convert value to payload."""
-        return DPTArray(self.dpt_class.to_knx(value))
+        return self.dpt_class.to_knx(value)
 
-    def from_knx(self, payload: DPTArray) -> time.struct_time:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> time.struct_time:
         """Convert current payload to value."""
-        return self.dpt_class.from_knx(payload.value)
+        return self.dpt_class.from_knx(payload)
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_dpt_2_byte_unsigned.py` & `xknx-2.8.0/xknx/remote_value/remote_value_dpt_2_byte_unsigned.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 DPT 7.001.
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from xknx.dpt import DPT2ByteUnsigned, DPTArray, DPTBinary
-from xknx.exceptions import CouldNotParseTelegram
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueDpt2ByteUnsigned(RemoteValue[DPTArray, int]):
+class RemoteValueDpt2ByteUnsigned(RemoteValue[int]):
     """Abstraction for remote value of KNX DPT 7.001."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -36,20 +35,14 @@
             group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == 2:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: int) -> DPTArray:
         """Convert value to payload."""
-        return DPTArray(DPT2ByteUnsigned.to_knx(value))
+        return DPT2ByteUnsigned.to_knx(value)
 
-    def from_knx(self, payload: DPTArray) -> int:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> int:
         """Convert current payload to value."""
-        return DPT2ByteUnsigned.from_knx(payload.value)
+        return DPT2ByteUnsigned.from_knx(payload)
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_raw.py` & `xknx-2.8.0/xknx/remote_value/remote_value_raw.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 Module for managing a remote value typically used within a sensor.
 
 The module maps a given value_type to a DPT class and uses this class
 for serialization and deserialization of the KNX value.
 """
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 
 from xknx.dpt.dpt import DPTArray, DPTBinary
 from xknx.exceptions import ConversionError, CouldNotParseTelegram
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueRaw(RemoteValue[Union[DPTArray, DPTBinary], int]):
+class RemoteValueRaw(RemoteValue[int]):
     """Abstraction for raw values."""
 
     def __init__(
         self,
         xknx: XKNX,
         payload_length: int,
         group_address: GroupAddressesType | None = None,
@@ -39,24 +39,14 @@
             group_address_state,
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
 
-    def payload_valid(
-        self, payload: DPTArray | DPTBinary | None
-    ) -> DPTArray | DPTBinary:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTBinary) and self.payload_length == 0:
-            return payload
-        if isinstance(payload, DPTArray) and len(payload.value) == self.payload_length:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: int) -> DPTArray | DPTBinary:
         """Convert value to payload."""
         if self.payload_length == 0:
             try:
                 return DPTBinary(value)
             except TypeError as err:
                 raise ConversionError(
@@ -65,13 +55,17 @@
         try:
             return DPTArray(value.to_bytes(length=self.payload_length, byteorder="big"))
         except (AttributeError, OverflowError) as err:
             raise ConversionError("Could not init DPTArray", value=str(value)) from err
 
     def from_knx(self, payload: DPTArray | DPTBinary) -> int:
         """Convert current payload to value."""
-        if isinstance(payload, DPTBinary):
+        if isinstance(payload, DPTBinary) and self.payload_length == 0:
             return payload.value
-        try:
-            return int.from_bytes(payload.value, byteorder="big")
-        except ValueError as err:
-            raise ConversionError("Could not parse payload", payload=payload) from err
+        if isinstance(payload, DPTArray) and len(payload.value) == self.payload_length:
+            try:
+                return int.from_bytes(payload.value, byteorder="big")
+            except ValueError as err:
+                raise ConversionError(
+                    "Could not parse payload", payload=payload
+                ) from err
+        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_scaling.py` & `xknx-2.8.0/xknx/remote_value/remote_value_scaling.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueScaling(RemoteValue[DPTArray, int]):
+class RemoteValueScaling(RemoteValue[int]):
     """Abstraction for remote value of KNX DPT 5.001 (DPT_Scaling)."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -40,28 +40,24 @@
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
         self.range_from = range_from
         self.range_to = range_to
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == 1:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: float) -> DPTArray:
         """Convert value to payload."""
         knx_value = self._calc_to_knx(self.range_from, self.range_to, value)
         return DPTArray(knx_value)
 
-    def from_knx(self, payload: DPTArray) -> int:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> int:
         """Convert current payload to value."""
-        return self._calc_from_knx(self.range_from, self.range_to, payload.value[0])
+        if isinstance(payload, DPTArray) and len(payload.value) == 1:
+            return self._calc_from_knx(self.range_from, self.range_to, payload.value[0])
+        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
 
     @property
     def unit_of_measurement(self) -> str | None:
         """Return the unit of measurement."""
         return "%"
 
     @staticmethod
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_scene_number.py` & `xknx-2.8.0/xknx/remote_value/remote_value_1count.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 """
-Module for managing a DTP Scene Number remote value.
+Module for managing an 1 count remote value.
 
-DPT 17.001.
+DPT 6.010.
 """
 from __future__ import annotations
 
-from xknx.dpt import DPTArray, DPTBinary, DPTSceneNumber
-from xknx.exceptions import CouldNotParseTelegram
+from xknx.dpt import DPTArray, DPTBinary, DPTValue1Count
 
 from .remote_value import RemoteValue
 
 
-class RemoteValueSceneNumber(RemoteValue[DPTArray, int]):
-    """Abstraction for remote value of KNX DPT 17.001 (DPT_Scene_Number)."""
-
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray) and len(payload.value) == 1:
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
+class RemoteValue1Count(RemoteValue[int]):
+    """Abstraction for remote value of KNX 6.010 (DPT_Value_1_Count)."""
 
     def to_knx(self, value: int) -> DPTArray:
         """Convert value to payload."""
-        return DPTArray(DPTSceneNumber.to_knx(value))
+        return DPTValue1Count.to_knx(value)
 
-    def from_knx(self, payload: DPTArray) -> int:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> int:
         """Convert current payload to value."""
-        return DPTSceneNumber.from_knx(payload.value)
+        return DPTValue1Count.from_knx(payload)
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_setpoint_shift.py` & `xknx-2.8.0/xknx/remote_value/remote_value_setpoint_shift.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class SetpointShiftMode(Enum):
     """Enum for setting the setpoint shift mode."""
 
     DPT6010 = DPTValue1Count
     DPT9002 = DPTTemperature
 
 
-class RemoteValueSetpointShift(RemoteValue[DPTArray, float]):
+class RemoteValueSetpointShift(RemoteValue[float]):
     """Abstraction for remote value of KNX DPT 6.010."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -50,40 +50,39 @@
         )
 
         self.dpt_class: type[DPTValue1Count | DPTTemperature] | None = (
             setpoint_shift_mode.value if setpoint_shift_mode is not None else None
         )
         self.setpoint_shift_step = setpoint_shift_step
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTArray:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTArray):
-            payload_length = len(payload.value)
-            if self.dpt_class is None:
-                if payload_length == DPTTemperature.payload_length:
-                    self.dpt_class = DPTTemperature
-                    return payload
-                if payload_length == DPTValue1Count.payload_length:
-                    self.dpt_class = DPTValue1Count
-                    return payload
-            elif payload_length == self.dpt_class.payload_length:
-                return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: float) -> DPTArray:
         """Convert value to payload."""
         if self.dpt_class is None:
             raise ConversionError(
                 f"Setpoint shift DPT not initialized for {self.device_name}"
             )
         if self.dpt_class == DPTValue1Count:
             converted_value = int(value / self.setpoint_shift_step)
-            return DPTArray(DPTValue1Count.to_knx(converted_value))
-        return DPTArray(DPTTemperature.to_knx(value))
+            return DPTValue1Count.to_knx(converted_value)
+        return DPTTemperature.to_knx(value)
 
-    def from_knx(self, payload: DPTArray) -> float:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> float:
         """Convert current payload to value."""
-        assert self.dpt_class is not None  # checked by payload_valid() from process()
-        payload_value = self.dpt_class.from_knx(payload.value)
+        if self.dpt_class is None:
+            self.dpt_class = self._determine_dpt_class(payload)
+
+        payload_value = self.dpt_class.from_knx(payload)
         if self.dpt_class == DPTValue1Count:
             return payload_value * self.setpoint_shift_step
         return payload_value
+
+    def _determine_dpt_class(
+        self, payload: DPTArray | DPTBinary
+    ) -> type[DPTValue1Count | DPTTemperature]:
+        """Test if telegram payload may be parsed."""
+        if isinstance(payload, DPTArray):
+            payload_length = len(payload.value)
+            if payload_length == DPTTemperature.payload_length:
+                return DPTTemperature
+            if payload_length == DPTValue1Count.payload_length:
+                return DPTValue1Count
+        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_step.py` & `xknx-2.8.0/xknx/remote_value/remote_value_step.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueStep(RemoteValue[DPTBinary, "RemoteValueStep.Direction"]):
+class RemoteValueStep(RemoteValue["RemoteValueStep.Direction"]):
     """Abstraction for remote value of KNX DPT 1.007 / DPT_Step."""
 
     class Direction(Enum):
         """Enum for indicating the direction."""
 
         DECREASE = 0
         INCREASE = 1
@@ -43,20 +43,14 @@
             group_address_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
         self.invert = invert
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTBinary:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTBinary):
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     # from KNX Association System Specifications AS v1.5.00:
     # 1.007 DPT_Step   0 = Decrease 1 = Increase
     # 1.008 DPT_UpDown 0 = Up       1 = Down
 
     def to_knx(self, value: RemoteValueStep.Direction) -> DPTBinary:
         """Convert value to payload."""
         if value == self.Direction.INCREASE:
@@ -66,22 +60,22 @@
         raise ConversionError(
             "value invalid",
             value=value,
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
-    def from_knx(self, payload: DPTBinary) -> RemoteValueStep.Direction:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> RemoteValueStep.Direction:
         """Convert current payload to value."""
-        if payload == DPTBinary(1):
+        if payload.value == 1:
             return self.Direction.DECREASE if self.invert else self.Direction.INCREASE
-        if payload == DPTBinary(0):
+        if payload.value == 0:
             return self.Direction.INCREASE if self.invert else self.Direction.DECREASE
         raise CouldNotParseTelegram(
-            "payload invalid",
+            "Payload invalid",
             payload=payload,
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
     async def increase(self) -> None:
         """Increase value."""
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_switch.py` & `xknx-2.8.0/xknx/remote_value/remote_value_switch.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueSwitch(RemoteValue[DPTBinary, bool]):
+class RemoteValueSwitch(RemoteValue[bool]):
     """Abstraction for remote value of KNX DPT 1.001 / DPT_Switch."""
 
     def __init__(
         self,
         xknx: XKNX,
         group_address: GroupAddressesType | None = None,
         group_address_state: GroupAddressesType | None = None,
@@ -38,39 +38,33 @@
             sync_state=sync_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
         self.invert = bool(invert)
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTBinary:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTBinary):
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: bool) -> DPTBinary:
         """Convert value to payload."""
         if isinstance(value, bool):
             return DPTBinary(value ^ self.invert)
         raise ConversionError(
             "value invalid",
             value=value,
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
-    def from_knx(self, payload: DPTBinary) -> bool:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> bool:
         """Convert current payload to value."""
-        if payload == DPTBinary(0):
+        if payload.value == 0:
             return self.invert
-        if payload == DPTBinary(1):
+        if payload.value == 1:
             return not self.invert
         raise CouldNotParseTelegram(
-            "payload invalid",
+            "Payload invalid",
             payload=payload,
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
     async def off(self) -> None:
         """Set value to OFF."""
```

### Comparing `xknx-2.7.0/xknx/remote_value/remote_value_updown.py` & `xknx-2.8.0/xknx/remote_value/remote_value_updown.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from .remote_value import AsyncCallbackType, GroupAddressesType, RemoteValue
 
 if TYPE_CHECKING:
     from xknx.xknx import XKNX
 
 
-class RemoteValueUpDown(RemoteValue[DPTBinary, "RemoteValueUpDown.Direction"]):
+class RemoteValueUpDown(RemoteValue["RemoteValueUpDown.Direction"]):
     """Abstraction for remote value of KNX DPT 1.008 / DPT_UpDown."""
 
     class Direction(Enum):
         """Enum for indicating the direction."""
 
         UP = 0
         DOWN = 1
@@ -43,41 +43,35 @@
             group_address_state,
             device_name=device_name,
             feature_name=feature_name,
             after_update_cb=after_update_cb,
         )
         self.invert = invert
 
-    def payload_valid(self, payload: DPTArray | DPTBinary | None) -> DPTBinary:
-        """Test if telegram payload may be parsed."""
-        if isinstance(payload, DPTBinary):
-            return payload
-        raise CouldNotParseTelegram("Payload invalid", payload=str(payload))
-
     def to_knx(self, value: RemoteValueUpDown.Direction) -> DPTBinary:
         """Convert value to payload."""
         if value == self.Direction.UP:
             return DPTBinary(1) if self.invert else DPTBinary(0)
         if value == self.Direction.DOWN:
             return DPTBinary(0) if self.invert else DPTBinary(1)
         raise ConversionError(
             "value invalid",
             value=value,
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
-    def from_knx(self, payload: DPTBinary) -> RemoteValueUpDown.Direction:
+    def from_knx(self, payload: DPTArray | DPTBinary) -> RemoteValueUpDown.Direction:
         """Convert current payload to value."""
-        if payload == DPTBinary(0):
+        if payload.value == 0:
             return self.Direction.DOWN if self.invert else self.Direction.UP
-        if payload == DPTBinary(1):
+        if payload.value == 1:
             return self.Direction.UP if self.invert else self.Direction.DOWN
         raise CouldNotParseTelegram(
-            "payload invalid",
+            "Payload invalid",
             payload=payload,
             device_name=self.device_name,
             feature_name=self.feature_name,
         )
 
     async def down(self) -> None:
         """Set value to down."""
```

### Comparing `xknx-2.7.0/xknx/secure/data_secure.py` & `xknx-2.8.0/xknx/secure/data_secure.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/secure/data_secure_asdu.py` & `xknx-2.8.0/xknx/secure/data_secure_asdu.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/secure/keyring.py` & `xknx-2.8.0/xknx/secure/keyring.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import asyncio
 import base64
 import enum
 from itertools import chain
 import logging
 import os
 from typing import Any
-from xml.dom.minidom import Attr, Document, parse
-from xml.etree.ElementTree import Element, ElementTree
+from xml.dom.minidom import Attr, Document, Element, parse
+from xml.etree.ElementTree import ElementTree
 import xml.sax
 from xml.sax.handler import ContentHandler
 from xml.sax.xmlreader import AttributesImpl
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
@@ -35,15 +35,15 @@
     USB = "USB"
 
 
 class AttributeReader(ABC):
     """Abstract base class for modelling attribute reader capabilities."""
 
     @abstractmethod
-    def parse_xml(self, node: Document) -> None:
+    def parse_xml(self, node: Element) -> None:
         """Parse all needed attributes from the given node map."""
 
     def decrypt_attributes(
         self, password_hash: bytes, initialization_vector: bytes
     ) -> None:
         """Decrypt attribute data."""
 
@@ -58,15 +58,15 @@
 
 class XMLAssignedGroupAddress(AttributeReader):
     """Assigned Group Addresses to an interface in a knxkeys file."""
 
     address: GroupAddress
     senders: list[IndividualAddress]
 
-    def parse_xml(self, node: Document) -> None:
+    def parse_xml(self, node: Element) -> None:
         """Parse all needed attributes from the given node map."""
         attributes = node.attributes
         self.address = GroupAddress(
             self.get_attribute_value(attributes.get("Address", None))
         )
         self.senders = [
             IndividualAddress(sender)
@@ -85,15 +85,15 @@
     user_id: int | None = None
     password: str | None = None
     decrypted_password: str | None = None
     decrypted_authentication: str | None = None
     authentication: str | None = None
     group_addresses: dict[GroupAddress, list[IndividualAddress]]
 
-    def parse_xml(self, node: Document) -> None:
+    def parse_xml(self, node: Element) -> None:
         """Parse all needed attributes from the given node map."""
         attributes = node.attributes
         self.type = InterfaceType(self.get_attribute_value(attributes.get("Type")))
         self.individual_address = IndividualAddress(
             self.get_attribute_value(attributes.get("IndividualAddress"))
         )
         _host = self.get_attribute_value(attributes.get("Host"))
@@ -143,15 +143,15 @@
     """Backbone in a knxkeys file."""
 
     decrypted_key: bytes | None = None
     key: str | None = None
     latency: int | None = None
     multicast_address: str | None = None
 
-    def parse_xml(self, node: Document) -> None:
+    def parse_xml(self, node: Element) -> None:
         """Parse all needed attributes from the given node map."""
         attributes = node.attributes
         self.key = self.get_attribute_value(attributes.get("Key"))
         if latency := self.get_attribute_value(attributes.get("Latency")):
             self.latency = int(latency)
         self.multicast_address = self.get_attribute_value(
             attributes.get("MulticastAddress")
@@ -170,15 +170,15 @@
 class XMLGroupAddress(AttributeReader):
     """Group Address in a knxkeys file."""
 
     address: GroupAddress
     decrypted_key: bytes | None = None
     key: str
 
-    def parse_xml(self, node: Document) -> None:
+    def parse_xml(self, node: Element) -> None:
         """Parse all needed attributes from the given node map."""
         attributes = node.attributes
         self.address = GroupAddress(self.get_attribute_value(attributes.get("Address")))
         self.key = self.get_attribute_value(attributes.get("Key"))
 
     def decrypt_attributes(
         self, password_hash: bytes, initialization_vector: bytes
@@ -198,15 +198,15 @@
     decrypted_tool_key: bytes | None = None
     management_password: str
     decrypted_management_password: str | None = None
     decrypted_authentication: str | None = None
     authentication: str
     sequence_number: int
 
-    def parse_xml(self, node: Document) -> None:
+    def parse_xml(self, node: Element) -> None:
         """Parse all needed attributes from the given node map."""
         attributes = node.attributes
         self.individual_address = IndividualAddress(
             self.get_attribute_value(attributes.get("IndividualAddress"))
         )
         self.tool_key = self.get_attribute_value(attributes.get("ToolKey"))
         self.management_password = self.get_attribute_value(
@@ -386,15 +386,15 @@
         # devices are only available if the full project was exported
         for device in self.devices:
             ia_seq_table[device.individual_address] = device.sequence_number
         # TODO: check if this should default to 0 or if devices without a sequence number
         # in keyfile should be excluded from the table (are there non-secure devices listed?)
         return ia_seq_table
 
-    def parse_xml(self, node: Document) -> None:
+    def parse_xml(self, node: Element) -> None:
         """Parse all needed attributes from the given node map."""
         attributes = node.attributes
         self.created_by = self.get_attribute_value(attributes.get("CreatedBy"))
         self.created = self.get_attribute_value(attributes.get("Created"))
         self.signature = base64.b64decode(
             self.get_attribute_value(attributes.get("Signature"))
         )
@@ -406,24 +406,24 @@
                 interface.parse_xml(sub_node)
                 self.interfaces.append(interface)
             if sub_node.nodeName == "Backbone":
                 backbone: XMLBackbone = XMLBackbone()
                 backbone.parse_xml(sub_node)
                 self.backbone = backbone
             if sub_node.nodeName == "Devices":
-                device_doc: Document
+                device_doc: Element
                 for device_doc in filter(
                     lambda x: x.nodeType != 3, sub_node.childNodes
                 ):
                     device: XMLDevice = XMLDevice()
                     device.parse_xml(device_doc)
                     self.devices.append(device)
 
             elif sub_node.nodeName == "GroupAddresses":
-                ga_doc: Document
+                ga_doc: Element
                 for ga_doc in filter(lambda x: x.nodeType != 3, sub_node.childNodes):
                     xml_ga: XMLGroupAddress = XMLGroupAddress()
                     xml_ga.parse_xml(ga_doc)
                     self.group_addresses.append(xml_ga)
 
     def decrypt(self, password: str) -> None:
         """Decrypt all data."""
@@ -459,15 +459,15 @@
             "Signature verification of keyring file failed. Invalid password or malformed file content."
         )
 
     keyring: Keyring = Keyring()
     try:
         with open(path, encoding="utf-8") as file:
             dom: Document = parse(file)
-            keyring.parse_xml(dom.getElementsByTagName("Keyring")[0])
+            keyring.parse_xml(dom.getElementsByTagName("Keyring")[0])  # type: ignore[arg-type]
 
         keyring.decrypt(password)
 
         return keyring
     except Exception as exception:
         logger.exception("There was an error during loading the knxkeys file.")
         raise InvalidSecureConfiguration() from exception
@@ -513,15 +513,15 @@
 
 
 def verify_keyring_signature(path: str | os.PathLike[Any], password: str) -> bool:
     """Verify the signature of the given knxkeys file."""
     handler = KeyringSAXContentHandler(password)
     signature: bytes
     with open(path, encoding="utf-8") as file:
-        element: Element = ElementTree().parse(file)
+        element = ElementTree().parse(file)
         signature = base64.b64decode(element.attrib.get("Signature", ""))
 
     with open(path, encoding="utf-8") as file:
         parser = xml.sax.make_parser()
         parser.setContentHandler(handler)  # type: ignore[no-untyped-call]
         parser.parse(file)  # type: ignore[no-untyped-call]
```

### Comparing `xknx-2.7.0/xknx/secure/security_primitives.py` & `xknx-2.8.0/xknx/secure/security_primitives.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/secure/util.py` & `xknx-2.8.0/xknx/secure/util.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/telegram/address.py` & `xknx-2.8.0/xknx/telegram/address.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/telegram/address_filter.py` & `xknx-2.8.0/xknx/telegram/address_filter.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/telegram/apci.py` & `xknx-2.8.0/xknx/telegram/apci.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/telegram/telegram.py` & `xknx-2.8.0/xknx/telegram/telegram.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/telegram/tpci.py` & `xknx-2.8.0/xknx/telegram/tpci.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx/tools/group_communication.py` & `xknx-2.8.0/xknx/tools/group_communication.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,23 +71,23 @@
     await xknx.telegrams.put(telegram)
 
 
 async def read_group_value(
     xknx: XKNX,
     group_address: DeviceAddressableType,
     value_type: int | str | type[DPTBase] | None = None,
-) -> DPTArray | DPTBinary | Any | None:
+) -> int | tuple[int, ...] | Any | None:
     """Read a value from a KNX group address."""
     transcoder = _parse_dpt(value_type)
     value_reader = ValueReader(xknx, parse_device_group_address(group_address))
     response = await value_reader.read()
     if response is not None:
         assert isinstance(response.payload, (GroupValueWrite, GroupValueResponse))
         if transcoder is not None:
-            return transcoder.from_knx(response.payload.value.value)  # type: ignore[arg-type]
+            return transcoder.from_knx(response.payload.value)
         return response.payload.value.value
     return None
 
 
 def _parse_dpt(value_type: int | str | type[DPTBase] | None) -> type[DPTBase] | None:
     if value_type is None:
         return None
@@ -106,11 +106,11 @@
 def _parse_payload(
     value: Any,
     value_type: int | str | type[DPTBase] | None = None,
 ) -> DPTBinary | DPTArray:
     if isinstance(value, (DPTArray, DPTBinary)):
         return value
     if transcoder := _parse_dpt(value_type):
-        return DPTArray(transcoder.to_knx(value))
+        return transcoder.to_knx(value)
     if isinstance(value, int):
         return DPTBinary(value)
     return DPTArray(value)
```

### Comparing `xknx-2.7.0/xknx/xknx.py` & `xknx-2.8.0/xknx/xknx.py`

 * *Files identical despite different names*

### Comparing `xknx-2.7.0/xknx.egg-info/PKG-INFO` & `xknx-2.8.0/xknx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: xknx
-Version: 2.7.0
+Version: 2.8.0
 Summary: An Asynchronous Library for the KNX protocol. Documentation: https://xknx.io/
 Home-page: https://xknx.io/
-Download-URL: https://github.com/XKNX/xknx/archive/2.7.0.zip
+Download-URL: https://github.com/XKNX/xknx/archive/2.8.0.zip
 Author: Julius Mittenzwei
 Author-email: julius@mittenzwei.com
 License: MIT
 Keywords: knx ip knxip eib home automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `xknx-2.7.0/xknx.egg-info/SOURCES.txt` & `xknx-2.8.0/xknx.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 xknx/dpt/dpt_color.py
 xknx/dpt/dpt_date.py
 xknx/dpt/dpt_datetime.py
 xknx/dpt/dpt_hvac_mode.py
 xknx/dpt/dpt_scaling.py
 xknx/dpt/dpt_string.py
 xknx/dpt/dpt_time.py
+xknx/dpt/payload.py
 xknx/exceptions/__init__.py
 xknx/exceptions/exception.py
 xknx/io/__init__.py
 xknx/io/connection.py
 xknx/io/const.py
 xknx/io/gateway_scanner.py
 xknx/io/interface.py
```

