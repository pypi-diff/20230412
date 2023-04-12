# Comparing `tmp/django-thorbanks-0.6.2.tar.gz` & `tmp/django_thorbanks-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-thorbanks-0.6.2.tar", last modified: Thu Feb 18 20:40:32 2021, max compression
+gzip compressed data, was "django_thorbanks-0.6.3.tar", max compression
```

## Comparing `django-thorbanks-0.6.2.tar` & `django_thorbanks-0.6.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1495 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/LICENSE
--rw-r--r--   0        0        0     3843 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/README.md
--rw-r--r--   0        0        0     1403 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       54 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/__init__.py
--rw-r--r--   0        0        0     2656 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/abstract_models.py
--rw-r--r--   0        0        0      186 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/apps.py
--rw-r--r--   0        0        0     5894 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/checks.py
--rw-r--r--   0        0        0    11603 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/forms.py
--rw-r--r--   0        0        0      743 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/loading.py
--rw-r--r--   0        0        0     4279 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/settings.py
--rw-r--r--   0        0        0      448 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/signals.py
--rw-r--r--   0        0        0     3322 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/amex.png
--rw-r--r--   0        0        0     1091 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/danske.png
--rw-r--r--   0        0        0     1233 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/discover.png
--rw-r--r--   0        0        0     2061 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/lhv.png
--rw-r--r--   0        0        0     1991 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/mastercard.png
--rw-r--r--   0        0        0     2866 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/nordea.png
--rw-r--r--   0        0        0     2146 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/paypal.png
--rw-r--r--   0        0        0     1816 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/seb.png
--rw-r--r--   0        0        0     2943 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/swedbank.png
--rw-r--r--   0        0        0     5429 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/static/img/payment/visa.png
--rw-r--r--   0        0        0      221 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/templates/thorbanks/auth-request.html
--rw-r--r--   0        0        0      155 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/templates/thorbanks/input_option.html
--rw-r--r--   0        0        0      215 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/templates/thorbanks/payment-request.html
--rw-r--r--   0        0        0      249 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/templates/thorbanks/payment_widget.html
--rw-r--r--   0        0        0      564 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/templates/thorbanks/test_response.html
--rw-r--r--   0        0        0      163 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/urls.py
--rw-r--r--   0        0        0     5196 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/utils.py
--rw-r--r--   0        0        0     6448 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks/views.py
--rw-r--r--   0        0        0       67 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks_models/__init__.py
--rw-r--r--   0        0        0      153 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks_models/admin.py
--rw-r--r--   0        0        0      137 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks_models/apps.py
--rw-r--r--   0        0        0      190 2021-02-18 20:36:52.410930 django-thorbanks-0.6.2/thorbanks_models/models.py
--rw-r--r--   0        0        0     4752 2021-02-18 20:40:32.638574 django-thorbanks-0.6.2/setup.py
--rw-r--r--   0        0        0     4862 2021-02-18 20:40:32.639211 django-thorbanks-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1495 2020-02-05 17:33:39.761985 django_thorbanks-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3842 2023-04-12 14:52:23.475802 django_thorbanks-0.6.3/README.md
+-rw-r--r--   0        0        0     1395 2023-04-12 14:56:11.482488 django_thorbanks-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0       54 2020-02-05 17:33:39.925985 django_thorbanks-0.6.3/thorbanks/__init__.py
+-rw-r--r--   0        0        0     2656 2023-04-12 14:39:39.966493 django_thorbanks-0.6.3/thorbanks/abstract_models.py
+-rw-r--r--   0        0        0      186 2020-02-05 17:33:39.937985 django_thorbanks-0.6.3/thorbanks/apps.py
+-rw-r--r--   0        0        0     5894 2020-03-24 16:14:12.165255 django_thorbanks-0.6.3/thorbanks/checks.py
+-rw-r--r--   0        0        0    11601 2023-04-12 14:54:59.266795 django_thorbanks-0.6.3/thorbanks/forms.py
+-rw-r--r--   0        0        0      743 2021-02-18 16:58:58.284308 django_thorbanks-0.6.3/thorbanks/loading.py
+-rw-r--r--   0        0        0     4279 2021-02-18 16:58:58.284308 django_thorbanks-0.6.3/thorbanks/settings.py
+-rw-r--r--   0        0        0      809 2023-04-12 14:39:39.966493 django_thorbanks-0.6.3/thorbanks/signals.py
+-rw-r--r--   0        0        0     3322 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/amex.png
+-rw-r--r--   0        0        0     1091 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/danske.png
+-rw-r--r--   0        0        0     1233 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/discover.png
+-rw-r--r--   0        0        0     2061 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/lhv.png
+-rw-r--r--   0        0        0     1991 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/mastercard.png
+-rw-r--r--   0        0        0     2866 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/nordea.png
+-rw-r--r--   0        0        0     2146 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/paypal.png
+-rw-r--r--   0        0        0     1816 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/seb.png
+-rw-r--r--   0        0        0     2943 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/swedbank.png
+-rw-r--r--   0        0        0     5429 2015-10-29 10:41:27.665773 django_thorbanks-0.6.3/thorbanks/static/img/payment/visa.png
+-rw-r--r--   0        0        0      221 2020-01-28 15:23:48.153628 django_thorbanks-0.6.3/thorbanks/templates/thorbanks/auth-request.html
+-rw-r--r--   0        0        0      155 2020-01-29 14:27:15.625927 django_thorbanks-0.6.3/thorbanks/templates/thorbanks/input_option.html
+-rw-r--r--   0        0        0      215 2020-01-28 15:23:48.153628 django_thorbanks-0.6.3/thorbanks/templates/thorbanks/payment-request.html
+-rw-r--r--   0        0        0      249 2020-01-29 14:27:15.625927 django_thorbanks-0.6.3/thorbanks/templates/thorbanks/payment_widget.html
+-rw-r--r--   0        0        0      564 2015-10-29 10:41:27.685773 django_thorbanks-0.6.3/thorbanks/templates/thorbanks/test_response.html
+-rw-r--r--   0        0        0      372 2023-04-12 14:57:10.195030 django_thorbanks-0.6.3/thorbanks/urls.py
+-rw-r--r--   0        0        0     5196 2021-02-18 16:58:58.284308 django_thorbanks-0.6.3/thorbanks/utils.py
+-rw-r--r--   0        0        0     6448 2023-04-12 14:39:39.966493 django_thorbanks-0.6.3/thorbanks/views.py
+-rw-r--r--   0        0        0       67 2020-02-05 17:33:39.961985 django_thorbanks-0.6.3/thorbanks_models/__init__.py
+-rw-r--r--   0        0        0      153 2020-02-05 17:33:39.961985 django_thorbanks-0.6.3/thorbanks_models/admin.py
+-rw-r--r--   0        0        0      137 2020-02-05 17:33:39.961985 django_thorbanks-0.6.3/thorbanks_models/apps.py
+-rw-r--r--   0        0        0      190 2020-02-05 17:33:39.961985 django_thorbanks-0.6.3/thorbanks_models/models.py
+-rw-r--r--   0        0        0     4755 1970-01-01 00:00:00.000000 django_thorbanks-0.6.3/setup.py
+-rw-r--r--   0        0        0     4913 1970-01-01 00:00:00.000000 django_thorbanks-0.6.3/PKG-INFO
```

### Comparing `django-thorbanks-0.6.2/LICENSE` & `django_thorbanks-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/README.md` & `django_thorbanks-0.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -108,12 +108,12 @@
 
 ### 8. Create views and forms for payments:
 
 see [example.shop.views](example/shop/views.py) and [example.shop.forms](example/shop/forms.py).
 
 ## iPizza protocol
 
