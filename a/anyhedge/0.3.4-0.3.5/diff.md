# Comparing `tmp/anyhedge-0.3.4.tar.gz` & `tmp/anyhedge-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyhedge-0.3.4.tar", last modified: Wed Apr 12 09:42:36 2023, max compression
+gzip compressed data, was "anyhedge-0.3.5.tar", last modified: Wed Apr 12 15:56:51 2023, max compression
```

## Comparing `anyhedge-0.3.4.tar` & `anyhedge-0.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.305355 anyhedge-0.3.4/
--rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.3.4/LICENSE
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 09:42:36.305355 anyhedge-0.3.4/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.3.4/README.md
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.301355 anyhedge-0.3.4/anyhedge/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.3.4/anyhedge/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2358 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    27899 2023-04-12 09:41:55.000000 anyhedge-0.3.4/anyhedge/contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.3.4/anyhedge/javascript.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.3.4/anyhedge/oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/role.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.305355 anyhedge-0.3.4/anyhedge/tests/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/test_bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    30745 2023-04-12 09:41:55.000000 anyhedge-0.3.4/anyhedge/tests/test_contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/test_fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/test_oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.3.4/anyhedge/validators.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.301355 anyhedge-0.3.4/anyhedge.egg-info/
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)      512 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/requires.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-12 09:41:55.000000 anyhedge-0.3.4/pyproject.toml
--rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-12 09:42:36.305355 anyhedge-0.3.4/setup.cfg
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.3.5/LICENSE
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 15:56:51.658821 anyhedge-0.3.5/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.3.5/README.md
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/anyhedge/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.3.5/anyhedge/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2358 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    28148 2023-04-12 15:19:00.000000 anyhedge-0.3.5/anyhedge/contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.3.5/anyhedge/javascript.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.3.5/anyhedge/oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/role.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/anyhedge/tests/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/test_bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    32328 2023-04-12 15:56:18.000000 anyhedge-0.3.5/anyhedge/tests/test_contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/test_fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.3.5/anyhedge/tests/test_oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.3.5/anyhedge/validators.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 15:56:51.658821 anyhedge-0.3.5/anyhedge.egg-info/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)      512 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/requires.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-12 15:56:51.000000 anyhedge-0.3.5/anyhedge.egg-info/top_level.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-12 15:55:23.000000 anyhedge-0.3.5/pyproject.toml
+-rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-12 15:56:51.658821 anyhedge-0.3.5/setup.cfg
```

### Comparing `anyhedge-0.3.4/LICENSE` & `anyhedge-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/PKG-INFO` & `anyhedge-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.3.4
+Version: 0.3.5
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.3.4/README.md` & `anyhedge-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/anyhedge/bch_primitives.py` & `anyhedge-0.3.5/anyhedge/bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/anyhedge/contract.py` & `anyhedge-0.3.5/anyhedge/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,16 +137,15 @@
     def _input_sats_lookup(self) -> dict[(Role | None, Side | None), UtxoSats | None]:
         # Total sats is a hard contract parameter established by whatever method during construction.
         # Here we split it back into its two parts: short side, and for strict numerical safety, everything else as long side
 
         # The definition of short's input is that it needs to be enough to fully cover the worst case outcome of selling low
         # and buying high. That amount is the difference between the cost of the nominal assets at short/high liquidation vs
         # the cost at the start price. Note that in our inverted price scheme of BCH/Asset, the lower cost is at the higher price.
