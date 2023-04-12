# Comparing `tmp/anyhedge-0.1.3.tar.gz` & `tmp/anyhedge-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyhedge-0.1.3.tar", last modified: Mon Apr  3 13:51:44 2023, max compression
+gzip compressed data, was "anyhedge-0.3.4.tar", last modified: Wed Apr 12 09:42:36 2023, max compression
```

## Comparing `anyhedge-0.1.3.tar` & `anyhedge-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-03 13:51:44.244826 anyhedge-0.1.3/
--rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.1.3/LICENSE
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-03 13:51:44.244826 anyhedge-0.1.3/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.1.3/README.md
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-03 13:51:44.240826 anyhedge-0.1.3/anyhedge/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.1.3/anyhedge/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2352 2022-11-18 19:46:07.000000 anyhedge-0.1.3/anyhedge/bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    21890 2023-03-16 15:28:21.000000 anyhedge-0.1.3/anyhedge/contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2228 2022-11-18 20:38:49.000000 anyhedge-0.1.3/anyhedge/fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.1.3/anyhedge/javascript.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    13667 2023-04-03 13:47:42.000000 anyhedge-0.1.3/anyhedge/oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      277 2023-03-16 14:59:33.000000 anyhedge-0.1.3/anyhedge/role.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3564 2022-11-18 23:32:45.000000 anyhedge-0.1.3/anyhedge/test_bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    26519 2023-03-16 15:28:21.000000 anyhedge-0.1.3/anyhedge/test_contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     1194 2022-11-18 23:32:19.000000 anyhedge-0.1.3/anyhedge/test_fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3783 2022-11-24 23:39:48.000000 anyhedge-0.1.3/anyhedge/test_oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.1.3/anyhedge/validators.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-03 13:51:44.244826 anyhedge-0.1.3/anyhedge.egg-info/
--rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-03 13:51:44.000000 anyhedge-0.1.3/anyhedge.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)      461 2023-04-03 13:51:44.000000 anyhedge-0.1.3/anyhedge.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-03 13:51:44.000000 anyhedge-0.1.3/anyhedge.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-03 13:51:44.000000 anyhedge-0.1.3/anyhedge.egg-info/requires.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-03 13:51:44.000000 anyhedge-0.1.3/anyhedge.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-03 13:49:15.000000 anyhedge-0.1.3/pyproject.toml
--rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-03 13:51:44.244826 anyhedge-0.1.3/setup.cfg
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.305355 anyhedge-0.3.4/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-0.3.4/LICENSE
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 09:42:36.305355 anyhedge-0.3.4/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-0.3.4/README.md
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.301355 anyhedge-0.3.4/anyhedge/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-0.3.4/anyhedge/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2358 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    27899 2023-04-12 09:41:55.000000 anyhedge-0.3.4/anyhedge/contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-0.3.4/anyhedge/javascript.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    13696 2023-04-12 09:41:55.000000 anyhedge-0.3.4/anyhedge/oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      303 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/role.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.305355 anyhedge-0.3.4/anyhedge/tests/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/test_bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    30745 2023-04-12 09:41:55.000000 anyhedge-0.3.4/anyhedge/tests/test_contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/test_fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-0.3.4/anyhedge/tests/test_oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-0.3.4/anyhedge/validators.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2023-04-12 09:42:36.301355 anyhedge-0.3.4/anyhedge.egg-info/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3620 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)      512 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        1 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)       57 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/requires.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        9 2023-04-12 09:42:36.000000 anyhedge-0.3.4/anyhedge.egg-info/top_level.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)      798 2023-04-12 09:41:55.000000 anyhedge-0.3.4/pyproject.toml
+-rw-rw-r--   0 alien     (1000) alien     (1000)       38 2023-04-12 09:42:36.305355 anyhedge-0.3.4/setup.cfg
```

### Comparing `anyhedge-0.1.3/LICENSE` & `anyhedge-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anyhedge-0.1.3/PKG-INFO` & `anyhedge-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.1.3
+Version: 0.3.4
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.1.3/README.md` & `anyhedge-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `anyhedge-0.1.3/anyhedge/bch_primitives.py` & `anyhedge-0.3.4/anyhedge/bch_primitives.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 SCRIPT_INT_MAX_WHEN_JAVASCRIPT = int(2 ** 53)
 SATS_PER_BCH = int(1e8)
 MAX_REASONABLE_SATS = int(10e6 * SATS_PER_BCH)  # 10 million BCH
 MIN_NLOCKTIME_TIMESTAMP = 500_000_000
 
 
 class PublicKey(str):
-    """Validated BCH public key that can be used as a string."""
+    """Validated BCH-VM public key that can be used as a string."""
     def __init__(self, value):
         super().__init__()
 
         # don't allow silent coercion
         validators.instance(value, str)
 
         # use a strict format
@@ -32,15 +32,15 @@
 
         # require strict length
         if len(self) != 2 * PUBLIC_KEY_BYTES_LENGTH:
             raise ValueError(f'public key should be 33 bytes but got {len(self) / 2} ({self})')
 
 
 class ScriptTimestamp(int):
-    """Validated BCH timestamp (seconds) that can be used as an integer."""
+    """Validated BCH-VM timestamp (seconds) that can be used as an integer."""
     def __init__(self, value):
         super().__init__()
         validators.instance(value, int)  # i.e. don't allow silent coercion
         validators.less_equal(self, SCRIPT_INT_MAX_WHEN_JAVASCRIPT)
         validators.greater_equal(self, MIN_NLOCKTIME_TIMESTAMP)
 
     def __str__(self):
```