-- [Test service](https://banks.maximum.thorgate.eu/et/info)
+- [Test service](https://banks.pastel.thorgate.eu/et/info)
 - [Swedbank](https://www.swedbank.ee/business/cash/ecommerce/ecommerce?language=EST)
     - [Spec](https://www.swedbank.ee/static/pdf/business/d2d/paymentcollection/Pangalingi_paringute_tehniline_spetsifikatsioon_09_10_2014.pdf)
 - [SEB](https://www.seb.ee/ariklient/igapaevapangandus/maksete-kogumine/maksete-kogumine-internetis/pangalingi-tehniline)
 - [LHV Bank](https://www.lhv.ee/pangateenused/pangalink/)
```

### Comparing `django-thorbanks-0.6.2/pyproject.toml` & `django_thorbanks-0.6.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-thorbanks"
-version = "0.6.2"
+version = "0.6.3"
 description = "`django-thorbanks` provides a Django application for Estonian banklinks (iPizza protocol)."
 authors = ["Thorgate <info@thorgate.eu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "http://thorgate.eu"
 repository = "https://github.com/thorgate/django-thorbanks"
 classifiers = [
@@ -26,34 +26,34 @@
     "thorbanks/static/img/payment/*",
     "thorbanks/templates/thorbanks/*"
 ]
 exclude = ["**/migrations/*"]
 
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 Django = ">=1.11.27"
 cryptography = ">=2.*"
 
 [tool.poetry.dev-dependencies]
 pytest = "==6.*"
 coverage = "==5.*"
 coveralls = "==3.*"
 pytest-cov = "==2.*"
 pytest-django = "==4.*"
 pytest-timeout = "==1.*"
 mock = ">=1.0.1"
 tox = "==3.*"
 pytest-selenium = "==2.*"
 selenium = "==3.*"
-black = "==20.8b1"
+black = "==23.3.0"
 isort = "*"
 prospector = "==1.3.*"
 
 
 [tool.black]
-target-version = ["py36", "py37", "py38"]
+target-version = ["py37", "py38"]
 include = "\\.pyi?$"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `django-thorbanks-0.6.2/thorbanks/abstract_models.py` & `django_thorbanks-0.6.3/thorbanks/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/checks.py` & `django_thorbanks-0.6.3/thorbanks/checks.py`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/forms.py` & `django_thorbanks-0.6.3/thorbanks/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def prepare(self, bank_name, redirect_to, response_url, *args, **kwargs):
         raise NotImplementedError  # pragma no cover
 
     def finalize(self):
         raise NotImplementedError  # pragma no cover
 
     def redirect_html(self):
-        """ Redirection html """
+        """Redirection html"""
         html = (
             '<form action="%s" method="POST" id="banklink_redirect_url" accept-charset="%s">'
             % (self.get_request_url(), self.get_encoding())
         )
 
         for field in self:
             html += force_str(field) + "\n"
```

### Comparing `django-thorbanks-0.6.2/thorbanks/loading.py` & `django_thorbanks-0.6.3/thorbanks/loading.py`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/settings.py` & `django_thorbanks-0.6.3/thorbanks/settings.py`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/amex.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/amex.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/danske.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/danske.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/discover.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/discover.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/lhv.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/lhv.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/mastercard.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/mastercard.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/nordea.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/nordea.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/paypal.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/paypal.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/seb.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/seb.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/swedbank.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/swedbank.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/static/img/payment/visa.png` & `django_thorbanks-0.6.3/thorbanks/static/img/payment/visa.png`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/templates/thorbanks/test_response.html` & `django_thorbanks-0.6.3/thorbanks/templates/thorbanks/test_response.html`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/utils.py` & `django_thorbanks-0.6.3/thorbanks/utils.py`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/thorbanks/views.py` & `django_thorbanks-0.6.3/thorbanks/views.py`

 * *Files identical despite different names*

### Comparing `django-thorbanks-0.6.2/setup.py` & `django_thorbanks-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*'], 'thorbanks': ['static/img/payment/*', 'templates/thorbanks/*']}
 
 install_requires = \
 ['Django>=1.11.27', 'cryptography>=2']
 
 setup_kwargs = {
     'name': 'django-thorbanks',
-    'version': '0.6.2',
+    'version': '0.6.3',
     'description': '`django-thorbanks` provides a Django application for Estonian banklinks (iPizza protocol).',
-    'long_description': '# django-thorbanks\n\n[![Build Status](https://travis-ci.org/thorgate/django-thorbanks.svg?branch=master)](https://travis-ci.org/thorgate/django-thorbanks)\n[![Coverage Status](https://coveralls.io/repos/github/thorgate/django-thorbanks/badge.svg?branch=master)](https://coveralls.io/github/thorgate/django-thorbanks?branch=master)\n[![PyPI release](https://badge.fury.io/py/django-thorbanks.png)](https://badge.fury.io/py/django-thorbanks)\n\n\nDjango app for integrating Estonian banklinks into your project.\n\n## Features\n\nBank            | Protocol    | Authentication      | Payment\n--------------- | ----------- | ------------------- | -------\nSwedbank        | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nSEB             | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nDanske          | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nLHV             | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nKrediidipank    | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nNordea          | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\n\n## Usage\n\n### 1. Install it:\n\n**Pip:**\n\n```bash\npip install django-thorbanks\n```\n\n**Pipenv:**\n\n```bash\npipenv install django-thorbanks\n```\n\n**Poetry:**\n\n```bash\npoetry add django-thorbanks\n```\n\n### 2. Add to installed apps\n\n```python\nINSTALLED_APPS = (\n    # Add the following apps:\n    "thorbanks",\n    "thorbanks_models",\n)\n```\n\n### 3. Configure and create migrations:\n\n**With MANUAL_MODELS:**\n\n- Remove `"thorbanks_models"` from `INSTALLED_APPS`\n- follow instructions from [thorbanks.settings.get_model](./thorbanks/settings.py#L59).\n\n**With default models:**\n\nMake django aware that thorbanks migrations are in your local apps folder via settings.MIGRATION_MODULES:\n\n> Note: Replace `shop` with the name of an existing app in your project.\n\n```python\n# Tell django that thorbanks_models migrations are in shop app (in thorbanks_migrations module)\nMIGRATION_MODULES = {"thorbanks_models": "shop.thorbanks_migrations"}\n```\n\nNow run `makemigrations thorbanks_models` and `migrate` management commands to create and apply the migrations.\n\n### 4. Add settings.BANKLINKS\n\nFor a working example see the definitions in [example/settings.py](example/settings.py).\n\n> Note:\n>You will need a public and private key for each bank integration.\n>In case you don\'t have the public key, you can generate one out of a certificate by:\n>```\n>openssl x509 -pubkey -noout -in cert.pem  > pubkey.pem\n>```\n\n### 5. Link Transaction to your Order model\n\n> Note: When using MANUAL_MODELS replace `thorbanks_models` with your local app name\n\n```python\nclass Order(models.Model):\n    # ... other fields\n    transaction = models.OneToOneField(\n        "thorbanks_models.Transaction", null=True, on_delete=models.SET_NULL\n    )\n```\n\n### 6. Include thorbanks urls\n\n```python\nurlpatterns = [\n    # This is where the user will be redirected after returning from the banklink page\n    url(r"^banks/", include("thorbanks.urls")),\n]\n```\n\n### 7. Add listeners to banklinks success & failure callbacks:\n\nSee [example.shop.models.banklink_success_callback](example/shop/models.py#L23) and [example.shop.models.banklink_failed_callback](example/shop/models.py#L44).\n\n### 8. Create views and forms for payments:\n\nsee [example.shop.views](example/shop/views.py) and [example.shop.forms](example/shop/forms.py).\n\n## iPizza protocol\n\n- [Test service](https://banks.maximum.thorgate.eu/et/info)\n- [Swedbank](https://www.swedbank.ee/business/cash/ecommerce/ecommerce?language=EST)\n    - [Spec](https://www.swedbank.ee/static/pdf/business/d2d/paymentcollection/Pangalingi_paringute_tehniline_spetsifikatsioon_09_10_2014.pdf)\n- [SEB](https://www.seb.ee/ariklient/igapaevapangandus/maksete-kogumine/maksete-kogumine-internetis/pangalingi-tehniline)\n- [LHV Bank](https://www.lhv.ee/pangateenused/pangalink/)\n',
+    'long_description': '# django-thorbanks\n\n[![Build Status](https://travis-ci.org/thorgate/django-thorbanks.svg?branch=master)](https://travis-ci.org/thorgate/django-thorbanks)\n[![Coverage Status](https://coveralls.io/repos/github/thorgate/django-thorbanks/badge.svg?branch=master)](https://coveralls.io/github/thorgate/django-thorbanks?branch=master)\n[![PyPI release](https://badge.fury.io/py/django-thorbanks.png)](https://badge.fury.io/py/django-thorbanks)\n\n\nDjango app for integrating Estonian banklinks into your project.\n\n## Features\n\nBank            | Protocol    | Authentication      | Payment\n--------------- | ----------- | ------------------- | -------\nSwedbank        | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nSEB             | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nDanske          | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nLHV             | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nKrediidipank    | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\nNordea          | iPizza      | :heavy_check_mark:  | :heavy_check_mark:\n\n## Usage\n\n### 1. Install it:\n\n**Pip:**\n\n```bash\npip install django-thorbanks\n```\n\n**Pipenv:**\n\n```bash\npipenv install django-thorbanks\n```\n\n**Poetry:**\n\n```bash\npoetry add django-thorbanks\n```\n\n### 2. Add to installed apps\n\n```python\nINSTALLED_APPS = (\n    # Add the following apps:\n    "thorbanks",\n    "thorbanks_models",\n)\n```\n\n### 3. Configure and create migrations:\n\n**With MANUAL_MODELS:**\n\n- Remove `"thorbanks_models"` from `INSTALLED_APPS`\n- follow instructions from [thorbanks.settings.get_model](./thorbanks/settings.py#L59).\n\n**With default models:**\n\nMake django aware that thorbanks migrations are in your local apps folder via settings.MIGRATION_MODULES:\n\n> Note: Replace `shop` with the name of an existing app in your project.\n\n```python\n# Tell django that thorbanks_models migrations are in shop app (in thorbanks_migrations module)\nMIGRATION_MODULES = {"thorbanks_models": "shop.thorbanks_migrations"}\n```\n\nNow run `makemigrations thorbanks_models` and `migrate` management commands to create and apply the migrations.\n\n### 4. Add settings.BANKLINKS\n\nFor a working example see the definitions in [example/settings.py](example/settings.py).\n\n> Note:\n>You will need a public and private key for each bank integration.\n>In case you don\'t have the public key, you can generate one out of a certificate by:\n>```\n>openssl x509 -pubkey -noout -in cert.pem  > pubkey.pem\n>```\n\n### 5. Link Transaction to your Order model\n\n> Note: When using MANUAL_MODELS replace `thorbanks_models` with your local app name\n\n```python\nclass Order(models.Model):\n    # ... other fields\n    transaction = models.OneToOneField(\n        "thorbanks_models.Transaction", null=True, on_delete=models.SET_NULL\n    )\n```\n\n### 6. Include thorbanks urls\n\n```python\nurlpatterns = [\n    # This is where the user will be redirected after returning from the banklink page\n    url(r"^banks/", include("thorbanks.urls")),\n]\n```\n\n### 7. Add listeners to banklinks success & failure callbacks:\n\nSee [example.shop.models.banklink_success_callback](example/shop/models.py#L23) and [example.shop.models.banklink_failed_callback](example/shop/models.py#L44).\n\n### 8. Create views and forms for payments:\n\nsee [example.shop.views](example/shop/views.py) and [example.shop.forms](example/shop/forms.py).\n\n## iPizza protocol\n\n- [Test service](https://banks.pastel.thorgate.eu/et/info)\n- [Swedbank](https://www.swedbank.ee/business/cash/ecommerce/ecommerce?language=EST)\n    - [Spec](https://www.swedbank.ee/static/pdf/business/d2d/paymentcollection/Pangalingi_paringute_tehniline_spetsifikatsioon_09_10_2014.pdf)\n- [SEB](https://www.seb.ee/ariklient/igapaevapangandus/maksete-kogumine/maksete-kogumine-internetis/pangalingi-tehniline)\n- [LHV Bank](https://www.lhv.ee/pangateenused/pangalink/)\n',
     'author': 'Thorgate',
     'author_email': 'info@thorgate.eu',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'http://thorgate.eu',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django-thorbanks-0.6.2/PKG-INFO` & `django_thorbanks-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: django-thorbanks
-Version: 0.6.2
+Version: 0.6.3
 Summary: `django-thorbanks` provides a Django application for Estonian banklinks (iPizza protocol).
 Home-page: http://thorgate.eu
 License: BSD-3-Clause
 Author: Thorgate
 Author-email: info@thorgate.eu
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=1.11.27)
 Requires-Dist: cryptography (>=2)
 Project-URL: Repository, https://github.com/thorgate/django-thorbanks
 Description-Content-Type: text/markdown
 
 # django-thorbanks
 
@@ -134,13 +135,13 @@
 
 ### 8. Create views and forms for payments:
 
 see [example.shop.views](example/shop/views.py) and [example.shop.forms](example/shop/forms.py).
 
 ## iPizza protocol
 
-- [Test service](https://banks.maximum.thorgate.eu/et/info)
+- [Test service](https://banks.pastel.thorgate.eu/et/info)
 - [Swedbank](https://www.swedbank.ee/business/cash/ecommerce/ecommerce?language=EST)
     - [Spec](https://www.swedbank.ee/static/pdf/business/d2d/paymentcollection/Pangalingi_paringute_tehniline_spetsifikatsioon_09_10_2014.pdf)
 - [SEB](https://www.seb.ee/ariklient/igapaevapangandus/maksete-kogumine/maksete-kogumine-internetis/pangalingi-tehniline)
 - [LHV Bank](https://www.lhv.ee/pangateenused/pangalink/)
```

