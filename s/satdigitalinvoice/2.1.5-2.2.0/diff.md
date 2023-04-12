# Comparing `tmp/satdigitalinvoice-2.1.5.tar.gz` & `tmp/satdigitalinvoice-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.1.5.tar", last modified: Mon Apr 10 16:52:37 2023, max compression
+gzip compressed data, was "satdigitalinvoice-2.2.0.tar", last modified: Wed Apr 12 02:20:04 2023, max compression
```

## Comparing `satdigitalinvoice-2.1.5.tar` & `satdigitalinvoice-2.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.804879 satdigitalinvoice-2.1.5/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    31211 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 16:52:37.000000 satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:52:37.808879 satdigitalinvoice-2.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-10 16:52:26.000000 satdigitalinvoice-2.1.5/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.187590 satdigitalinvoice-2.2.0/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31866 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.187590 satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.187590 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.1.5/PKG-INFO` & `satdigitalinvoice-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.5
+Version: 2.2.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/__init__.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import logging
 import os
 
 import PySimpleGUI as sg
 
 SOURCE_DIRECTORY = os.path.dirname(__file__)
 DATA_DIRECTORY = ".data"
+ARCHIVOS_DIRECTORY = "archivos"
+TEMPLATES_DIRECTORY = "templates"
+
 PPD = "PPD"
 PUE = "PUE"
 
 
 def add_file_handler():
     os.makedirs(DATA_DIRECTORY, exist_ok=True)
     fh = logging.FileHandler(
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/__version__.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/environments.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/environments.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import jinja2
 from jinja2 import Environment, Undefined
 from jinja2.filters import do_mark_safe
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import iterate as h_iterate
 
+from satdigitalinvoice import TEMPLATES_DIRECTORY
+
 
 class FacturacionEnvironment(Environment):
     @property
     def filter(self):
         def sub(f):
             self.filters[f.__name__] = f
             return f
@@ -23,15 +25,15 @@
             self.globals[f.__name__] = f
             return f
 
         return sub
 
     def __init__(self):
         super().__init__(
-            loader=jinja2.FileSystemLoader(searchpath=['templates']),
+            loader=jinja2.FileSystemLoader(searchpath=[TEMPLATES_DIRECTORY]),
             autoescape=True,
             trim_blocks=True,
             lstrip_blocks=True,
             undefined=jinja2.StrictUndefined,
         )
 
         @self.glob
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/facturacion.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 from satcfdi.transform.catalog import CATALOGS
 from tabulate import tabulate
 
 from . import __version__, PPD, PUE
 from .client_validation import validar_client
 from .file_data_managers import ClientsManager, FacturasManager
 from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, facturas_filename, \
-    periodo_desc, generate_html_template, mf_pago_fmt, print_invoices, print_cfdis, print_cfdi_details, ajustes, ajustes_directory
+    generate_html_template, mf_pago_fmt, print_invoices, print_cfdis, print_cfdi_details, ajustes, facturas_folder, year_month_desc
 from .layout import make_layout, ActionButtonManager
 from .localdb import LocalDBSatCFDI, LiquidatedState
 from .log_tools import log_line, log_item, cfdi_header, header_line, print_yaml
 from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder
-from .utils import random_string, to_uuid, parse_date_period, parse_ym_date, load_certificate, to_int, cert_info
+from .utils import random_string, to_uuid, parse_date_period, load_certificate, to_int, cert_info, parse_rango
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
@@ -93,16 +93,15 @@
         self.set_folio()
         self.window['serie'].update(self.serie)
 
         self.window['factura_pagar'].bind("<Return>", "_enter")
         self.window['periodo'].bind("<Return>", "_enter")
         self.window['importe_pago'].bind("<Return>", "_enter")
         self.window['fecha_pago'].bind("<Return>", "_enter")
-        self.window['inicio'].bind("<Return>", "_enter")
-        self.window['final'].bind("<Return>", "_enter")
+        self.window['rango'].bind("<Return>", "_enter")
         self.window['forma_pago'].bind("<Return>", "_enter")
         # self.window['console'].bind('<Button-3>', '_double_click')
 
         # Add logging to the window
         h = logging.StreamHandler(self.window['console'])
         h.setLevel(logging.INFO)
         logging.root.addHandler(h)
@@ -286,19 +285,23 @@
 
         # PPD
         is_ppd_active = i \
                         and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                         and i.get("MetodoPago") == PPD \
                         and i.estatus == "1" \
                         and i.saldo_pendiente
-        self.window["prepare_pago"].update(disabled=not is_ppd_active)
-        self.window["fecha_pago_select"].update(disabled=not is_ppd_active)
-        self.window["fecha_pago"].update(disabled=not is_ppd_active)
-        self.window["importe_pago"].update(disabled=not is_ppd_active)
-        self.window["forma_pago"].update(disabled=not is_ppd_active)
+        is_ppd_active = bool(is_ppd_active)
+        self.window["fecha_pago_select"].update(visible=is_ppd_active)
+        self.window["fecha_pago"].update(visible=is_ppd_active)
+        self.window["forma_pago_text"].update(visible=is_ppd_active)
+        self.window["forma_pago"].update(visible=is_ppd_active)
+
+        self.window["prepare_pago"].update(visible=is_ppd_active)
+        self.window["imp_pagado_text"].update(visible=is_ppd_active)
+        self.window["importe_pago"].update(visible=is_ppd_active)
 
     def print_satcfdis(self, cfdis):
         def info_fmt(i):
             return "" if self.local_db.notified(i) else "📧"
 
         if cfdis := sorted(cfdis, key=lambda i: (i["Fecha"], i.name), reverse=True):
             if self.window['detallado'].get():
@@ -349,22 +352,24 @@
         if clear:
             self.console.update("")
         log_line(name)
 
     def main_loop(self):
         while True:
             event, values = self.window.read()
+            dp = parse_date_period(values["periodo"])
+
             try:
                 if event in ("Exit", PySimpleGUI.WIN_CLOSED):
                     return
 
                 action_name, action_items = self.action_button_manager.clear()
 
                 if event in ("prepare_correos", "prepare_clientes", "prepare_facturas", "crear_facturas",
-                             "inicio_enter", "final_enter", "preparar_ajuste_anual", "recuperar_emitidas", "recuperar_recibidas"):
+                             "rango_enter", "preparar_ajuste_anual", "recuperar_emitidas", "recuperar_recibidas"):
                     self.set_selected_satcfdi([])
 
                 match event:
                     case "folio":
                         self.set_folio(to_int(values["folio"]))
 
                     case "about":