### Comparing `anyhedge-0.1.3/anyhedge/contract.py` & `anyhedge-0.3.4/anyhedge/contract.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Built-in imports
 from __future__ import annotations  # allow pre-definition use of types
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
-from math import ceil
+from math import ceil, floor
 from typing import Type
 
 # Local imports
 from . import validators
 from .bch_primitives import (
     DUST,
     SATS_PER_BCH,
@@ -31,42 +31,52 @@
 
 
 class UnredeemableError(Exception):
     pass
 
 
 class Side(str, Enum):
-    HEDGE = 'Hedge'
+    SHORT = 'Short'
     LONG = 'Long'
 
     def __str__(self):
         return self.value
 
     def __repr__(self):
         return self.__str__()
 
     @property
     def other_side(self) -> Side:
         # use a lookup to ensure KeyError with unknown value
-        return {Side.HEDGE: Side.LONG, Side.LONG: Side.HEDGE}[self]
+        return {Side.SHORT: Side.LONG, Side.LONG: Side.SHORT}[self]
 
     @classmethod
     def from_string(cls, side_string: str) -> Side:
         # use a lookup to ensure KeyError with unknown value
-        return {'hedge': cls.HEDGE, 'long': cls.LONG}[side_string.lower()]
+        return {'short': cls.SHORT, 'long': cls.LONG}[side_string.lower()]
 
 
 class NominalOracleUnitsXSatsPerBch(int):
     def __init__(self, value):
         super().__init__()
         validators.instance(value, int)  # i.e. don't allow silent coercion
         validators.less_equal(self, SCRIPT_INT_MAX_WHEN_JAVASCRIPT)
         validators.greater_equal(self, SATS_PER_BCH)  # i.e. minimum is 1 nominal oracle unit
 
 
+class ShortLeverage(float):
+    min_allowed: float = 1.0
+    max_allowed: float = 50.0
+
+    def __init__(self, _):
+        super().__init__()
+        validators.less_equal(self, self.max_allowed * 1.00001)  # some room for floating point error
+        validators.greater_equal(self, self.min_allowed)  # strict boundary for flat hedge position, below one is undefined
+
+
 class LongLeverage(float):
     min_allowed: float = 1.1
     max_allowed: float = 50.0
 
     def __init__(self, _):
         super().__init__()
         validators.less_equal(self, self.max_allowed * 1.00001)  # some room for floating point error
@@ -95,53 +105,61 @@
     """Details of a proposed contract between a maker and taker. Does not include any funding oriented details such as fees."""
     # Time
     start_timestamp: ScriptTimestamp
     maturity_timestamp: ScriptTimestamp
 
     # Position settings
     nominal_oracleUnits_x_satsPerBch: NominalOracleUnitsXSatsPerBch
+    cost_sats_for_nominal_value_at_short_liquidation: Sats
+    total_input_sats: UtxoSats
 
     # Start price is not an actual contract parameter, but one of start price, leverage,
     # or separated side inputs are needed in order for the contract to be fully specified.
     start_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch
+
+    # Liquidation prices
+    short_liquidation_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch
     long_liquidation_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch
+
+    # Price oracle
     oracle_public_key: PublicKey
 
     # Relationship between Roles and Sides
     maker_side: Side
 
     def __post_init__(self):
         # Note: can make validation a switch with unsafe construction if needed
         self.validate()
 
     ###############
     # Parameterized Input Values
     ###############
     @cached_property
     def _input_sats_lookup(self) -> dict[(Role | None, Side | None), UtxoSats | None]:
-        # Total input sats is basically the definition of an AnyHedge contract
-        total_input_sats = UtxoSats(ceil(self.nominal_oracleUnits_x_satsPerBch / self.long_liquidation_price_oracleUnits_per_bch))
+        # Total sats is a hard contract parameter established by whatever method during construction.
+        # Here we split it back into its two parts: short side, and for strict numerical safety, everything else as long side
 
-        # Hedge input sats defines the starting point
-        # Round gets a potentially slightly more accurate number.
-        # The precision to zero-sum comes from defining long position as "everything else needed to cover liquidation".
-        hedge_input_sats = UtxoSats(round_half_up(self.nominal_oracleUnits_x_satsPerBch / self.start_price_oracleUnits_per_bch))
+        # The definition of short's input is that it needs to be enough to fully cover the worst case outcome of selling low
+        # and buying high. That amount is the difference between the cost of the nominal assets at short/high liquidation vs
+        # the cost at the start price. Note that in our inverted price scheme of BCH/Asset, the lower cost is at the higher price.
+        cost_sats_for_nominal_value_at_start = UtxoSats(round_half_up(self.nominal_oracleUnits_x_satsPerBch / self.start_price_oracleUnits_per_bch))
+        short_input_sats = UtxoSats(cost_sats_for_nominal_value_at_start - self.cost_sats_for_nominal_value_at_short_liquidation)
 
-        # Long input sats is just everything needed to cover the rest of the total
-        long_input_sats = UtxoSats(total_input_sats - hedge_input_sats)
+        # Long input sats is everything needed to cover the rest of the total
+        long_input_sats = UtxoSats(self.total_input_sats - short_input_sats)
 
         return {
-            (None,       None):       total_input_sats,
-            (None,       Side.HEDGE): hedge_input_sats,
+            (None,       None):       self.total_input_sats,
+            (None,       Side.SHORT): short_input_sats,
             (None,       Side.LONG):  long_input_sats,
-            (Role.MAKER, None):       hedge_input_sats if self.maker_side == Side.HEDGE else long_input_sats,
-            (Role.MAKER, Side.HEDGE): hedge_input_sats if self.maker_side == Side.HEDGE else None,
+            (Role.MAKER, None):       short_input_sats if self.maker_side == Side.SHORT else long_input_sats,
+            (Role.MAKER, Side.SHORT): short_input_sats if self.maker_side == Side.SHORT else None,
             (Role.MAKER, Side.LONG):  long_input_sats  if self.maker_side == Side.LONG  else None,
-            (Role.TAKER, None):       hedge_input_sats if self.taker_side == Side.HEDGE else long_input_sats,
-            (Role.TAKER, Side.HEDGE): hedge_input_sats if self.taker_side == Side.HEDGE else None,
+            (Role.TAKER, None):       short_input_sats if self.taker_side == Side.SHORT else long_input_sats,
+            (Role.TAKER, Side.SHORT): short_input_sats if self.taker_side == Side.SHORT else None,
             (Role.TAKER, Side.LONG):  long_input_sats  if self.taker_side == Side.LONG  else None,
         }
 
     def input_sats(self, role: Role | None = None, side: Side | None = None) -> UtxoSats:
         key = (role, side)
         value = self._input_sats_lookup[key]
         if value is None:
@@ -157,40 +175,52 @@
     # Derivative values
     ###############
     @property
     def oracle_unit_cls(self) -> Type[OracleUnit]:
         return oracle_pubkey_to_unit_class[self.oracle_public_key]
 
     @property
-    def short_liquidation_price_oracleUnits_per_bch(self) -> ScriptPriceInOracleUnitsPerBch | None:
-        # Until two-sided leverage is enabled in AnyHedge, this is always None
-        return None
-
-    @property
     def duration_seconds(self) -> int:
         return self.maturity_timestamp - self.start_timestamp
 
     @property
+    def effective_short_leverage(self) -> ShortLeverage:
+        # There is a special case where even if the liquidation price must be recorded at some max value,
+        # The fundamental cost for the position at liquidation is hard-lined at zero. That is the definition
+        # of a hard hedge position, emulating the original anyhedge contract behavior.
+        if self.cost_sats_for_nominal_value_at_short_liquidation == 0:
+            return ShortLeverage(1)
+
+        # Derivation of the calculation:
+        #   short liq price = start price (1 + 1 / (short leverage - 1))
+        #   1 + 1 / (short leverage - 1) = short liq price / start price
+        #   1 / (short leverage - 1) = (short liq price / start price) - 1
+        #   short leverage - 1 = 1 / ((short liq price / start price) - 1)
+        #   short leverage = 1 + 1 / ((short liq price / start price) - 1)
+        return ShortLeverage(1 + 1 / (self.short_liquidation_price_oracleUnits_per_bch / self.start_price_oracleUnits_per_bch - 1))
+
+    @property
     def effective_long_leverage(self) -> LongLeverage:
+        # Derivation of the calculation:
+        #   long liq price = start price (1 - 1 / long leverage)
+        #   1 - 1 / long leverage = long liq price / start price
+        #   1 / long leverage = 1 - (long liq price / start price)
+        #   long leverage = 1 / (1 - (long liq price / start price))
         return LongLeverage(1 / (1 - self.long_liquidation_price_oracleUnits_per_bch / self.start_price_oracleUnits_per_bch))
 
     @property
     def taker_side(self) -> Side:
         return self.maker_side.other_side
 
     ###############
     # Property access to input sats
     ###############
     @property
-    def total_input_sats(self) -> UtxoSats:
-        return self.input_sats()
-
-    @property
-    def hedge_input_sats(self) -> UtxoSats:
-        return self.input_sats(side=Side.HEDGE)
+    def short_input_sats(self) -> UtxoSats:
+        return self.input_sats(side=Side.SHORT)
 
     @property
     def long_input_sats(self) -> UtxoSats:
         return self.input_sats(side=Side.LONG)
 
     @property
     def maker_input_sats(self) -> UtxoSats:
@@ -204,16 +234,16 @@
     # Property access to unit conversions of inputs
     ###############
     @property
     def total_input_oracleUnits(self) -> OracleUnit:
         return self.input_oracleUnits()
 
     @property
-    def hedge_input_oracleUnits(self) -> OracleUnit:
-        return self.input_oracleUnits(side=Side.HEDGE)
+    def short_input_oracleUnits(self) -> OracleUnit:
+        return self.input_oracleUnits(side=Side.SHORT)
 
     @property
     def long_input_oracleUnits(self) -> OracleUnit:
         return self.input_oracleUnits(side=Side.LONG)
 
     @property
     def maker_input_oracleUnits(self) -> OracleUnit:
@@ -229,23 +259,59 @@
     @staticmethod
     def new_from_intent(start_timestamp: ScriptTimestamp,
                         maturity_timestamp: ScriptTimestamp,
                         nominal_oracleUnits: OracleUnit,
                         long_leverage: LongLeverage,
                         start_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch,
                         maker_side: Side,
+                        # For upgrade to leveraged shorts, we establish a default of 1 representing the pure hedge position
+                        short_leverage: ShortLeverage = ShortLeverage(1),
                         ) -> ContractProposal:
         nominal_oracleUnits_x_satsPerBch = NominalOracleUnitsXSatsPerBch(round_half_up(nominal_oracleUnits * SATS_PER_BCH))
-        low_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(float(start_price_oracleUnits_per_bch) * (1 - 1 / long_leverage)))
+
+        try:
+            # Short liquidation price is a hard contract parameter, and is also used as a base number to derive other contract details.
+            # We calculate short liquidation price from the more abstract leverage input and then discard leverage.
+            # Short liquidation price is rounded for accuracy - in the contract it's used as for testing, but not calculations
+            short_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(float(start_price_oracleUnits_per_bch) * (1 + 1 / (short_leverage - 1))))
+
+            # Each side of the contract has a worst-case price (the liquidation price) at which it needs to be able to settle the contract.
+            # In nominal terms, there is a full cost for that position, but in input/output terms, the counterparties only need to cover the difference in cost.
+            # In order to achieve the simplest possible in-contract calculation, we use the full cost for short liquidation price as a contract parameter.
+            # cost is floored for safety - it's a hard contract value subtracted from another during contract execution, and that result must never be a negative number
+            cost_sats_for_nominal_value_at_short_liquidation = Sats(floor(nominal_oracleUnits_x_satsPerBch / short_liquidation_price_oracleUnits_per_bch))
+        except ZeroDivisionError:
+            # For short leverage exactly 1 (or any floating point result that still causes the error), the implication
+            # is that short liquidation is at infinity on a continuous number line. However, for the contract purposes,
+            # we need a concrete test price for liquidation and the cost value. We establish those directly:
+            short_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch.largest_allowed()
+            cost_sats_for_nominal_value_at_short_liquidation = Sats(0)
+
+        # Long liquidation has the same considerations as short liquidation above, except long leverage of 1 is strictly disallowed,
+        # avoiding the problem of a zero price, infinite cost. Note that a short leverage of 1 is useful in the sense that it gives the short
+        # party the equivalent of simply holding another asset, while long leverage of 1 is nonsensical in that it gives the long
+        # the equivalent of simply holding the underlying asset (BCH) which by definition they already have.
+        long_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(float(start_price_oracleUnits_per_bch) * (1 - 1 / long_leverage)))
+
+        # Cost at long liquidation has the same considerations as short liquidation above, except we are on the opposite side so we use ceil to be conservative instead of floor
+        cost_sats_for_nominal_value_at_long_liquidation = UtxoSats(ceil(nominal_oracleUnits_x_satsPerBch / long_liquidation_price_oracleUnits_per_bch))
+
+        # Total input sats is the total of the two party's required amounts. In the contract base terms that we are using, it is the difference between
+        # the cost at the two liquidation points
+        total_input_sats = UtxoSats(cost_sats_for_nominal_value_at_long_liquidation - cost_sats_for_nominal_value_at_short_liquidation)
+
         return ContractProposal(
             start_timestamp=start_timestamp,
             maturity_timestamp=maturity_timestamp,
             nominal_oracleUnits_x_satsPerBch=nominal_oracleUnits_x_satsPerBch,
+            cost_sats_for_nominal_value_at_short_liquidation=cost_sats_for_nominal_value_at_short_liquidation,
+            total_input_sats=total_input_sats,
             start_price_oracleUnits_per_bch=start_price_oracleUnits_per_bch,
-            long_liquidation_price_oracleUnits_per_bch=low_liquidation_price_oracleUnits_per_bch,
+            short_liquidation_price_oracleUnits_per_bch=short_liquidation_price_oracleUnits_per_bch,
+            long_liquidation_price_oracleUnits_per_bch=long_liquidation_price_oracleUnits_per_bch,
             oracle_public_key=nominal_oracleUnits.public_key,
             maker_side=maker_side,
         )
 
     def fund(self, fee_agreements: list[FeeAgreement]) -> ContractFunding:
         return ContractFunding(
             base_proposal=self,
@@ -270,16 +336,16 @@
         return aggregate_fee_sats_to_role(self.fee_agreements, Role.MAKER)
 
     @property
     def fee_sats_to_taker(self) -> Sats:
         return aggregate_fee_sats_to_role(self.fee_agreements, Role.TAKER)
 
     @property
-    def fee_sats_to_hedge(self) -> Sats:
-        if self.base_proposal.maker_side == Side.HEDGE:
+    def fee_sats_to_short(self) -> Sats:
+        if self.base_proposal.maker_side == Side.SHORT:
             return self.fee_sats_to_maker
         return self.fee_sats_to_taker
 
     @property
     def fee_sats_to_long(self) -> Sats:
         if self.base_proposal.maker_side == Side.LONG:
             return self.fee_sats_to_maker
@@ -297,16 +363,16 @@
     @property
     def fee_oracleUnits_to_taker(self) -> OracleUnit:
         fee_bch = self.fee_sats_to_taker.bch
         fee_oracleUnits = self.base_proposal.oracle_unit_cls(fee_bch * float(self.base_proposal.start_price_oracleUnits_per_bch))
         return fee_oracleUnits
 
     @property
-    def fee_oracleUnits_to_hedge(self) -> OracleUnit:
-        if self.base_proposal.maker_side == Side.HEDGE:
+    def fee_oracleUnits_to_short(self) -> OracleUnit:
+        if self.base_proposal.maker_side == Side.SHORT:
             return self.fee_oracleUnits_to_maker
         return self.fee_oracleUnits_to_taker
 
     @property
     def fee_oracleUnits_to_long(self) -> OracleUnit:
         if self.base_proposal.maker_side == Side.LONG:
             return self.fee_oracleUnits_to_maker
@@ -318,15 +384,19 @@
     def redeem(self,
                price_timestamp: ScriptTimestamp,
                price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch,
                force_maturity: bool,
                ) -> ContractRedemption:
         """Redeem the contract according to market conditions or raise an unredeemable error for invalid conditions."""
         reached_maturity_time = price_timestamp >= self.base_proposal.maturity_timestamp
-        reached_liquidation_price = price_oracleUnits_per_bch <= self.base_proposal.long_liquidation_price_oracleUnits_per_bch
+        reached_liquidation_price = (
+                price_oracleUnits_per_bch <= self.base_proposal.long_liquidation_price_oracleUnits_per_bch
+                or
+                price_oracleUnits_per_bch >= self.base_proposal.short_liquidation_price_oracleUnits_per_bch
+        )
         if reached_maturity_time or force_maturity:
             # Maturation, even in the case of a liquidation price
             return ContractRedemption(
                 base_funding=self,
                 end_price_timestamp=price_timestamp,
                 naive_end_price_oracleUnits_per_bch=price_oracleUnits_per_bch,
                 redemption_type=RedemptionType.MATURATION,
@@ -357,39 +427,43 @@
     ###############
     @cached_property
     def _payout_sats_lookup(self) -> dict[(Role | None, Side | None), UtxoSats | None]:
         # Hedge payout sats is the payout side of the fundamental definition of an AnyHedge contract
         # Note that due to dust safety in the contract, the total actual payout can be greater than total inputs.
         # In reality, the extra dust is covered by an amount sitting on the contract that the contract is not aware of.
         # Use divmod (instead of //) to make it crystal clear this represents integer division of the contract.
-        unsafe_hedge_payout_sats, _ = divmod(self.base_funding.base_proposal.nominal_oracleUnits_x_satsPerBch, self.clamped_end_price_oracleUnits_per_bch)
-        hedge_payout_sats = UtxoSats(max(DUST, unsafe_hedge_payout_sats))
+        _unsafe_hedge_payout_sats, _ = divmod(self.base_funding.base_proposal.nominal_oracleUnits_x_satsPerBch, self.clamped_end_price_oracleUnits_per_bch)
+
+        # With leveraged shorts, the short is no longer necessarily paying out the full value of the nominal position.
+        # If short leverage is not 1, the short only pays up to the planned liquidation point
+        unsafe_short_payout_sats = _unsafe_hedge_payout_sats - self.base_funding.base_proposal.cost_sats_for_nominal_value_at_short_liquidation
+        short_payout_sats = UtxoSats(max(DUST, unsafe_short_payout_sats))
 
         # Long Payout Sats
-        unsafe_long_payout_sats = self.base_funding.base_proposal.total_input_sats - hedge_payout_sats
+        unsafe_long_payout_sats = self.base_funding.base_proposal.total_input_sats - short_payout_sats
         long_payout_sats = UtxoSats(max(DUST, unsafe_long_payout_sats))
 
-        # Total payout sats is just the combination of hedge and long
+        # Total payout sats is just the combination of short and long
         # Note: This can be different from total input in the case of liquidation where dust protection is pulled in from outside the contract
-        # Any extra dust is covered by an amount sitting on the contract that the contract is not aware of.
-        total_payout_sats = UtxoSats(hedge_payout_sats + long_payout_sats)
+        # Any extra dust is covered by an amount sitting on the contract's utxo that the contract is not aware of.
+        total_payout_sats = UtxoSats(short_payout_sats + long_payout_sats)
 
         # visual shortcut for the maker/taker sides
         maker_side = self.base_funding.base_proposal.maker_side
         taker_side = self.base_funding.base_proposal.taker_side
 
         return {
             (None,       None):       total_payout_sats,
-            (None,       Side.HEDGE): hedge_payout_sats,
+            (None,       Side.SHORT): short_payout_sats,
             (None,       Side.LONG):  long_payout_sats,
-            (Role.MAKER, None):       hedge_payout_sats if maker_side == Side.HEDGE else long_payout_sats,
-            (Role.MAKER, Side.HEDGE): hedge_payout_sats if maker_side == Side.HEDGE else None,
+            (Role.MAKER, None):       short_payout_sats if maker_side == Side.SHORT else long_payout_sats,
+            (Role.MAKER, Side.SHORT): short_payout_sats if maker_side == Side.SHORT else None,
             (Role.MAKER, Side.LONG):  long_payout_sats  if maker_side == Side.LONG  else None,
-            (Role.TAKER, None):       hedge_payout_sats if taker_side == Side.HEDGE else long_payout_sats,
-            (Role.TAKER, Side.HEDGE): hedge_payout_sats if taker_side == Side.HEDGE else None,
+            (Role.TAKER, None):       short_payout_sats if taker_side == Side.SHORT else long_payout_sats,
+            (Role.TAKER, Side.SHORT): short_payout_sats if taker_side == Side.SHORT else None,
             (Role.TAKER, Side.LONG):  long_payout_sats  if taker_side == Side.LONG  else None,
         }
 
     def payout_sats(self, role: Role | None = None, side: Side | None = None) -> UtxoSats:
         key = (role, side)
         value = self._payout_sats_lookup[key]
         if value is None:
@@ -413,16 +487,16 @@
     # Property access to payout sats
     ###############
     @property
     def total_payout_sats(self) -> UtxoSats:
         return self.payout_sats()
 
     @property
-    def hedge_payout_sats(self) -> UtxoSats:
-        return self.payout_sats(side=Side.HEDGE)
+    def short_payout_sats(self) -> UtxoSats:
+        return self.payout_sats(side=Side.SHORT)
 
     @property
     def long_payout_sats(self) -> UtxoSats:
         return self.payout_sats(side=Side.LONG)
 
     @property
     def maker_payout_sats(self) -> UtxoSats:
@@ -436,16 +510,16 @@
     # Property access to unit conversions of payouts
     ###############
     @property
     def total_payout_oracleUnits(self) -> OracleUnit:
         return self.payout_oracleUnits()
 
     @property
-    def hedge_payout_oracleUnits(self) -> OracleUnit:
-        return self.payout_oracleUnits(side=Side.HEDGE)
+    def short_payout_oracleUnits(self) -> OracleUnit:
+        return self.payout_oracleUnits(side=Side.SHORT)
 
     @property
     def long_payout_oracleUnits(self) -> OracleUnit:
         return self.payout_oracleUnits(side=Side.LONG)
 
     @property
     def maker_payout_oracleUnits(self) -> OracleUnit:
@@ -456,34 +530,34 @@
         return self.payout_oracleUnits(role=Role.TAKER)
 
     ###############
     # Gains - see funding class for details of fee and gain calculations
     # TODO: These could also be parameterized with a lookup
     ###############
     @property
-    def hedge_gain_sats(self) -> Sats:
-        payout_sats = self.hedge_payout_sats
-        input_sats = self.base_funding.base_proposal.hedge_input_sats
-        fee_sats = self.base_funding.fee_sats_to_hedge
+    def short_gain_sats(self) -> Sats:
+        payout_sats = self.short_payout_sats
+        input_sats = self.base_funding.base_proposal.short_input_sats
+        fee_sats = self.base_funding.fee_sats_to_short
         return Sats(payout_sats - input_sats + fee_sats)
 
     @property
     def long_gain_sats(self) -> Sats:
         payout_sats = self.long_payout_sats
         input_sats = self.base_funding.base_proposal.long_input_sats
         fee_sats = self.base_funding.fee_sats_to_long
         return Sats(payout_sats - input_sats + fee_sats)
 
     @property
-    def hedge_gain_oracleUnits(self) -> OracleUnit:
+    def short_gain_oracleUnits(self) -> OracleUnit:
         # Note that this is not the same as (end sats - start sats) * end price. start value depends on start price.
         # Note that we use naive end price. This represents reality of slippage in liquidations.
-        payout_oracleUnits = self.hedge_payout_oracleUnits
-        input_oracleUnits = self.base_funding.base_proposal.hedge_input_oracleUnits
-        fee_oracleUnits = self.base_funding.fee_oracleUnits_to_hedge
+        payout_oracleUnits = self.short_payout_oracleUnits
+        input_oracleUnits = self.base_funding.base_proposal.short_input_oracleUnits
+        fee_oracleUnits = self.base_funding.fee_oracleUnits_to_short
         return self.base_funding.base_proposal.oracle_unit_cls(payout_oracleUnits - input_oracleUnits + fee_oracleUnits)
 
     @property
     def long_gain_oracleUnits(self) -> OracleUnit:
         # Note that this is not the same as (end sats - start sats) * end price. start value depends on start price.
         # Note that we use naive end price. This represents reality of slippage in liquidations.
         payout_oracleUnits = self.long_payout_oracleUnits
@@ -491,52 +565,52 @@
         fee_oracleUnits = self.base_funding.fee_oracleUnits_to_long
         return self.base_funding.base_proposal.oracle_unit_cls(payout_oracleUnits - input_oracleUnits + fee_oracleUnits)
 
     ###############
     # Relative gains
     ###############
     @property
-    def hedge_gain_percent_of_own_input(self) -> float:
-        return 100.0 * float(self.hedge_gain_sats) / float(self.base_funding.base_proposal.hedge_input_sats)
+    def short_gain_percent_of_own_input(self) -> float:
+        return 100.0 * float(self.short_gain_sats) / float(self.base_funding.base_proposal.short_input_sats)
 
     @property
     def long_gain_percent_of_own_input(self) -> float:
         return 100.0 * float(self.long_gain_sats) / float(self.base_funding.base_proposal.long_input_sats)
 
     ###############
     # Sided views on gains
     ###############
     @property
     def maker_gain_sats(self) -> Sats:
-        if self.base_funding.base_proposal.maker_side == Side.HEDGE:
-            return self.hedge_gain_sats
+        if self.base_funding.base_proposal.maker_side == Side.SHORT:
+            return self.short_gain_sats
         return self.long_gain_sats
 
     @property
     def taker_gain_sats(self) -> Sats:
-        if self.base_funding.base_proposal.taker_side == Side.HEDGE:
-            return self.hedge_gain_sats
+        if self.base_funding.base_proposal.taker_side == Side.SHORT:
+            return self.short_gain_sats
         return self.long_gain_sats
 
     @property
     def maker_gain_oracleUnits(self) -> OracleUnit:
-        if self.base_funding.base_proposal.maker_side == Side.HEDGE:
-            return self.hedge_gain_oracleUnits
+        if self.base_funding.base_proposal.maker_side == Side.SHORT:
+            return self.short_gain_oracleUnits
         return self.long_gain_oracleUnits
 
     @property
     def taker_gain_oracleUnits(self) -> OracleUnit:
-        if self.base_funding.base_proposal.taker_side == Side.HEDGE:
-            return self.hedge_gain_oracleUnits
+        if self.base_funding.base_proposal.taker_side == Side.SHORT:
+            return self.short_gain_oracleUnits
         return self.long_gain_oracleUnits
 
     @property
     def maker_gain_percent_of_own_input(self) -> float:
-        if self.base_funding.base_proposal.maker_side == Side.HEDGE:
-            return self.hedge_gain_percent_of_own_input
+        if self.base_funding.base_proposal.maker_side == Side.SHORT:
+            return self.short_gain_percent_of_own_input
         return self.long_gain_percent_of_own_input
 
     @property
     def taker_gain_percent_of_own_input(self) -> float:
-        if self.base_funding.base_proposal.taker_side == Side.HEDGE:
-            return self.hedge_gain_percent_of_own_input
+        if self.base_funding.base_proposal.taker_side == Side.SHORT:
+            return self.short_gain_percent_of_own_input
         return self.long_gain_percent_of_own_input
```

### Comparing `anyhedge-0.1.3/anyhedge/fee.py` & `anyhedge-0.3.4/anyhedge/fee.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # TODO: make an aggregate "FeeAgreements" that packs them up and makes them available in parts if desired
 #       or in total with full consistency between parts and total. i.e. no discrepancy between total and sum of parts
 
 
 @dataclass(frozen=True)
 class FeeRequirement:
     name: str
-    amount_sats: Sats
     # note that amount can be negative indicating the "to" role is paying, not receiving
+    amount_sats: Sats
     receiving: Role
 
     def __str__(self):
         return f'FeeRequirement ({self.name}): ____ --> {self.amount_sats} Sats ({self.amount_sats.bch} BCH) --> {self.receiving}'
 
     def __repr__(self):
         return self.__str__()
@@ -56,19 +56,19 @@
 
 def fees_to_role(
         fees: Sequence[FeeAgreement],
         role: Role,
         fee_name: str | None = None) -> list[FeeAgreement]:
     return [
         fee for fee in fees
-        if (fee.receiving == role) and ((fee_name is None) or fee.name == fee_name)
+        if (fee.receiving == role) and ((fee_name is None) or (fee.name == fee_name))
     ]
 
 
 def fees_from_role(
         fees: Sequence[FeeAgreement],
         role: Role,
         fee_name: str | None = None) -> list[FeeAgreement]:
     return [
         fee for fee in fees
-        if (fee.paying == role) and ((fee_name is None) or fee.name == fee_name)
+        if (fee.paying == role) and ((fee_name is None) or (fee.name == fee_name))
     ]
```

### Comparing `anyhedge-0.1.3/anyhedge/oracle.py` & `anyhedge-0.3.4/anyhedge/oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,17 +186,14 @@
             return False
         if self.public_key != other.public_key:
             return False
         if float(self) != float(other):
             return False
         return True
 
-    def __hash__(self):
-        return self.public_key
-
     @property
     def in_standard_units(self) -> float:
         return float(self) / self.oracleUnits_per_standardUnit
 
 
 class ScriptPriceInOracleUnitsPerBch(int):
     def __new__(cls, value, *args, **kwargs):
@@ -204,14 +201,18 @@
 
     def __init__(self, value):
         super().__init__()
         validators.instance(value, int)  # i.e. don't allow silent coercion
         validators.less_equal(self, ORACLE_MAX_PRICE)
         validators.greater_equal(self, 1)
 
+    @classmethod
+    def largest_allowed(cls):
+        return cls(ORACLE_MAX_PRICE)
+
 
 # GP Oracles
 class BtcEM6(OracleUnit):
     name_of_oracleUnits = 'BTC(e-6)'
     name_of_standardUnits = 'BTC'
     oracleUnits_per_standardUnit = 1000000
     public_key = PublicKey('0245a107de5c6aabc9e7b976f26625b01474f90d1a7d11c180bec990b6938e731e')
```

### Comparing `anyhedge-0.1.3/anyhedge/test_bch_primitives.py` & `anyhedge-0.3.4/anyhedge/tests/test_bch_primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Built-in imports
 import unittest
 
 # Local imports
-from . import bch_primitives as bchp
+from .. import bch_primitives as bchp
 
 
 VALID_PUBLIC_KEY_HEX = '0123456789abcdef0123456789ABCDEF0123456789abcdef0123456789abcdef01'
 VALID_TIMESTAMP_INT = 5_000_000_000
 VALID_SATS = 1
```

### Comparing `anyhedge-0.1.3/anyhedge/test_contract.py` & `anyhedge-0.3.4/anyhedge/tests/test_contract.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,191 +1,217 @@
 # Built-in imports
 import unittest
 
 # Library imports
 from arrow import Arrow
 
 # Local imports
-from .bch_primitives import (
+from ..bch_primitives import (
     SATS_PER_BCH,
     Sats,
     ScriptTimestamp,
     UtxoSats,
 )
-from .contract import (
+from ..contract import (
     ContractFunding,
     ContractProposal,
     LongLeverage,
     NominalOracleUnitsXSatsPerBch,
     RedemptionType,
+    ShortLeverage,
     Side,
     UnredeemableError,
 )
-from .fee import FeeAgreement
-from .oracle import (
+from ..fee import FeeAgreement
+from ..oracle import (
     OracleUnit,
     ScriptPriceInOracleUnitsPerBch,
     UsdEM2Beta,
 )
-from .role import Role
+from ..role import Role
 
 
 ###################
 # Contract Tests
 ###################
 # Generic intent values, not always perfectly reproducible from the contract
 START_TIMESTAMP = ScriptTimestamp(Arrow(year=2021, month=10, day=21).int_timestamp)
 MATURITY_TIMESTAMP = ScriptTimestamp(Arrow(year=2021, month=10, day=23).int_timestamp)  # 2 days later
-NOMINAL_USDEM2 = UsdEM2Beta(100_00.0)  # $100.00
+NOMINAL_VALUE_USDEM2 = UsdEM2Beta(100_00.0)  # $100.00
 LONG_LEVERAGE = LongLeverage(4.5)
+SHORT_LEVERAGE_1_AS_HEDGE = ShortLeverage(1)
+SHORT_LEVERAGE_NOT_1 = ShortLeverage(2.2)
 START_PRICE_USDEM2_PER_BCH = ScriptPriceInOracleUnitsPerBch(200_00)  # $200.00 / BCH
 
 # Derived values
 
 # The compound nominal value is a giant number stored in the original AnyHedge contract and needed
 # to get around the lack of multiplication by optimizing the contract into a single division operation
-# = NominalOracleUnitsXSatsPerBch(round(NOMINAL_USDEM2 * SATS_PER_BCH))
-DERIVED_NOMINAL_UNITS_X_SATS_PER_BCH = NominalOracleUnitsXSatsPerBch(1_000_000_000_000)
+# = NominalOracleUnitsXSatsPerBch(round(NOMINAL_VALUE_USDEM2 * SATS_PER_BCH))
+NOMINAL_UNITS_X_SATS_PER_BCH = NominalOracleUnitsXSatsPerBch(1_000_000_000_000)
 
-# Long liquidation Price is the price where total bch covers exactly nominal units
-# At this price, the long party is liquidated (has no funds remaining in the contract)
-# Calculate as round(START_PRICE_USDEM2_PER_BCH * (1 - 1 / LONG_LEVERAGE))
-# $155.56 / BCH
-DERIVED_LONG_LIQUIDATION_PRICE = ScriptPriceInOracleUnitsPerBch(155_56)
-
-# Short liquidation Price is the price where the short party is
-# liquidated (has no funds remaining in the contract). In the current design of
-# AnyHedge where hedge is always a 1x short, there is no meaningful short
-# liquidation price. In the real contract, there is a "high" settlement price
-# that can trigger early settlement, but it is an unused contract feature
-# rather than a liquidation price.
-NO_SHORT_LIQUIDATION_PRICE = None
-
-# The bch amount to cover the initial nominal units at the start price
-# = round(NOMINAL_USDEM2 * SATS_PER_BCH / START_PRICE_USDEM2_PER_BCH)
+# Long liquidation Price is the price where all of long's input is consumed to cover short's agreed payout
+# Calculate in terms of leverage intent as round(START_PRICE_USDEM2_PER_BCH * (1 - 1 / LONG_LEVERAGE))
+# 15556 cents/BCH ($155.56 / BCH)
+LONG_LIQUIDATION_PRICE = ScriptPriceInOracleUnitsPerBch(155_56)
+
+# Short liquidation Price is the price where all of short's input is consumed to cover long's agreed payout
+# When short is exactly a 1x short, there is no meaningful liquidation price (infinity) but the stored liquidation price is still
+# used to trigger early settlement. By definition, we set it to the max possible price in the 4 byte oracle price message scheme.
+SHORT_LIQUIDATION_PRICE_AS_HEDGE = ScriptPriceInOracleUnitsPerBch.largest_allowed()
+# In the case of a leveraged short, it is calculated as round(START_PRICE_USDEM2_PER_BCH * (1 + 1 / (SHORT_LEVERAGE_NOT_1 - 1)))
+# 36667 cents/BCH ($366.67 / BCH)
+SHORT_LIQUIDATION_PRICE_AS_LEVERAGED_SHORT = ScriptPriceInOracleUnitsPerBch(366_67)
+
+# Cost of nominal value at short liquidation is a new value that was always zero for pure hedges
+# and therefore not documented explicitly anywhere. With leveraged shorts, short does not always
+# pay the full cost of the nominal value and so the contract needs to track the cost.
+# Fixed for pure hedge at 0
+ZERO_COST_OF_NOMINAL_VALUE_AT_HEDGE_LIQUIDATION = Sats(0)
+# Calculated for leveraged short as floor(NOMINAL_UNITS_X_SATS_PER_BCH / SHORT_LIQUIDATION_PRICE_FOR_LEVERAGED_SHORT)
+COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION = Sats(27_272_479)
+
+# The bch amount to cover the short's payout obligations to long
+# For a pure hedge, it is the full cost of the nominal contract at starting price,
+# effectively allowing the price to increase to any value and still be able to pay out
+# Calculated as round(NOMINAL_UNITS_X_SATS_PER_BCH / START_PRICE_USDEM2_PER_BCH)
 # 0.5 BCH
-DERIVED_HEDGE_INPUT_SATS = UtxoSats(50_000_000)
-
-# The total bch amount needed to cover nominal units at liquidation
-# Calculated as ceil((NOMINAL_USDEM2 * SATS_PER_BCH) / DERIVED_LIQUIDATION_PRICE_UNITS_PER_BCH)
-DERIVED_TOTAL_INPUT_SATS = UtxoSats(64_283_878)
+SHORT_INPUT_SATS_AS_HEDGE = UtxoSats(50_000_000)
+# For a leveraged short, it is the cost at starting price less the cost at short liquidation price
+# Calculated as SHORT_INPUT_SATS_AS_HEDGE - COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION
+SHORT_INPUT_SATS_AS_LEVERAGED_SHORT = UtxoSats(22_727_521)
+
+# Similar to cost at short liquidation, there is also the cost at long liquidation.
+# In the contract, this is not stored anywhere, but it is a useful intermediary for confirming tests.
+# It is the amount needed to cover the nominal unit value at long liquidation price
+# Calculated as ceil((NOMINAL_UNITS_X_SATS_PER_BCH) / DERIVED_LIQUIDATION_PRICE_UNITS_PER_BCH)
+COST_SATS_OF_NOMINAL_VALUE_AT_LONG_LIQUIDATION = UtxoSats(64_283_878)
+
+# The total input sats needed to cover all positions is the sum of the short and long inputs.
+# However, from base contract values, it is the difference between the cost at the two liquidation points
+# For a pure hedge, it has to cover the cost between long liquidation and zero
+TOTAL_INPUT_SATS_AS_HEDGE = COST_SATS_OF_NOMINAL_VALUE_AT_LONG_LIQUIDATION - 0
+# For a leveraged short, it has to cover the cost between long liquidation and short liquidation (which also might be zero)
+# Calculated as COST_SATS_OF_NOMINAL_VALUE_AT_LONG_LIQUIDATION - COST_SATS_OF_NOMINAL_VALUE_AT_SHORT_LIQUIDATION
+TOTAL_INPUT_SATS_AS_LEVERAGED_SHORT = UtxoSats(37_011_399)
 
 # The bch amount to provide volatility protection as specified by the multiplier
-# This is the amount to cover the difference between hedge bch at start and hedge bch at liquidation
-# Calculated as DERIVED_TOTAL_INPUT_SATS - DERIVED_HEDGE_INPUT_SATS
-DERIVED_LONG_INPUT_SATS = UtxoSats(14_283_878)
-
-# Converting the input amounts into original units at start
-# for hedge, it's DERIVED_NOMINAL_UNITS_X_SATS_PER_BCH / SATS_PER_BCH
-DERIVED_HEDGE_INPUT_ORACLE_UNITS = UsdEM2Beta(100_00.0)
-# for long, it's DERIVED_LONG_INPUT_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH
-DERIVED_LONG_INPUT_ORACLE_UNITS = UsdEM2Beta(2856.7756)
-DERIVED_TOTAL_INPUT_ORACLE_UNITS = UsdEM2Beta(DERIVED_HEDGE_INPUT_ORACLE_UNITS + DERIVED_LONG_INPUT_ORACLE_UNITS)
+# This is the amount to cover the difference between payout bch at start and payout bch at long's liquidation price
+# Calculated as DERIVED_TOTAL_INPUT_SATS - SHORT_INPUT_SATS_AS_HEDGE
+LONG_INPUT_SATS = UtxoSats(14_283_878)
+
+# Converting the input amounts into ORACLE units at start
+# for pure hedge, it's NOMINAL_UNITS_X_SATS_PER_BCH / SATS_PER_BCH
+SHORT_INPUT_ORACLE_UNITS_AS_HEDGE = UsdEM2Beta(100_00.0)
+# for long, it's LONG_INPUT_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH
+LONG_INPUT_ORACLE_UNITS = UsdEM2Beta(2856.7756)
+TOTAL_INPUT_ORACLE_UNITS_AS_HEDGE = UsdEM2Beta(SHORT_INPUT_ORACLE_UNITS_AS_HEDGE + LONG_INPUT_ORACLE_UNITS)
 
 
 def standard_contract_proposal(
     start_timestamp: ScriptTimestamp = START_TIMESTAMP,
     maturity_timestamp: ScriptTimestamp = MATURITY_TIMESTAMP,
-    nominal_oracleUnits: OracleUnit = NOMINAL_USDEM2,
+    nominal_oracleUnits: OracleUnit = NOMINAL_VALUE_USDEM2,
     long_leverage: LongLeverage = LONG_LEVERAGE,
     start_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch = START_PRICE_USDEM2_PER_BCH,
-    maker_side: Side = Side.HEDGE,
+    maker_side: Side = Side.SHORT,
+    short_leverage: ShortLeverage = SHORT_LEVERAGE_1_AS_HEDGE,
 ) -> ContractProposal:
     return ContractProposal.new_from_intent(
         start_timestamp=start_timestamp,
         maturity_timestamp=maturity_timestamp,
         nominal_oracleUnits=nominal_oracleUnits,
         long_leverage=long_leverage,
         start_price_oracleUnits_per_bch=start_price_oracleUnits_per_bch,
         maker_side=maker_side,
+        short_leverage=short_leverage,
     )
 
 
 class TestContractProposalDerivedValues(unittest.TestCase):
     ######################
     # Exact contract parameters, some root values, some derived from root values
     ######################
     def test_nominal_oracleUnits_x_satsPerBch(self):
-        self.assertEqual(standard_contract_proposal().nominal_oracleUnits_x_satsPerBch, DERIVED_NOMINAL_UNITS_X_SATS_PER_BCH)
+        self.assertEqual(standard_contract_proposal().nominal_oracleUnits_x_satsPerBch, NOMINAL_UNITS_X_SATS_PER_BCH)
+
+    def test_total_input_sats(self):
+        self.assertEqual(standard_contract_proposal().total_input_sats, TOTAL_INPUT_SATS_AS_HEDGE)
 
     def test_long_liquidation_price_oracleUnits_per_bch(self):
-        self.assertEqual(standard_contract_proposal().long_liquidation_price_oracleUnits_per_bch, DERIVED_LONG_LIQUIDATION_PRICE)
+        self.assertEqual(standard_contract_proposal().long_liquidation_price_oracleUnits_per_bch, LONG_LIQUIDATION_PRICE)
 
     def test_short_liquidation_price_oracleUnits_per_bch(self):
-        # Until two-sided leverage is enabled in AnyHedge, this is always None
-        self.assertEqual(standard_contract_proposal().short_liquidation_price_oracleUnits_per_bch, NO_SHORT_LIQUIDATION_PRICE)
+        self.assertEqual(standard_contract_proposal().short_liquidation_price_oracleUnits_per_bch, SHORT_LIQUIDATION_PRICE_AS_HEDGE)
 
     def test_maker_side(self):
-        self.assertEqual(standard_contract_proposal().maker_side, Side.HEDGE)
+        self.assertEqual(standard_contract_proposal().maker_side, Side.SHORT)
 
     ######################
     # Exact secondary values derived from contract parameters
     ######################
-    def test_hedge_input_sats(self):
-        self.assertEqual(standard_contract_proposal().hedge_input_sats, DERIVED_HEDGE_INPUT_SATS)
-
-    def test_total_input_sats(self):
-        self.assertEqual(standard_contract_proposal().total_input_sats, DERIVED_TOTAL_INPUT_SATS)
+    def test_short_input_sats(self):
+        self.assertEqual(standard_contract_proposal().short_input_sats, SHORT_INPUT_SATS_AS_HEDGE)
 
     def test_long_input_sats(self):
-        self.assertEqual(standard_contract_proposal().long_input_sats, DERIVED_LONG_INPUT_SATS)
+        self.assertEqual(standard_contract_proposal().long_input_sats, LONG_INPUT_SATS)
 
     ######################
     # Reverse calculated intent values from the contract's perspective
     ######################
     def test_effective_long_leverage(self):
         self.assertAlmostEqual(standard_contract_proposal().effective_long_leverage, LONG_LEVERAGE, delta=.001)
 
     ######################
     # Unit values
     ######################
     def test_total_input_oracleUnits(self):
-        self.assertEqual(standard_contract_proposal().total_input_oracleUnits, DERIVED_TOTAL_INPUT_ORACLE_UNITS)
+        self.assertEqual(standard_contract_proposal().total_input_oracleUnits, TOTAL_INPUT_ORACLE_UNITS_AS_HEDGE)
 
-    def test_hedge_input_oracleUnits(self):
-        self.assertEqual(standard_contract_proposal().hedge_input_oracleUnits, DERIVED_HEDGE_INPUT_ORACLE_UNITS)
+    def test_short_input_oracleUnits(self):
+        self.assertEqual(standard_contract_proposal().short_input_oracleUnits, SHORT_INPUT_ORACLE_UNITS_AS_HEDGE)
 
     def test_long_input_oracleUnits(self):
-        self.assertEqual(standard_contract_proposal().long_input_oracleUnits, DERIVED_LONG_INPUT_ORACLE_UNITS)
+        self.assertEqual(standard_contract_proposal().long_input_oracleUnits, LONG_INPUT_ORACLE_UNITS)
 
     ######################
     # Role versions of values
     ######################
     def test_all_sided_values(self):
-        hedge_maker_contract = standard_contract_proposal(maker_side=Side.HEDGE)
-        self.assertEqual(hedge_maker_contract.maker_side, Side.HEDGE)
-        self.assertEqual(hedge_maker_contract.taker_side, Side.LONG)
-        self.assertEqual(hedge_maker_contract.maker_input_sats, DERIVED_HEDGE_INPUT_SATS)
-        self.assertEqual(hedge_maker_contract.taker_input_sats, DERIVED_LONG_INPUT_SATS)
-        self.assertEqual(hedge_maker_contract.maker_input_oracleUnits, DERIVED_HEDGE_INPUT_ORACLE_UNITS)
-        self.assertEqual(hedge_maker_contract.taker_input_oracleUnits, DERIVED_LONG_INPUT_ORACLE_UNITS)
+        short_maker_contract = standard_contract_proposal(maker_side=Side.SHORT)
+        self.assertEqual(short_maker_contract.maker_side, Side.SHORT)
+        self.assertEqual(short_maker_contract.taker_side, Side.LONG)
+        self.assertEqual(short_maker_contract.maker_input_sats, SHORT_INPUT_SATS_AS_HEDGE)
+        self.assertEqual(short_maker_contract.taker_input_sats, LONG_INPUT_SATS)
+        self.assertEqual(short_maker_contract.maker_input_oracleUnits, SHORT_INPUT_ORACLE_UNITS_AS_HEDGE)
+        self.assertEqual(short_maker_contract.taker_input_oracleUnits, LONG_INPUT_ORACLE_UNITS)
 
         long_maker_contract = standard_contract_proposal(maker_side=Side.LONG)
         self.assertEqual(long_maker_contract.maker_side, Side.LONG)
-        self.assertEqual(long_maker_contract.taker_side, Side.HEDGE)
-        self.assertEqual(long_maker_contract.maker_input_sats, DERIVED_LONG_INPUT_SATS)
-        self.assertEqual(long_maker_contract.taker_input_sats, DERIVED_HEDGE_INPUT_SATS)
-        self.assertEqual(long_maker_contract.maker_input_oracleUnits, DERIVED_LONG_INPUT_ORACLE_UNITS)
-        self.assertEqual(long_maker_contract.taker_input_oracleUnits, DERIVED_HEDGE_INPUT_ORACLE_UNITS)
+        self.assertEqual(long_maker_contract.taker_side, Side.SHORT)
+        self.assertEqual(long_maker_contract.maker_input_sats, LONG_INPUT_SATS)
+        self.assertEqual(long_maker_contract.taker_input_sats, SHORT_INPUT_SATS_AS_HEDGE)
+        self.assertEqual(long_maker_contract.maker_input_oracleUnits, LONG_INPUT_ORACLE_UNITS)
+        self.assertEqual(long_maker_contract.taker_input_oracleUnits, SHORT_INPUT_ORACLE_UNITS_AS_HEDGE)
 
     ######################
     # Role versions of values
     ######################
     def test_parameterized_lookup_error_on_invalid_combinations(self):
-        maker_hedge_contract = standard_contract_proposal(maker_side=Side.HEDGE)
+        maker_short_contract = standard_contract_proposal(maker_side=Side.SHORT)
         with self.assertRaises(ValueError):
-            maker_hedge_contract.input_sats(role=Role.MAKER, side=Side.LONG)
+            maker_short_contract.input_sats(role=Role.MAKER, side=Side.LONG)
         with self.assertRaises(ValueError):
-            maker_hedge_contract.input_sats(role=Role.TAKER, side=Side.HEDGE)
+            maker_short_contract.input_sats(role=Role.TAKER, side=Side.SHORT)
 
-        taker_hedge_contract = standard_contract_proposal(maker_side=Side.LONG)
+        taker_short_contract = standard_contract_proposal(maker_side=Side.LONG)
         with self.assertRaises(ValueError):
-            taker_hedge_contract.input_sats(role=Role.TAKER, side=Side.LONG)
+            taker_short_contract.input_sats(role=Role.TAKER, side=Side.LONG)
         with self.assertRaises(ValueError):
-            taker_hedge_contract.input_sats(role=Role.MAKER, side=Side.HEDGE)
+            taker_short_contract.input_sats(role=Role.MAKER, side=Side.SHORT)
 
 
 class TestContractProposalValidation(unittest.TestCase):
     def test_ValueError_if_duration_too_short(self):
         with self.assertRaises(ValueError):
             too_short_maturity_timestamp = ScriptTimestamp(START_TIMESTAMP + 60 - 1)
             standard_contract_proposal(maturity_timestamp=too_short_maturity_timestamp)
@@ -199,100 +225,100 @@
 
 
 # Group them for reference
 TOTAL_FEES_TO_MAKER_SATS = Sats(
     + FEE_100000_TAKER_TO_MAKER.amount_sats
     + FEE_200000_TAKER_TO_MAKER.amount_sats
 )
-DERIVED_TOTAL_FEES_TO_MAKER_ORACLE_UNITS = UsdEM2Beta(TOTAL_FEES_TO_MAKER_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH)
+TOTAL_FEES_TO_MAKER_ORACLE_UNITS = UsdEM2Beta(TOTAL_FEES_TO_MAKER_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH)
 TOTAL_FEES_TO_TAKER_SATS = Sats(
     - FEE_100000_TAKER_TO_MAKER.amount_sats
     - FEE_200000_TAKER_TO_MAKER.amount_sats
     - FEE_400000_TAKER_TO_SETTLEMENT_SERVICE.amount_sats
 )
-DERIVED_TOTAL_FEES_TO_TAKER_ORACLE_UNITS = UsdEM2Beta(TOTAL_FEES_TO_TAKER_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH)
+TOTAL_FEES_TO_TAKER_ORACLE_UNITS = UsdEM2Beta(TOTAL_FEES_TO_TAKER_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH)
 
 
 def standard_contract_funding(proposal: ContractProposal | None = None) -> ContractFunding:
     proposal = proposal or standard_contract_proposal()
     return proposal.fund(fee_agreements=FEES)
 
 
 class TestContractFundingDerivedValues(unittest.TestCase):
     def test_fee_sats_to_side(self):
-        # Confirm hedge maker and long taker
-        hedge_maker_contract = standard_contract_funding(standard_contract_proposal(maker_side=Side.HEDGE))
+        # Confirm short maker and long taker
+        short_maker_contract = standard_contract_funding(standard_contract_proposal(maker_side=Side.SHORT))
         long_maker_contract = standard_contract_funding(standard_contract_proposal(maker_side=Side.LONG))
 
         expected_fees_sats_to_maker = TOTAL_FEES_TO_MAKER_SATS
         expected_fees_sats_to_taker = TOTAL_FEES_TO_TAKER_SATS
 
-        # Hedge Maker
-        self.assertEqual(hedge_maker_contract.fee_sats_to_hedge, expected_fees_sats_to_maker)
-        self.assertEqual(hedge_maker_contract.fee_sats_to_maker, expected_fees_sats_to_maker)
+        # Short Maker
+        self.assertEqual(short_maker_contract.fee_sats_to_short, expected_fees_sats_to_maker)
+        self.assertEqual(short_maker_contract.fee_sats_to_maker, expected_fees_sats_to_maker)
 
         # Long Taker
-        self.assertEqual(hedge_maker_contract.fee_sats_to_long, expected_fees_sats_to_taker)
-        self.assertEqual(hedge_maker_contract.fee_sats_to_taker, expected_fees_sats_to_taker)
+        self.assertEqual(short_maker_contract.fee_sats_to_long, expected_fees_sats_to_taker)
+        self.assertEqual(short_maker_contract.fee_sats_to_taker, expected_fees_sats_to_taker)
 
         # Long Maker
         self.assertEqual(long_maker_contract.fee_sats_to_long, expected_fees_sats_to_maker)
         self.assertEqual(long_maker_contract.fee_sats_to_maker, expected_fees_sats_to_maker)
 
-        # Hedge Taker
-        self.assertEqual(long_maker_contract.fee_sats_to_hedge, expected_fees_sats_to_taker)
+        # Short Taker
+        self.assertEqual(long_maker_contract.fee_sats_to_short, expected_fees_sats_to_taker)
         self.assertEqual(long_maker_contract.fee_sats_to_taker, expected_fees_sats_to_taker)
 
     def test_fee_oracleUnits_to_side(self):
-        # Confirm hedge maker and long taker
-        hedge_maker_contract = standard_contract_funding(standard_contract_proposal(maker_side=Side.HEDGE))
+        # Confirm short maker and long taker
+        short_maker_contract = standard_contract_funding(standard_contract_proposal(maker_side=Side.SHORT))
         long_maker_contract = standard_contract_funding(standard_contract_proposal(maker_side=Side.LONG))
-        oracle_class = hedge_maker_contract.base_proposal.oracle_unit_cls
+        oracle_class = short_maker_contract.base_proposal.oracle_unit_cls
 
         expected_fee_oracleUnits_to_maker_at_funding = oracle_class(TOTAL_FEES_TO_MAKER_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH)
         expected_fee_oracleUnits_to_taker_at_funding = oracle_class(TOTAL_FEES_TO_TAKER_SATS * START_PRICE_USDEM2_PER_BCH / SATS_PER_BCH)
 
-        # Hedge Maker
-        self.assertEqual(hedge_maker_contract.fee_oracleUnits_to_hedge, expected_fee_oracleUnits_to_maker_at_funding)
-        self.assertEqual(hedge_maker_contract.fee_oracleUnits_to_maker, expected_fee_oracleUnits_to_maker_at_funding)
+        # Short Maker
+        self.assertEqual(short_maker_contract.fee_oracleUnits_to_short, expected_fee_oracleUnits_to_maker_at_funding)
+        self.assertEqual(short_maker_contract.fee_oracleUnits_to_maker, expected_fee_oracleUnits_to_maker_at_funding)
 
         # Long Taker
-        self.assertEqual(hedge_maker_contract.fee_oracleUnits_to_long, expected_fee_oracleUnits_to_taker_at_funding)
-        self.assertEqual(hedge_maker_contract.fee_oracleUnits_to_taker, expected_fee_oracleUnits_to_taker_at_funding)
+        self.assertEqual(short_maker_contract.fee_oracleUnits_to_long, expected_fee_oracleUnits_to_taker_at_funding)
+        self.assertEqual(short_maker_contract.fee_oracleUnits_to_taker, expected_fee_oracleUnits_to_taker_at_funding)
 
         # Long Maker
         self.assertEqual(long_maker_contract.fee_oracleUnits_to_long, expected_fee_oracleUnits_to_maker_at_funding)
         self.assertEqual(long_maker_contract.fee_oracleUnits_to_maker, expected_fee_oracleUnits_to_maker_at_funding)
 
-        # Hedge Taker
-        self.assertEqual(long_maker_contract.fee_oracleUnits_to_hedge, expected_fee_oracleUnits_to_taker_at_funding)
+        # Short Taker
+        self.assertEqual(long_maker_contract.fee_oracleUnits_to_short, expected_fee_oracleUnits_to_taker_at_funding)
         self.assertEqual(long_maker_contract.fee_oracleUnits_to_taker, expected_fee_oracleUnits_to_taker_at_funding)
 
 
 # Valid timestamp, just before maturity
 BEFORE_MATURITY_TIMESTAMP = ScriptTimestamp(MATURITY_TIMESTAMP - 1)
 
 # A valid maturity price, just somewhat over the start price so no chance of low liquidation
 NAIVE_MATURITY_PRICE_USDEM2_PER_BCH = ScriptPriceInOracleUnitsPerBch(220_00)  # $220.00
-BELOW_LIQUIDATING_PRICE_USDEM2_PER_BCH = ScriptPriceInOracleUnitsPerBch(DERIVED_LONG_LIQUIDATION_PRICE - 10)
+BELOW_LIQUIDATING_PRICE_USDEM2_PER_BCH = ScriptPriceInOracleUnitsPerBch(LONG_LIQUIDATION_PRICE - 10)
 
 
 class TestMaturityRedemption(unittest.TestCase):
     def test_matures_at_maturity_time(self):
         redemption = standard_contract_funding().redeem(
             price_timestamp=MATURITY_TIMESTAMP,
             price_oracleUnits_per_bch=NAIVE_MATURITY_PRICE_USDEM2_PER_BCH,
             force_maturity=False,
         )
         self.assertEqual(redemption.redemption_type, RedemptionType.MATURATION)
 
     def test_matures_at_maturity_time_even_if_liquidating_price(self):
         redemption = standard_contract_funding().redeem(
             price_timestamp=MATURITY_TIMESTAMP,
-            price_oracleUnits_per_bch=DERIVED_LONG_LIQUIDATION_PRICE,
+            price_oracleUnits_per_bch=LONG_LIQUIDATION_PRICE,
             force_maturity=False,
         )
         self.assertEqual(redemption.redemption_type, RedemptionType.MATURATION)
 
     def test_fails_to_mature_before_maturity_time(self):
         with self.assertRaises(UnredeemableError):
             standard_contract_funding().redeem(
@@ -300,22 +326,22 @@
                 price_oracleUnits_per_bch=NAIVE_MATURITY_PRICE_USDEM2_PER_BCH,
                 force_maturity=False,
             )
 
     def test_liquidates_before_maturity_time_at_low_liquidation_price(self):
         redemption = standard_contract_funding().redeem(
             price_timestamp=BEFORE_MATURITY_TIMESTAMP,
-            price_oracleUnits_per_bch=DERIVED_LONG_LIQUIDATION_PRICE,
+            price_oracleUnits_per_bch=LONG_LIQUIDATION_PRICE,
             force_maturity=False,
         )
         self.assertEqual(redemption.redemption_type, RedemptionType.LIQUIDATION)
 
     def test_fails_to_liquidate_before_maturity_time_at_one_over_low_liquidation_price(self):
         valid_liquidation_timestamp = ScriptTimestamp(MATURITY_TIMESTAMP - 1)
-        one_over_liquidation_price = ScriptPriceInOracleUnitsPerBch(DERIVED_LONG_LIQUIDATION_PRICE + 1)
+        one_over_liquidation_price = ScriptPriceInOracleUnitsPerBch(LONG_LIQUIDATION_PRICE + 1)
         with self.assertRaises(UnredeemableError):
             standard_contract_funding().redeem(
                 price_timestamp=valid_liquidation_timestamp,
                 price_oracleUnits_per_bch=one_over_liquidation_price,
                 force_maturity=False,
             )
 
@@ -328,31 +354,36 @@
         )
         self.assertEqual(redemption.redemption_type, RedemptionType.MATURATION)
 
 
 ###################
 # Redeemed Contract Tests
 ###################
-# Derived hedge payout sats and units
-# Calculated as max(dust, HEDGE_COMPOSITE // CLAMPED_PRICE) (Note the integer division //)
-DERIVED_HEDGE_PAYOUT_SATS = UtxoSats(45_454_545)  # 0.45454545... Bch
-# Calculated as DERIVED_HEDGE_PAYOUT_SATS * MATURITY_PRICE / SATS_PER_BCH
-DERIVED_HEDGE_PAYOUT_ORACLE_UNITS = UsdEM2Beta(9999.999900)  # 99.99999900000 USD
+# Derived short payout sats and units
+# For pure hedge, calculated as max(dust, HEDGE_COMPOSITE // CLAMPED_PRICE - 0) (Note the integer division //)
+SHORT_PAYOUT_SATS_AS_HEDGE = UtxoSats(45_454_545)  # 0.45454545... Bch
+# For leveraged short, same calculation but the cost at short liquidation is not zero
+# Calculated as SHORT_PAYOUT_SATS_AS_HEDGE - COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION
+# Due to integer math, this *can* be zero like a perfect hedge in some extreme values.
+SHORT_PAYOUT_SATS_AS_LEVERAGED_SHORT = UtxoSats(18_182_066)
+
+# Calculated as SHORT_PAYOUT_SATS_AS_HEDGE * MATURITY_PRICE / SATS_PER_BCH
+SHORT_PAYOUT_ORACLE_UNITS_AS_HEDGE = UsdEM2Beta(9999.999900)  # 99.99999900000 USD
 
 # Derived long payout sats and units
 # Calculated as max(dust, TOTAL_INPUT - HEDGE_PAYOUT)
-DERIVED_LONG_PAYOUT_SATS = UtxoSats(18_829_333)  # 0.18829... Bch
-# Calculated as DERIVED_LONG_PAYOUT_SATS * MATURITY_PRICE / SATS_PER_BCH
-DERIVED_LONG_PAYOUT_ORACLE_UNITS = UsdEM2Beta(4142.45326)
+LONG_PAYOUT_SATS = UtxoSats(18_829_333)  # 0.18829... Bch
+# Calculated as LONG_PAYOUT_SATS * MATURITY_PRICE / SATS_PER_BCH
+LONG_PAYOUT_ORACLE_UNITS = UsdEM2Beta(4142.45326)
 
 # Derived total payout sats and units
-# Calculated as hedge + long
-DERIVED_TOTAL_PAYOUT_SATS = UtxoSats(64283878)
-# Calculated as DERIVED_HEDGE_PAYOUT_ORACLE_UNITS + DERIVED_LONG_PAYOUT_ORACLE_UNITS
-DERIVED_TOTAL_PAYOUT_ORACLE_UNITS = UsdEM2Beta(14142.4532)
+# Calculated as SHORT_PAYOUT_SATS_AS_HEDGE + LONG_PAYOUT_SATS
+TOTAL_PAYOUT_SATS_AS_HEDGE = UtxoSats(64283878)
+# Calculated as SHORT_PAYOUT_ORACLE_UNITS_AS_HEDGE + LONG_PAYOUT_ORACLE_UNITS
+TOTAL_PAYOUT_ORACLE_UNITS_AS_HEDGE = UsdEM2Beta(14142.4532)
 
 
 def standard_maturation(
         funding: ContractFunding | None = None
 ):
     funding = funding if funding is not None else standard_contract_funding()
     return funding.redeem(
@@ -360,15 +391,15 @@
         price_oracleUnits_per_bch=NAIVE_MATURITY_PRICE_USDEM2_PER_BCH,
         force_maturity=False,
     )
 
 
 def standard_liquidation(
     price_timestamp: ScriptTimestamp = MATURITY_TIMESTAMP,
-    price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch = DERIVED_LONG_LIQUIDATION_PRICE,
+    price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch = LONG_LIQUIDATION_PRICE,
     force_maturity: bool = False,
 ):
     return standard_contract_funding().redeem(
         price_timestamp=price_timestamp,
         price_oracleUnits_per_bch=price_oracleUnits_per_bch,
         force_maturity=force_maturity,
     )
@@ -383,136 +414,167 @@
         self.assertEqual(liquidation.clamped_end_price_oracleUnits_per_bch, liquidation.naive_end_price_oracleUnits_per_bch)
 
     def test_price_is_clamped_below_liquidation(self):
         liquidation = standard_liquidation(price_oracleUnits_per_bch=BELOW_LIQUIDATING_PRICE_USDEM2_PER_BCH)
         self.assertGreater(liquidation.clamped_end_price_oracleUnits_per_bch, liquidation.naive_end_price_oracleUnits_per_bch)
 
     def test_total_payout_sats_has_correct_value(self):
-        self.assertEqual(standard_maturation().total_payout_sats, DERIVED_TOTAL_PAYOUT_SATS)
+        self.assertEqual(standard_maturation().total_payout_sats, TOTAL_PAYOUT_SATS_AS_HEDGE)
 
-    def test_hedge_payout_sats_has_correct_value(self):
-        self.assertEqual(standard_maturation().hedge_payout_sats, DERIVED_HEDGE_PAYOUT_SATS)
+    def test_short_payout_sats_has_correct_value(self):
+        self.assertEqual(standard_maturation().short_payout_sats, SHORT_PAYOUT_SATS_AS_HEDGE)
 
     def test_long_payout_sats_has_correct_value(self):
-        self.assertEqual(standard_maturation().long_payout_sats, DERIVED_LONG_PAYOUT_SATS)
+        self.assertEqual(standard_maturation().long_payout_sats, LONG_PAYOUT_SATS)
 
     ######################
     # Exact secondary unit values
     ######################
     def test_total_payout_units_has_correct_value(self):
-        self.assertAlmostEqual(standard_maturation().total_payout_oracleUnits, DERIVED_TOTAL_PAYOUT_ORACLE_UNITS, delta=.001)
+        self.assertAlmostEqual(standard_maturation().total_payout_oracleUnits, TOTAL_PAYOUT_ORACLE_UNITS_AS_HEDGE, delta=.001)
 
-    def test_hedge_payout_units_has_correct_value(self):
-        self.assertAlmostEqual(standard_maturation().hedge_payout_oracleUnits, DERIVED_HEDGE_PAYOUT_ORACLE_UNITS, delta=.001)
+    def test_short_payout_units_has_correct_value(self):
+        self.assertAlmostEqual(standard_maturation().short_payout_oracleUnits, SHORT_PAYOUT_ORACLE_UNITS_AS_HEDGE, delta=.001)
 
     def test_long_payout_units_has_correct_value(self):
-        self.assertAlmostEqual(standard_maturation().long_payout_oracleUnits, DERIVED_LONG_PAYOUT_ORACLE_UNITS, delta=.001)
+        self.assertAlmostEqual(standard_maturation().long_payout_oracleUnits, LONG_PAYOUT_ORACLE_UNITS, delta=.001)
 
     ######################
     # Exact secondary gain values
     ######################
     def test_gain_sats(self):
-        # Hedge Maker / Long Taker
-        expected_gain_sats_to_hedge_maker_at_redemption = DERIVED_HEDGE_PAYOUT_SATS - DERIVED_HEDGE_INPUT_SATS + TOTAL_FEES_TO_MAKER_SATS
-        expected_gain_sats_to_long_taker_at_redemption = DERIVED_LONG_PAYOUT_SATS - DERIVED_LONG_INPUT_SATS + TOTAL_FEES_TO_TAKER_SATS
-        hedge_maker_contract = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.HEDGE)))
-
-        # Hedge Maker
-        self.assertEqual(hedge_maker_contract.hedge_gain_sats, expected_gain_sats_to_hedge_maker_at_redemption)
-        self.assertEqual(hedge_maker_contract.maker_gain_sats, expected_gain_sats_to_hedge_maker_at_redemption)
+        # Short Maker / Long Taker
+        expected_gain_sats_to_short_maker_at_redemption = SHORT_PAYOUT_SATS_AS_HEDGE - SHORT_INPUT_SATS_AS_HEDGE + TOTAL_FEES_TO_MAKER_SATS
+        expected_gain_sats_to_long_taker_at_redemption = LONG_PAYOUT_SATS - LONG_INPUT_SATS + TOTAL_FEES_TO_TAKER_SATS
+        short_maker_contract = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.SHORT)))
+
+        # Short Maker
+        self.assertEqual(short_maker_contract.short_gain_sats, expected_gain_sats_to_short_maker_at_redemption)
+        self.assertEqual(short_maker_contract.maker_gain_sats, expected_gain_sats_to_short_maker_at_redemption)
 
         # Long Taker
