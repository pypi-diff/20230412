# Comparing `tmp/servey-2.7.0.tar.gz` & `tmp/servey-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/servey-2.7.0.tar", last modified: Wed Apr 12 03:34:09 2023, max compression
+gzip compressed data, was "dist/servey-2.7.2.tar", last modified: Wed Apr 12 03:59:13 2023, max compression
```

## Comparing `servey-2.7.0.tar` & `servey-2.7.2.tar`

### file list

```diff
@@ -1,304 +1,304 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.720146 servey-2.7.0/
--rw-r--r--   0 tofarr     (501) staff       (20)    17979 2023-04-12 03:34:09.719808 servey-2.7.0/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)    17465 2023-04-05 22:22:08.000000 servey-2.7.0/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.016892 servey-2.7.0/marshy_config_servey/
--rw-r--r--   0 tofarr     (501) staff       (20)    14671 2023-04-12 03:15:09.000000 servey-2.7.0/marshy_config_servey/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.021455 servey-2.7.0/servey/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-20 13:05:09.000000 servey-2.7.0/servey/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2478 2023-04-05 21:10:12.000000 servey-2.7.0/servey/__main__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.039388 servey-2.7.0/servey/action/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/action/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2763 2023-01-20 16:29:37.000000 servey-2.7.0/servey/action/action.py
--rw-r--r--   0 tofarr     (501) staff       (20)      233 2023-01-05 15:20:43.000000 servey-2.7.0/servey/action/batch_invoker.py
--rw-r--r--   0 tofarr     (501) staff       (20)      460 2022-12-09 15:33:15.000000 servey-2.7.0/servey/action/example.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4148 2023-01-06 03:56:01.000000 servey-2.7.0/servey/action/util.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.066033 servey-2.7.0/servey/cache_control/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-11-17 03:52:02.000000 servey-2.7.0/servey/cache_control/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      467 2022-12-09 17:19:54.000000 servey-2.7.0/servey/cache_control/cache_control_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2307 2023-04-05 21:10:12.000000 servey-2.7.0/servey/cache_control/cache_header.py
--rw-r--r--   0 tofarr     (501) staff       (20)      704 2023-02-03 15:04:24.000000 servey-2.7.0/servey/cache_control/secure_hash_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1356 2022-12-24 00:22:46.000000 servey-2.7.0/servey/cache_control/timestamp_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1274 2023-04-05 21:10:12.000000 servey-2.7.0/servey/cache_control/ttl_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)       39 2022-11-30 20:16:33.000000 servey-2.7.0/servey/errors.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.074027 servey-2.7.0/servey/finder/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/finder/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      836 2023-01-05 15:20:43.000000 servey-2.7.0/servey/finder/action_finder_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1777 2023-01-20 16:29:37.000000 servey-2.7.0/servey/finder/module_action_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1601 2023-01-20 16:29:37.000000 servey-2.7.0/servey/finder/module_subscription_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)      653 2023-01-05 15:20:43.000000 servey-2.7.0/servey/finder/subscription_finder_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.076104 servey-2.7.0/servey/security/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/security/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.085018 servey-2.7.0/servey/security/access_control/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/security/access_control/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      335 2023-03-19 15:03:39.000000 servey-2.7.0/servey/security/access_control/access_control_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      357 2023-01-05 15:20:43.000000 servey-2.7.0/servey/security/access_control/allow_all.py
--rw-r--r--   0 tofarr     (501) staff       (20)      361 2023-01-05 15:20:43.000000 servey-2.7.0/servey/security/access_control/allow_none.py
--rw-r--r--   0 tofarr     (501) staff       (20)      516 2023-01-05 15:20:43.000000 servey-2.7.0/servey/security/access_control/scope_access_control.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.124840 servey-2.7.0/servey/security/authenticator/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 00:28:02.000000 servey-2.7.0/servey/security/authenticator/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      614 2023-01-18 13:36:34.000000 servey-2.7.0/servey/security/authenticator/password_authenticator_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1200 2023-01-18 13:36:35.000000 servey-2.7.0/servey/security/authenticator/root_password_authenticator.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2407 2022-12-18 16:01:20.000000 servey-2.7.0/servey/security/authorization.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.134340 servey-2.7.0/servey/security/authorizer/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/security/authorizer/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      446 2022-09-16 02:42:12.000000 servey-2.7.0/servey/security/authorizer/authorizer_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1343 2022-12-09 15:17:12.000000 servey-2.7.0/servey/security/authorizer/authorizer_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2821 2022-12-16 15:10:54.000000 servey-2.7.0/servey/security/authorizer/jwt_authorizer.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1154 2022-11-30 20:16:33.000000 servey-2.7.0/servey/security/authorizer/jwt_authorizer_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.169910 servey-2.7.0/servey/servey_aws/
--rw-r--r--   0 tofarr     (501) staff       (20)       91 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.174940 servey-2.7.0/servey/servey_aws/authorizer/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_aws/authorizer/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4516 2022-12-17 21:34:00.000000 servey-2.7.0/servey/servey_aws/authorizer/kms_authorizer.py
--rw-r--r--   0 tofarr     (501) staff       (20)      923 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/authorizer/kms_authorizer_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.188226 servey-2.7.0/servey/servey_aws/event_handler/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/event_handler/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5959 2023-04-02 17:53:57.000000 servey-2.7.0/servey/servey_aws/event_handler/api_gateway_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1847 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/event_handler/appsync_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5272 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/event_handler/event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1071 2023-04-02 13:21:49.000000 servey-2.7.0/servey/servey_aws/event_handler/event_handler_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2644 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/event_handler/sqs_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2089 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_aws/lambda_invoker.py
--rw-r--r--   0 tofarr     (501) staff       (20)      878 2023-04-04 04:13:04.000000 servey-2.7.0/servey/servey_aws/lambda_router.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4214 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/lambda_websocket.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.214009 servey-2.7.0/servey/servey_aws/router/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-02 13:29:47.000000 servey-2.7.0/servey/servey_aws/router/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1114 2023-04-05 21:30:44.000000 servey-2.7.0/servey/servey_aws/router/api_gateway_router.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1255 2023-04-05 21:30:44.000000 servey-2.7.0/servey/servey_aws/router/appsync_router.py
--rw-r--r--   0 tofarr     (501) staff       (20)      717 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_aws/router/router.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1480 2023-04-05 21:35:02.000000 servey-2.7.0/servey/servey_aws/router/router_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.215959 servey-2.7.0/servey/servey_aws/serverless/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_aws/serverless/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1245 2023-03-30 22:57:04.000000 servey-2.7.0/servey/servey_aws/serverless/__main__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.221969 servey-2.7.0/servey/servey_aws/serverless/trigger_handler/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_aws/serverless/trigger_handler/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1265 2023-01-18 13:36:35.000000 servey-2.7.0/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)      442 2022-12-17 21:14:47.000000 servey-2.7.0/servey/servey_aws/serverless/trigger_handler/trigger_handler_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1090 2023-01-07 16:53:22.000000 servey-2.7.0/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.238575 servey-2.7.0/servey/servey_aws/serverless/yml_config/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3987 2023-04-05 23:49:53.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/action_function_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5177 2023-04-06 00:37:56.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/appsync_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)    10317 2023-04-12 03:12:37.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/cloudfront_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3593 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/kms_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      592 2023-01-20 16:29:37.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/serverless_template.yml
--rw-r--r--   0 tofarr     (501) staff       (20)     5051 2023-04-12 03:18:28.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     7374 2023-04-06 12:59:59.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/subscription_function_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2947 2023-01-18 13:16:57.000000 servey-2.7.0/servey/servey_aws/serverless/yml_config/yml_config_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2179 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/sqs_subscription_service.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3210 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_aws/websocket_subscription_service.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.262037 servey-2.7.0/servey/servey_celery/
--rw-r--r--   0 tofarr     (501) staff       (20)       86 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_celery/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1429 2023-01-07 16:31:15.000000 servey-2.7.0/servey/servey_celery/celery_app.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.267820 servey-2.7.0/servey/servey_celery/celery_config/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-07 16:19:02.000000 servey-2.7.0/servey/servey_celery/celery_config/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      241 2023-01-07 16:53:22.000000 servey-2.7.0/servey/servey_celery/celery_config/celery_config_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1004 2023-04-01 19:42:31.000000 servey-2.7.0/servey/servey_celery/celery_config/fixed_rate_trigger_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      592 2023-01-07 16:53:22.000000 servey-2.7.0/servey/servey_celery/celery_config/subscription_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1050 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_celery/celery_subscription_service.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.270065 servey-2.7.0/servey/servey_direct/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-16 16:23:58.000000 servey-2.7.0/servey/servey_direct/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1313 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_direct/__main__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.273950 servey-2.7.0/servey/servey_starlette/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_starlette/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.285240 servey-2.7.0/servey/servey_starlette/action_endpoint/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 15:42:17.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)    11862 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1134 2023-01-19 13:50:13.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/action_endpoint_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3401 2023-03-19 15:03:39.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2836 2023-03-19 15:03:39.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/caching_action_endpoint.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.314842 servey-2.7.0/servey/servey_starlette/action_endpoint/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 17:29:46.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2786 2023-01-06 15:28:44.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      822 2022-12-11 13:56:30.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2183 2022-12-11 14:21:14.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1444 2022-12-16 15:10:54.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2260 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      201 2022-12-24 01:22:04.000000 servey-2.7.0/servey/servey_starlette/error_response.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.328989 servey-2.7.0/servey/servey_starlette/route_factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_starlette/route_factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1600 2023-01-06 15:28:44.000000 servey-2.7.0/servey/servey_starlette/route_factory/action_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3026 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_starlette/route_factory/asyncapi_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1928 2023-01-18 13:36:35.000000 servey-2.7.0/servey/servey_starlette/route_factory/authenticator_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2441 2023-01-20 16:29:37.000000 servey-2.7.0/servey/servey_starlette/route_factory/openapi_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      242 2023-01-14 15:50:20.000000 servey-2.7.0/servey/servey_starlette/route_factory/route_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      718 2023-01-18 13:36:35.000000 servey-2.7.0/servey/servey_starlette/route_factory/static_site_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6329 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_starlette/route_factory/subscription_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      521 2023-01-18 13:36:35.000000 servey-2.7.0/servey/servey_starlette/starlette_app.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.379851 servey-2.7.0/servey/servey_starlette/statics/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-11-30 19:30:04.000000 servey-2.7.0/servey/servey_starlette/statics/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      794 2022-09-16 02:41:41.000000 servey-2.7.0/servey/servey_starlette/statics/index.html
--rw-r--r--   0 tofarr     (501) staff       (20)  1079398 2022-12-04 20:38:25.000000 servey-2.7.0/servey/servey_starlette/statics/swagger-ui-bundle.js
--rw-r--r--   0 tofarr     (501) staff       (20)   192198 2022-09-16 02:41:41.000000 servey-2.7.0/servey/servey_starlette/statics/swagger-ui.css
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.392356 servey-2.7.0/servey/servey_strawberry/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_strawberry/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.421998 servey-2.7.0/servey/servey_strawberry/entity_factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_strawberry/entity_factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5804 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_strawberry/entity_factory/dataclass_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      515 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_strawberry/entity_factory/entity_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1105 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_strawberry/entity_factory/enum_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      890 2022-12-16 11:34:08.000000 servey-2.7.0/servey/servey_strawberry/entity_factory/forward_ref_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1343 2022-12-18 22:53:24.000000 servey-2.7.0/servey/servey_strawberry/entity_factory/generic_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      688 2022-12-18 22:59:58.000000 servey-2.7.0/servey/servey_strawberry/entity_factory/no_op_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.429021 servey-2.7.0/servey/servey_strawberry/handler_filter/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_strawberry/handler_filter/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3179 2023-01-07 04:41:39.000000 servey-2.7.0/servey/servey_strawberry/handler_filter/authorization_handler_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      687 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_strawberry/handler_filter/handler_filter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1406 2022-12-27 15:18:15.000000 servey-2.7.0/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     7228 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_strawberry/schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      754 2022-12-16 15:10:54.000000 servey-2.7.0/servey/servey_strawberry/schema_factory_lazy_input.py
--rw-r--r--   0 tofarr     (501) staff       (20)      752 2022-12-16 15:10:54.000000 servey-2.7.0/servey/servey_strawberry/schema_factory_lazy_type.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.431376 servey-2.7.0/servey/servey_strawberry/statics/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-11-30 19:30:04.000000 servey-2.7.0/servey/servey_strawberry/statics/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1872 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_strawberry/statics/index.html
--rw-r--r--   0 tofarr     (501) staff       (20)     1726 2023-01-20 16:29:37.000000 servey-2.7.0/servey/servey_strawberry/strawberry_starlette_route_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.434250 servey-2.7.0/servey/servey_test/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-04 20:47:53.000000 servey-2.7.0/servey/servey_test/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1164 2022-12-16 20:57:24.000000 servey-2.7.0/servey/servey_test/test_servey_actions.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.442450 servey-2.7.0/servey/servey_thread/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/servey_thread/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      905 2023-01-05 15:10:21.000000 servey-2.7.0/servey/servey_thread/__main__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1315 2023-01-05 15:20:43.000000 servey-2.7.0/servey/servey_thread/asyncio_subscription_service.py
--rw-r--r--   0 tofarr     (501) staff       (20)      515 2022-12-16 18:31:33.000000 servey-2.7.0/servey/servey_thread/fixed_rate_trigger_thread.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.472900 servey-2.7.0/servey/servey_web_page/
--rw-r--r--   0 tofarr     (501) staff       (20)      213 2023-01-20 16:29:37.000000 servey-2.7.0/servey/servey_web_page/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      103 2023-03-19 15:03:39.000000 servey-2.7.0/servey/servey_web_page/redirect.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1687 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_web_page/web_page_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2604 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_web_page/web_page_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4335 2023-04-05 21:10:12.000000 servey-2.7.0/servey/servey_web_page/web_page_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)      709 2023-01-20 16:29:37.000000 servey-2.7.0/servey/servey_web_page/web_page_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)      848 2023-01-20 16:29:37.000000 servey-2.7.0/servey/servey_web_page/web_page_trigger_handler.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.484312 servey-2.7.0/servey/subscription/
--rw-r--r--   0 tofarr     (501) staff       (20)      595 2023-01-05 15:20:43.000000 servey-2.7.0/servey/subscription/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      392 2023-01-05 15:20:43.000000 servey-2.7.0/servey/subscription/event_filter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1698 2023-01-05 15:20:43.000000 servey-2.7.0/servey/subscription/subscription.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1009 2023-01-05 15:20:43.000000 servey-2.7.0/servey/subscription/subscription_event.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1367 2023-01-05 15:20:43.000000 servey-2.7.0/servey/subscription/subscription_service.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.509930 servey-2.7.0/servey/trigger/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.0/servey/trigger/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      165 2022-12-08 23:20:52.000000 servey-2.7.0/servey/trigger/fixed_rate_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)       92 2022-09-16 02:42:12.000000 servey-2.7.0/servey/trigger/trigger_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      762 2023-01-05 22:00:38.000000 servey-2.7.0/servey/trigger/web_trigger.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.516067 servey-2.7.0/servey/util/
--rw-r--r--   0 tofarr     (501) staff       (20)      836 2023-01-05 15:20:43.000000 servey-2.7.0/servey/util/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      839 2022-08-10 15:17:22.000000 servey-2.7.0/servey/util/singleton_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      472 2022-12-17 21:18:47.000000 servey-2.7.0/servey/util/to_second_datetime_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-12 03:15:10.000000 servey-2.7.0/servey/version.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.028331 servey-2.7.0/servey.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)    17979 2023-04-12 03:34:08.000000 servey-2.7.0/servey.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)    11054 2023-04-12 03:34:08.000000 servey-2.7.0/servey.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-12 03:34:08.000000 servey-2.7.0/servey.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)      530 2023-04-12 03:34:08.000000 servey-2.7.0/servey.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       46 2023-04-12 03:34:08.000000 servey-2.7.0/servey.egg-info/top_level.txt
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.006973 servey-2.7.0/servey_main/
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.516715 servey-2.7.0/servey_main/templates/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-20 16:29:37.000000 servey-2.7.0/servey_main/templates/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-12 03:34:09.720304 servey-2.7.0/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)     1678 2023-04-05 21:10:12.000000 servey-2.7.0/setup.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.519948 servey-2.7.0/tests/
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.526080 servey-2.7.0/tests/action/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 22:53:16.000000 servey-2.7.0/tests/action/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2144 2023-01-21 19:57:16.000000 servey-2.7.0/tests/action/test_action.py
--rw-r--r--   0 tofarr     (501) staff       (20)      206 2023-01-05 15:20:43.000000 servey-2.7.0/tests/action/test_batch_invoker.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2481 2023-01-05 15:20:43.000000 servey-2.7.0/tests/action/test_util.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.534735 servey-2.7.0/tests/cache_control/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 23:17:15.000000 servey-2.7.0/tests/cache_control/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1456 2023-04-05 21:10:12.000000 servey-2.7.0/tests/cache_control/test_cache_header.py
--rw-r--r--   0 tofarr     (501) staff       (20)      967 2022-12-17 21:18:13.000000 servey-2.7.0/tests/cache_control/test_secure_hash_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)      648 2022-12-17 22:08:34.000000 servey-2.7.0/tests/cache_control/test_timestamp_cache_control.py
--rw-r--r--   0 tofarr     (501) staff       (20)      539 2022-12-09 15:33:15.000000 servey-2.7.0/tests/cache_control/test_ttl_cache_control.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.542122 servey-2.7.0/tests/finder/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 23:43:42.000000 servey-2.7.0/tests/finder/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.560210 servey-2.7.0/tests/finder/actions/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.0/tests/finder/actions/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       89 2023-01-05 15:20:43.000000 servey-2.7.0/tests/finder/actions/test_actions.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.562775 servey-2.7.0/tests/finder/subscriptions/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.0/tests/finder/subscriptions/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      176 2023-01-05 15:20:43.000000 servey-2.7.0/tests/finder/subscriptions/test_subscriptions.py
--rw-r--r--   0 tofarr     (501) staff       (20)      396 2023-01-05 15:20:43.000000 servey-2.7.0/tests/finder/test_action_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1317 2023-01-05 15:20:43.000000 servey-2.7.0/tests/finder/test_module_action_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1075 2023-01-05 15:20:43.000000 servey-2.7.0/tests/finder/test_module_subscription_finder.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.565036 servey-2.7.0/tests/security/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 00:06:37.000000 servey-2.7.0/tests/security/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.570936 servey-2.7.0/tests/security/access_control/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 01:00:09.000000 servey-2.7.0/tests/security/access_control/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      346 2022-12-23 22:40:15.000000 servey-2.7.0/tests/security/access_control/test_allow_all.py
--rw-r--r--   0 tofarr     (501) staff       (20)      349 2023-01-05 15:20:43.000000 servey-2.7.0/tests/security/access_control/test_allow_none.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1179 2022-12-23 22:39:43.000000 servey-2.7.0/tests/security/access_control/test_scope_access_control.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.575046 servey-2.7.0/tests/security/authorizer/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 01:57:56.000000 servey-2.7.0/tests/security/authorizer/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      691 2022-12-09 15:33:15.000000 servey-2.7.0/tests/security/authorizer/test_authorizer_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3291 2022-12-18 15:39:56.000000 servey-2.7.0/tests/security/authorizer/test_jwt_authorizer.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5926 2023-01-05 15:20:43.000000 servey-2.7.0/tests/security/test_authorization.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.609821 servey-2.7.0/tests/servey_aws/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-24 02:48:37.000000 servey-2.7.0/tests/servey_aws/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2127 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_aws/test_kms_authorizer.py
--rw-r--r--   0 tofarr     (501) staff       (20)    11013 2023-03-19 15:03:39.000000 servey-2.7.0/tests/servey_aws/test_lambda_invoker.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2705 2023-04-05 21:37:18.000000 servey-2.7.0/tests/servey_aws/test_lambda_router.py
--rw-r--r--   0 tofarr     (501) staff       (20)     9461 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_aws/test_lambda_websocket.py
--rw-r--r--   0 tofarr     (501) staff       (20)     9017 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_aws/test_serverless.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1847 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_aws/test_sqs_subscription_service.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3806 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_aws/test_websocket_subscription_service.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.612198 servey-2.7.0/tests/servey_celery/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-24 02:16:58.000000 servey-2.7.0/tests/servey_celery/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4311 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_celery/test_celery_app.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.615076 servey-2.7.0/tests/servey_direct/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-18 14:22:06.000000 servey-2.7.0/tests/servey_direct/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1175 2023-04-04 03:50:22.000000 servey-2.7.0/tests/servey_direct/test_servey_direct.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.617168 servey-2.7.0/tests/servey_starlette/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-11 16:01:52.000000 servey-2.7.0/tests/servey_starlette/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.631234 servey-2.7.0/tests/servey_starlette/action_endpoint/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-11 16:02:12.000000 servey-2.7.0/tests/servey_starlette/action_endpoint/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)    29340 2023-04-05 21:10:13.000000 servey-2.7.0/tests/servey_starlette/action_endpoint/test_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1565 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_starlette/action_endpoint/test_action_endpoint_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     7342 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_starlette/action_endpoint/test_authorizing_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2569 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_starlette/action_endpoint/test_self_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6440 2023-03-19 15:03:39.000000 servey-2.7.0/tests/servey_starlette/action_endpoint/test_static_caching_action_endpoint.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.642410 servey-2.7.0/tests/servey_starlette/route_factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-24 01:19:36.000000 servey-2.7.0/tests/servey_starlette/route_factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2859 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_starlette/route_factory/test_asyncapi_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1854 2023-01-18 13:36:35.000000 servey-2.7.0/tests/servey_starlette/route_factory/test_authenticator_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1073 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_starlette/route_factory/test_statc_site_route_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     9426 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_starlette/route_factory/test_subscription_route.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1721 2023-03-16 02:11:16.000000 servey-2.7.0/tests/servey_starlette/test_starlette_app.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.668182 servey-2.7.0/tests/servey_strawberry/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-15 23:35:01.000000 servey-2.7.0/tests/servey_strawberry/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      207 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_strawberry/actions.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.671987 servey-2.7.0/tests/servey_strawberry/entity_factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-15 23:35:48.000000 servey-2.7.0/tests/servey_strawberry/entity_factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      565 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_strawberry/entity_factory/test_dataclass_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      554 2022-12-17 21:34:29.000000 servey-2.7.0/tests/servey_strawberry/entity_factory/test_enum_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.675971 servey-2.7.0/tests/servey_strawberry/handler_filter/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-18 23:00:44.000000 servey-2.7.0/tests/servey_strawberry/handler_filter/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2735 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_strawberry/handler_filter/test_authorization_handler_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      126 2022-12-23 15:50:38.000000 servey-2.7.0/tests/servey_strawberry/handler_filter/test_handler_filter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)    11356 2023-01-07 17:02:07.000000 servey-2.7.0/tests/servey_strawberry/test_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      174 2022-12-18 16:12:35.000000 servey-2.7.0/tests/servey_strawberry/test_statics.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1584 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_strawberry/test_strawberry_starlette_route_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.677941 servey-2.7.0/tests/servey_test/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 00:15:49.000000 servey-2.7.0/tests/servey_test/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1312 2022-12-18 14:33:32.000000 servey-2.7.0/tests/servey_test/test_test_servey_actions.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.682423 servey-2.7.0/tests/servey_thread/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-16 13:19:25.000000 servey-2.7.0/tests/servey_thread/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1388 2023-01-05 15:20:43.000000 servey-2.7.0/tests/servey_thread/test_asyncio_subscription_service.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1394 2022-12-18 15:20:29.000000 servey-2.7.0/tests/servey_thread/test_threaded_app.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.688292 servey-2.7.0/tests/servey_web_page/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-02 16:41:20.000000 servey-2.7.0/tests/servey_web_page/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.689529 servey-2.7.0/tests/servey_web_page/templates/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-02 17:10:03.000000 servey-2.7.0/tests/servey_web_page/templates/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4895 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_web_page/test_web_page_action_endpoint.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2730 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_web_page/test_web_page_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)      774 2023-04-05 21:10:12.000000 servey-2.7.0/tests/servey_web_page/test_web_page_trigger_handler.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.690155 servey-2.7.0/tests/specs/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.0/tests/specs/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.712893 servey-2.7.0/tests/specs/number_spec/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.0/tests/specs/number_spec/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      749 2023-01-05 15:20:43.000000 servey-2.7.0/tests/specs/number_spec/actions.py
--rw-r--r--   0 tofarr     (501) staff       (20)      982 2023-01-05 15:20:43.000000 servey-2.7.0/tests/specs/number_spec/models.py
--rw-r--r--   0 tofarr     (501) staff       (20)      725 2023-01-05 15:20:43.000000 servey-2.7.0/tests/specs/number_spec/subscriptions.py
--rw-r--r--   0 tofarr     (501) staff       (20)      173 2022-12-18 16:12:35.000000 servey-2.7.0/tests/test_bootstrap.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3017 2023-04-05 21:10:12.000000 servey-2.7.0/tests/test_marshy.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:34:09.719109 servey-2.7.0/tests/util/
--rw-r--r--   0 tofarr     (501) staff       (20)      706 2022-12-17 21:16:24.000000 servey-2.7.0/tests/util/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      591 2022-12-08 00:07:14.000000 servey-2.7.0/tests/util/test_singleton.py
--rw-r--r--   0 tofarr     (501) staff       (20)      810 2022-12-17 21:33:00.000000 servey-2.7.0/tests/util/test_to_second_datetime_marshaller.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.712518 servey-2.7.2/
+-rw-r--r--   0 tofarr     (501) staff       (20)    17979 2023-04-12 03:59:13.712188 servey-2.7.2/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)    17465 2023-04-05 22:22:08.000000 servey-2.7.2/README.md
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.356016 servey-2.7.2/marshy_config_servey/
+-rw-r--r--   0 tofarr     (501) staff       (20)    14673 2023-04-12 03:49:23.000000 servey-2.7.2/marshy_config_servey/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.358751 servey-2.7.2/servey/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-20 13:05:09.000000 servey-2.7.2/servey/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2478 2023-04-05 21:10:12.000000 servey-2.7.2/servey/__main__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.368072 servey-2.7.2/servey/action/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/action/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2763 2023-01-20 16:29:37.000000 servey-2.7.2/servey/action/action.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      233 2023-01-05 15:20:43.000000 servey-2.7.2/servey/action/batch_invoker.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      460 2022-12-09 15:33:15.000000 servey-2.7.2/servey/action/example.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4148 2023-01-06 03:56:01.000000 servey-2.7.2/servey/action/util.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.372606 servey-2.7.2/servey/cache_control/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2021-11-17 03:52:02.000000 servey-2.7.2/servey/cache_control/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      467 2022-12-09 17:19:54.000000 servey-2.7.2/servey/cache_control/cache_control_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2307 2023-04-05 21:10:12.000000 servey-2.7.2/servey/cache_control/cache_header.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      704 2023-02-03 15:04:24.000000 servey-2.7.2/servey/cache_control/secure_hash_cache_control.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1356 2022-12-24 00:22:46.000000 servey-2.7.2/servey/cache_control/timestamp_cache_control.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1274 2023-04-05 21:10:12.000000 servey-2.7.2/servey/cache_control/ttl_cache_control.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       39 2022-11-30 20:16:33.000000 servey-2.7.2/servey/errors.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.377898 servey-2.7.2/servey/finder/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/finder/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      836 2023-01-05 15:20:43.000000 servey-2.7.2/servey/finder/action_finder_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1777 2023-01-20 16:29:37.000000 servey-2.7.2/servey/finder/module_action_finder.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1601 2023-01-20 16:29:37.000000 servey-2.7.2/servey/finder/module_subscription_finder.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      653 2023-01-05 15:20:43.000000 servey-2.7.2/servey/finder/subscription_finder_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.379963 servey-2.7.2/servey/security/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/security/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.385399 servey-2.7.2/servey/security/access_control/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/security/access_control/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      335 2023-03-19 15:03:39.000000 servey-2.7.2/servey/security/access_control/access_control_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      357 2023-01-05 15:20:43.000000 servey-2.7.2/servey/security/access_control/allow_all.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      361 2023-01-05 15:20:43.000000 servey-2.7.2/servey/security/access_control/allow_none.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      516 2023-01-05 15:20:43.000000 servey-2.7.2/servey/security/access_control/scope_access_control.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.388026 servey-2.7.2/servey/security/authenticator/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 00:28:02.000000 servey-2.7.2/servey/security/authenticator/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      614 2023-01-18 13:36:34.000000 servey-2.7.2/servey/security/authenticator/password_authenticator_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1200 2023-01-18 13:36:35.000000 servey-2.7.2/servey/security/authenticator/root_password_authenticator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2407 2022-12-18 16:01:20.000000 servey-2.7.2/servey/security/authorization.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.392542 servey-2.7.2/servey/security/authorizer/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/security/authorizer/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      446 2022-09-16 02:42:12.000000 servey-2.7.2/servey/security/authorizer/authorizer_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1343 2022-12-09 15:17:12.000000 servey-2.7.2/servey/security/authorizer/authorizer_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2821 2022-12-16 15:10:54.000000 servey-2.7.2/servey/security/authorizer/jwt_authorizer.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1154 2022-11-30 20:16:33.000000 servey-2.7.2/servey/security/authorizer/jwt_authorizer_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.403936 servey-2.7.2/servey/servey_aws/
+-rw-r--r--   0 tofarr     (501) staff       (20)       91 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.406732 servey-2.7.2/servey/servey_aws/authorizer/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_aws/authorizer/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4516 2022-12-17 21:34:00.000000 servey-2.7.2/servey/servey_aws/authorizer/kms_authorizer.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      923 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/authorizer/kms_authorizer_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.414532 servey-2.7.2/servey/servey_aws/event_handler/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/event_handler/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5959 2023-04-02 17:53:57.000000 servey-2.7.2/servey/servey_aws/event_handler/api_gateway_event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1847 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/event_handler/appsync_event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5272 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/event_handler/event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1071 2023-04-02 13:21:49.000000 servey-2.7.2/servey/servey_aws/event_handler/event_handler_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2644 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/event_handler/sqs_event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2089 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_aws/lambda_invoker.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      878 2023-04-04 04:13:04.000000 servey-2.7.2/servey/servey_aws/lambda_router.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4214 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/lambda_websocket.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.420877 servey-2.7.2/servey/servey_aws/router/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-02 13:29:47.000000 servey-2.7.2/servey/servey_aws/router/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1114 2023-04-05 21:30:44.000000 servey-2.7.2/servey/servey_aws/router/api_gateway_router.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1255 2023-04-05 21:30:44.000000 servey-2.7.2/servey/servey_aws/router/appsync_router.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      717 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_aws/router/router.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1480 2023-04-05 21:35:02.000000 servey-2.7.2/servey/servey_aws/router/router_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.421897 servey-2.7.2/servey/servey_aws/serverless/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_aws/serverless/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1245 2023-03-30 22:57:04.000000 servey-2.7.2/servey/servey_aws/serverless/__main__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.425709 servey-2.7.2/servey/servey_aws/serverless/trigger_handler/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_aws/serverless/trigger_handler/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1265 2023-01-18 13:36:35.000000 servey-2.7.2/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      442 2022-12-17 21:14:47.000000 servey-2.7.2/servey/servey_aws/serverless/trigger_handler/trigger_handler_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1090 2023-01-07 16:53:22.000000 servey-2.7.2/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.447485 servey-2.7.2/servey/servey_aws/serverless/yml_config/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3987 2023-04-05 23:49:53.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/action_function_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5177 2023-04-06 00:37:56.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/appsync_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    10420 2023-04-12 03:53:52.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/cloudfront_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3593 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/kms_key_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      592 2023-01-20 16:29:37.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/serverless_template.yml
+-rw-r--r--   0 tofarr     (501) staff       (20)     5051 2023-04-12 03:56:40.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     7374 2023-04-06 12:59:59.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/subscription_function_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2947 2023-01-18 13:16:57.000000 servey-2.7.2/servey/servey_aws/serverless/yml_config/yml_config_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2179 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/sqs_subscription_service.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3210 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_aws/websocket_subscription_service.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.455192 servey-2.7.2/servey/servey_celery/
+-rw-r--r--   0 tofarr     (501) staff       (20)       86 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_celery/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1429 2023-01-07 16:31:15.000000 servey-2.7.2/servey/servey_celery/celery_app.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.475915 servey-2.7.2/servey/servey_celery/celery_config/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-07 16:19:02.000000 servey-2.7.2/servey/servey_celery/celery_config/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      241 2023-01-07 16:53:22.000000 servey-2.7.2/servey/servey_celery/celery_config/celery_config_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1004 2023-04-01 19:42:31.000000 servey-2.7.2/servey/servey_celery/celery_config/fixed_rate_trigger_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      592 2023-01-07 16:53:22.000000 servey-2.7.2/servey/servey_celery/celery_config/subscription_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1050 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_celery/celery_subscription_service.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.478720 servey-2.7.2/servey/servey_direct/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-16 16:23:58.000000 servey-2.7.2/servey/servey_direct/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1313 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_direct/__main__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.483456 servey-2.7.2/servey/servey_starlette/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_starlette/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.516108 servey-2.7.2/servey/servey_starlette/action_endpoint/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 15:42:17.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    11862 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/action_endpoint.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1134 2023-01-19 13:50:13.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/action_endpoint_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3401 2023-03-19 15:03:39.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2836 2023-03-19 15:03:39.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/caching_action_endpoint.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.524515 servey-2.7.2/servey/servey_starlette/action_endpoint/factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 17:29:46.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2786 2023-01-06 15:28:44.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      822 2022-12-11 13:56:30.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2183 2022-12-11 14:21:14.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1444 2022-12-16 15:10:54.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2260 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      201 2022-12-24 01:22:04.000000 servey-2.7.2/servey/servey_starlette/error_response.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.552673 servey-2.7.2/servey/servey_starlette/route_factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_starlette/route_factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1600 2023-01-06 15:28:44.000000 servey-2.7.2/servey/servey_starlette/route_factory/action_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3026 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_starlette/route_factory/asyncapi_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1928 2023-01-18 13:36:35.000000 servey-2.7.2/servey/servey_starlette/route_factory/authenticator_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2441 2023-01-20 16:29:37.000000 servey-2.7.2/servey/servey_starlette/route_factory/openapi_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      242 2023-01-14 15:50:20.000000 servey-2.7.2/servey/servey_starlette/route_factory/route_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      718 2023-01-18 13:36:35.000000 servey-2.7.2/servey/servey_starlette/route_factory/static_site_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6329 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_starlette/route_factory/subscription_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      521 2023-01-18 13:36:35.000000 servey-2.7.2/servey/servey_starlette/starlette_app.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.562049 servey-2.7.2/servey/servey_starlette/statics/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-11-30 19:30:04.000000 servey-2.7.2/servey/servey_starlette/statics/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      794 2022-09-16 02:41:41.000000 servey-2.7.2/servey/servey_starlette/statics/index.html
+-rw-r--r--   0 tofarr     (501) staff       (20)  1079398 2022-12-04 20:38:25.000000 servey-2.7.2/servey/servey_starlette/statics/swagger-ui-bundle.js
+-rw-r--r--   0 tofarr     (501) staff       (20)   192198 2022-09-16 02:41:41.000000 servey-2.7.2/servey/servey_starlette/statics/swagger-ui.css
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.572037 servey-2.7.2/servey/servey_strawberry/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_strawberry/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.585751 servey-2.7.2/servey/servey_strawberry/entity_factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_strawberry/entity_factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5804 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_strawberry/entity_factory/dataclass_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      515 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_strawberry/entity_factory/entity_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1105 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_strawberry/entity_factory/enum_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      890 2022-12-16 11:34:08.000000 servey-2.7.2/servey/servey_strawberry/entity_factory/forward_ref_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1343 2022-12-18 22:53:24.000000 servey-2.7.2/servey/servey_strawberry/entity_factory/generic_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      688 2022-12-18 22:59:58.000000 servey-2.7.2/servey/servey_strawberry/entity_factory/no_op_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.603355 servey-2.7.2/servey/servey_strawberry/handler_filter/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_strawberry/handler_filter/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3179 2023-01-07 04:41:39.000000 servey-2.7.2/servey/servey_strawberry/handler_filter/authorization_handler_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      687 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_strawberry/handler_filter/handler_filter_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1406 2022-12-27 15:18:15.000000 servey-2.7.2/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     7228 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_strawberry/schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      754 2022-12-16 15:10:54.000000 servey-2.7.2/servey/servey_strawberry/schema_factory_lazy_input.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      752 2022-12-16 15:10:54.000000 servey-2.7.2/servey/servey_strawberry/schema_factory_lazy_type.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.604966 servey-2.7.2/servey/servey_strawberry/statics/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-11-30 19:30:04.000000 servey-2.7.2/servey/servey_strawberry/statics/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1872 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_strawberry/statics/index.html
+-rw-r--r--   0 tofarr     (501) staff       (20)     1726 2023-01-20 16:29:37.000000 servey-2.7.2/servey/servey_strawberry/strawberry_starlette_route_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.606144 servey-2.7.2/servey/servey_test/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-04 20:47:53.000000 servey-2.7.2/servey/servey_test/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1164 2022-12-16 20:57:24.000000 servey-2.7.2/servey/servey_test/test_servey_actions.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.609266 servey-2.7.2/servey/servey_thread/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/servey_thread/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      905 2023-01-05 15:10:21.000000 servey-2.7.2/servey/servey_thread/__main__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1315 2023-01-05 15:20:43.000000 servey-2.7.2/servey/servey_thread/asyncio_subscription_service.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      515 2022-12-16 18:31:33.000000 servey-2.7.2/servey/servey_thread/fixed_rate_trigger_thread.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.615047 servey-2.7.2/servey/servey_web_page/
+-rw-r--r--   0 tofarr     (501) staff       (20)      213 2023-01-20 16:29:37.000000 servey-2.7.2/servey/servey_web_page/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      103 2023-03-19 15:03:39.000000 servey-2.7.2/servey/servey_web_page/redirect.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1687 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_web_page/web_page_action_endpoint.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2604 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_web_page/web_page_action_endpoint_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4335 2023-04-05 21:10:12.000000 servey-2.7.2/servey/servey_web_page/web_page_event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      709 2023-01-20 16:29:37.000000 servey-2.7.2/servey/servey_web_page/web_page_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      848 2023-01-20 16:29:37.000000 servey-2.7.2/servey/servey_web_page/web_page_trigger_handler.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.618351 servey-2.7.2/servey/subscription/
+-rw-r--r--   0 tofarr     (501) staff       (20)      595 2023-01-05 15:20:43.000000 servey-2.7.2/servey/subscription/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      392 2023-01-05 15:20:43.000000 servey-2.7.2/servey/subscription/event_filter_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1698 2023-01-05 15:20:43.000000 servey-2.7.2/servey/subscription/subscription.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1009 2023-01-05 15:20:43.000000 servey-2.7.2/servey/subscription/subscription_event.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1367 2023-01-05 15:20:43.000000 servey-2.7.2/servey/subscription/subscription_service.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.620954 servey-2.7.2/servey/trigger/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-09-16 02:42:12.000000 servey-2.7.2/servey/trigger/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      165 2022-12-08 23:20:52.000000 servey-2.7.2/servey/trigger/fixed_rate_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       92 2022-09-16 02:42:12.000000 servey-2.7.2/servey/trigger/trigger_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      762 2023-01-05 22:00:38.000000 servey-2.7.2/servey/trigger/web_trigger.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.623295 servey-2.7.2/servey/util/
+-rw-r--r--   0 tofarr     (501) staff       (20)      836 2023-01-05 15:20:43.000000 servey-2.7.2/servey/util/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      839 2022-08-10 15:17:22.000000 servey-2.7.2/servey/util/singleton_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      472 2022-12-17 21:18:47.000000 servey-2.7.2/servey/util/to_second_datetime_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-12 03:56:45.000000 servey-2.7.2/servey/version.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.364616 servey-2.7.2/servey.egg-info/
+-rw-r--r--   0 tofarr     (501) staff       (20)    17979 2023-04-12 03:59:13.000000 servey-2.7.2/servey.egg-info/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)    11054 2023-04-12 03:59:13.000000 servey-2.7.2/servey.egg-info/SOURCES.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-12 03:59:13.000000 servey-2.7.2/servey.egg-info/dependency_links.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)      530 2023-04-12 03:59:13.000000 servey-2.7.2/servey.egg-info/requires.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       46 2023-04-12 03:59:13.000000 servey-2.7.2/servey.egg-info/top_level.txt
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.346347 servey-2.7.2/servey_main/
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.624533 servey-2.7.2/servey_main/templates/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-20 16:29:37.000000 servey-2.7.2/servey_main/templates/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-12 03:59:13.712647 servey-2.7.2/setup.cfg
+-rw-r--r--   0 tofarr     (501) staff       (20)     1678 2023-04-05 21:10:12.000000 servey-2.7.2/setup.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.626510 servey-2.7.2/tests/
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.630596 servey-2.7.2/tests/action/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 22:53:16.000000 servey-2.7.2/tests/action/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2144 2023-01-21 19:57:16.000000 servey-2.7.2/tests/action/test_action.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      206 2023-01-05 15:20:43.000000 servey-2.7.2/tests/action/test_batch_invoker.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2481 2023-01-05 15:20:43.000000 servey-2.7.2/tests/action/test_util.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.635351 servey-2.7.2/tests/cache_control/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 23:17:15.000000 servey-2.7.2/tests/cache_control/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1456 2023-04-05 21:10:12.000000 servey-2.7.2/tests/cache_control/test_cache_header.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      967 2022-12-17 21:18:13.000000 servey-2.7.2/tests/cache_control/test_secure_hash_cache_control.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      648 2022-12-17 22:08:34.000000 servey-2.7.2/tests/cache_control/test_timestamp_cache_control.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      539 2022-12-09 15:33:15.000000 servey-2.7.2/tests/cache_control/test_ttl_cache_control.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.638117 servey-2.7.2/tests/finder/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 23:43:42.000000 servey-2.7.2/tests/finder/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.639406 servey-2.7.2/tests/finder/actions/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.2/tests/finder/actions/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       89 2023-01-05 15:20:43.000000 servey-2.7.2/tests/finder/actions/test_actions.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.640492 servey-2.7.2/tests/finder/subscriptions/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.2/tests/finder/subscriptions/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      176 2023-01-05 15:20:43.000000 servey-2.7.2/tests/finder/subscriptions/test_subscriptions.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      396 2023-01-05 15:20:43.000000 servey-2.7.2/tests/finder/test_action_finder.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1317 2023-01-05 15:20:43.000000 servey-2.7.2/tests/finder/test_module_action_finder.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1075 2023-01-05 15:20:43.000000 servey-2.7.2/tests/finder/test_module_subscription_finder.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.641609 servey-2.7.2/tests/security/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 00:06:37.000000 servey-2.7.2/tests/security/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.644080 servey-2.7.2/tests/security/access_control/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 01:00:09.000000 servey-2.7.2/tests/security/access_control/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      346 2022-12-23 22:40:15.000000 servey-2.7.2/tests/security/access_control/test_allow_all.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      349 2023-01-05 15:20:43.000000 servey-2.7.2/tests/security/access_control/test_allow_none.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1179 2022-12-23 22:39:43.000000 servey-2.7.2/tests/security/access_control/test_scope_access_control.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.646054 servey-2.7.2/tests/security/authorizer/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-09 01:57:56.000000 servey-2.7.2/tests/security/authorizer/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      691 2022-12-09 15:33:15.000000 servey-2.7.2/tests/security/authorizer/test_authorizer_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3291 2022-12-18 15:39:56.000000 servey-2.7.2/tests/security/authorizer/test_jwt_authorizer.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5926 2023-01-05 15:20:43.000000 servey-2.7.2/tests/security/test_authorization.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.652971 servey-2.7.2/tests/servey_aws/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-24 02:48:37.000000 servey-2.7.2/tests/servey_aws/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2127 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_aws/test_kms_authorizer.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    11013 2023-03-19 15:03:39.000000 servey-2.7.2/tests/servey_aws/test_lambda_invoker.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2705 2023-04-05 21:37:18.000000 servey-2.7.2/tests/servey_aws/test_lambda_router.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     9461 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_aws/test_lambda_websocket.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     9017 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_aws/test_serverless.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1847 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_aws/test_sqs_subscription_service.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3806 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_aws/test_websocket_subscription_service.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.655061 servey-2.7.2/tests/servey_celery/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-24 02:16:58.000000 servey-2.7.2/tests/servey_celery/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4311 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_celery/test_celery_app.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.656063 servey-2.7.2/tests/servey_direct/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-18 14:22:06.000000 servey-2.7.2/tests/servey_direct/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1175 2023-04-04 03:50:22.000000 servey-2.7.2/tests/servey_direct/test_servey_direct.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.659015 servey-2.7.2/tests/servey_starlette/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-11 16:01:52.000000 servey-2.7.2/tests/servey_starlette/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.663551 servey-2.7.2/tests/servey_starlette/action_endpoint/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-11 16:02:12.000000 servey-2.7.2/tests/servey_starlette/action_endpoint/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    29340 2023-04-05 21:10:13.000000 servey-2.7.2/tests/servey_starlette/action_endpoint/test_action_endpoint.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1565 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_starlette/action_endpoint/test_action_endpoint_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     7342 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_starlette/action_endpoint/test_authorizing_action_endpoint.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2569 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_starlette/action_endpoint/test_self_action_endpoint.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6440 2023-03-19 15:03:39.000000 servey-2.7.2/tests/servey_starlette/action_endpoint/test_static_caching_action_endpoint.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.666932 servey-2.7.2/tests/servey_starlette/route_factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-24 01:19:36.000000 servey-2.7.2/tests/servey_starlette/route_factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2859 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_starlette/route_factory/test_asyncapi_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1854 2023-01-18 13:36:35.000000 servey-2.7.2/tests/servey_starlette/route_factory/test_authenticator_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1073 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_starlette/route_factory/test_statc_site_route_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     9426 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_starlette/route_factory/test_subscription_route.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1721 2023-03-16 02:11:16.000000 servey-2.7.2/tests/servey_starlette/test_starlette_app.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.673885 servey-2.7.2/tests/servey_strawberry/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-15 23:35:01.000000 servey-2.7.2/tests/servey_strawberry/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      207 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_strawberry/actions.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.676501 servey-2.7.2/tests/servey_strawberry/entity_factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-15 23:35:48.000000 servey-2.7.2/tests/servey_strawberry/entity_factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      565 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_strawberry/entity_factory/test_dataclass_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      554 2022-12-17 21:34:29.000000 servey-2.7.2/tests/servey_strawberry/entity_factory/test_enum_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.679812 servey-2.7.2/tests/servey_strawberry/handler_filter/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-18 23:00:44.000000 servey-2.7.2/tests/servey_strawberry/handler_filter/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2735 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_strawberry/handler_filter/test_authorization_handler_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      126 2022-12-23 15:50:38.000000 servey-2.7.2/tests/servey_strawberry/handler_filter/test_handler_filter_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    11356 2023-01-07 17:02:07.000000 servey-2.7.2/tests/servey_strawberry/test_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      174 2022-12-18 16:12:35.000000 servey-2.7.2/tests/servey_strawberry/test_statics.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1584 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_strawberry/test_strawberry_starlette_route_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.681644 servey-2.7.2/tests/servey_test/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-08 00:15:49.000000 servey-2.7.2/tests/servey_test/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1312 2022-12-18 14:33:32.000000 servey-2.7.2/tests/servey_test/test_test_servey_actions.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.685147 servey-2.7.2/tests/servey_thread/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-12-16 13:19:25.000000 servey-2.7.2/tests/servey_thread/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1388 2023-01-05 15:20:43.000000 servey-2.7.2/tests/servey_thread/test_asyncio_subscription_service.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1394 2022-12-18 15:20:29.000000 servey-2.7.2/tests/servey_thread/test_threaded_app.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.703283 servey-2.7.2/tests/servey_web_page/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-02 16:41:20.000000 servey-2.7.2/tests/servey_web_page/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.704227 servey-2.7.2/tests/servey_web_page/templates/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-02 17:10:03.000000 servey-2.7.2/tests/servey_web_page/templates/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4895 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_web_page/test_web_page_action_endpoint.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2730 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_web_page/test_web_page_event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      774 2023-04-05 21:10:12.000000 servey-2.7.2/tests/servey_web_page/test_web_page_trigger_handler.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.704692 servey-2.7.2/tests/specs/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.2/tests/specs/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.708866 servey-2.7.2/tests/specs/number_spec/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 15:20:43.000000 servey-2.7.2/tests/specs/number_spec/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      749 2023-01-05 15:20:43.000000 servey-2.7.2/tests/specs/number_spec/actions.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      982 2023-01-05 15:20:43.000000 servey-2.7.2/tests/specs/number_spec/models.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      725 2023-01-05 15:20:43.000000 servey-2.7.2/tests/specs/number_spec/subscriptions.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      173 2022-12-18 16:12:35.000000 servey-2.7.2/tests/test_bootstrap.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3017 2023-04-05 21:10:12.000000 servey-2.7.2/tests/test_marshy.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-12 03:59:13.711147 servey-2.7.2/tests/util/
+-rw-r--r--   0 tofarr     (501) staff       (20)      706 2022-12-17 21:16:24.000000 servey-2.7.2/tests/util/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      591 2022-12-08 00:07:14.000000 servey-2.7.2/tests/util/test_singleton.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      810 2022-12-17 21:33:00.000000 servey-2.7.2/tests/util/test_to_second_datetime_marshaller.py
```

### Comparing `servey-2.7.0/PKG-INFO` & `servey-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servey
-Version: 2.7.0
+Version: 2.7.2
 Summary: A better API layer for python
 Home-page: https://github.com/tofarr/servey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `servey-2.7.0/README.md` & `servey-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/marshy_config_servey/__init__.py` & `servey-2.7.2/marshy_config_servey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,41 +255,43 @@
             ActionFunctionConfig,
         )
         from servey.servey_aws.serverless.yml_config.appsync_config import AppsyncConfig
         from servey.servey_aws.serverless.yml_config.kms_key_config import KmsKeyConfig
         from servey.servey_aws.serverless.yml_config.subscription_function_config import (
             SubscriptionFunctionConfig,
         )