@@ -393,15 +398,15 @@
                             self.print_satcfdis(fac_iter())
                             self.window["descarga"].update(disabled=not search_uuid)
 
                     case "preparar_ajuste_anual":
                         self.header(f"AJUSTES")
                         ajustes(
                             emisor_rfc=self.csd_signer.rfc,
-                            ym_date=parse_ym_date(values['periodo'])
+                            dp=dp
                         )
 
                     case "recuperar_emitidas" | "recuperar_recibidas":
                         self.header("RECUPERAR")
                         fecha_final = date.today()
                         fecha_inicial = fecha_final - timedelta(days=int(values["recuperar_dias"]))
                         id_solicitud = self.local_db.get(event)
@@ -430,17 +435,16 @@
                                         self.unzip_cfdi(b)
                                 del self.local_db[event]
                             print("FIN")
 
                     case "prepare_clientes":
                         self.header("CLIENTES")
                         clients = ClientsManager()
-                        ym_date = parse_ym_date(values['periodo'])
                         if clients:
-                            facturas = FacturasManager(ym_date)["Facturas"]
+                            facturas = FacturasManager(dp)["Facturas"]
                             print(
                                 tabulate(
                                     [
                                         [
                                             i,
                                             client["RazonSocial"][:36],
                                             client["Rfc"],
@@ -463,29 +467,28 @@
                                     colalign=("right", "left", "left", "left", "left", "right"),
                                 )
                             )
                             self.action_button_manager.set_items(ACTION_CLIENTS, clients)
                         else:
                             print("No hay clientes")
 
-                    case "prepare_facturas" | "inicio_enter" | "final_enter":
-                        ym_date = parse_ym_date(values["periodo"])
+                    case "prepare_facturas" | "rango_enter":
                         self.header(f"PREPARAR FACTURAS {values['periodo']}")
-                        print('Periodo:', periodo_desc(ym_date, 'Mensual.1'), '[AL ...]')
-                        inicio = int(values["inicio"])
+                        print('Periodo:', year_month_desc(dp), '[AL ...]')
+                        inicio, final = parse_rango(values["rango"])
 
                         if cfdis := generate_ingresos(
-                            folio=int(values["folio"]),
-                            serie=self.serie,
-                            clients=ClientsManager(),
-                            facturas=FacturasManager(ym_date)["Facturas"],
-                            ym_date=ym_date,
-                            csd_signer=self.csd_signer
+                                folio=int(values["folio"]),
+                                serie=self.serie,
+                                clients=ClientsManager(),
+                                facturas=FacturasManager(dp)["Facturas"],
+                                dp=dp,
+                                csd_signer=self.csd_signer
                         ):
-                            final = to_int(values["final"]) or len(cfdis)
+                            final = final or len(cfdis)
                             cfdis = cfdis[max(inicio - 1, 0):max(final, 0)]
 
                         self.print_prepared_cfdis(cfdis, start=inicio)
 
                     case "prepare_pago" | "importe_pago_enter" | "fecha_pago_enter" | "forma_pago_enter":
                         self.header("COMPROBANTE PAGO")
                         if i := self.selected_satcfdi:
@@ -532,38 +535,38 @@
                             self.header(self.window[event].ButtonText.upper())
                             self.print_satcfdis([i])
                             print(f"FACTURA MARCADA COMO {'' if st else '-NO- '}NOTIFICADA")
 
                     case "prepare_correos":
                         self.header("CORREOS")
                         now = date.today()
-                        dp = DatePeriod(now.year, now.month)
+                        dp_now = DatePeriod(now.year, now.month)
                         clients = ClientsManager()
                         a_invoices = self.get_all_invoices()
 
                         cfdi_correos = []
                         for receptor_rfc, notify_invoices in itertools.groupby(
                                 sorted(
                                     (i for i in a_invoices.values() if i.estatus == "1" and not self.local_db.notified(i)),
                                     key=lambda r: r["Receptor"]["Rfc"]
                                 ),
                                 lambda r: r["Receptor"]["Rfc"]
                         ):
                             notify_invoices = list(notify_invoices)
 
-                            def fac_iter():
+                            def fac_pen_iter():
                                 for i in self.get_all_invoices().values():
                                     if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                                             and self.local_db.liquidated_state(i) == LiquidatedState.NO \
-                                            and i["Fecha"] < dp \
+                                            and i["Fecha"] < dp_now \
                                             and i["Receptor"]["Rfc"] == receptor_rfc:
                                         yield i
 
                             fac_pen = sorted(
-                                fac_iter(),
+                                fac_pen_iter(),
                                 key=lambda r: r["Fecha"]
                             )
                             receptor = clients[receptor_rfc]
                             cfdi_correos.append((receptor, notify_invoices, fac_pen))
 
                         if cfdi_correos:
                             print(tabulate(
@@ -624,72 +627,87 @@
                             self.all_invoices = None
                             cfdi = move_to_folder(res.xml, pdf_data=res.pdf)
                             cfdi = self.get_all_invoices()[to_uuid(cfdi["Complemento"]["TimbreFiscalDigital"]["UUID"])]
                             self.print_satcfdis([cfdi])
                         except DocumentNotFoundError:
                             logger.info("Factura no encontrada")
 
-                    case "ver_excel":
-                        self.header("EXCEL")
-                        clients = ClientsManager()
-                        emisor_cif = clients[self.csd_signer.rfc]
-                        exportar_facturas(
-                            self.get_all_invoices(),
-                            parse_date_period(values["periodo"]),
-                            emisor_cif,
-                            self.rfc_prediales
-                        )
-
-                        archivo_excel = facturas_filename(parse_date_period(values["periodo"]))
-                        os.startfile(
-                            os.path.abspath(archivo_excel)
-                        )
-
                     case "facturas_emitidas" | "periodo_enter":
                         self.header(f"FACTURAS EMITIDAS {values['periodo']}")
-                        dp = parse_date_period(values["periodo"])
 
                         def fact_iter():
                             for i in self.get_all_invoices().values():
                                 if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                                         and i["Fecha"] == dp:
                                     yield i
 
                         self.print_satcfdis(fact_iter())
 
+                    case "ver_excel":
+                        self.header("EXCEL")
+                        clients = ClientsManager()
+                        emisor_cif = clients[self.csd_signer.rfc]
+                        if archivo_excel := exportar_facturas(
+                                self.get_all_invoices(),
+                                dp,
+                                emisor_cif,
+                                self.rfc_prediales
+                        ):
+                            print("Archivo generado: " + archivo_excel)
+                            os.startfile(
+                                os.path.abspath(archivo_excel)
+                            )
+                        else:
+                            print("No se pudo crear el archivo, cierra el archivo si se tiene abierto")
+
                     case "ver_html":
                         self.header("HTML")
-                        dp = parse_date_period(values["periodo"])
 
                         def fact_iter():
                             for i in self.get_all_invoices().values():
                                 if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                                         and i["Fecha"] == dp:
                                     yield i
 
-                        outfile = facturas_filename(dp, ext="html")
-                        Representable.html_write_all(
-                            objs=fact_iter(),
-                            target=outfile,
-                        )
-                        os.startfile(
-                            os.path.abspath(outfile)
-                        )
+                        if cfdis := list(fact_iter()):
+                            outfile = facturas_filename(dp, ext="html")
+                            Representable.html_write_all(
+                                objs=cfdis,
+                                target=outfile,
+                            )
+                            print("Archivo generado: " + outfile)
+                            os.startfile(
+                                os.path.abspath(outfile)
+                            )
+                        else:
+                            print("No hay facturas para periodo seleccionado")
 
                     case "ver_carpeta":
-                        archivo = facturas_filename(parse_date_period(values["periodo"]))
+                        directory = facturas_folder(dp)
                         os.startfile(
-                            os.path.abspath(os.path.dirname(archivo))
+                            os.path.abspath(directory)
                         )
 
-                    case "ver_carpeta_ajustes":
-                        ajustes_dir = ajustes_directory(parse_ym_date(values['periodo']))
-                        os.startfile(
-                            os.path.abspath(ajustes_dir)
-                        )
+                    case "sat_status_todas":
+                        self.console.update(autoscroll=True)
+                        self.header("SAT STATUS")
+
+                        def fact_iter():
+                            for i in self.get_all_invoices().values():
+                                if i["Fecha"] == dp:
+                                    yield i
+
+                        for cfdi in fact_iter():
+                            print(f"Estado SAT: {cfdi.name} - {cfdi.uuid}")
+                            self._read()
+                            estado = self.local_db.status_sat(cfdi, update=True)
+                            print_yaml(estado)
+
+                        print("FIN")
+                        self.console.update(autoscroll=False)
 
                     case "periodo" | "inicio" | "final" | "fecha_pago" | "forma_pago" | "importe_pago" | ' ':
                         pass
 
                     case _:
                         logger.error(f"Unknown event '{event}'")
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/file_data_managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 from datetime import date
 from decimal import Decimal
 
 import jsonschema as jsonschema
 import yaml
-from satcfdi import Code
+from satcfdi import Code, DatePeriod
 from satcfdi.pacs import sat
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import Xint
 from yaml import MappingNode, SafeLoader
 from yaml.constructor import ConstructorError
 
@@ -94,30 +94,30 @@
             self[k]["Rfc"] = k
             self[k]["RegimenFiscal"] = Code(self[k]["RegimenFiscal"], REGIMEN_FISCAL.get(self[k]["RegimenFiscal"]))
 
 
 class FacturasManager(LocalData):
     file_source = "facturas.yaml"
 
-    def __init__(self, emission_date: date | None):
+    def __init__(self, dp: DatePeriod | None):
         def loading_function(loader, node):
             cases = loader.construct_mapping(node, deep=True)
-            if emission_date is None:
+            if dp is None:
                 return cases
             return find_best_match(
                 cases,
-                emission_date
+                dp
             )[1]
 
         DuplicateKeySafeLoader.add_constructor("!case", loading_function)
         super().__init__()
         if dup := first_duplicate(json.dumps(x, sort_keys=True, default=str) for x in self["Facturas"]):
             raise ValueError("Factura Duplicada: {}".format(dup))
 
-        if emission_date:
+        if dp:
             for v in self["Facturas"]:
                 if error := jsonschema.exceptions.best_match(factura_validator.iter_errors(v)):
                     raise error
 
 
 DuplicateKeySafeLoader.add_constructor("!decimal", lambda loader, node: Decimal(loader.construct_scalar(node)))
 DuplicateKeySafeLoader.add_constructor("!read", lambda loader, node: open(loader.construct_scalar(node), 'rb').read())
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/gui_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from decimal import Decimal
 
 import xlsxwriter
 from babel.dates import format_date
 from markdown2 import markdown
 from satcfdi import DatePeriod
 from satcfdi.accounting import filter_invoices_iter, filter_payments_iter, invoices_export, payments_export, SatCFDI
+from satcfdi.accounting.process import payments_groupby_receptor, payments_retentions_export
 from satcfdi.create.cfd import cfdi40
 from satcfdi.create.cfd.cfdi40 import Comprobante, PagoComprobante
 from satcfdi.pacs import sat
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from tabulate import tabulate
 from weasyprint import HTML, CSS
 from xlsxwriter.exceptions import FileCreateError
 
-from . import SOURCE_DIRECTORY, PPD
+from . import SOURCE_DIRECTORY, PPD, ARCHIVOS_DIRECTORY
 from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
 from .formatting_functions.common import fecha, pesos, porcentaje
 from .log_tools import print_yaml
 from .utils import clear_directory, find_best_match, months_between, add_month
 
 logger = logging.getLogger(__name__)
@@ -121,43 +122,48 @@
         if factura_details["MetodoPago"] == "PPD" and factura_details["FormaPago"] != "99":
             logger.info(f"{factura_details['Receptor']}: FormaPago '{factura_details['FormaPago']}' is invalid, expected '99' for PPD")
             is_valid = False
 
     return is_valid
 
 
-def year_month_desc(year, month):
-    return format_date(date(year=year, month=month, day=1), locale='es_MX', format="'Mes de' MMMM 'del' y").upper()
+def year_month_desc(dp: DatePeriod):
+    return format_date(date(year=dp.year, month=dp.month, day=1), locale='es_MX', format="'Mes de' MMMM 'del' y").upper()
 
 
-def periodo_desc(ym_date, periodo_mes_ajuste):
+def periodo_desc(dp: DatePeriod, periodo_mes_ajuste, offset):
     periodo, mes_ajuste = parse_periodo_mes_ajuste(periodo_mes_ajuste)
     periodo_meses = PERIODOS[periodo]
 
-    if (ym_date.month - mes_ajuste) % periodo_meses == 0:
-        periodo = year_month_desc(ym_date.year, ym_date.month)
+    if (dp.month - mes_ajuste) % periodo_meses == 0:
+        if offset:
+            dp = add_month(dp, offset)
+
+        periodo = year_month_desc(dp)
         if periodo_meses > 1:
-            mes_final = (ym_date.month + periodo_meses - 2) % 12 + 1
             periodo += " AL " + year_month_desc(
-                year=ym_date.year + int(mes_final < ym_date.month),
-                month=mes_final
+                dp=add_month(dp, periodo_meses - 1)
             )
 
         return periodo
     return None
 
 
-def generate_ingresos(folio, serie, clients, facturas, ym_date, csd_signer):
+def generate_ingresos(folio, serie, clients, facturas, dp, csd_signer):
     if not validad_facturas(clients, facturas):
         return
 
     emisor_cif = clients[csd_signer.rfc]
 
     def prepare_concepto(concepto):
-        periodo = periodo_desc(ym_date, concepto['_periodo_mes_ajuste'])
+        periodo = periodo_desc(
+            dp,
+            concepto['_periodo_mes_ajuste'],
+            concepto.get('_desfase_mes')
+        )
         if periodo and concepto['ValorUnitario'] is not None:
             return format_concepto_desc(concepto, periodo=periodo)
 
     def facturas_iter():
         i = 0
         for f in facturas:
             receptor_cif = clients[f['Receptor']]
@@ -233,28 +239,29 @@
             _, mes_aj = parse_periodo_mes_ajuste(concepto['_periodo_mes_ajuste'])
             if mes_aj == mes_ajuste:
                 yield rfc, concepto
 
 
 def facturas_folder(dp: DatePeriod):
     if dp.month:
-        return f"facturas/{dp.year}/{dp}"
-    return f"facturas/{dp.year}/{dp}"
+        return os.path.join(ARCHIVOS_DIRECTORY, str(dp.year), str(dp.year) + "-{:02d}".format(dp.month))
+    return os.path.join(ARCHIVOS_DIRECTORY, str(dp.year))
 
 
 def facturas_filename(dp: DatePeriod, ext="xlsx"):
     return os.path.join(facturas_folder(dp), f"{dp}.{ext}")
 
 
 def exportar_facturas(all_invoices, dp: DatePeriod, emisor_cif, rfc_prediales):
     emisor_rfc = emisor_cif['Rfc']
     emisor_regimen = emisor_cif['RegimenFiscal']
 
     emitidas = filter_invoices_iter(invoices=all_invoices.values(), fecha=dp, rfc_emisor=emisor_rfc)
     emitidas_pagos = filter_payments_iter(invoices=all_invoices, fecha=dp, rfc_emisor=emisor_rfc)
+    emitidas_pagos = list(emitidas_pagos)
 
     recibidas = filter_invoices_iter(invoices=all_invoices.values(), fecha=dp, rfc_receptor=emisor_rfc)
     recibidas_pagos = filter_payments_iter(invoices=all_invoices, fecha=dp, rfc_receptor=emisor_rfc)
 
     recibidas_pagos = list(recibidas_pagos)
     pagos_hechos_iva = [
         p
@@ -277,19 +284,25 @@
     payments_export(workbook, "RECIBIDAS PAGOS", recibidas_pagos)
 
     # SPECIALES
     payments_export(workbook, f"RECIBIDAS PAGOS IVA {emisor_regimen.code}", pagos_hechos_iva)
     if prediales:
         payments_export(workbook, "PREDIALES", prediales)
 
+    # RETENCIONES
+    if dp.month is None:
+        archivo_retenciones = facturas_filename(dp, ext="retenciones.txt")
+        pagos_agrupados = payments_groupby_receptor(emitidas_pagos)
+        payments_retentions_export(archivo_retenciones, pagos_agrupados)
+
     try:
         workbook.close()
-        print(f"Archivo {archivo_excel} creado")
+        return archivo_excel
     except FileCreateError:
-        print(f"No se pudo crear el archivo {archivo_excel}")
+        return None
 
 
 def generate_pdf_template(template_name, fields):
     increment_template = facturacion_environment.get_template(template_name)
     md5_document = increment_template.render(
         fields
     )
@@ -388,15 +401,15 @@
                 "DoctoRelacionado": [{
                     "Factura": d.get("Serie", "") + d.get("Folio", ""),
                     "IdDocumento": d.get("IdDocumento"),
                     "NumParcialidad": d.get("NumParcialidad"),
                     "ImpSaldoAnt": d.get("ImpSaldoAnt"),
                     "ImpPagado": d.get("ImpPagado"),
                     "ImpSaldoInsoluto": d.get("ImpSaldoInsoluto"),
-                } for d in p["DoctoRelacionado"]]
+                } for d in p.get("DoctoRelacionado", [])]
             } for p in pagos]
         })
     else:
         if isinstance(cfdi, SatCFDI) and cfdi.get("MetodoPago") == PPD:
             print_yaml({
                 "Conceptos": [x['Descripcion'] for x in i["Conceptos"]],
                 "Pendiente": cfdi.saldo_pendiente,
@@ -404,36 +417,36 @@
             })
         else:
             print_yaml({
                 "Conceptos": [x['Descripcion'] for x in i["Conceptos"]]
             })
 
 