-        self.assertEqual(hedge_maker_contract.long_gain_sats, expected_gain_sats_to_long_taker_at_redemption)
-        self.assertEqual(hedge_maker_contract.taker_gain_sats, expected_gain_sats_to_long_taker_at_redemption)
+        self.assertEqual(short_maker_contract.long_gain_sats, expected_gain_sats_to_long_taker_at_redemption)
+        self.assertEqual(short_maker_contract.taker_gain_sats, expected_gain_sats_to_long_taker_at_redemption)
 
-        # Long Maker / Hedge Taker
-        expected_gain_sats_to_long_maker_at_redemption = DERIVED_LONG_PAYOUT_SATS - DERIVED_LONG_INPUT_SATS + TOTAL_FEES_TO_MAKER_SATS
-        expected_gain_sats_to_hedge_taker_at_redemption = DERIVED_HEDGE_PAYOUT_SATS - DERIVED_HEDGE_INPUT_SATS + TOTAL_FEES_TO_TAKER_SATS
+        # Long Maker / Short Taker
+        expected_gain_sats_to_long_maker_at_redemption = LONG_PAYOUT_SATS - LONG_INPUT_SATS + TOTAL_FEES_TO_MAKER_SATS
+        expected_gain_sats_to_short_taker_at_redemption = SHORT_PAYOUT_SATS_AS_HEDGE - SHORT_INPUT_SATS_AS_HEDGE + TOTAL_FEES_TO_TAKER_SATS
         long_maker_contract = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.LONG)))
 
         # Long Maker
         self.assertEqual(long_maker_contract.long_gain_sats, expected_gain_sats_to_long_maker_at_redemption)
         self.assertEqual(long_maker_contract.maker_gain_sats, expected_gain_sats_to_long_maker_at_redemption)
 
