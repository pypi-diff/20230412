# Comparing `tmp/ShopifyAPI-8.4.2.tar.gz` & `tmp/ShopifyAPI-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ShopifyAPI-8.4.2.tar", last modified: Thu Aug  5 20:13:40 2021, max compression
+gzip compressed data, was "dist/ShopifyAPI-9.0.0.tar", last modified: Mon Oct 18 18:41:55 2021, max compression
```

## Comparing `ShopifyAPI-8.4.2.tar` & `ShopifyAPI-9.0.0.tar`

### file list

```diff
@@ -1,118 +1,117 @@
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.711104 ShopifyAPI-8.4.2/
--rw-r--r--   0 kevinosullivan   (501) staff       (20)    10104 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/CHANGELOG
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1061 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/LICENSE
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       79 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/MANIFEST.in
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1391 2021-08-05 20:13:40.710872 ShopifyAPI-8.4.2/PKG-INFO
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     9521 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/README.md
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.672085 ShopifyAPI-8.4.2/ShopifyAPI.egg-info/
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1391 2021-08-05 20:13:40.000000 ShopifyAPI-8.4.2/ShopifyAPI.egg-info/PKG-INFO
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     3267 2021-08-05 20:13:40.000000 ShopifyAPI-8.4.2/ShopifyAPI.egg-info/SOURCES.txt
--rw-r--r--   0 kevinosullivan   (501) staff       (20)        1 2021-08-05 20:13:40.000000 ShopifyAPI-8.4.2/ShopifyAPI.egg-info/dependency_links.txt
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      117 2021-08-05 20:13:40.000000 ShopifyAPI-8.4.2/ShopifyAPI.egg-info/requires.txt
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       40 2021-08-05 20:13:40.000000 ShopifyAPI-8.4.2/ShopifyAPI.egg-info/top_level.txt
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.672402 ShopifyAPI-8.4.2/bin/
--rwxr-xr-x   0 kevinosullivan   (501) staff       (20)      416 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/bin/shopify_api.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       70 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/pyproject.toml
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.672896 ShopifyAPI-8.4.2/scripts/
--rwxr-xr-x   0 kevinosullivan   (501) staff       (20)     9199 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/scripts/shopify_api.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       38 2021-08-05 20:13:40.711185 ShopifyAPI-8.4.2/setup.cfg
--rwxr-xr-x   0 kevinosullivan   (501) staff       (20)     1941 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/setup.py
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.678047 ShopifyAPI-8.4.2/shopify/
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      275 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/__init__.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     2010 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/api_access.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     2008 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/api_version.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     7625 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/base.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     5364 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/collection.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1611 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/limits.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1100 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/mixins.py
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.709319 ShopifyAPI-8.4.2/shopify/resources/
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     3020 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/__init__.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      150 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/access_scope.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       78 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/address.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      241 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/api_permission.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      170 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/application_charge.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       88 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/application_credit.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      664 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/article.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     2613 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/asset.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      193 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/balance.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       85 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/billing_address.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      219 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/blog.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      302 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/carrier_service.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       75 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/cart.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       79 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/checkout.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       78 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/collect.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      199 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/collection_listing.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      137 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/collection_publication.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      512 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/comment.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       78 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/country.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       79 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/currency.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      547 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/custom_collection.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1039 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/customer.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      108 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/customer_group.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       85 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/customer_invite.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      220 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/customer_saved_search.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      126 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/discount_code.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      517 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/discount_code_creation.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      158 2020-12-01 16:24:11.000000 ShopifyAPI-8.4.2/shopify/resources/disputes.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      650 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/draft_order.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       88 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/draft_order_invoice.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      350 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/event.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1040 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/fulfillment.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      961 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/fulfillment_event.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      306 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/fulfillment_service.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1038 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/gift_card.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      193 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/gift_card_adjustment.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1066 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/graphql.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1423 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/image.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       84 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/inventory_item.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     2249 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/inventory_level.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      120 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/line_item.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      304 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/location.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      267 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/marketing_event.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      354 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/metafield.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       84 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/note_attribute.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       77 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/option.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      929 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/order.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      158 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/order_risk.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      136 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/page.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       85 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/payment_details.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      157 2020-12-01 16:24:11.000000 ShopifyAPI-8.4.2/shopify/resources/payouts.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      153 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/policy.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      912 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/price_rule.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1597 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/product.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      210 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/product_listing.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      134 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/product_publication.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      123 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/province.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       82 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/publication.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       78 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/receipt.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      863 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/recurring_application_charge.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       79 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/redirect.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1072 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/refund.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       77 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/report.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      383 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/resource_feedback.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       75 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/rule.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       80 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/script_tag.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       86 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/shipping_address.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       83 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/shipping_line.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       83 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/shipping_zone.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      556 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/shop.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      236 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/smart_collection.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       92 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/storefront_access_token.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       78 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/tax_line.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       88 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/tender_transaction.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       76 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/theme.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      115 2020-05-04 19:32:47.000000 ShopifyAPI-8.4.2/shopify/resources/transaction.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      170 2020-12-01 16:24:11.000000 ShopifyAPI-8.4.2/shopify/resources/transactions.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      490 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/usage_charge.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      145 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/user.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     1001 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/variant.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      295 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/resources/webhook.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     6109 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/session.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     2107 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/session_token.py
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.709982 ShopifyAPI-8.4.2/shopify/utils/
--rw-r--r--   0 kevinosullivan   (501) staff       (20)        0 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/utils/__init__.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      699 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/utils/shop_url.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)       18 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/version.py
--rw-r--r--   0 kevinosullivan   (501) staff       (20)      682 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/shopify/yamlobjects.py
-drwxr-xr-x   0 kevinosullivan   (501) staff       (20)        0 2021-08-05 20:13:40.710334 ShopifyAPI-8.4.2/test/
--rw-r--r--   0 kevinosullivan   (501) staff       (20)     2040 2021-08-04 15:15:06.000000 ShopifyAPI-8.4.2/test/test_helper.py
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/
+-rw-rw-r--   0 appuser  (32767)     8192       79 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/MANIFEST.in
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/test/
+-rw-rw-r--   0 appuser  (32767)     8192     2040 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/test/test_helper.py
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/ShopifyAPI.egg-info/
+-rw-r--r--   0 appuser  (32767)     8192     3252 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/ShopifyAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 appuser  (32767)     8192     1293 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/ShopifyAPI.egg-info/PKG-INFO
+-rw-r--r--   0 appuser  (32767)     8192       40 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/ShopifyAPI.egg-info/top_level.txt
+-rw-r--r--   0 appuser  (32767)     8192        1 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/ShopifyAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 appuser  (32767)     8192       50 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/ShopifyAPI.egg-info/requires.txt
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/shopify/
+-rw-rw-r--   0 appuser  (32767)     8192      275 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/__init__.py
+-rw-rw-r--   0 appuser  (32767)     8192      682 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/yamlobjects.py
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/shopify/resources/
+-rw-rw-r--   0 appuser  (32767)     8192     3020 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/__init__.py
+-rw-rw-r--   0 appuser  (32767)     8192      490 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/usage_charge.py
+-rw-rw-r--   0 appuser  (32767)     8192       76 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/theme.py
+-rw-rw-r--   0 appuser  (32767)     8192      350 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/event.py
+-rw-rw-r--   0 appuser  (32767)     8192      961 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/fulfillment_event.py
+-rw-rw-r--   0 appuser  (32767)     8192      354 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/metafield.py
+-rw-rw-r--   0 appuser  (32767)     8192      219 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/blog.py
+-rw-rw-r--   0 appuser  (32767)     8192      210 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/product_listing.py
+-rw-rw-r--   0 appuser  (32767)     8192       75 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/cart.py
+-rw-rw-r--   0 appuser  (32767)     8192      241 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/api_permission.py
+-rw-rw-r--   0 appuser  (32767)     8192      136 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/page.py
+-rw-rw-r--   0 appuser  (32767)     8192     1072 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/refund.py
+-rw-rw-r--   0 appuser  (32767)     8192      863 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/recurring_application_charge.py
+-rw-rw-r--   0 appuser  (32767)     8192       92 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/storefront_access_token.py
+-rw-rw-r--   0 appuser  (32767)     8192      120 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/line_item.py
+-rw-rw-r--   0 appuser  (32767)     8192       77 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/report.py
+-rw-rw-r--   0 appuser  (32767)     8192      193 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/balance.py
+-rw-rw-r--   0 appuser  (32767)     8192      912 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/price_rule.py
+-rw-rw-r--   0 appuser  (32767)     8192      115 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/transaction.py
+-rw-rw-r--   0 appuser  (32767)     8192       78 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/tax_line.py
+-rw-rw-r--   0 appuser  (32767)     8192       84 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/note_attribute.py
+-rw-rw-r--   0 appuser  (32767)     8192     1597 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/product.py
+-rw-rw-r--   0 appuser  (32767)     8192      547 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/custom_collection.py
+-rw-rw-r--   0 appuser  (32767)     8192      108 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/customer_group.py
+-rw-rw-r--   0 appuser  (32767)     8192      126 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/discount_code.py
+-rw-rw-r--   0 appuser  (32767)     8192      199 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/collection_listing.py
+-rw-rw-r--   0 appuser  (32767)     8192       78 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/country.py
+-rw-rw-r--   0 appuser  (32767)     8192       78 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/address.py
+-rw-rw-r--   0 appuser  (32767)     8192      137 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/collection_publication.py
+-rw-rw-r--   0 appuser  (32767)     8192      150 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/access_scope.py
+-rw-rw-r--   0 appuser  (32767)     8192      158 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/order_risk.py
+-rw-rw-r--   0 appuser  (32767)     8192     1001 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/variant.py
+-rw-rw-r--   0 appuser  (32767)     8192     1423 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/image.py
+-rw-rw-r--   0 appuser  (32767)     8192       78 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/collect.py
+-rw-rw-r--   0 appuser  (32767)     8192     1066 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/graphql.py
+-rw-rw-r--   0 appuser  (32767)     8192       78 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/receipt.py
+-rw-rw-r--   0 appuser  (32767)     8192      193 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/gift_card_adjustment.py
+-rw-rw-r--   0 appuser  (32767)     8192      145 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/user.py
+-rw-rw-r--   0 appuser  (32767)     8192      157 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/payouts.py
+-rw-rw-r--   0 appuser  (32767)     8192      220 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/customer_saved_search.py
+-rw-rw-r--   0 appuser  (32767)     8192       83 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/shipping_line.py
+-rw-rw-r--   0 appuser  (32767)     8192      556 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/shop.py
+-rw-rw-r--   0 appuser  (32767)     8192     1040 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/fulfillment.py
+-rw-rw-r--   0 appuser  (32767)     8192       80 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/script_tag.py
+-rw-rw-r--   0 appuser  (32767)     8192       84 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/inventory_item.py
+-rw-rw-r--   0 appuser  (32767)     8192      236 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/smart_collection.py
+-rw-rw-r--   0 appuser  (32767)     8192       88 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/draft_order_invoice.py
+-rw-rw-r--   0 appuser  (32767)     8192       88 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/application_credit.py
+-rw-rw-r--   0 appuser  (32767)     8192      517 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/discount_code_creation.py
+-rw-rw-r--   0 appuser  (32767)     8192      306 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/fulfillment_service.py
+-rw-rw-r--   0 appuser  (32767)     8192      512 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/comment.py
+-rw-rw-r--   0 appuser  (32767)     8192      302 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/carrier_service.py
+-rw-rw-r--   0 appuser  (32767)     8192       79 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/checkout.py
+-rw-rw-r--   0 appuser  (32767)     8192     2613 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/asset.py
+-rw-rw-r--   0 appuser  (32767)     8192     2249 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/inventory_level.py
+-rw-rw-r--   0 appuser  (32767)     8192      929 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/order.py
+-rw-rw-r--   0 appuser  (32767)     8192       77 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/option.py
+-rw-rw-r--   0 appuser  (32767)     8192      153 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/policy.py
+-rw-rw-r--   0 appuser  (32767)     8192       85 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/customer_invite.py
+-rw-rw-r--   0 appuser  (32767)     8192      650 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/draft_order.py
+-rw-rw-r--   0 appuser  (32767)     8192      158 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/disputes.py
+-rw-rw-r--   0 appuser  (32767)     8192      295 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/webhook.py
+-rw-rw-r--   0 appuser  (32767)     8192      170 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/transactions.py
+-rw-rw-r--   0 appuser  (32767)     8192       86 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/shipping_address.py
+-rw-rw-r--   0 appuser  (32767)     8192       75 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/rule.py
+-rw-rw-r--   0 appuser  (32767)     8192      134 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/product_publication.py
+-rw-rw-r--   0 appuser  (32767)     8192      267 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/marketing_event.py
+-rw-rw-r--   0 appuser  (32767)     8192       79 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/currency.py
+-rw-rw-r--   0 appuser  (32767)     8192      383 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/resource_feedback.py
+-rw-rw-r--   0 appuser  (32767)     8192       88 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/tender_transaction.py
+-rw-rw-r--   0 appuser  (32767)     8192       85 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/billing_address.py
+-rw-rw-r--   0 appuser  (32767)     8192      123 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/province.py
+-rw-rw-r--   0 appuser  (32767)     8192      170 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/application_charge.py
+-rw-rw-r--   0 appuser  (32767)     8192      304 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/location.py
+-rw-rw-r--   0 appuser  (32767)     8192       85 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/payment_details.py
+-rw-rw-r--   0 appuser  (32767)     8192       82 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/publication.py
+-rw-rw-r--   0 appuser  (32767)     8192     1039 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/customer.py
+-rw-rw-r--   0 appuser  (32767)     8192       79 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/redirect.py
+-rw-rw-r--   0 appuser  (32767)     8192      664 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/article.py
+-rw-rw-r--   0 appuser  (32767)     8192       83 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/shipping_zone.py
+-rw-rw-r--   0 appuser  (32767)     8192     1038 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/resources/gift_card.py
+-rw-rw-r--   0 appuser  (32767)     8192     1611 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/limits.py
+-rw-rw-r--   0 appuser  (32767)     8192     2010 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/api_access.py
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/shopify/utils/
+-rw-rw-r--   0 appuser  (32767)     8192        0 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/utils/__init__.py
+-rw-rw-r--   0 appuser  (32767)     8192      699 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/utils/shop_url.py
+-rw-rw-r--   0 appuser  (32767)     8192     7625 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/base.py
+-rw-rw-r--   0 appuser  (32767)     8192     5364 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/collection.py
+-rw-rw-r--   0 appuser  (32767)     8192     6109 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/session.py
+-rw-rw-r--   0 appuser  (32767)     8192     1100 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/mixins.py
+-rw-rw-r--   0 appuser  (32767)     8192     2008 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/api_version.py
+-rw-rw-r--   0 appuser  (32767)     8192       18 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/version.py
+-rw-rw-r--   0 appuser  (32767)     8192     2107 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/shopify/session_token.py
+-rw-r--r--   0 appuser  (32767)     8192     1293 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/PKG-INFO
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/scripts/
+-rwxrwxr-x   0 appuser  (32767)     8192     9199 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/scripts/shopify_api.py
+drwxr-sr-x   0 appuser  (32767)     8192        0 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/bin/
+-rwxrwxr-x   0 appuser  (32767)     8192      416 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/bin/shopify_api.py
+-rw-r--r--   0 appuser  (32767)     8192       59 2021-10-18 18:41:55.000000 ShopifyAPI-9.0.0/setup.cfg
+-rw-rw-r--   0 appuser  (32767)     8192    10347 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/CHANGELOG
+-rw-rw-r--   0 appuser  (32767)     8192     9634 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/README.md
+-rwxrwxr-x   0 appuser  (32767)     8192     1769 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/setup.py
+-rw-rw-r--   0 appuser  (32767)     8192     1061 2021-10-15 15:54:07.000000 ShopifyAPI-9.0.0/LICENSE
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ShopifyAPI-8.4.2/CHANGELOG` & `ShopifyAPI-9.0.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 == Unreleased
 