-def ajustes_directory(ym_date):
-    return os.path.join(facturas_folder(DatePeriod(year=ym_date.year, month=ym_date.month)), 'ajustes')
+def ajustes_directory(dp: DatePeriod):
+    return os.path.join(facturas_folder(dp), 'ajustes')
 
 
-def ajustes(emisor_rfc, ym_date):
-    ym_date_effective = add_month(ym_date)
+def ajustes(emisor_rfc, dp: DatePeriod):
+    dp_effective = add_month(dp, 1)
 
     # clear directory
-    ajustes_dir = ajustes_directory(ym_date)
+    ajustes_dir = ajustes_directory(DatePeriod(dp.year, dp.month))
     clear_directory(ajustes_dir)
 
     clients = ClientsManager()
     facturas = FacturasManager(None)["Facturas"]
 
     def ajustes_iter():
-        for i, (rfc, concepto) in enumerate(find_ajustes(facturas, ym_date_effective.month)):
+        for i, (rfc, concepto) in enumerate(find_ajustes(facturas, dp_effective.month)):
             receptor = clients[rfc]
             valor_unitario_raw = concepto["ValorUnitario"]
 
             if isinstance(valor_unitario_raw, dict):
-                vud, vu = find_best_match(valor_unitario_raw, ym_date)
-                vund, vun = find_best_match(valor_unitario_raw, ym_date_effective)
+                vud, vu = find_best_match(valor_unitario_raw, dp)
+                vund, vun = find_best_match(valor_unitario_raw, dp_effective)
                 meses = months_between(vund, vud)
                 ajuste_porcentaje = (vun / vu - 1)
             else:
                 vu = valor_unitario_raw
                 vun = None
                 meses = None
                 ajuste_porcentaje = None