-        # Hedge Taker
-        self.assertEqual(long_maker_contract.hedge_gain_sats, expected_gain_sats_to_hedge_taker_at_redemption)
-        self.assertEqual(long_maker_contract.taker_gain_sats, expected_gain_sats_to_hedge_taker_at_redemption)
+        # Short Taker
+        self.assertEqual(long_maker_contract.short_gain_sats, expected_gain_sats_to_short_taker_at_redemption)
+        self.assertEqual(long_maker_contract.taker_gain_sats, expected_gain_sats_to_short_taker_at_redemption)
 
     def test_gain_oracleUnits(self):
-        # Hedge Maker / Long Taker
-        expected_gain_oracleUnits_to_hedge_maker_at_redemption = UsdEM2Beta(
-            DERIVED_HEDGE_PAYOUT_ORACLE_UNITS - DERIVED_HEDGE_INPUT_ORACLE_UNITS + DERIVED_TOTAL_FEES_TO_MAKER_ORACLE_UNITS
+        # Short Maker / Long Taker
+        expected_gain_oracleUnits_to_short_maker_at_redemption = UsdEM2Beta(
+            SHORT_PAYOUT_ORACLE_UNITS_AS_HEDGE - SHORT_INPUT_ORACLE_UNITS_AS_HEDGE + TOTAL_FEES_TO_MAKER_ORACLE_UNITS
         )
         expected_gain_oracleUnits_to_long_taker_at_redemption = UsdEM2Beta(
-            DERIVED_LONG_PAYOUT_ORACLE_UNITS - DERIVED_LONG_INPUT_ORACLE_UNITS + DERIVED_TOTAL_FEES_TO_TAKER_ORACLE_UNITS
+            LONG_PAYOUT_ORACLE_UNITS - LONG_INPUT_ORACLE_UNITS + TOTAL_FEES_TO_TAKER_ORACLE_UNITS
         )
-        hedge_maker_contract = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.HEDGE)))
+        short_maker_contract = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.SHORT)))
 