-        from servey.servey_aws.serverless.yml_config.cloudfront_config import (
-            CloudfrontConfig
-        )
-        from servey.servey_aws.serverless.yml_config.static_site_bucket_config import (
-            StaticSiteBucketConfig
-        )
 
         register_impl(YmlConfigABC, ActionFunctionConfig, context)
         register_impl(YmlConfigABC, AppsyncConfig, context)
         register_impl(YmlConfigABC, KmsKeyConfig, context)
         register_impl(YmlConfigABC, SubscriptionFunctionConfig, context)
-        register_impl(YmlConfigABC, CloudfrontConfig, context)
-        register_impl(YmlConfigABC, StaticSiteBucketConfig, context)
 
         from servey.servey_aws.serverless.trigger_handler.trigger_handler_abc import (
             TriggerHandlerABC,
         )
         from servey.servey_aws.serverless.trigger_handler.web_trigger_handler import (
             WebTriggerHandler,
         )
         from servey.servey_aws.serverless.trigger_handler.fixed_rate_trigger_handler import (
             FixedRateTriggerHandler,
         )
 
         register_impl(TriggerHandlerABC, WebTriggerHandler, context)
         register_impl(TriggerHandlerABC, FixedRateTriggerHandler, context)
 
+        from servey.servey_aws.serverless.yml_config.cloudfront_config import (
+            CloudfrontConfig
+        )
+        from servey.servey_aws.serverless.yml_config.static_site_bucket_config import (
+            StaticSiteBucketConfig
+        )
+
+        register_impl(YmlConfigABC, CloudfrontConfig, context)
+        register_impl(YmlConfigABC, StaticSiteBucketConfig, context)
+
     except ModuleNotFoundError as e:
         raise_non_ignored(e)
 
 
 def configure_celery(context: MarshallerContext):
     try:
         from servey.servey_celery.celery_subscription_service import (
```

### Comparing `servey-2.7.0/servey/__main__.py` & `servey-2.7.2/servey/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/action/action.py` & `servey-2.7.2/servey/action/action.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/action/util.py` & `servey-2.7.2/servey/action/util.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/cache_control/cache_header.py` & `servey-2.7.2/servey/cache_control/cache_header.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/cache_control/secure_hash_cache_control.py` & `servey-2.7.2/servey/cache_control/secure_hash_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/cache_control/timestamp_cache_control.py` & `servey-2.7.2/servey/cache_control/timestamp_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/cache_control/ttl_cache_control.py` & `servey-2.7.2/servey/cache_control/ttl_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/finder/action_finder_abc.py` & `servey-2.7.2/servey/finder/action_finder_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/finder/module_action_finder.py` & `servey-2.7.2/servey/finder/module_action_finder.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/finder/module_subscription_finder.py` & `servey-2.7.2/servey/finder/module_subscription_finder.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/finder/subscription_finder_abc.py` & `servey-2.7.2/servey/finder/subscription_finder_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/security/access_control/scope_access_control.py` & `servey-2.7.2/servey/security/access_control/scope_access_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/security/authenticator/password_authenticator_abc.py` & `servey-2.7.2/servey/security/authenticator/password_authenticator_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/security/authenticator/root_password_authenticator.py` & `servey-2.7.2/servey/security/authenticator/root_password_authenticator.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/security/authorization.py` & `servey-2.7.2/servey/security/authorization.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/security/authorizer/authorizer_factory_abc.py` & `servey-2.7.2/servey/security/authorizer/authorizer_factory_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/security/authorizer/jwt_authorizer.py` & `servey-2.7.2/servey/security/authorizer/jwt_authorizer.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/security/authorizer/jwt_authorizer_factory.py` & `servey-2.7.2/servey/security/authorizer/jwt_authorizer_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/authorizer/kms_authorizer.py` & `servey-2.7.2/servey/servey_aws/authorizer/kms_authorizer.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/authorizer/kms_authorizer_factory.py` & `servey-2.7.2/servey/servey_aws/authorizer/kms_authorizer_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/event_handler/api_gateway_event_handler.py` & `servey-2.7.2/servey/servey_aws/event_handler/api_gateway_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/event_handler/appsync_event_handler.py` & `servey-2.7.2/servey/servey_aws/event_handler/appsync_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/event_handler/event_handler.py` & `servey-2.7.2/servey/servey_aws/event_handler/event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/event_handler/event_handler_abc.py` & `servey-2.7.2/servey/servey_aws/event_handler/event_handler_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/event_handler/sqs_event_handler.py` & `servey-2.7.2/servey/servey_aws/event_handler/sqs_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/lambda_invoker.py` & `servey-2.7.2/servey/servey_aws/lambda_invoker.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/lambda_router.py` & `servey-2.7.2/servey/servey_aws/lambda_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/lambda_websocket.py` & `servey-2.7.2/servey/servey_aws/lambda_websocket.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/router/api_gateway_router.py` & `servey-2.7.2/servey/servey_aws/router/api_gateway_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/router/appsync_router.py` & `servey-2.7.2/servey/servey_aws/router/appsync_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/router/router.py` & `servey-2.7.2/servey/servey_aws/router/router.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/router/router_abc.py` & `servey-2.7.2/servey/servey_aws/router/router_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/__main__.py` & `servey-2.7.2/servey/servey_aws/serverless/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py` & `servey-2.7.2/servey/servey_aws/serverless/trigger_handler/fixed_rate_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py` & `servey-2.7.2/servey/servey_aws/serverless/trigger_handler/web_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/action_function_config.py` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/action_function_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/appsync_config.py` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/appsync_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/cloudfront_config.py` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/cloudfront_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 
 from servey.finder.action_finder_abc import find_actions_with_trigger_type
 from servey.servey_aws.serverless.yml_config.yml_config_abc import (
     YmlConfigABC,
     ensure_ref_in_file,
     create_yml_file,
 )
-from servey.servey_web_page.web_page_trigger import WebPageTrigger
 
 
 class CloudfrontConfig(YmlConfigABC):
     """
     Set up some aspect of the serverless environment yml files. (For example, functions, resources, etc...)
     """
     static_site_directory: Path = Path(os.environ.get("SERVEY_STATIC_SITE_DIR") or "static_site")
     static_site_bucket_resource_yml_file: str = "serverless_servey/cloudfront_resource.yml"
 
     def configure(self, main_serverless_yml_file: str):
         has_static_site = self.static_site_directory.exists()
-        has_web_page = next((True for _ in find_actions_with_trigger_type(WebPageTrigger)), False)
+        has_web_page = False
+        try:
+            from servey.servey_web_page.web_page_trigger import WebPageTrigger
+            has_web_page = next((True for _ in find_actions_with_trigger_type(WebPageTrigger)), False)
+        except ImportError:
+            pass
         if not has_static_site and not has_web_page:
             return
         # If there is a static site
         ensure_ref_in_file(
             main_serverless_yml_file,
             ["resources"],
             self.static_site_bucket_resource_yml_file,
```

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/kms_key_config.py` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/kms_key_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/serverless_template.yml` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/serverless_template.yml`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/static_site_bucket_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         yaml = YAML()
         with open(main_serverless_yml_file, "r") as reader:
             root = yaml.load(reader)
             custom = root.get('custom')
             static_bucket = custom.get('staticBucket')
             if static_bucket:
                 return static_bucket
-        static_bucket = ''.join(ALPHABET[randint(0, 36)] for _ in range(10))
+        static_bucket = ''.join(ALPHABET[randint(0, 35)] for _ in range(10))
         custom['staticBucket'] = static_bucket
         with open(main_serverless_yml_file, "w") as writer:
             yaml.dump(root, writer)
         return static_bucket
 
     @staticmethod
     def build_static_site_bucket_resource_yml() -> ExternalItemType:
```

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/subscription_function_config.py` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/subscription_function_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/serverless/yml_config/yml_config_abc.py` & `servey-2.7.2/servey/servey_aws/serverless/yml_config/yml_config_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/sqs_subscription_service.py` & `servey-2.7.2/servey/servey_aws/sqs_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_aws/websocket_subscription_service.py` & `servey-2.7.2/servey/servey_aws/websocket_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_celery/celery_app.py` & `servey-2.7.2/servey/servey_celery/celery_app.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_celery/celery_config/fixed_rate_trigger_config.py` & `servey-2.7.2/servey/servey_celery/celery_config/fixed_rate_trigger_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_celery/celery_config/subscription_config.py` & `servey-2.7.2/servey/servey_celery/celery_config/subscription_config.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_celery/celery_subscription_service.py` & `servey-2.7.2/servey/servey_celery/celery_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_direct/__main__.py` & `servey-2.7.2/servey/servey_direct/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/action_endpoint.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/action_endpoint_abc.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/action_endpoint_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/authorizing_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/caching_action_endpoint.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/caching_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/factory/action_endpoint_factory_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/factory/authorizing_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/factory/caching_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py` & `servey-2.7.2/servey/servey_starlette/action_endpoint/factory/self_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/route_factory/action_route_factory.py` & `servey-2.7.2/servey/servey_starlette/route_factory/action_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/route_factory/asyncapi_route_factory.py` & `servey-2.7.2/servey/servey_starlette/route_factory/asyncapi_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/route_factory/authenticator_route_factory.py` & `servey-2.7.2/servey/servey_starlette/route_factory/authenticator_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/route_factory/openapi_route_factory.py` & `servey-2.7.2/servey/servey_starlette/route_factory/openapi_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/route_factory/static_site_route_factory.py` & `servey-2.7.2/servey/servey_starlette/route_factory/static_site_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/route_factory/subscription_route_factory.py` & `servey-2.7.2/servey/servey_starlette/route_factory/subscription_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/starlette_app.py` & `servey-2.7.2/servey/servey_starlette/starlette_app.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/statics/index.html` & `servey-2.7.2/servey/servey_starlette/statics/index.html`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/statics/swagger-ui-bundle.js` & `servey-2.7.2/servey/servey_starlette/statics/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_starlette/statics/swagger-ui.css` & `servey-2.7.2/servey/servey_starlette/statics/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/entity_factory/dataclass_factory.py` & `servey-2.7.2/servey/servey_strawberry/entity_factory/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/entity_factory/entity_factory_abc.py` & `servey-2.7.2/servey/servey_strawberry/entity_factory/entity_factory_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/entity_factory/enum_factory.py` & `servey-2.7.2/servey/servey_strawberry/entity_factory/enum_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/entity_factory/forward_ref_factory.py` & `servey-2.7.2/servey/servey_strawberry/entity_factory/forward_ref_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/entity_factory/generic_factory.py` & `servey-2.7.2/servey/servey_strawberry/entity_factory/generic_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/entity_factory/no_op_factory.py` & `servey-2.7.2/servey/servey_strawberry/entity_factory/no_op_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/handler_filter/authorization_handler_filter.py` & `servey-2.7.2/servey/servey_strawberry/handler_filter/authorization_handler_filter.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/handler_filter/handler_filter_abc.py` & `servey-2.7.2/servey/servey_strawberry/handler_filter/handler_filter_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py` & `servey-2.7.2/servey/servey_strawberry/handler_filter/strawberry_type_handler_filter.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/schema_factory.py` & `servey-2.7.2/servey/servey_strawberry/schema_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/schema_factory_lazy_input.py` & `servey-2.7.2/servey/servey_strawberry/schema_factory_lazy_input.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/schema_factory_lazy_type.py` & `servey-2.7.2/servey/servey_strawberry/schema_factory_lazy_type.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/statics/index.html` & `servey-2.7.2/servey/servey_strawberry/statics/index.html`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_strawberry/strawberry_starlette_route_factory.py` & `servey-2.7.2/servey/servey_strawberry/strawberry_starlette_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_test/test_servey_actions.py` & `servey-2.7.2/servey/servey_test/test_servey_actions.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_thread/__main__.py` & `servey-2.7.2/servey/servey_thread/__main__.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_thread/asyncio_subscription_service.py` & `servey-2.7.2/servey/servey_thread/asyncio_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_thread/fixed_rate_trigger_thread.py` & `servey-2.7.2/servey/servey_thread/fixed_rate_trigger_thread.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_web_page/web_page_action_endpoint.py` & `servey-2.7.2/servey/servey_web_page/web_page_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_web_page/web_page_action_endpoint_factory.py` & `servey-2.7.2/servey/servey_web_page/web_page_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_web_page/web_page_event_handler.py` & `servey-2.7.2/servey/servey_web_page/web_page_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_web_page/web_page_trigger.py` & `servey-2.7.2/servey/servey_web_page/web_page_trigger.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/servey_web_page/web_page_trigger_handler.py` & `servey-2.7.2/servey/servey_web_page/web_page_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/subscription/__init__.py` & `servey-2.7.2/servey/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/subscription/subscription.py` & `servey-2.7.2/servey/subscription/subscription.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/subscription/subscription_event.py` & `servey-2.7.2/servey/subscription/subscription_event.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/subscription/subscription_service.py` & `servey-2.7.2/servey/subscription/subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/trigger/web_trigger.py` & `servey-2.7.2/servey/trigger/web_trigger.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/util/__init__.py` & `servey-2.7.2/servey/util/__init__.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey/util/singleton_abc.py` & `servey-2.7.2/servey/util/singleton_abc.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey.egg-info/PKG-INFO` & `servey-2.7.2/servey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servey
-Version: 2.7.0
+Version: 2.7.2
 Summary: A better API layer for python
 Home-page: https://github.com/tofarr/servey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `servey-2.7.0/servey.egg-info/SOURCES.txt` & `servey-2.7.2/servey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/servey.egg-info/requires.txt` & `servey-2.7.2/servey.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 marshy~=3.0
 schemey~=5.7
 json-urley~=1.0
 pyjwt~=2.4
 cryptography~=37.0
 
 [all]
-pyyaml~=6.0
-celery~=5.2
-python-multipart~=0.0
 black
-Jinja2~=3.1
-pygments~=2.13
+uvicorn[standard]~=0.18
+strawberry-graphql~=0.151
+celery~=5.2
 pytest
+pyyaml~=6.0
+ruamel.yaml~=0.17
+pygments~=2.13
 requests~=2.28
+Jinja2~=3.1
 starlette~=0.19
-ruamel.yaml~=0.17
-strawberry-graphql~=0.151
-uvicorn[standard]~=0.18
+python-multipart~=0.0
 
 [dev]
 black
 pytest
 
 [scheduler]
 celery~=5.2
```

### Comparing `servey-2.7.0/setup.py` & `servey-2.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/action/test_action.py` & `servey-2.7.2/tests/action/test_action.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/action/test_util.py` & `servey-2.7.2/tests/action/test_util.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/cache_control/test_cache_header.py` & `servey-2.7.2/tests/cache_control/test_cache_header.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/cache_control/test_secure_hash_cache_control.py` & `servey-2.7.2/tests/cache_control/test_secure_hash_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/cache_control/test_timestamp_cache_control.py` & `servey-2.7.2/tests/cache_control/test_timestamp_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/cache_control/test_ttl_cache_control.py` & `servey-2.7.2/tests/cache_control/test_ttl_cache_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/finder/test_module_action_finder.py` & `servey-2.7.2/tests/finder/test_module_action_finder.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/finder/test_module_subscription_finder.py` & `servey-2.7.2/tests/finder/test_module_subscription_finder.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/security/access_control/test_scope_access_control.py` & `servey-2.7.2/tests/security/access_control/test_scope_access_control.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/security/authorizer/test_authorizer_factory.py` & `servey-2.7.2/tests/security/authorizer/test_authorizer_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/security/authorizer/test_jwt_authorizer.py` & `servey-2.7.2/tests/security/authorizer/test_jwt_authorizer.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/security/test_authorization.py` & `servey-2.7.2/tests/security/test_authorization.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_aws/test_kms_authorizer.py` & `servey-2.7.2/tests/servey_aws/test_kms_authorizer.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_aws/test_lambda_invoker.py` & `servey-2.7.2/tests/servey_aws/test_lambda_invoker.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_aws/test_lambda_router.py` & `servey-2.7.2/tests/servey_aws/test_lambda_router.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_aws/test_lambda_websocket.py` & `servey-2.7.2/tests/servey_aws/test_lambda_websocket.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_aws/test_serverless.py` & `servey-2.7.2/tests/servey_aws/test_serverless.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_aws/test_sqs_subscription_service.py` & `servey-2.7.2/tests/servey_aws/test_sqs_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_aws/test_websocket_subscription_service.py` & `servey-2.7.2/tests/servey_aws/test_websocket_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_celery/test_celery_app.py` & `servey-2.7.2/tests/servey_celery/test_celery_app.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_direct/test_servey_direct.py` & `servey-2.7.2/tests/servey_direct/test_servey_direct.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/action_endpoint/test_action_endpoint.py` & `servey-2.7.2/tests/servey_starlette/action_endpoint/test_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/action_endpoint/test_action_endpoint_factory.py` & `servey-2.7.2/tests/servey_starlette/action_endpoint/test_action_endpoint_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/action_endpoint/test_authorizing_action_endpoint.py` & `servey-2.7.2/tests/servey_starlette/action_endpoint/test_authorizing_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/action_endpoint/test_self_action_endpoint.py` & `servey-2.7.2/tests/servey_starlette/action_endpoint/test_self_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/action_endpoint/test_static_caching_action_endpoint.py` & `servey-2.7.2/tests/servey_starlette/action_endpoint/test_static_caching_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/route_factory/test_asyncapi_route_factory.py` & `servey-2.7.2/tests/servey_starlette/route_factory/test_asyncapi_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/route_factory/test_authenticator_route_factory.py` & `servey-2.7.2/tests/servey_starlette/route_factory/test_authenticator_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/route_factory/test_statc_site_route_factory.py` & `servey-2.7.2/tests/servey_starlette/route_factory/test_statc_site_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/route_factory/test_subscription_route.py` & `servey-2.7.2/tests/servey_starlette/route_factory/test_subscription_route.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_starlette/test_starlette_app.py` & `servey-2.7.2/tests/servey_starlette/test_starlette_app.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_strawberry/entity_factory/test_dataclass_factory.py` & `servey-2.7.2/tests/servey_strawberry/entity_factory/test_dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_strawberry/entity_factory/test_enum_factory.py` & `servey-2.7.2/tests/servey_strawberry/entity_factory/test_enum_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_strawberry/handler_filter/test_authorization_handler_filter.py` & `servey-2.7.2/tests/servey_strawberry/handler_filter/test_authorization_handler_filter.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_strawberry/test_schema_factory.py` & `servey-2.7.2/tests/servey_strawberry/test_schema_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_strawberry/test_strawberry_starlette_route_factory.py` & `servey-2.7.2/tests/servey_strawberry/test_strawberry_starlette_route_factory.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_test/test_test_servey_actions.py` & `servey-2.7.2/tests/servey_test/test_test_servey_actions.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_thread/test_asyncio_subscription_service.py` & `servey-2.7.2/tests/servey_thread/test_asyncio_subscription_service.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_thread/test_threaded_app.py` & `servey-2.7.2/tests/servey_thread/test_threaded_app.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_web_page/test_web_page_action_endpoint.py` & `servey-2.7.2/tests/servey_web_page/test_web_page_action_endpoint.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_web_page/test_web_page_event_handler.py` & `servey-2.7.2/tests/servey_web_page/test_web_page_event_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/servey_web_page/test_web_page_trigger_handler.py` & `servey-2.7.2/tests/servey_web_page/test_web_page_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/specs/number_spec/actions.py` & `servey-2.7.2/tests/specs/number_spec/actions.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/specs/number_spec/models.py` & `servey-2.7.2/tests/specs/number_spec/models.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/specs/number_spec/subscriptions.py` & `servey-2.7.2/tests/specs/number_spec/subscriptions.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/test_marshy.py` & `servey-2.7.2/tests/test_marshy.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/util/__init__.py` & `servey-2.7.2/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/util/test_singleton.py` & `servey-2.7.2/tests/util/test_singleton.py`

 * *Files identical despite different names*

### Comparing `servey-2.7.0/tests/util/test_to_second_datetime_marshaller.py` & `servey-2.7.2/tests/util/test_to_second_datetime_marshaller.py`

 * *Files identical despite different names*