@@ -445,55 +458,57 @@
                 "receptor": receptor,
                 "emisor": clients[emisor_rfc],
                 "concepto": concepto,
                 "valor_unitario": pesos(vu),
                 "valor_unitario_nuevo": pesos(vun) if vun else "",
                 "ajuste_porcentaje": porcentaje(ajuste_porcentaje, 2) if ajuste_porcentaje is not None else "",
                 "ajuste_periodo": f"{meses} MESES",
-                "ajuste_efectivo_al": fecha(ym_date_effective),
+                "efectivo_periodo_desc": periodo_desc(dp_effective, concepto['_periodo_mes_ajuste'], concepto.get('_desfase_mes')),  # fecha(ym_date_effective),
                 "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
                 "fecha_hoy": fecha(date.today()),
                 'file_name': file_name
             }
             if ajuste_porcentaje is not None:
                 res = generate_pdf_template(
                     template_name='incremento_template.md',
                     fields=data
                 )
                 with open(file_name, 'wb') as f:
                     f.write(res)
             yield data
 
     ajustes_iter = list(ajustes_iter())
-    print("Ajuste Efectivo Al:", fecha(ym_date_effective))
+    print("Ajuste Efectivo Al:", year_month_desc(dp_effective))
     if ajustes_iter:
         print(
             tabulate(
                 [
                     [
                         i,
                         ajuste["receptor"]["RazonSocial"][:36],
                         ajuste["receptor"]["Rfc"],
                         ajuste["valor_unitario"].split(' ')[0],
                         ajuste["valor_unitario_nuevo"].split(' ')[0],
                         ajuste["ajuste_porcentaje"].split(' ')[0],
                         ajuste["periodo"],
                         ajuste["ajuste_periodo"],
+                        ajuste["efectivo_periodo_desc"]
                     ]
                     for i, ajuste in enumerate(ajustes_iter, start=1)
                 ],
                 headers=(
                     "",
                     "Receptor Razon Social",
                     "Recep. Rfc",
                     "Actual",
                     "Nuevo",
                     "Ajuste %",
                     "Periodo",
                     "Ajuste Periodo",
+                    "Ajuste Efectivo"
                 ),
                 disable_numparse=True,
                 colalign=("right", "left", "left", "right", "right", "right", "left", "left"),
             )
         )
     else:
         print("No hay ajustes para este mes")
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-2.2.0/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/layout.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,41 +41,41 @@
 
 ABOUT_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAABP0lEQVR4nOWVTU7DMBCFvxuwKmrX0G4o5QLtQboDFXEbwrLkGNDucwB" \
              "+VvQObS5ApCxAIz1LCNmOG68QTxopst882y/jMfwHnAIroAQ2ilJjgxzhkYRa4AvYA6" \
              "+KvcZacYx7FBZADXwC98DUw7GxAmjEXRwjbkkfwHkCfyyu5cy7yCPtxhJOUnckruUcgGGMWMqWs8D8UhE6iZ3iMVYtrTwPoVKEUEjDW123qowL" \
              "+uNSGjche6z8YlhGLHI4hGzaAi8dyVWHReiePPsmNprMXeAdeOprUZWwQB2yaKUfNM1Y4Eoa17EyLTIWeIiVqbOp0aXx4U7hw0S565RWsevRKnYpreJ3sxsniE8kntTsHObaTaN" \
              "/MvNwZvK8ETdZ3GGocnMPjom8KeofD846xZYYBuotJmQ31MK+bSzryfwb+AbymF7gpXVM1QAAAABJRU5ErkJggg=="
 