-        # Hedge Maker
-        self.assertAlmostEqual(hedge_maker_contract.hedge_gain_oracleUnits, expected_gain_oracleUnits_to_hedge_maker_at_redemption)
-        self.assertAlmostEqual(hedge_maker_contract.maker_gain_oracleUnits, expected_gain_oracleUnits_to_hedge_maker_at_redemption)
+        # Short Maker
+        self.assertAlmostEqual(short_maker_contract.short_gain_oracleUnits, expected_gain_oracleUnits_to_short_maker_at_redemption)
+        self.assertAlmostEqual(short_maker_contract.maker_gain_oracleUnits, expected_gain_oracleUnits_to_short_maker_at_redemption)
 
         # Long Taker
-        self.assertAlmostEqual(hedge_maker_contract.long_gain_oracleUnits, expected_gain_oracleUnits_to_long_taker_at_redemption)
-        self.assertAlmostEqual(hedge_maker_contract.taker_gain_oracleUnits, expected_gain_oracleUnits_to_long_taker_at_redemption)
+        self.assertAlmostEqual(short_maker_contract.long_gain_oracleUnits, expected_gain_oracleUnits_to_long_taker_at_redemption)
+        self.assertAlmostEqual(short_maker_contract.taker_gain_oracleUnits, expected_gain_oracleUnits_to_long_taker_at_redemption)
 