+== Version 9.0.0
+
+- Drop Python 2 support ([#549](https://github.com/Shopify/shopify_python_api/pull/549))
+- Update API version with 2021-10 release, remove API version 2020-04 ([#548](https://github.com/Shopify/shopify_python_api/pull/548))
+
 == Version 8.4.2
 - Update API version with 2021-07 release, remove API version 2020-01 ([#521](https://github.com/Shopify/shopify_python_api/pull/521))
 
 == Version 8.4.1
 - Bug fix: `sanitize_shop_domain` now returns `None` rather than `'none.myshopify.com'` if no `shop_domain` arg is passed in ([#499](https://github.com/Shopify/shopify_python_api/pull/499))
 
 == Version 8.4.0
```

### Comparing `ShopifyAPI-8.4.2/LICENSE` & `ShopifyAPI-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/PKG-INFO` & `ShopifyAPI-9.0.0/ShopifyAPI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ShopifyAPI
-Version: 8.4.2
+Version: 9.0.0
 Summary: Shopify API for Python
 Home-page: https://github.com/Shopify/shopify_python_api
 Author: Shopify
 Author-email: developers@shopify.com
 License: MIT License
 Description: The ShopifyAPI library allows python developers to programmatically
         access the admin section of stores using an ActiveResource like
@@ -13,16 +13,14 @@
         resources (e.g. Order, Product, Collection).
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
```

### Comparing `ShopifyAPI-8.4.2/README.md` & `ShopifyAPI-9.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ### Table of Contents
 
 - [Getting Started](#getting-started)
   - [Public and Custom Apps](#public-and-custom-apps)
   - [Private Apps](#private-apps)
 - [Billing](#billing)
-- [Session Tokens](docs/session-tokens)
+- [Session Tokens](docs/session-tokens.md)
 - [Handling Access Scope Operations](docs/api-access.md)
 - [Advanced Usage](#advanced-usage)
 - [Prefix Options](#prefix-options)
 - [Console](#console)
 - [GraphQL](#graphql)
 - [Using Development Version](#using-development-version)
 - [Relative Cursor Pagination](#relative-cursor-pagination)
@@ -230,7 +230,10 @@
 * persistent connections
 
 ## Additional Resources
 * [Partners Dashboard](https://partners.shopify.com)
 * [developers.shopify.com](https://developers.shopify.com)
 * [Shopify.dev](https://shopify.dev)
 * [Ask questions on the Shopify forums](http://ecommerce.shopify.com/c/shopify-apis-and-technology)
+
+### Sample apps built using this library
+* [Sample Django app](https://github.com/shopify/sample-django-app)
```

### Comparing `ShopifyAPI-8.4.2/ShopifyAPI.egg-info/PKG-INFO` & `ShopifyAPI-9.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ShopifyAPI
-Version: 8.4.2
+Version: 9.0.0
 Summary: Shopify API for Python
 Home-page: https://github.com/Shopify/shopify_python_api
 Author: Shopify
 Author-email: developers@shopify.com
 License: MIT License
 Description: The ShopifyAPI library allows python developers to programmatically
         access the admin section of stores using an ActiveResource like
@@ -13,16 +13,14 @@
         resources (e.g. Order, Product, Collection).
 Platform: Any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
```

### Comparing `ShopifyAPI-8.4.2/ShopifyAPI.egg-info/SOURCES.txt` & `ShopifyAPI-9.0.0/ShopifyAPI.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 CHANGELOG
 LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.py
 ShopifyAPI.egg-info/PKG-INFO
 ShopifyAPI.egg-info/SOURCES.txt
 ShopifyAPI.egg-info/dependency_links.txt
 ShopifyAPI.egg-info/requires.txt
 ShopifyAPI.egg-info/top_level.txt
 bin/shopify_api.py
```

### Comparing `ShopifyAPI-8.4.2/scripts/shopify_api.py` & `ShopifyAPI-9.0.0/scripts/shopify_api.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/setup.py` & `ShopifyAPI-9.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,32 +19,29 @@
     author_email="developers@shopify.com",
     url="https://github.com/Shopify/shopify_python_api",
     packages=["shopify", "shopify/resources", "shopify/utils"],
     scripts=["scripts/shopify_api.py"],
     license="MIT License",
     install_requires=[
         "pyactiveresource>=2.2.2",
-        "PyJWT <= 1.7.1; python_version == '2.7'",
-        "PyJWT >= 2.0.0; python_version >= '3.6'",
+        "PyJWT >= 2.0.0",
         "PyYAML",
         "six",
     ],
     test_suite="test",
     tests_require=[
         "mock>=1.0.1",
     ],
     platforms="Any",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development",
```

### Comparing `ShopifyAPI-8.4.2/shopify/api_access.py` & `ShopifyAPI-9.0.0/shopify/api_access.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/api_version.py` & `ShopifyAPI-9.0.0/shopify/api_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     def define_version(cls, version):
         cls.versions[version.name] = version
         return version
 
     @classmethod
     def define_known_versions(cls):
         cls.define_version(Unstable())
-        cls.define_version(Release("2020-04"))
         cls.define_version(Release("2020-07"))
         cls.define_version(Release("2020-10"))
         cls.define_version(Release("2021-01"))
         cls.define_version(Release("2021-04"))
         cls.define_version(Release("2021-07"))
+        cls.define_version(Release("2021-10"))
 
     @classmethod
     def clear_defined_versions(cls):
         cls.versions = {}
 
     @property
     def numeric_version(self):
```

### Comparing `ShopifyAPI-8.4.2/shopify/base.py` & `ShopifyAPI-9.0.0/shopify/base.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/collection.py` & `ShopifyAPI-9.0.0/shopify/collection.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/limits.py` & `ShopifyAPI-9.0.0/shopify/limits.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/mixins.py` & `ShopifyAPI-9.0.0/shopify/mixins.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/__init__.py` & `ShopifyAPI-9.0.0/shopify/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/article.py` & `ShopifyAPI-9.0.0/shopify/resources/article.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/asset.py` & `ShopifyAPI-9.0.0/shopify/resources/asset.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/comment.py` & `ShopifyAPI-9.0.0/shopify/resources/comment.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/custom_collection.py` & `ShopifyAPI-9.0.0/shopify/resources/custom_collection.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/customer.py` & `ShopifyAPI-9.0.0/shopify/resources/customer.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/discount_code_creation.py` & `ShopifyAPI-9.0.0/shopify/resources/discount_code_creation.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/draft_order.py` & `ShopifyAPI-9.0.0/shopify/resources/draft_order.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/fulfillment.py` & `ShopifyAPI-9.0.0/shopify/resources/fulfillment.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/fulfillment_event.py` & `ShopifyAPI-9.0.0/shopify/resources/fulfillment_event.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/gift_card.py` & `ShopifyAPI-9.0.0/shopify/resources/gift_card.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/graphql.py` & `ShopifyAPI-9.0.0/shopify/resources/graphql.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/image.py` & `ShopifyAPI-9.0.0/shopify/resources/image.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/inventory_level.py` & `ShopifyAPI-9.0.0/shopify/resources/inventory_level.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/order.py` & `ShopifyAPI-9.0.0/shopify/resources/order.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/price_rule.py` & `ShopifyAPI-9.0.0/shopify/resources/price_rule.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/product.py` & `ShopifyAPI-9.0.0/shopify/resources/product.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/recurring_application_charge.py` & `ShopifyAPI-9.0.0/shopify/resources/recurring_application_charge.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/refund.py` & `ShopifyAPI-9.0.0/shopify/resources/refund.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/shop.py` & `ShopifyAPI-9.0.0/shopify/resources/shop.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/resources/variant.py` & `ShopifyAPI-9.0.0/shopify/resources/variant.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/session.py` & `ShopifyAPI-9.0.0/shopify/session.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/session_token.py` & `ShopifyAPI-9.0.0/shopify/session_token.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/utils/shop_url.py` & `ShopifyAPI-9.0.0/shopify/utils/shop_url.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/shopify/yamlobjects.py` & `ShopifyAPI-9.0.0/shopify/yamlobjects.py`

 * *Files identical despite different names*

### Comparing `ShopifyAPI-8.4.2/test/test_helper.py` & `ShopifyAPI-9.0.0/test/test_helper.py`

 * *Files identical despite different names*