+INCREASE_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAAAf0lEQVR4nO2QwQmAMAwAbwkX8CXiGM7iBA6Qp+s4gduITqEUKpQiNLUVH/Ug0Ed6B4GfhyzA4Y0o" \
+                "/ondDTIAEzC/FTC0wGYne6ABVmAHukDAlaoCvpycAfcs5n3RAzUZAuONPEaqOlEVWiAxwFcBUUgLDEiktJCAJEiljMAPLieZDXZ8v71fBQAAAABJRU5ErkJggg=="
+
 BUTTON_COLOR = (sg.theme_background_color(), sg.theme_background_color())
 
 
 def make_layout(has_fiel):
     # LAYOUT
     button_column = [
-        sg.Button("Emitidas", key="facturas_emitidas", border_width=0),
-        sg.Text("Año-Mes:", pad=TEXT_PADDING),
+        sg.Button("Emitidas:", key="facturas_emitidas", border_width=0, pad=TEXT_PADDING),
+        # sg.Text("Año-Mes:", pad=TEXT_PADDING),
         sg.Input(date.today().strftime('%Y-%m'), size=(11, 1), key="periodo"),
+
+        sg.Button("Preparar:", key="prepare_facturas", border_width=0, pad=TEXT_PADDING),
+        sg.Input("", key="rango", size=(8, 1)),
+
+        sg.VSeparator(),
         sg.Button(image_data=EXCEL_ICON, key="ver_excel", border_width=0, button_color=BUTTON_COLOR),
         sg.Button(image_data=HTML_ICON, key="ver_html", border_width=0, button_color=BUTTON_COLOR),
+        sg.Button(image_data=INCREASE_ICON, key="preparar_ajuste_anual", border_width=0, button_color=BUTTON_COLOR),
         sg.Button(image_data=FOLDER_ICON, key="ver_carpeta", border_width=0, button_color=BUTTON_COLOR),
 
-        sg.VSeparator(),
-        sg.Button("Preparar", key="prepare_facturas", border_width=0),
-        sg.Text("De La:", pad=TEXT_PADDING),
-        sg.Input("1", key="inicio", size=(4, 1)),
-        sg.Text("Hasta:", pad=TEXT_PADDING),
-        sg.Input("", key="final", size=(4, 1)),
-
-        sg.VSeparator(),
-        sg.Button("Ajustes", key="preparar_ajuste_anual", border_width=0),
-        sg.Button(image_data=FOLDER_ICON, key="ver_carpeta_ajustes", border_width=0, button_color=BUTTON_COLOR),
+        # sg.Button(image_data=FOLDER_ICON, key="ver_carpeta_ajustes", border_width=0, button_color=BUTTON_COLOR),
 
         sg.Push(),
         sg.Text("Serie:", pad=TEXT_PADDING),
-        sg.Text("", key="serie", pad=TEXT_PADDING),
+        sg.Text("", key="serie", pad=TEXT_PADDING, text_color="black"),
         sg.Text("Folio:", pad=TEXT_PADDING),
         sg.Input("", key="folio", size=(10, 1), enable_events=True),
     ]
     c_second = [
         sg.Column(
             [
                 [
@@ -94,46 +94,47 @@
             pad=0
         ),
         sg.VSeparator(),
         sg.Column(
             [
                 [
                     sg.CalendarButton("FechaPago:", format='%Y-%m-%d', title="FechaPago", no_titlebar=False, target="fecha_pago", pad=TEXT_PADDING, border_width=0,
-                                      key="fecha_pago_select", disabled=True),
-                    sg.Input("", size=(12, 1), key="fecha_pago", disabled=True),
-                    sg.Text("FormaPago:", pad=TEXT_PADDING),
+                                      key="fecha_pago_select", visible=False),
+                    sg.Input("", size=(12, 1), key="fecha_pago", visible=False),
+                    sg.Text("FormaPago:", pad=TEXT_PADDING, visible=False, key="forma_pago_text"),
                     sg.Combo([Code(k, v) for k, v in FORMA_PAGO.items()], default_value=Code("03", FORMA_PAGO["03"]), key="forma_pago", size=(34, 1),
-                             disabled=True),
+                             visible=False),
                 ],
                 [
-                    sg.Button("Comprobante Pago", key="prepare_pago", border_width=0, disabled=True),
-                    sg.Text("       ImpPagado:", pad=TEXT_PADDING),
-                    sg.Input("", size=(12, 1), key="importe_pago", disabled=True),
+                    sg.Button("Comprobante Pago", key="prepare_pago", border_width=0, visible=False),
+                    sg.Text("       ImpPagado:", pad=TEXT_PADDING, visible=False, key="imp_pagado_text"),
+                    sg.Input("", size=(12, 1), key="importe_pago", visible=False),
                 ]
             ],
             pad=0
         )
     ]
 
     button_column_third = [
-        sg.Button("Correos", key="prepare_correos", border_width=0),
+        sg.Button(" Correos ", key="prepare_correos", border_width=0),
         sg.Button("Pendientes", key="facturas_pendientes", border_width=0),
-        sg.Button("Clientes", key="prepare_clientes", border_width=0),
+        sg.Button(" Clientes ", key="prepare_clientes", border_width=0),
         sg.VSeparator(),
+        sg.Button("SAT Status", key="sat_status_todas", border_width=0, visible=has_fiel),
         sg.Text("Recuperar:", pad=TEXT_PADDING, visible=has_fiel),
-        sg.Button("Emitidas", key="recuperar_emitidas", border_width=0, visible=has_fiel),
+        sg.Button("Emitidas ", key="recuperar_emitidas", border_width=0, visible=has_fiel),
         sg.Button("Recibidas", key="recuperar_recibidas", border_width=0, visible=has_fiel),
         sg.Text("Dias:", pad=TEXT_PADDING, visible=has_fiel),
         sg.Input("40", size=(4, 1), key="recuperar_dias", visible=has_fiel),
     ]
 
     button_column_low = [
         sg.Button("Procesar ", disabled=True, key="crear_facturas", border_width=0),
         sg.Push(),
-        sg.Checkbox("Ver Detallado", default=False, key="detallado"),
+        sg.Checkbox("Detallado", default=False, key="detallado"),
         sg.Button(image_data=ABOUT_ICON, key="about", border_width=0, button_color=BUTTON_COLOR),
     ]
 
     # ----- Full layout -----
     return [
         button_column,
         [sg.HSeparator()],
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/localdb.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-2.2.0/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/mycfdi.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 from collections.abc import Mapping
 from datetime import datetime
 from typing import MutableMapping
 from uuid import UUID
 
 from satcfdi.accounting import complement_invoices_data, SatCFDI
 
-from .localdb import load_data, save_data
+from . import ARCHIVOS_DIRECTORY
+from .localdb import load_data, save_data, LocalDBSatCFDI
 from .utils import to_uuid
 
 ALL_INVOICES = 'all_invoices'
 ALL_RETENCIONES = 'all_retenciones'
 logger = logging.getLogger(__name__)
 
 
 class MyCFDI(SatCFDI):
-    local_db = None
+    local_db = None  # type: LocalDBSatCFDI
 
     @SatCFDI.estatus.getter
     def estatus(self) -> str:
         Estatus = {
             "Cancelado": "0",
             "Vigente": "1"
         }
-        estado = self.local_db.status_sat(self).get('Estado')
+        estado = self.consulta_estado().get('Estado')
         return Estatus.get(estado, "1")
 
+    def consulta_estado(self):
+        return self.local_db.status_sat(self)
+
     @SatCFDI.fecha_cancelacion.getter
     def fecha_cancelacion(self) -> datetime:
         return None
 
     @classmethod
     def get_all_invoices(cls, invoices: MutableMapping, search_path="*.xml") -> bool:
         # Check that all names are correct
@@ -69,28 +73,32 @@
         # if the length does not match, then we need to try again :-/
         return was_updated
 
     @property
     def filename(self):
         match self.tag:
             case '{http://www.sat.gob.mx/cfd/3}Comprobante' | '{http://www.sat.gob.mx/cfd/4}Comprobante':
-                return "facturas/{3:%Y}/{3:%Y-%m}/{4}_{0}_[{1}]_{2}".format(
+                path = "{3:%Y}/{3:%Y-%m}/facturas/{4}_{0}_[{1}]_{2}".format(
                     self.name,
                     self["TipoDeComprobante"].code,
                     self.uuid,
                     self["Fecha"],
                     self["Emisor"]["Rfc"],
                 )
             case '{http://www.sat.gob.mx/esquemas/retencionpago/1}Retenciones' | '{http://www.sat.gob.mx/esquemas/retencionpago/2}Retenciones':
-                return "retenciones/{2:%Y}/{2:%Y-%m}/{3}_{0}_{1}".format(
+                path = "{2:%Y}/{2:%Y-%m}/retenciones/{3}_{0}_{1}".format(
                     self.get("FolioInt", ""),
                     self.uuid,
                     self["FechaExp"],
                     self["Emisor"].get('RFCEmisor') or self["Emisor"].get('RfcE')
                 )
+            case _:
+                raise Exception("Unknown Tag", self.tag)
+
+        return os.path.join(ARCHIVOS_DIRECTORY, path)
 
     @classmethod
     def uuid_from_filename(cls, filename):
         filename = os.path.basename(filename)
         parts = os.path.splitext(filename)[0].split("_")
         if len(parts) >= 3:
             return to_uuid(parts[-1])
@@ -141,23 +149,23 @@
 
     return cfdi
 
 
 def get_all_cfdi() -> Mapping[UUID, MyCFDI]:
     all_invoices = load_data(ALL_INVOICES, {})
 
-    has_updates = MyCFDI.get_all_invoices(invoices=all_invoices, search_path="facturas/**/*.xml")
+    has_updates = MyCFDI.get_all_invoices(invoices=all_invoices, search_path=os.path.join(ARCHIVOS_DIRECTORY, "**/facturas/*.xml"))
     if has_updates:
         save_data(ALL_INVOICES, all_invoices)
 
     complement_invoices_data(all_invoices)
     return all_invoices
 
 
 def get_all_retenciones() -> Mapping[UUID, MyCFDI]:
     all_invoices = load_data(ALL_RETENCIONES, {})
 
-    has_updates = MyCFDI.get_all_invoices(invoices=all_invoices, search_path="retenciones/**/*.xml")
+    has_updates = MyCFDI.get_all_invoices(invoices=all_invoices, search_path=os.path.join(ARCHIVOS_DIRECTORY, "**/retenciones/*.xml"))
     if has_updates:
         save_data(ALL_RETENCIONES, all_invoices)
 
     return all_invoices
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/factura.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,16 @@
           type: number
         ClaveUnidad:
           type: string
         Descripcion:
           type: string
         _periodo_mes_ajuste:
           type: string
+        _desfase_mes:
+          type: integer
         ValorUnitario:
           type:
           - number
           - 'null'
         Impuestos:
           type: object
           properties:
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice/utils.py` & `satdigitalinvoice-2.2.0/satdigitalinvoice/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,18 +22,14 @@
         try:
             return fmt, datetime.strptime(text, fmt)
         except ValueError:
             pass
     raise ValueError('no valid date format found')
 
 
-def parse_ym_date(periodo):
-    return try_parsing_date(periodo)[1]
-
-
 def to_uuid(s):
     try:
         return UUID(s)
     except ValueError:
         return None
 
 
@@ -41,15 +37,15 @@
     try:
         return int(s)
     except ValueError:
         return None
 
 
 def random_string():
-    chars = "0123456789abcdefghijklmnopqrstuvwxzyABCDEFGHIJKLMNOPQRSTUVWXZY"
+    chars = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
     return "".join(random.choice(chars) for _ in range(32))
 
 
 def convert_ans1_date(ans1_date):
     return datetime.strptime(ans1_date.decode('utf-8'), '%Y%m%d%H%M%SZ')
 
 
@@ -66,19 +62,19 @@
             # "emailAddress": signer.certificate.get_subject().emailAddress,
             #
             "Expira": convert_ans1_date(signer.certificate.get_notAfter()),
             "Creado": convert_ans1_date(signer.certificate.get_notBefore()),
         }
 
 
-def find_best_match(cases, emission_date):
+def find_best_match(cases, dp: DatePeriod):
     fk, fv = (None, None)
     for k, v in cases.items():
-        k = parse_ym_date(k)
-        if k <= emission_date:
+        k = datetime.strptime(k, '%Y-%m')
+        if k <= dp:
             if fk is None or k > fk:
                 fk, fv = k, v
     return fk, fv
 
 
 def clear_directory(directory):
     shutil.rmtree(directory, ignore_errors=True)
@@ -86,18 +82,18 @@
 
 
 # calculate the number of months between two dates
 def months_between(d1, d2):
     return (d1.year - d2.year) * 12 + d1.month - d2.month
 
 
-def add_month(d):
-    m = d.month % 12 + 1
-    y = d.year + d.month // 12
-    return d.replace(year=y, month=m)
+def add_month(dp: DatePeriod, months):
+    year, month = divmod(dp.year * 12 + dp.month + months - 1, 12)
+    month += 1
+    return DatePeriod(year, month)
 
 
 def load_certificate(data):
     if 'data' in data:
         return Signer.load_pkcs12(
             **data,
         )
@@ -110,7 +106,17 @@
 def first_duplicate(seq):
     seen = set()
     for x in seq:
         if x in seen:
             return x
         seen.add(x)
     return None
+
+
+def parse_rango(rango):
+    if rango == "":
+        return 1, None
+    if rango.isdigit():
+        return int(rango), int(rango)
+    if "-" in rango:
+        start, end = rango.split("-")
+        return int(start), int(end)
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.1.5
+Version: 2.2.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.1.5/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/setup.py` & `satdigitalinvoice-2.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         package: [
             "markdown_styles/*",
             "schemas/*",
             'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.6',
+        'satcfdi==4.0.10',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'markdown2',
         'PySimpleGUI',
         'XlsxWriter',
```

### Comparing `satdigitalinvoice-2.1.5/tests/test_crear_facturas.py` & `satdigitalinvoice-2.2.0/tests/test_crear_facturas.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 import logging
 from datetime import date, datetime
 from decimal import Decimal
+from unittest import mock
 
-from satcfdi import Signer
+from satcfdi import Signer, DatePeriod
 
+from satdigitalinvoice.__version__ import __package__
 from satdigitalinvoice.file_data_managers import ClientsManager, FacturasManager, ConfigManager
 from satdigitalinvoice.gui_functions import generate_ingresos, periodo_desc
 from satdigitalinvoice.utils import find_best_match
+from tests.utils import verify_result, XElementPrettyPrinter
 
 csd_signer = Signer.load(
     certificate=open('csd/cacx7605101p8.cer', 'rb').read(),
     key=open('csd/cacx7605101p8.key', 'rb').read(),
     password=open('csd/cacx7605101p8.txt', 'rb').read(),
 )
 ym_date = datetime(year=2023, month=4, day=1)
 clients = ClientsManager()
+module = __package__
 
 
 def test_generar_ingresos(caplog):
     caplog.set_level(logging.INFO)
     config = ConfigManager()
     facturas = FacturasManager(ym_date)["Facturas"]
 
-    facturas = generate_ingresos(
-        serie=config["serie"],
-        folio=1000,
-        clients=clients,
-        facturas=facturas,
-        ym_date=date(year=2023, month=4, day=1),
-        csd_signer=csd_signer,
-    )
+    with mock.patch(f'satcfdi.create.cfd.cfdi40.datetime') as m:
+        m.now = mock.Mock(return_value=datetime(2022, 1, 1))
+
+        facturas = generate_ingresos(
+            serie=config["serie"],
+            folio=1000,
+            clients=clients,
+            facturas=facturas,
+            dp=date(year=2023, month=4, day=1),
+            csd_signer=csd_signer,
+        )
+
+        assert caplog.records == []
+        assert len(facturas) == 3
+
+        pp = XElementPrettyPrinter()
+        verify = verify_result(data=pp.pformat(facturas), filename=f"facturas.pretty.py")
+        assert verify
 
-    assert caplog.records == []
-    assert len(facturas) == 3
-    assert facturas[0]["Total"] == Decimal('18065.66')
+    # assert facturas[0]["Total"] == Decimal('18065.66')
+    # assert facturas[0]["Conceptos"][0]["Descripcion"] == 1000
 
 
 def test_generar_ingresos_error(caplog):
     caplog.set_level(logging.INFO)
     config = ConfigManager()
     facturas = FacturasManager(ym_date)["FacturasIncorrectas"]
     print(len(facturas))
 
     ingresos = generate_ingresos(
         serie=config["serie"],
         folio=1000,
         clients=clients,
         facturas=facturas,
-        ym_date=date(year=2023, month=4, day=1),
+        dp=date(year=2023, month=4, day=1),
         csd_signer=csd_signer,
     )
 
     assert len(caplog.records) == 1
     assert caplog.records[0].message == "ABMG891115PD7: Total '41000.16' is invalid, expected '37019.16'"
     assert ingresos is None
 
@@ -63,37 +76,51 @@
     print(len(facturas))
 
     ingresos = generate_ingresos(
         serie=config["serie"],
         folio=1000,
         clients=ClientsManager(),
         facturas=facturas,
-        ym_date=date(year=2023, month=4, day=1),
+        dp=date(year=2023, month=4, day=1),
         csd_signer=csd_signer,
     )
 
     assert len(caplog.records) == 1
     assert caplog.records[0].message == "XXXNOEXISTO: client not found"
     assert ingresos is None
 
 
 def test_periodo_desc():
-    assert periodo_desc(date(year=2021, month=1, day=1), 'Mensual.1') == 'MES DE ENERO DEL 2021'
-    assert periodo_desc(date(year=2021, month=1, day=1), 'Bimestral.2') is None
-    assert periodo_desc(date(year=2021, month=1, day=1), 'Trimestral.3') is None
-    assert periodo_desc(date(year=2021, month=1, day=1), 'Cuatrimestral.4') is None
-    assert periodo_desc(date(year=2021, month=1, day=1), 'Semestral.5') is None
-    assert periodo_desc(date(year=2021, month=1, day=1), 'Anual.6') is None
-
-    assert periodo_desc(date(year=2021, month=12, day=1), 'Mensual.7') == 'MES DE DICIEMBRE DEL 2021'
-    assert periodo_desc(date(year=2021, month=12, day=1), 'Bimestral.8') == 'MES DE DICIEMBRE DEL 2021 AL MES DE ENERO DEL 2022'
-    assert periodo_desc(date(year=2021, month=12, day=1), 'Trimestral.9') == 'MES DE DICIEMBRE DEL 2021 AL MES DE FEBRERO DEL 2022'
-    assert periodo_desc(date(year=2021, month=12, day=1), 'Cuatrimestral.8') == 'MES DE DICIEMBRE DEL 2021 AL MES DE MARZO DEL 2022'
-    assert periodo_desc(date(year=2021, month=12, day=1), 'Semestral.6') == 'MES DE DICIEMBRE DEL 2021 AL MES DE MAYO DEL 2022'
-    assert periodo_desc(date(year=2021, month=12, day=1), 'Anual.12') == 'MES DE DICIEMBRE DEL 2021 AL MES DE NOVIEMBRE DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=0) == 'MES DE ENERO DEL 2021'
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=0) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=0) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Cuatrimestral.4', offset=0) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Semestral.5', offset=0) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Anual.6', offset=0) is None
+
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Mensual.7', offset=0) == 'MES DE DICIEMBRE DEL 2021'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Bimestral.8', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE ENERO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Trimestral.9', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE FEBRERO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Cuatrimestral.8', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE MARZO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Semestral.6', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE MAYO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Anual.12', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE NOVIEMBRE DEL 2022'
+
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=1) == 'MES DE FEBRERO DEL 2021'
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=1) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=1) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Cuatrimestral.4', offset=1) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Semestral.5', offset=1) is None
+    assert periodo_desc(DatePeriod(year=2021, month=1), 'Anual.6', offset=1) is None
+
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Mensual.7', offset=1) == 'MES DE ENERO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Bimestral.8', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE FEBRERO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Trimestral.9', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE MARZO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Cuatrimestral.8', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE ABRIL DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Semestral.6', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE JUNIO DEL 2022'
+    assert periodo_desc(DatePeriod(year=2021, month=12), 'Anual.12', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE DICIEMBRE DEL 2022'
 
 
 def test_find_best_match():
     casesA = {
         '2022-12': Decimal('20.00'),
         '2023-12': Decimal('30.00'),
         '2024-12': Decimal('40.00'),
```

### Comparing `satdigitalinvoice-2.1.5/tests/test_localdb.py` & `satdigitalinvoice-2.2.0/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.1.5/tests/test_main.py` & `satdigitalinvoice-2.2.0/tests/test_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from datetime import date, datetime
 
 import pytest
+from satcfdi import DatePeriod
+
 from satdigitalinvoice.facturacion import FacturacionGUI
 from yaml.constructor import ConstructorError
 
 from satdigitalinvoice.file_data_managers import LocalData, ConfigManager, FacturasManager
 
 from satdigitalinvoice.layout import make_layout
 from satdigitalinvoice.utils import random_string, add_month
@@ -52,22 +54,22 @@
 def test_duplicated_facturas():
     class MyFacturasManager(FacturasManager):
         file_source = "facturas_duplicated.yaml"
 
     # expect exception thrown
 
     with pytest.raises(ValueError) as e:
-        MyFacturasManager(datetime(2021, 1, 1))
+        MyFacturasManager(DatePeriod(2021, 1, 1))
     assert str(e.value)[0:20] == 'Factura Duplicada: {'
 
 
 def test_increase_month():
-    d = datetime(2021, 1, 28)
-    d = add_month(d)
-    assert d == datetime(2021, 2, 28)
+    d = DatePeriod(2021, 1)
+    d = add_month(d, 1)
+    assert d.year == 2021 and d.month == 2
 
 
 def test_app_setup():
     config = ConfigManager()
     a = FacturacionGUI(
         config
     )
```