-        # Long Maker / Hedge Taker
+        # Long Maker / Short Taker
         expected_gain_oracleUnits_to_long_maker_at_redemption = UsdEM2Beta(
-            DERIVED_LONG_PAYOUT_ORACLE_UNITS - DERIVED_LONG_INPUT_ORACLE_UNITS + DERIVED_TOTAL_FEES_TO_MAKER_ORACLE_UNITS
+            LONG_PAYOUT_ORACLE_UNITS - LONG_INPUT_ORACLE_UNITS + TOTAL_FEES_TO_MAKER_ORACLE_UNITS
         )
-        expected_gain_oracleUnits_to_hedge_taker_at_redemption = UsdEM2Beta(
-            DERIVED_HEDGE_PAYOUT_ORACLE_UNITS - DERIVED_HEDGE_INPUT_ORACLE_UNITS + DERIVED_TOTAL_FEES_TO_TAKER_ORACLE_UNITS
+        expected_gain_oracleUnits_to_short_taker_at_redemption = UsdEM2Beta(
+            SHORT_PAYOUT_ORACLE_UNITS_AS_HEDGE - SHORT_INPUT_ORACLE_UNITS_AS_HEDGE + TOTAL_FEES_TO_TAKER_ORACLE_UNITS
         )
         long_maker_contract = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.LONG)))
 
         # Long Maker
         self.assertAlmostEqual(long_maker_contract.long_gain_oracleUnits, expected_gain_oracleUnits_to_long_maker_at_redemption)
         self.assertAlmostEqual(long_maker_contract.maker_gain_oracleUnits, expected_gain_oracleUnits_to_long_maker_at_redemption)
 
