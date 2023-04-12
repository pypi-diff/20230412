# Comparing `tmp/anyhedge-0.3.5.tar.gz` & `tmp/anyhedge-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyhedge-0.3.5.tar", last modified: Wed Apr 12 15:56:51 2023, max compression
+gzip compressed data, was "anyhedge-0.3.6.tar", last modified: Wed Apr 12 18:14:41 2023, max compression
```

## Comparing `anyhedge-0.3.5.tar` & `anyhedge-0.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/
--rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.3.5/LICENSE
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 15:56:51.658821 anyhedge-0.3.5/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.3.5/README.md
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/anyhedge/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.3.5/anyhedge/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2358 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    28148 2023-04-12 15:19:00.000000 anyhedge-0.3.5/anyhedge/contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.3.5/anyhedge/javascript.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.3.5/anyhedge/oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/role.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/anyhedge/tests/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/test_bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    32328 2023-04-12 15:56:18.000000 anyhedge-0.3.5/anyhedge/tests/test_contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/test_fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/test_oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.3.5/anyhedge/validators.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/anyhedge.egg-info/
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)      512 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/requires.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-12 15:55:23.000000 anyhedge-0.3.5/pyproject.toml
--rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-12 15:56:51.658821 anyhedge-0.3.5/setup.cfg
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.3.6/LICENSE
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 18:14:41.786326 anyhedge-0.3.6/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.3.6/README.md
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/anyhedge/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.3.6/anyhedge/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2358 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    28401 2023-04-12 18:08:28.000000 anyhedge-0.3.6/anyhedge/contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.3.6/anyhedge/javascript.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.3.6/anyhedge/oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/role.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/anyhedge/tests/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/test_bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    33305 2023-04-12 18:09:52.000000 anyhedge-0.3.6/anyhedge/tests/test_contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/test_fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.3.6/anyhedge/tests/test_oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.3.6/anyhedge/validators.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 18:14:41.786326 anyhedge-0.3.6/anyhedge.egg-info/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)      512 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/requires.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-12 18:14:41.000000 anyhedge-0.3.6/anyhedge.egg-info/top_level.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-12 18:14:17.000000 anyhedge-0.3.6/pyproject.toml
+-rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-12 18:14:41.786326 anyhedge-0.3.6/setup.cfg
```

### Comparing `anyhedge-0.3.5/LICENSE` & `anyhedge-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/PKG-INFO` & `anyhedge-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.3.5
+Version: 0.3.6
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.3.5/README.md` & `anyhedge-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/anyhedge/bch_primitives.py` & `anyhedge-0.3.6/anyhedge/bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/anyhedge/contract.py` & `anyhedge-0.3.6/anyhedge/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,14 +486,18 @@
     ###############
     # Derivative values
     ###############
     @property
     def clamped_end_price_oracleUnits_per_bch(self) -> ScriptPriceInOracleUnitsPerBch:
         return max(self.naive_end_price_oracleUnits_per_bch, self.base_funding.base_proposal.long_liquidation_price_oracleUnits_per_bch)
 
+    @property
+    def cost_sats_for_nominal_value_at_redemption(self) -> Sats:
+        return Sats(round_half_up(SATS_PER_BCH * (self.base_funding.base_proposal.effective_nominal_value_oracleUnits / float(self.clamped_end_price_oracleUnits_per_bch))))
+
     ###############
     # Property access to payout sats
     ###############
     @property
     def total_payout_sats(self) -> UtxoSats:
         return self.payout_sats()
```

### Comparing `anyhedge-0.3.5/anyhedge/fee.py` & `anyhedge-0.3.6/anyhedge/fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/anyhedge/oracle.py` & `anyhedge-0.3.6/anyhedge/oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/anyhedge/tests/test_bch_primitives.py` & `anyhedge-0.3.6/anyhedge/tests/test_bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/anyhedge/tests/test_contract.py` & `anyhedge-0.3.6/anyhedge/tests/test_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,18 @@
 
 # Derived total payout sats and units
 # Calculated as SHORT_PAYOUT_SATS_AS_HEDGE + LONG_PAYOUT_SATS
 TOTAL_PAYOUT_SATS_AS_HEDGE = UtxoSats(64283878)
 # Calculated as SHORT_PAYOUT_ORACLE_UNITS_AS_HEDGE + LONG_PAYOUT_ORACLE_UNITS
 TOTAL_PAYOUT_ORACLE_UNITS_AS_HEDGE = UsdEM2Beta(14142.4532)
 
+# Nominal value at payout
+# Calculated as round_half_up(NOMINAL_VALUE_USDEM2 / float(CLAMPED_PRICE)) * SATS_PER_BCH
+COST_SATS_FOR_NOMINAL_VALUE_AT_REDEMPTION = Sats(45_454_545)
+
 
 def standard_maturation(
         funding: ContractFunding | None = None
 ):
     funding = funding if funding is not None else standard_contract_funding()
     return funding.redeem(
         price_timestamp=MATURITY_TIMESTAMP,
@@ -594,10 +598,21 @@
         # Should report according to calculation for leveraged short (which can also be 1)
         self.assertAlmostEqual(self.leveraged_short.effective_short_leverage, SHORT_LEVERAGE_NOT_1, delta=.001)
 
     def test_short_payout_for_leveraged_short(self):
         leveraged_short_redemption = standard_maturation(standard_contract_funding(self.leveraged_short))
         self.assertEqual(leveraged_short_redemption.short_payout_sats, SHORT_PAYOUT_SATS_AS_LEVERAGED_SHORT)
 
+    def test_cost_at_redemption_for_hedge_vs_leveraged_short(self):
+        hedge_redemption = standard_maturation(standard_contract_funding(self.hedge_short))
+        leveraged_short_redemption = standard_maturation(standard_contract_funding(self.leveraged_short))
+
+        # hedge redemption should just be the short payout
+        self.assertEqual(hedge_redemption.cost_sats_for_nominal_value_at_redemption, hedge_redemption.short_payout_sats)
+
+        # leveraged short redemption is different from short payout
+        self.assertNotEqual(leveraged_short_redemption.cost_sats_for_nominal_value_at_redemption, leveraged_short_redemption.short_payout_sats)
+        self.assertEqual(leveraged_short_redemption.cost_sats_for_nominal_value_at_redemption, COST_SATS_FOR_NOMINAL_VALUE_AT_REDEMPTION)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `anyhedge-0.3.5/anyhedge/tests/test_fee.py` & `anyhedge-0.3.6/anyhedge/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/anyhedge/tests/test_oracle.py` & `anyhedge-0.3.6/anyhedge/tests/test_oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/anyhedge.egg-info/PKG-INFO` & `anyhedge-0.3.6/anyhedge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.3.5
+Version: 0.3.6
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.3.5/anyhedge.egg-info/SOURCES.txt` & `anyhedge-0.3.6/anyhedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.5/pyproject.toml` & `anyhedge-0.3.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'anyhedge'
-version = '0.3.5'
+version = '0.3.6'
 authors = [
   { name='emergent_reasons', email='emergent_reasons@gmail.com' },
 ]
 license = { file = "LICENSE" }
 description = 'Basic components of AnyHedge contracts'
 readme = 'README.md'
 requires-python = '>=3.10'
```