-        cost_sats_for_nominal_value_at_start = UtxoSats(round_half_up(self.nominal_oracleUnits_x_satsPerBch / self.start_price_oracleUnits_per_bch))
-        short_input_sats = UtxoSats(cost_sats_for_nominal_value_at_start - self.cost_sats_for_nominal_value_at_short_liquidation)
+        short_input_sats = UtxoSats(self.cost_sats_for_nominal_value_at_start - self.cost_sats_for_nominal_value_at_short_liquidation)
 
         # Long input sats is everything needed to cover the rest of the total
         long_input_sats = UtxoSats(self.total_input_sats - short_input_sats)
 
         return {
             (None,       None):       self.total_input_sats,
             (None,       Side.SHORT): short_input_sats,
@@ -179,14 +178,22 @@
         return oracle_pubkey_to_unit_class[self.oracle_public_key]
 
     @property
     def duration_seconds(self) -> int:
         return self.maturity_timestamp - self.start_timestamp
 
     @property
+    def effective_nominal_value_oracleUnits(self) -> OracleUnit:
+        return self.oracle_unit_cls(self.nominal_oracleUnits_x_satsPerBch / SATS_PER_BCH)
+
+    @property
+    def cost_sats_for_nominal_value_at_start(self) -> UtxoSats:
+        return UtxoSats(round_half_up((self.effective_nominal_value_oracleUnits / float(self.start_price_oracleUnits_per_bch)) * SATS_PER_BCH))
+
+    @property
     def effective_short_leverage(self) -> ShortLeverage:
         # There is a special case where even if the liquidation price must be recorded at some max value,
         # The fundamental cost for the position at liquidation is hard-lined at zero. That is the definition
         # of a hard hedge position, emulating the original anyhedge contract behavior.
         if self.cost_sats_for_nominal_value_at_short_liquidation == 0:
             return ShortLeverage(1)
```

### Comparing `anyhedge-0.3.4/anyhedge/fee.py` & `anyhedge-0.3.5/anyhedge/fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/anyhedge/oracle.py` & `anyhedge-0.3.5/anyhedge/oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/anyhedge/tests/test_bch_primitives.py` & `anyhedge-0.3.5/anyhedge/tests/test_bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/anyhedge/tests/test_contract.py` & `anyhedge-0.3.5/anyhedge/tests/test_contract.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,19 +40,29 @@
 LONG_LEVERAGE = LongLeverage(4.5)
 SHORT_LEVERAGE_1_AS_HEDGE = ShortLeverage(1)
 SHORT_LEVERAGE_NOT_1 = ShortLeverage(2.2)
 START_PRICE_USDEM2_PER_BCH = ScriptPriceInOracleUnitsPerBch(200_00)  # $200.00 / BCH
 
 # Derived values
 
+# The cost of the short position at start is equal to the hedge input for a pure hedge.
+# However, they are not equal for a leveraged short.
+# Calculated as round_half_up((NOMINAL_VALUE_USDEM2 / START_PRICE_USDEM2_PER_BCH) * SATS_PER_BCH)
+COST_SATS_FOR_NOMINAL_VALUE_AT_START = UtxoSats(50_000_000)
+
 # The compound nominal value is a giant number stored in the original AnyHedge contract and needed
 # to get around the lack of multiplication by optimizing the contract into a single division operation
 # = NominalOracleUnitsXSatsPerBch(round(NOMINAL_VALUE_USDEM2 * SATS_PER_BCH))
 NOMINAL_UNITS_X_SATS_PER_BCH = NominalOracleUnitsXSatsPerBch(1_000_000_000_000)
 
+# The contract stores the compound nominal value but not the original value. Therefore, the nominal value
+# of a contract exists only as an effective value back-calculated from the parameters.
+# Calculated as NOMINAL_UNITS_X_SATS_PER_BCH / SATS_PER_BCH
+EFFECTIVE_NOMINAL_VALUE_ORALCEUNITS = UsdEM2Beta(100_00.0)
+
 # Long liquidation Price is the price where all of long's input is consumed to cover short's agreed payout
 # Calculate in terms of leverage intent as round(START_PRICE_USDEM2_PER_BCH * (1 - 1 / LONG_LEVERAGE))
 # 15556 cents/BCH ($155.56 / BCH)
 LONG_LIQUIDATION_PRICE = ScriptPriceInOracleUnitsPerBch(155_56)
 
 # Short liquidation Price is the price where all of short's input is consumed to cover long's agreed payout
 # When short is exactly a 1x short, there is no meaningful liquidation price (infinity) but the stored liquidation price is still
@@ -64,38 +74,36 @@
 
 # Cost of nominal value at short liquidation is a new value that was always zero for pure hedges
 # and therefore not documented explicitly anywhere. With leveraged shorts, short does not always
 # pay the full cost of the nominal value and so the contract needs to track the cost.
 # Fixed for pure hedge at 0
 ZERO_COST_OF_NOMINAL_VALUE_AT_HEDGE_LIQUIDATION = Sats(0)
 # Calculated for leveraged short as floor(NOMINAL_UNITS_X_SATS_PER_BCH / SHORT_LIQUIDATION_PRICE_FOR_LEVERAGED_SHORT)
-COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION = Sats(27_272_479)
+COST_SATS_FOR_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION = Sats(27_272_479)
 
 # The bch amount to cover the short's payout obligations to long
 # For a pure hedge, it is the full cost of the nominal contract at starting price,
 # effectively allowing the price to increase to any value and still be able to pay out
-# Calculated as round(NOMINAL_UNITS_X_SATS_PER_BCH / START_PRICE_USDEM2_PER_BCH)
-# 0.5 BCH
-SHORT_INPUT_SATS_AS_HEDGE = UtxoSats(50_000_000)
+SHORT_INPUT_SATS_AS_HEDGE = COST_SATS_FOR_NOMINAL_VALUE_AT_START
 # For a leveraged short, it is the cost at starting price less the cost at short liquidation price
-# Calculated as SHORT_INPUT_SATS_AS_HEDGE - COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION
+# Calculated as SHORT_INPUT_SATS_AS_HEDGE - COST_SATS_FOR_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION
 SHORT_INPUT_SATS_AS_LEVERAGED_SHORT = UtxoSats(22_727_521)
 
 # Similar to cost at short liquidation, there is also the cost at long liquidation.
 # In the contract, this is not stored anywhere, but it is a useful intermediary for confirming tests.
 # It is the amount needed to cover the nominal unit value at long liquidation price
 # Calculated as ceil((NOMINAL_UNITS_X_SATS_PER_BCH) / DERIVED_LIQUIDATION_PRICE_UNITS_PER_BCH)
-COST_SATS_OF_NOMINAL_VALUE_AT_LONG_LIQUIDATION = UtxoSats(64_283_878)
+COST_SATS_FOR_NOMINAL_VALUE_AT_LONG_LIQUIDATION = UtxoSats(64_283_878)
 
 # The total input sats needed to cover all positions is the sum of the short and long inputs.
 # However, from base contract values, it is the difference between the cost at the two liquidation points
 # For a pure hedge, it has to cover the cost between long liquidation and zero
-TOTAL_INPUT_SATS_AS_HEDGE = COST_SATS_OF_NOMINAL_VALUE_AT_LONG_LIQUIDATION - 0
+TOTAL_INPUT_SATS_AS_HEDGE = COST_SATS_FOR_NOMINAL_VALUE_AT_LONG_LIQUIDATION - 0
 # For a leveraged short, it has to cover the cost between long liquidation and short liquidation (which also might be zero)
-# Calculated as COST_SATS_OF_NOMINAL_VALUE_AT_LONG_LIQUIDATION - COST_SATS_OF_NOMINAL_VALUE_AT_SHORT_LIQUIDATION
+# Calculated as COST_SATS_FOR_NOMINAL_VALUE_AT_LONG_LIQUIDATION - COST_SATS_FOR_NOMINAL_VALUE_AT_SHORT_LIQUIDATION
 TOTAL_INPUT_SATS_AS_LEVERAGED_SHORT = UtxoSats(37_011_399)
 
 # The bch amount to provide volatility protection as specified by the multiplier
 # This is the amount to cover the difference between payout bch at start and payout bch at long's liquidation price
 # Calculated as DERIVED_TOTAL_INPUT_SATS - SHORT_INPUT_SATS_AS_HEDGE
 LONG_INPUT_SATS = UtxoSats(14_283_878)
 
@@ -358,15 +366,15 @@
 ###################
 # Redeemed Contract Tests
 ###################
 # Derived short payout sats and units
 # For pure hedge, calculated as max(dust, HEDGE_COMPOSITE // CLAMPED_PRICE - 0) (Note the integer division //)
 SHORT_PAYOUT_SATS_AS_HEDGE = UtxoSats(45_454_545)  # 0.45454545... Bch
 # For leveraged short, same calculation but the cost at short liquidation is not zero
-# Calculated as SHORT_PAYOUT_SATS_AS_HEDGE - COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION
+# Calculated as SHORT_PAYOUT_SATS_AS_HEDGE - COST_SATS_FOR_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION
 # Due to integer math, this *can* be zero like a perfect hedge in some extreme values.
 SHORT_PAYOUT_SATS_AS_LEVERAGED_SHORT = UtxoSats(18_182_066)
 
 # Calculated as SHORT_PAYOUT_SATS_AS_HEDGE * MATURITY_PRICE / SATS_PER_BCH
 SHORT_PAYOUT_ORACLE_UNITS_AS_HEDGE = UsdEM2Beta(9999.999900)  # 99.99999900000 USD
 
 # Derived long payout sats and units
@@ -547,20 +555,35 @@
 
 class TestHedgeVsLeveragedShort(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.hedge_short = standard_contract_proposal()
         cls.leveraged_short = standard_contract_proposal(short_leverage=SHORT_LEVERAGE_NOT_1)
 
+    def test_effective_nominal_value_oracleUnits(self):
+        # The asset value is the same in both pure hedge and leveraged short
+        self.assertEqual(self.hedge_short.effective_nominal_value_oracleUnits, EFFECTIVE_NOMINAL_VALUE_ORALCEUNITS)
+        self.assertEqual(self.leveraged_short.effective_nominal_value_oracleUnits, EFFECTIVE_NOMINAL_VALUE_ORALCEUNITS)
+
+    def test_cost_of_nominal_value_at_start_not_equivalent_to_short_input(self):
+        # in the pure hedge case so far on AnyHedge, hedge input is equal to cost of nominal value at the start
+        self.assertEqual(self.hedge_short.short_input_sats, self.hedge_short.cost_sats_for_nominal_value_at_start)
+
+        # For leveraged shorts, they are not equal.
+        self.assertNotEqual(self.leveraged_short.short_input_sats, self.leveraged_short.cost_sats_for_nominal_value_at_start)
+
+        # Confirm that the new cost at start is correct
+        self.assertEqual(self.leveraged_short.cost_sats_for_nominal_value_at_start, COST_SATS_FOR_NOMINAL_VALUE_AT_START)
+
     def test_short_liquidation_price_for_leveraged_short(self):
         self.assertEqual(self.leveraged_short.short_liquidation_price_oracleUnits_per_bch, SHORT_LIQUIDATION_PRICE_AS_LEVERAGED_SHORT)
 
     def test_cost_at_short_liquidation_for_hedge_vs_leveraged_short(self):
         self.assertEqual(self.hedge_short.cost_sats_for_nominal_value_at_short_liquidation, ZERO_COST_OF_NOMINAL_VALUE_AT_HEDGE_LIQUIDATION)
-        self.assertEqual(self.leveraged_short.cost_sats_for_nominal_value_at_short_liquidation, COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION)
+        self.assertEqual(self.leveraged_short.cost_sats_for_nominal_value_at_short_liquidation, COST_SATS_FOR_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION)
 
     def test_short_input_sats_for_leveraged_short(self):
         self.assertEqual(self.leveraged_short.short_input_sats, SHORT_INPUT_SATS_AS_LEVERAGED_SHORT)
 
     def test_total_input_sats_for_leveraged_short(self):
         self.assertEqual(self.leveraged_short.total_input_sats, TOTAL_INPUT_SATS_AS_LEVERAGED_SHORT)
```

### Comparing `anyhedge-0.3.4/anyhedge/tests/test_fee.py` & `anyhedge-0.3.5/anyhedge/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/anyhedge/tests/test_oracle.py` & `anyhedge-0.3.5/anyhedge/tests/test_oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/anyhedge.egg-info/PKG-INFO` & `anyhedge-0.3.5/anyhedge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.3.4
+Version: 0.3.5
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.3.4/anyhedge.egg-info/SOURCES.txt` & `anyhedge-0.3.5/anyhedge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyhedge-0.3.4/pyproject.toml` & `anyhedge-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'anyhedge'
-version = '0.3.4'
+version = '0.3.5'
 authors = [
   { name='emergent_reasons', email='emergent_reasons@gmail.com' },
 ]
 license = { file = "LICENSE" }
 description = 'Basic components of AnyHedge contracts'
 readme = 'README.md'
 requires-python = '>=3.10'
```