-        # Hedge Taker
-        self.assertAlmostEqual(long_maker_contract.hedge_gain_oracleUnits, expected_gain_oracleUnits_to_hedge_taker_at_redemption)
-        self.assertAlmostEqual(long_maker_contract.taker_gain_oracleUnits, expected_gain_oracleUnits_to_hedge_taker_at_redemption)
+        # Short Taker
+        self.assertAlmostEqual(long_maker_contract.short_gain_oracleUnits, expected_gain_oracleUnits_to_short_taker_at_redemption)
+        self.assertAlmostEqual(long_maker_contract.taker_gain_oracleUnits, expected_gain_oracleUnits_to_short_taker_at_redemption)
 
     ######################
     # Sided versions of values
     ######################
     def test_all_sided_values(self):
         c = standard_maturation()
-        self.assertEqual(c.maker_payout_sats, c.hedge_payout_sats)
+        self.assertEqual(c.maker_payout_sats, c.short_payout_sats)
         self.assertEqual(c.taker_payout_sats, c.long_payout_sats)
-        self.assertEqual(c.maker_payout_oracleUnits, c.hedge_payout_oracleUnits)
+        self.assertEqual(c.maker_payout_oracleUnits, c.short_payout_oracleUnits)
         self.assertEqual(c.taker_payout_oracleUnits, c.long_payout_oracleUnits)
-        self.assertEqual(c.maker_gain_sats, c.hedge_gain_sats)
+        self.assertEqual(c.maker_gain_sats, c.short_gain_sats)
         self.assertEqual(c.taker_gain_sats, c.long_gain_sats)
-        self.assertEqual(c.maker_gain_oracleUnits, c.hedge_gain_oracleUnits)
+        self.assertEqual(c.maker_gain_oracleUnits, c.short_gain_oracleUnits)
         self.assertEqual(c.taker_gain_oracleUnits, c.long_gain_oracleUnits)
-        self.assertEqual(c.maker_gain_percent_of_own_input, c.hedge_gain_percent_of_own_input)
+        self.assertEqual(c.maker_gain_percent_of_own_input, c.short_gain_percent_of_own_input)
         self.assertEqual(c.taker_gain_percent_of_own_input, c.long_gain_percent_of_own_input)
 
         c = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.LONG)))
         self.assertEqual(c.maker_payout_sats, c.long_payout_sats)
-        self.assertEqual(c.taker_payout_sats, c.hedge_payout_sats)
+        self.assertEqual(c.taker_payout_sats, c.short_payout_sats)
         self.assertEqual(c.maker_payout_oracleUnits, c.long_payout_oracleUnits)
-        self.assertEqual(c.taker_payout_oracleUnits, c.hedge_payout_oracleUnits)
+        self.assertEqual(c.taker_payout_oracleUnits, c.short_payout_oracleUnits)
         self.assertEqual(c.maker_gain_sats, c.long_gain_sats)
-        self.assertEqual(c.taker_gain_sats, c.hedge_gain_sats)
+        self.assertEqual(c.taker_gain_sats, c.short_gain_sats)
         self.assertEqual(c.maker_gain_oracleUnits, c.long_gain_oracleUnits)
-        self.assertEqual(c.taker_gain_oracleUnits, c.hedge_gain_oracleUnits)
+        self.assertEqual(c.taker_gain_oracleUnits, c.short_gain_oracleUnits)
         self.assertEqual(c.maker_gain_percent_of_own_input, c.long_gain_percent_of_own_input)
-        self.assertEqual(c.taker_gain_percent_of_own_input, c.hedge_gain_percent_of_own_input)
+        self.assertEqual(c.taker_gain_percent_of_own_input, c.short_gain_percent_of_own_input)
 
     def test_parameterized_lookup_error_on_invalid_combinations(self):
-        maker_hedge_maturation = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.HEDGE)))
+        maker_short_maturation = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.SHORT)))
         with self.assertRaises(ValueError):
-            maker_hedge_maturation.payout_sats(role=Role.MAKER, side=Side.LONG)
+            maker_short_maturation.payout_sats(role=Role.MAKER, side=Side.LONG)
         with self.assertRaises(ValueError):
-            maker_hedge_maturation.payout_sats(role=Role.TAKER, side=Side.HEDGE)
+            maker_short_maturation.payout_sats(role=Role.TAKER, side=Side.SHORT)
 
-        taker_hedge_maturation = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.LONG)))
+        taker_short_maturation = standard_maturation(standard_contract_funding(standard_contract_proposal(maker_side=Side.LONG)))
         with self.assertRaises(ValueError):
-            taker_hedge_maturation.payout_sats(role=Role.TAKER, side=Side.LONG)
+            taker_short_maturation.payout_sats(role=Role.TAKER, side=Side.LONG)
         with self.assertRaises(ValueError):
-            taker_hedge_maturation.payout_sats(role=Role.MAKER, side=Side.HEDGE)
+            taker_short_maturation.payout_sats(role=Role.MAKER, side=Side.SHORT)
+
+
+class TestHedgeVsLeveragedShort(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        cls.hedge_short = standard_contract_proposal()
+        cls.leveraged_short = standard_contract_proposal(short_leverage=SHORT_LEVERAGE_NOT_1)
+
+    def test_short_liquidation_price_for_leveraged_short(self):
+        self.assertEqual(self.leveraged_short.short_liquidation_price_oracleUnits_per_bch, SHORT_LIQUIDATION_PRICE_AS_LEVERAGED_SHORT)
+
+    def test_cost_at_short_liquidation_for_hedge_vs_leveraged_short(self):
+        self.assertEqual(self.hedge_short.cost_sats_for_nominal_value_at_short_liquidation, ZERO_COST_OF_NOMINAL_VALUE_AT_HEDGE_LIQUIDATION)
+        self.assertEqual(self.leveraged_short.cost_sats_for_nominal_value_at_short_liquidation, COST_SATS_OF_NOMINAL_VALUE_AT_LEVERAGED_SHORT_LIQUIDATION)
+
+    def test_short_input_sats_for_leveraged_short(self):
+        self.assertEqual(self.leveraged_short.short_input_sats, SHORT_INPUT_SATS_AS_LEVERAGED_SHORT)
+
+    def test_total_input_sats_for_leveraged_short(self):
+        self.assertEqual(self.leveraged_short.total_input_sats, TOTAL_INPUT_SATS_AS_LEVERAGED_SHORT)
+
+    def test_effective_short_leverage_when_hedge_vs_leveraged_short(self):
+        # Should report as exactly 1 for pure hedge
+        self.assertEqual(self.hedge_short.effective_short_leverage, SHORT_LEVERAGE_1_AS_HEDGE)
+
+        # Should report according to calculation for leveraged short (which can also be 1)
+        self.assertAlmostEqual(self.leveraged_short.effective_short_leverage, SHORT_LEVERAGE_NOT_1, delta=.001)
+
+    def test_short_payout_for_leveraged_short(self):
+        leveraged_short_redemption = standard_maturation(standard_contract_funding(self.leveraged_short))
+        self.assertEqual(leveraged_short_redemption.short_payout_sats, SHORT_PAYOUT_SATS_AS_LEVERAGED_SHORT)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `anyhedge-0.1.3/anyhedge/test_fee.py` & `anyhedge-0.3.4/anyhedge/tests/test_fee.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Built-in imports
 import unittest
 
 # Local imports
-from .bch_primitives import Sats
-from .role import Role
-from .fee import (
+from ..bch_primitives import Sats
+from ..role import Role
+from ..fee import (
     fees_from_role,
     fees_to_role,
     FeeAgreement,
 )
 
 
 fee_100000_taker_to_ss = FeeAgreement(name='a', amount_sats=Sats(100000), receiving=Role.SETTLEMENT_SERVICE, paying=Role.TAKER)
```

### Comparing `anyhedge-0.1.3/anyhedge/test_oracle.py` & `anyhedge-0.3.4/anyhedge/tests/test_oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Built-in imports
 import unittest
 
 # Local imports
-from .bch_primitives import (
+from ..bch_primitives import (
     PublicKey,
     ScriptTimestamp,
 )
-from .oracle import (
+from ..oracle import (
     Pricepoint,
     ScriptPriceInOracleUnitsPerBch,
 )
 
 
 # Known price message for Usd(e-2) oracle:
 #   public key: 02d3c1de9d4bc77d6c3608cbe44d10138c7488e592dc2b1e10a6cf0e92c2ecb047
```

### Comparing `anyhedge-0.1.3/anyhedge.egg-info/PKG-INFO` & `anyhedge-0.3.4/anyhedge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 0.1.3
+Version: 0.3.4
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-0.1.3/pyproject.toml` & `anyhedge-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'anyhedge'
-version = '0.1.3'
+version = '0.3.4'
 authors = [
   { name='emergent_reasons', email='emergent_reasons@gmail.com' },
 ]
 license = { file = "LICENSE" }
 description = 'Basic components of AnyHedge contracts'
 readme = 'README.md'
 requires-python = '>=3.10'
```

