# Comparing `tmp/anyhedge-2.1.4.tar.gz` & `tmp/anyhedge-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyhedge-2.1.4.tar", last modified: Tue May 14 20:21:40 2024, max compression
+gzip compressed data, was "anyhedge-3.0.0.tar", last modified: Sat May 18 07:11:13 2024, max compression
```

## Comparing `anyhedge-2.1.4.tar` & `anyhedge-3.0.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 20:21:40.550658 anyhedge-2.1.4/
--rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-2.1.4/LICENSE
--rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-14 20:21:40.550658 anyhedge-2.1.4/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-2.1.4/README.md
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 20:21:40.550658 anyhedge-2.1.4/anyhedge/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-2.1.4/anyhedge/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2426 2024-04-10 20:22:29.000000 anyhedge-2.1.4/anyhedge/bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    45310 2024-05-14 20:20:02.000000 anyhedge-2.1.4/anyhedge/contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2024-05-08 03:40:10.000000 anyhedge-2.1.4/anyhedge/fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-2.1.4/anyhedge/javascript.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    13939 2024-05-14 20:20:47.000000 anyhedge-2.1.4/anyhedge/oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      303 2024-05-08 03:40:10.000000 anyhedge-2.1.4/anyhedge/role.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 20:21:40.550658 anyhedge-2.1.4/anyhedge/tests/
--rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-2.1.4/anyhedge/tests/__init__.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-2.1.4/anyhedge/tests/test_bch_primitives.py
--rw-rw-r--   0 alien     (1000) alien     (1000)    43176 2024-05-14 20:20:02.000000 anyhedge-2.1.4/anyhedge/tests/test_contract.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2024-05-08 03:40:10.000000 anyhedge-2.1.4/anyhedge/tests/test_fee.py
--rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-2.1.4/anyhedge/tests/test_oracle.py
--rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-2.1.4/anyhedge/validators.py
-drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-14 20:21:40.550658 anyhedge-2.1.4/anyhedge.egg-info/
--rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-14 20:21:40.000000 anyhedge-2.1.4/anyhedge.egg-info/PKG-INFO
--rw-rw-r--   0 alien     (1000) alien     (1000)      512 2024-05-14 20:21:40.000000 anyhedge-2.1.4/anyhedge.egg-info/SOURCES.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        1 2024-05-14 20:21:40.000000 anyhedge-2.1.4/anyhedge.egg-info/dependency_links.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)       57 2024-05-14 20:21:40.000000 anyhedge-2.1.4/anyhedge.egg-info/requires.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)        9 2024-05-14 20:21:40.000000 anyhedge-2.1.4/anyhedge.egg-info/top_level.txt
--rw-rw-r--   0 alien     (1000) alien     (1000)      798 2024-05-14 20:21:08.000000 anyhedge-2.1.4/pyproject.toml
--rw-rw-r--   0 alien     (1000) alien     (1000)       38 2024-05-14 20:21:40.550658 anyhedge-2.1.4/setup.cfg
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-18 07:11:13.933162 anyhedge-3.0.0/
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1060 2022-11-18 22:24:58.000000 anyhedge-3.0.0/LICENSE
+-rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-18 07:11:13.933162 anyhedge-3.0.0/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1833 2022-11-19 01:20:40.000000 anyhedge-3.0.0/README.md
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-18 07:11:13.933162 anyhedge-3.0.0/anyhedge/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2022-11-19 00:09:43.000000 anyhedge-3.0.0/anyhedge/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2426 2024-04-10 20:22:29.000000 anyhedge-3.0.0/anyhedge/bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    53693 2024-05-18 07:09:10.000000 anyhedge-3.0.0/anyhedge/contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2194 2024-05-18 07:09:10.000000 anyhedge-3.0.0/anyhedge/contract_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     2232 2024-05-08 03:40:10.000000 anyhedge-3.0.0/anyhedge/fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)       46 2022-10-09 03:40:43.000000 anyhedge-3.0.0/anyhedge/javascript.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    13984 2024-05-18 07:09:10.000000 anyhedge-3.0.0/anyhedge/oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      303 2024-05-08 03:40:10.000000 anyhedge-3.0.0/anyhedge/role.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-18 07:11:13.933162 anyhedge-3.0.0/anyhedge/tests/
+-rw-rw-r--   0 alien     (1000) alien     (1000)        0 2023-04-11 04:30:35.000000 anyhedge-3.0.0/anyhedge/tests/__init__.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3565 2023-04-11 04:30:35.000000 anyhedge-3.0.0/anyhedge/tests/test_bch_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)    47505 2024-05-18 07:09:10.000000 anyhedge-3.0.0/anyhedge/tests/test_contract.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      498 2024-05-18 07:09:10.000000 anyhedge-3.0.0/anyhedge/tests/test_contract_primitives.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     1197 2024-05-08 03:40:10.000000 anyhedge-3.0.0/anyhedge/tests/test_fee.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)     3785 2023-04-11 04:30:35.000000 anyhedge-3.0.0/anyhedge/tests/test_oracle.py
+-rw-rw-r--   0 alien     (1000) alien     (1000)      249 2022-10-11 17:25:11.000000 anyhedge-3.0.0/anyhedge/validators.py
+drwxrwxr-x   0 alien     (1000) alien     (1000)        0 2024-05-18 07:11:13.933162 anyhedge-3.0.0/anyhedge.egg-info/
+-rw-r--r--   0 alien     (1000) alien     (1000)     3722 2024-05-18 07:11:13.000000 anyhedge-3.0.0/anyhedge.egg-info/PKG-INFO
+-rw-rw-r--   0 alien     (1000) alien     (1000)      587 2024-05-18 07:11:13.000000 anyhedge-3.0.0/anyhedge.egg-info/SOURCES.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        1 2024-05-18 07:11:13.000000 anyhedge-3.0.0/anyhedge.egg-info/dependency_links.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)       57 2024-05-18 07:11:13.000000 anyhedge-3.0.0/anyhedge.egg-info/requires.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)        9 2024-05-18 07:11:13.000000 anyhedge-3.0.0/anyhedge.egg-info/top_level.txt
+-rw-rw-r--   0 alien     (1000) alien     (1000)      798 2024-05-18 07:09:38.000000 anyhedge-3.0.0/pyproject.toml
+-rw-rw-r--   0 alien     (1000) alien     (1000)       38 2024-05-18 07:11:13.933162 anyhedge-3.0.0/setup.cfg
```

### Comparing `anyhedge-2.1.4/LICENSE` & `anyhedge-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.4/PKG-INFO` & `anyhedge-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 2.1.4
+Version: 3.0.0
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-2.1.4/README.md` & `anyhedge-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.4/anyhedge/bch_primitives.py` & `anyhedge-3.0.0/anyhedge/bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.4/anyhedge/contract.py` & `anyhedge-3.0.0/anyhedge/contract.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,52 @@
 # Built-in imports
 from __future__ import annotations  # allow pre-definition use of types
 from dataclasses import dataclass
 from enum import Enum
 from functools import cached_property
-from math import ceil, floor
 from typing import Sequence, Type
 
 # Local imports
-from . import validators
 from .bch_primitives import (
     DUST,
     MAX_REASONABLE_SATS,
     MIN_REASONABLE_DIVISION_STEPS,
     SATS_PER_BCH,
     SCRIPT_INT_MAX,
     PublicKey,
     Sats,
     ScriptTimestamp,
     UtxoSats,
 )
+from .contract_primitives import (
+    LongLeverage,
+    NominalOracleUnitsXSatsPerBch,
+    Role,
+    ShortLeverage,
+    Side,
+)
 from .fee import (
     aggregate_fee_sats_to_role,
     FeeAgreement,
 )
 from .javascript import round_half_up
 from .oracle import (
     oracle_pubkey_to_unit_class,
     OracleUnit,
     ScriptPriceInOracleUnitsPerBch,
 )
-from .role import Role
 
 
 class UnredeemableError(Exception):
     pass
 
 
-class Side(str, Enum):
-    SHORT = 'Short'
-    LONG = 'Long'
-
-    def __str__(self):
-        return self.value
-
-    def __repr__(self):
-        return self.__str__()
-
-    @property
-    def other_side(self) -> Side:
-        # use a lookup to ensure KeyError with unknown value
-        return {Side.SHORT: Side.LONG, Side.LONG: Side.SHORT}[self]
-
-    @classmethod
-    def from_string(cls, side_string: str) -> Side:
-        # use a lookup to ensure KeyError with unknown value
-        lookup = {
-            'short': cls.SHORT,
-            'hedge': cls.SHORT,
-            'long': cls.LONG,
-        }
-        return lookup[side_string.lower()]
-
-
-class NominalOracleUnitsXSatsPerBch(int):
-    def __init__(self, value):
-        super().__init__()
-        validators.instance(value, int)  # i.e. don't allow silent coercion
-        validators.less_equal(self, SCRIPT_INT_MAX)
-        validators.greater_equal(self, SATS_PER_BCH)  # i.e. minimum is 1 nominal oracle unit
-
-
-class ShortLeverage(float):
-    min_allowed: float = 1.0
-    max_allowed: float = 50.0
-
-    def __init__(self, _):
-        super().__init__()
-        validators.less_equal(self, self.max_allowed * 1.00001)  # some room for floating point error
-        validators.greater_equal(self, self.min_allowed)  # strict boundary for flat hedge position, below one is undefined
-
-
-class LongLeverage(float):
-    min_allowed: float = 1.1
-    max_allowed: float = 50.0
-
-    def __init__(self, _):
-        super().__init__()
-        validators.less_equal(self, self.max_allowed * 1.00001)  # some room for floating point error
-        validators.greater_equal(self, self.min_allowed * 0.99999)  # some room for floating point error
+# In this library design, there is no explicit multiplier to establish a liquidation price
+# in the case of a simple hedge (short leverage = 1). We choose simply 10x.
+DEFAULT_HIGH_LIQUIDATION_PRICE_MULTIPLIER_FOR_SIMPLE_HEDGE = 10.0
 
 
 # TODO: add "forced maturation" to differentiate from normal case in records?
 class RedemptionType(str, Enum):
     LIQUIDATION = 'Liquidation'
     MATURATION = 'Maturation'
     MUTUAL = 'Mutual'
@@ -110,14 +65,336 @@
             'maturation': cls.MATURATION,
             'mutual': cls.MUTUAL,
         }
         redemption_type = lookup[redemption_type_string.lower()]
         return redemption_type
 
 
+# TODO: this should be broken into independent parts TimingIntent, UserIntent, MoneyIntent
+@dataclass(frozen=True)
+class GenericContractIntent:
+    """A representation of intent for a contract that translates to a Contract Proposal."""
+    # 1. A specific intent pattern must provide a set of parameters from which a contract can be created
+
+    # 2. The proposal property (or it could be parameterized... maybe... implements the translation from intent parameters to a contract
+    @property
+    def proposal(self, *args, **kwargs) -> ContractProposal:
+        raise NotImplementedError()
+
+
+@dataclass(frozen=True)
+class ContractFromNominalHedgeAndLeverages(GenericContractIntent):
+    """This is the canonical intent, although it turns out to be a pain to use in user interfaces."""
+    # Timing Intent
+    start_timestamp: ScriptTimestamp
+    maturity_timestamp: ScriptTimestamp
+
+    # Money Intent
+    nominal_oracleUnits: OracleUnit
+    short_leverage: ShortLeverage
+    long_leverage: LongLeverage
+    start_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch
+
+    # User Intent
+    maker_side: Side
+    short_mutual_redeem_public_key: PublicKey | '' = ''
+    long_mutual_redeem_public_key: PublicKey | '' = ''
+
+    @property
+    def proposal(self) -> ContractProposal:
+        # Before calculating key values below, this is an outline of the setup, using relevant variable names.
+        #
+        # AnyHedge 0.12 with leveraged shorts works on the same concept as previous "simple/nominal hedge" versions.
+        # By including one more number, explained below, the contract can now provide independent leverage to Short and Long.
+        #
+        # In summary, Long uses AnyHedge to "buy" an asset now, "selling" it later for hopefully a higher price, and
+        # Short uses AnyHedge to "sell" an asset now, "buying" it later for hopefully a lower price.
+        #
+        # The hedge value / simple hedge / nominal hedge is a fixed asset value that the rest of the contract centers around.
+        # The original idea of AnyHedge is that at any price within the liquidation (more commonly "margin call") range,
+        # Short receives exactly the nominal hedge value at the end, paid in Bch. This is the definition of behavior for
+        # short leverage = 1, i.e. virtually holding another asset, using BCH as the vehicle instead of the asset itself.
+        #
+        # The setting of liquidation values is mathematically equivalent to setting leverage for Short and Long.
+        # In the original setup, only Long was mathematically bound to the liquidation price, establishing leverage.
+        # Short on the other hand had a liquidation price for safety purposes, but the behavior of Short payout was not bound
+        # mathematically to that liquidation price. The contract simply always paid out Short for the full hedge value,
+        # which at the absurd extreme can be achieved with one satoshi at a price approaching infinity.
+        #
+        # The current arrangement described below allows Short to achieve leverage by tying behavior to the high
+        # liquidation price if desired, or to retain original behavior by disconnecting from the high liquidation price.
+        # Given this setup at start, the contract is fully collateralized to handle any outcome within the liquidation range.
+        #
+        # The relationship between liquidation prices and effective leverage are not explained in depth here,
+        # but the summary is:
+        #     shortLeverage = 1 + (1 / ((highLiquidationPrice / startPrice) - 1))
+        #     longLeverage  = 1 / (1 - (lowLiquidationPrice / startPrice))
+        #
+        #  *Price in Asset/Bch*            *Cost of Hedge at Price (higher price ==> lower cost)*
+        # --------------------------------------------------------------------------------------------------------------------
+        #                        ^
+        #                        |
+        #  highLiquidationPrice  -    ---- satsForHedgeAtHighLiq (this is the new reference that allows short leverage)
+        #                        |    ||||                       (in the past, the assumption was zero cost at infinity)
+        #                        |    ||||
+        #                        |    |||| } shortInputSats = worst case "sell low buy high" case for short
+        #                        |    ||||                  = satsForHedgeAtStart - satsForHedgeAtHighLiq
+        #                        |    ||||
+        #                        |    ||||
+        #            startPrice  -    ---- satsForHedgeAtStart
+        #                        |    ||||
+        #                        |    |||| } longInputSats = worst case "buy high sell low" case for long
+        #                        |    ||||                 = satsForHedgeAtLowLiq - satsForHedgeAtStart
+        #                        |    ||||
+        #   lowLiquidationPrice  -    ---- satsForHedgeAtLowLiq (to reiterate, lowest price ==> highest cost)
+        #                        |
+        #                        |
+        #                        - 0
+        #
+        # Payout at the end of the contract is the same picture, except based on the end price instead of start Price.
+        #
+        #  *Price in Asset/Bch*            *Cost of Hedge at Price (higher price ==> lower cost)*
+        # --------------------------------------------------------------------------------------------------------------------
+        #                        ^
+        #                        |
+        #  highLiquidationPrice  -    ---- satsForHedgeAtHighLiq (zero at infinity for simple hedge)
+        #                        |    ||||
+        #                        |    |||| } shortPayoutSats = satsForHedgeAtEnd - satsForHedgeAtHighLiq
+        #                        |    ||||
+        #              endPrice  -    ---- satsForHedgeAtEnd (price moved up, Short gets more Bch, Long gets less)
+        #                        |    ||||
+        #                        |    ||||
+        #            startPrice  -    ||||
+        #                        |    ||||
+        #                        |    |||| } longPayinSats = satsForHedgeAtLowLiq - satsForHedgeAtEnd
+        #                        |    ||||
+        #                        |    ||||
+        #   lowLiquidationPrice  -    ---- satsForHedgeAtLowLiq
+        #                        |
+        #                        |
+        #                        - 0
+
+        # 1. Low liquidation price: the low price that triggers liquidation of the Long party.
+        # The value is rounded to achieve a result as close as possible to intent.
+        # There should be no integer-level loss of precision given the 32-bit range of oracle prices.
+        # In order to align with methodology of the canonical anyhedge library,
+        # we do an initial step to convert leverage to a price multiplier
+        low_liquidation_price_multiplier = 1 - (1 / self.long_leverage)
+        low_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(low_liquidation_price_multiplier * float(self.start_price_oracleUnits_per_bch)))
+
+        # 2. High liquidation price: the high price that triggers liquidation of the Short party.
+        # The value is rounded to achieve a result as close as possible to intent.
+        # There should be no integer-level loss of precision given the 32-bit range of oracle prices.
+        # In order to align with methodology of the canonical anyhedge library,
+        # we do an initial step to convert leverage to a price multiplier and detect if this is effectively
+        # a simple hedge or not.
+        try:
+            high_liquidation_price_multiplier = 1 + (1 / (self.short_leverage - 1))
+            is_simple_hedge = False
+        except ZeroDivisionError:
+            high_liquidation_price_multiplier = DEFAULT_HIGH_LIQUIDATION_PRICE_MULTIPLIER_FOR_SIMPLE_HEDGE
+            is_simple_hedge = True
+
+        # Use the multiplier to set the price
+        high_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(high_liquidation_price_multiplier * float(self.start_price_oracleUnits_per_bch)))
+
+        # 3. Composite number representing the nominal hedge value in asset terms.
+        # In the diagrams above, this is the value discussed as "Hedge"
+        # Note: Rather than using the nominal hedge value alone, the number is calculated as
+        #       (nominal hedge units * 1e8 sats/bch). This allows the critical calculation in the contract to be simple
+        #       division, and is also a carryover from previous BCH VM versions (before May 2022) that did not have
+        #       multiplication. I.e. this value divided by the oracle price directly yields satoshis for
+        #       nominal hedge value at the given price, which is the final units we need to establish payouts.
+        # Note: DO NOT CONVERT THE COMPOSITE VALUE TO A floating point NUMBER FOR ANY REASON.
+        #       Any such calculations or transmissions (e.g. through simple JSON) must be
+        #       considered to introduce undefined behavior and be rejected.
+        #       The initial float calculation is a one way translation from floating precision
+        #       nominalUnits input to BigInt.
+        nominal_oracleUnits_x_satsPerBch = NominalOracleUnitsXSatsPerBch(round_half_up(self.nominal_oracleUnits * SATS_PER_BCH))
+
+        # 4. Cost in sats of the nominal hedge at high liquidation price.
+        # This is the value satsForHedgeAtHighLiq in the diagrams above.
+        # In summary, this value is needed to calculate Short's payout.
+        # Calculation of the value is discontinuous as follows:
+        if is_simple_hedge:
+            # a) For a simple hedge (short leverage = 1), the value is exactly 0. This
+            # represents the concept and calculation that Long must cover the full range
+            # of Short payouts from current price to infinity (where the cost becomes zero, this value).
+            cost_sats_for_nominal_value_at_high_liquidation = Sats(0)
+        else:
+            # b) For a leveraged short (short leverage > 1), the value is calculated from the
+            # other parameters in a simple cost relationship.
+            # Note: cost is floored for safety by bigint division in order to ensure that the
+            #       total sats in the contract cover a range that may be at worst +1 or +2 from
+            #       the "real" full precision value. This is valuable to ensure that contract
+            #       calculations never result in a value more than the total sats available.
+            cost_sats_for_nominal_value_at_high_liquidation = Sats(nominal_oracleUnits_x_satsPerBch // high_liquidation_price_oracleUnits_per_bch)
+
+        # 5. Cost in sats of the nominal hedge at low liquidation.
+        # This is the value satsForHedgeAtLowLiq in the diagrams above.
+        # In summary, this value is needed to calculate total input.
+        # Note: Here we use simple integer division and accept the loss of rounding.
+        #       Safety is ensured outside the zero case by validation.
+        # Note: We do zero testing here because this happens before parameter validation
+        #       which would catch it otherwise.
+        if low_liquidation_price_oracleUnits_per_bch <= 0:
+            raise ValueError('low liquidation price must be greater than zero')
+        cost_sats_for_nominal_value_at_low_liquidation = UtxoSats(nominal_oracleUnits_x_satsPerBch // low_liquidation_price_oracleUnits_per_bch)
+
+        # 6. Total input satoshis: the difference between worst case long and short outcomes.
+        total_input_sats = UtxoSats(cost_sats_for_nominal_value_at_low_liquidation - cost_sats_for_nominal_value_at_high_liquidation)
+
+        return ContractProposal(
+            address='',
+            short_mutual_redeem_public_key=self.short_mutual_redeem_public_key,
+            long_mutual_redeem_public_key=self.long_mutual_redeem_public_key,
+            start_timestamp=self.start_timestamp,
+            maturity_timestamp=self.maturity_timestamp,
+            nominal_oracleUnits_x_satsPerBch=nominal_oracleUnits_x_satsPerBch,
+            cost_sats_for_nominal_value_at_high_liquidation=cost_sats_for_nominal_value_at_high_liquidation,
+            total_input_sats=total_input_sats,
+            start_price_oracleUnits_per_bch=self.start_price_oracleUnits_per_bch,
+            high_liquidation_price_oracleUnits_per_bch=high_liquidation_price_oracleUnits_per_bch,
+            low_liquidation_price_oracleUnits_per_bch=low_liquidation_price_oracleUnits_per_bch,
+            oracle_public_key=self.nominal_oracleUnits.public_key,
+            maker_side=self.maker_side,
+        )
+
+
+@dataclass(frozen=True)
+class ContractFromInputSatsAndLeverages(GenericContractIntent):
+    """This is a more user-interface friendly intent."""
+    # TODO: when TimingIntent intent is isolated, it will make more sense to have both duration and maturity TimingIntent. For now, user is expected to translate as needed.
+    # Timing Intent
+    start_timestamp: ScriptTimestamp
+    maturity_timestamp: ScriptTimestamp
+
+    # Money Intent
+    # Note here that we can set either the short or long input sats, but not both
+    fixed_input_sats: Sats
+    fixed_input_side: Side
+    oracle: Type[OracleUnit]
+    short_leverage: ShortLeverage
+    long_leverage: LongLeverage
+    start_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch
+
+    # User Intent
+    maker_side: Side
+    short_mutual_redeem_public_key: PublicKey | '' = ''
+    long_mutual_redeem_public_key: PublicKey | '' = ''
+
+    @property
+    def proposal(self) -> ContractProposal:
+        # 1. Low liquidation price: the low price that triggers liquidation of the Long party.
+        # The value is rounded to achieve a result as close as possible to intent.
+        # There should be no integer-level loss of precision given the 32-bit range of oracle prices.
+        # In order to align with methodology of the canonical anyhedge library,
+        # we do an initial step to convert leverage to a price multiplier
+        low_liquidation_price_multiplier = 1 - (1 / self.long_leverage)
+        low_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(low_liquidation_price_multiplier * float(self.start_price_oracleUnits_per_bch)))
+
+        # 2. High liquidation price: the high price that triggers liquidation of the Short party.
+        # The value is rounded to achieve a result as close as possible to intent.
+        # There should be no integer-level loss of precision given the 32-bit range of oracle prices.
+        # In order to align with methodology of the canonical anyhedge library,
+        # we do an initial step to convert leverage to a price multiplier and detect if this is effectively
+        # a simple hedge or not.
+        try:
+            high_liquidation_price_multiplier = 1 + (1 / (self.short_leverage - 1))
+            is_simple_hedge = False
+        except ZeroDivisionError:
+            high_liquidation_price_multiplier = DEFAULT_HIGH_LIQUIDATION_PRICE_MULTIPLIER_FOR_SIMPLE_HEDGE
+            is_simple_hedge = True
+
+        # Use the multiplier to set the price
+        high_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(high_liquidation_price_multiplier * float(self.start_price_oracleUnits_per_bch)))
+
+        # 3. nominal hedge value in asset terms.
+        # Departing from the canonical intent derivation, here we calculate nominal hedge from the other parameters available
+        if self.fixed_input_side == Side.SHORT:
+            # Derive from short input sats
+            # Short needs to put in enough to cover movement on the short-losing (price increasing) side of the contract
+            #   short_input_sats = cost_sats_for_nominal_value_at_start - cost_sats_for_nominal_value_at_high_liquidation
+            # This further depends on whether this is a simple hedge or not as follows
+            if is_simple_hedge:
+                # For simple hedge, the cost at high liquidation is 0 (price is infinity). Therefore:
+                #   short_input_sats = cost_sats_for_nominal_value_at_start
+                # Expanding so that we can get at the nominal value
+                #   short_input_sats = nominal_oracleUnits_x_satsPerBch / start_price_oracleUnits_per_bch
+                #   nominal_oracleUnits_x_satsPerBch = short_input_sats * start_price_oracleUnits_per_bch
+                raw_nominal_oracleUnits_x_satsPerBch = self.fixed_input_sats * self.start_price_oracleUnits_per_bch
+                nominal_oracleUnits_x_satsPerBch = NominalOracleUnitsXSatsPerBch(round(raw_nominal_oracleUnits_x_satsPerBch))
+            else:
+                # For a leveraged short, the cost at high liquidation must be included as it is not zero.
+                # Expanding so that we can get at the nominal value
+                #   short_input_sats = (nominal_oracleUnits_x_satsPerBch / start_price_oracleUnits_per_bch) - (nominal_oracleUnits_x_satsPerBch / high_liquidation_price_oracleUnits_per_bch)
+                #   short_input_sats = nominal_oracleUnits_x_satsPerBch (1/start_price_oracleUnits_per_bch - 1/high_liquidation_price_oracleUnits_per_bch)
+                #   nominal_oracleUnits_x_satsPerBch = short_input_sats / (1/start_price_oracleUnits_per_bch - 1/high_liquidation_price_oracleUnits_per_bch)
+                raw_nominal_oracleUnits_x_satsPerBch = float(self.fixed_input_sats) / ((1 / self.start_price_oracleUnits_per_bch) - (1 / high_liquidation_price_oracleUnits_per_bch))
+                nominal_oracleUnits_x_satsPerBch = NominalOracleUnitsXSatsPerBch(round(raw_nominal_oracleUnits_x_satsPerBch))
+        else:
+            # Derive from long input sats
+            # Long needs to put in enough to cover movement on the long-losing (price decreasing) side of the contract
+            #   long_input_sats = cost_sats_for_nominal_value_at_low_liquidation - cost_sats_for_nominal_value_at_start
+            # Expanding so that we can get at the nominal value
+            #   long_input_sats = (nominal_oracleUnits_x_satsPerBch / low_liquidation_price_oracleUnits_per_bch) - (nominal_oracleUnits_x_satsPerBch / start_price_oracleUnits_per_bch)
+            #   long_input_sats = nominal_oracleUnits_x_satsPerBch (1/low_liquidation_price_oracleUnits_per_bch - 1/start_price_oracleUnits_per_bch)
+            #   nominal_oracleUnits_x_satsPerBch = long_input_sats / (1/low_liquidation_price_oracleUnits_per_bch - 1/start_price_oracleUnits_per_bch)
+            raw_nominal_oracleUnits_x_satsPerBch = float(self.fixed_input_sats) / ((1 / low_liquidation_price_oracleUnits_per_bch) - (1 / self.start_price_oracleUnits_per_bch))
+            nominal_oracleUnits_x_satsPerBch = NominalOracleUnitsXSatsPerBch(round(raw_nominal_oracleUnits_x_satsPerBch))
+
+        # 5. Cost in sats of the nominal hedge at high liquidation price.
+        # This is the value satsForHedgeAtHighLiq in the diagrams above.
+        # In summary, this value is needed to calculate Short's payout.
+        # Calculation of the value is discontinuous as follows:
+        if is_simple_hedge:
+            # a) For a simple hedge (short leverage = 1), the value is exactly 0. This
+            # represents the concept and calculation that Long must cover the full range
+            # of Short payouts from current price to infinity (where the cost becomes zero, this value).
+            cost_sats_for_nominal_value_at_high_liquidation = Sats(0)
+        else:
+            # b) For a leveraged short (short leverage > 1), the value is calculated from the
+            # other parameters in a simple cost relationship.
+            # Note: cost is floored for safety by bigint division in order to ensure that the
+            #       total sats in the contract cover a range that may be at worst +1 or +2 from
+            #       the "real" full precision value. This is valuable to ensure that contract
+            #       calculations never result in a value more than the total sats available.
+            cost_sats_for_nominal_value_at_high_liquidation = Sats(nominal_oracleUnits_x_satsPerBch // high_liquidation_price_oracleUnits_per_bch)
+
+        # 6. Cost in sats of the nominal hedge at low liquidation.
+        # This is the value satsForHedgeAtLowLiq in the diagrams above.
+        # In summary, this value is needed to calculate total input.
+        # Note: Here we use simple integer division and accept the loss of rounding.
+        #       Safety is ensured outside the zero case by validation.
+        # Note: We do zero testing here because this happens before parameter validation
+        #       which would catch it otherwise.
+        if low_liquidation_price_oracleUnits_per_bch <= 0:
+            raise ValueError('low liquidation price must be greater than zero')
+        cost_sats_for_nominal_value_at_low_liquidation = UtxoSats(nominal_oracleUnits_x_satsPerBch // low_liquidation_price_oracleUnits_per_bch)
+
+        # 7. Total input satoshis: the difference between worst case long and short outcomes.
+        total_input_sats = UtxoSats(cost_sats_for_nominal_value_at_low_liquidation - cost_sats_for_nominal_value_at_high_liquidation)
+
+        return ContractProposal(
+            address='',
+            short_mutual_redeem_public_key=self.short_mutual_redeem_public_key,
+            long_mutual_redeem_public_key=self.long_mutual_redeem_public_key,
+            start_timestamp=self.start_timestamp,
+            maturity_timestamp=self.maturity_timestamp,
+            nominal_oracleUnits_x_satsPerBch=nominal_oracleUnits_x_satsPerBch,
+            cost_sats_for_nominal_value_at_high_liquidation=cost_sats_for_nominal_value_at_high_liquidation,
+            total_input_sats=total_input_sats,
+            start_price_oracleUnits_per_bch=self.start_price_oracleUnits_per_bch,
+            high_liquidation_price_oracleUnits_per_bch=high_liquidation_price_oracleUnits_per_bch,
+            low_liquidation_price_oracleUnits_per_bch=low_liquidation_price_oracleUnits_per_bch,
+            oracle_public_key=self.oracle.public_key,
+            maker_side=self.maker_side,
+        )
+
+
 @dataclass(frozen=True)
 class ContractProposal:
     """Details of a proposed contract between a maker and taker. Does not include any funding oriented details such as fees."""
     # Unvalidated items, use empty string when unknown
     address: str
     short_mutual_redeem_public_key: PublicKey | ''
     long_mutual_redeem_public_key: PublicKey | ''
@@ -287,191 +564,14 @@
     def maker_input_oracleUnits(self) -> OracleUnit:
         return self.input_oracleUnits(role=Role.MAKER)
 
     @property
     def taker_input_oracleUnits(self) -> OracleUnit:
         return self.input_oracleUnits(role=Role.TAKER)
 
-    ###############
-    # Constructors
-    ###############
-    @staticmethod
-    def new_from_intent(start_timestamp: ScriptTimestamp,
-                        maturity_timestamp: ScriptTimestamp,
-                        nominal_oracleUnits: OracleUnit,
-                        long_leverage: LongLeverage,
-                        start_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch,
-                        maker_side: Side,
-                        # For upgrade to leveraged shorts, we establish a default of 1 representing the pure hedge position
-                        short_leverage: ShortLeverage = ShortLeverage(1),
-                        address: str = '',
-                        short_mutual_redeem_public_key: PublicKey | '' = '',
-                        long_mutual_redeem_public_key: PublicKey | '' = '',
-                        ) -> ContractProposal:
-
-        # Before calculating key values below, this is an outline of the setup, using relevant variable names.
-        #
-        # AnyHedge 0.12 with leveraged shorts works on the same concept as previous "simple/nominal hedge" versions.
-        # By including one more number, explained below, the contract can now provide independent leverage to Short and Long.
-        #
-        # In summary, Long uses AnyHedge to "buy" an asset now, "selling" it later for hopefully a higher price, and
-        # Short uses AnyHedge to "sell" an asset now, "buying" it later for hopefully a lower price.
-        #
-        # The hedge value / simple hedge / nominal hedge is a fixed asset value that the rest of the contract centers around.
-        # The original idea of AnyHedge is that at any price within the liquidation (more commonly "margin call") range,
-        # Short receives exactly the nominal hedge value at the end, paid in Bch. This is the definition of behavior for
-        # short leverage = 1, i.e. virtually holding another asset, using BCH as the vehicle instead of the asset itself.
-        #
-        # The setting of liquidation values is mathematically equivalent to setting leverage for Short and Long.
-        # In the original setup, only Long was mathematically bound to the liquidation price, establishing leverage.
-        # Short on the other hand had a liquidation price for safety purposes, but the behavior of Short payout was not bound
-        # mathematically to that liquidation price. The contract simply always paid out Short for the full hedge value,
-        # which at the absurd extreme can be achieved with one satoshi at a price approaching infinity.
-        #
-        # The current arrangement described below allows Short to achieve leverage by tying behavior to the high
-        # liquidation price if desired, or to retain original behavior by disconnecting from the high liquidation price.
-        # Given this setup at start, the contract is fully collateralized to handle any outcome within the liquidation range.
-        #
-        # The relationship between liquidation prices and effective leverage are not explained in depth here,
-        # but the summary is:
-        #     shortLeverage = 1 + (1 / ((highLiquidationPrice / startPrice) - 1))
-        #     longLeverage  = 1 / (1 - (lowLiquidationPrice / startPrice))
-        #
-        #  *Price in Asset/Bch*            *Cost of Hedge at Price (higher price ==> lower cost)*
-        # --------------------------------------------------------------------------------------------------------------------
-        #                        ^
-        #                        |
-        #  highLiquidationPrice  -    ---- satsForHedgeAtHighLiq (this is the new reference that allows short leverage)
-        #                        |    ||||                       (in the past, the assumption was zero cost at infinity)
-        #                        |    ||||
-        #                        |    |||| } shortInputSats = worst case "sell low buy high" case for short
-        #                        |    ||||                  = satsForHedgeAtStart - satsForHedgeAtHighLiq
-        #                        |    ||||
-        #                        |    ||||
-        #            startPrice  -    ---- satsForHedgeAtStart
-        #                        |    ||||
-        #                        |    |||| } longInputSats = worst case "buy high sell low" case for long
-        #                        |    ||||                 = satsForHedgeAtLowLiq - satsForHedgeAtStart
-        #                        |    ||||
-        #   lowLiquidationPrice  -    ---- satsForHedgeAtLowLiq (to reiterate, lowest price ==> highest cost)
-        #                        |
-        #                        |
-        #                        - 0
-        #
-        # Payout at the end of the contract is the same picture, except based on the end price instead of start Price.
-        #
-        #  *Price in Asset/Bch*            *Cost of Hedge at Price (higher price ==> lower cost)*
-        # --------------------------------------------------------------------------------------------------------------------
-        #                        ^
-        #                        |
-        #  highLiquidationPrice  -    ---- satsForHedgeAtHighLiq (zero at infinity for simple hedge)
-        #                        |    ||||
-        #                        |    |||| } shortPayoutSats = satsForHedgeAtEnd - satsForHedgeAtHighLiq
-        #                        |    ||||
-        #              endPrice  -    ---- satsForHedgeAtEnd (price moved up, Short gets more Bch, Long gets less)
-        #                        |    ||||
-        #                        |    ||||
-        #            startPrice  -    ||||
-        #                        |    ||||
-        #                        |    |||| } longPayinSats = satsForHedgeAtLowLiq - satsForHedgeAtEnd
-        #                        |    ||||
-        #                        |    ||||
-        #   lowLiquidationPrice  -    ---- satsForHedgeAtLowLiq
-        #                        |
-        #                        |
-        #                        - 0
-
-        # 1. Low liquidation price: the low price that triggers liquidation of the Long party.
-        # The value is rounded to achieve a result as close as possible to intent.
-        # There should be no integer-level loss of precision given the 32-bit range of oracle prices.
-        # In order to align with methodology of the canonical anyhedge library,
-        # we do an initial step to convert leverage to a price multiplier
-        low_liquidation_price_multiplier = 1 - (1 / long_leverage)
-        low_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(low_liquidation_price_multiplier * float(start_price_oracleUnits_per_bch)))
-
-        # 2. High liquidation price: the high price that triggers liquidation of the Short party.
-        # The value is rounded to achieve a result as close as possible to intent.
-        # There should be no integer-level loss of precision given the 32-bit range of oracle prices.
-        # In order to align with methodology of the canonical anyhedge library,
-        # we do an initial step to convert leverage to a price multiplier and detect if this is effectively
-        # a simple hedge or not.
-        try:
-            high_liquidation_price_multiplier = 1 + (1 / (short_leverage - 1))
-            is_simple_hedge = False
-        except ZeroDivisionError:
-            # In this library design, there is no explicit multiplier to establish a liquidation price
-            # in the case of a simple hedge (short leverage = 1). We choose simply 10x.
-            high_liquidation_price_multiplier = 10.0
-            is_simple_hedge = True
-
-        # Use the multiplier to set the price
-        high_liquidation_price_oracleUnits_per_bch = ScriptPriceInOracleUnitsPerBch(round_half_up(high_liquidation_price_multiplier * float(start_price_oracleUnits_per_bch)))
-
-        # 3. Composite number representing the nominal hedge value in asset terms.
-        # In the diagrams above, this is the value discussed as "Hedge"
-        # Note: Rather than using the nominal hedge value alone, the number is calculated as
-        #       (nominal hedge units * 1e8 sats/bch). This allows the critical calculation in the contract to be simple
-        #       division, and is also a carryover from previous BCH VM versions (before May 2022) that did not have
-        #       multiplication. I.e. this value divided by the oracle price directly yields satoshis for
-        #       nominal hedge value at the given price, which is the final units we need to establish payouts.
-        # Note: DO NOT CONVERT THE COMPOSITE VALUE TO A floating point NUMBER FOR ANY REASON.
-        #       Any such calculations or transmissions (e.g. through simple JSON) must be
-        #       considered to introduce undefined behavior and be rejected.
-        #       The initial float calculation is a one way translation from floating precision
-        #       nominalUnits input to BigInt.
-        nominal_oracleUnits_x_satsPerBch = NominalOracleUnitsXSatsPerBch(round_half_up(nominal_oracleUnits * SATS_PER_BCH))
-
-        # 4. Cost in sats of the nominal hedge at high liquidation price.
-        # This is the value satsForHedgeAtHighLiq in the diagrams above.
-        # In summary, this value is needed to calculate Short's payout.
-        # Calculation of the value is discontinuous as follows:
-        if is_simple_hedge:
-            # a) For a simple hedge (short leverage = 1), the value is exactly 0. This
-            # represents the concept and calculation that Long must cover the full range
-            # of Short payouts from current price to infinity (where the cost becomes zero, this value).
-            cost_sats_for_nominal_value_at_high_liquidation = Sats(0)
-        else:
-            # b) For a leveraged short (short leverage > 1), the value is calculated from the
-            # other parameters in a simple cost relationship.
-            # Note: cost is floored for safety by bigint division in order to ensure that the
-            #       total sats in the contract cover a range that may be at worst +1 or +2 from
-            #       the "real" full precision value. This is valuable to ensure that contract
-            #       calculations never result in a value more than the total sats available.
-            cost_sats_for_nominal_value_at_high_liquidation = nominal_oracleUnits_x_satsPerBch // high_liquidation_price_oracleUnits_per_bch
-
-        # 5. Cost in sats of the nominal hedge at low liquidation.
-        # This is the value satsForHedgeAtLowLiq in the diagrams above.
-        # In summary, this value is needed to calculate total input.
-        # Note: Here we use simple integer division and accept the loss of rounding.
-        #       Safety is ensured outside the zero case by validation.
-        # Note: We do zero testing here because this happens before parameter validation
-        #       which would catch it otherwise.
-        if low_liquidation_price_oracleUnits_per_bch <= 0:
-            raise ValueError('low liquidation price must be greater than zero')
-        cost_sats_for_nominal_value_at_low_liquidation = UtxoSats(nominal_oracleUnits_x_satsPerBch // low_liquidation_price_oracleUnits_per_bch)
-
-        # 6. Total input satoshis: the difference between worst case long and short outcomes.
-        total_input_sats = UtxoSats(cost_sats_for_nominal_value_at_low_liquidation - cost_sats_for_nominal_value_at_high_liquidation)
-
-        return ContractProposal(
-            address=address,
-            short_mutual_redeem_public_key=short_mutual_redeem_public_key,
-            long_mutual_redeem_public_key=long_mutual_redeem_public_key,
-            start_timestamp=start_timestamp,
-            maturity_timestamp=maturity_timestamp,
-            nominal_oracleUnits_x_satsPerBch=nominal_oracleUnits_x_satsPerBch,
-            cost_sats_for_nominal_value_at_high_liquidation=cost_sats_for_nominal_value_at_high_liquidation,
-            total_input_sats=total_input_sats,
-            start_price_oracleUnits_per_bch=start_price_oracleUnits_per_bch,
-            high_liquidation_price_oracleUnits_per_bch=high_liquidation_price_oracleUnits_per_bch,
-            low_liquidation_price_oracleUnits_per_bch=low_liquidation_price_oracleUnits_per_bch,
-            oracle_public_key=nominal_oracleUnits.public_key,
-            maker_side=maker_side,
-        )
-
     def neutralize(self,
                    current_price_oracleUnitsPerBch: ScriptPriceInOracleUnitsPerBch,
                    current_timestamp: ScriptTimestamp,
                    ) -> ContractProposal:
         neutralizing_proposal = ContractProposal(
             # reset / unimplemented
             address='',
```

### Comparing `anyhedge-2.1.4/anyhedge/fee.py` & `anyhedge-3.0.0/anyhedge/fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.4/anyhedge/oracle.py` & `anyhedge-3.0.0/anyhedge/oracle.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,20 +55,20 @@
         validators.equal(pricepoints, unique_pricepoints)
 
         # ensure sorting. not efficient but performance is not yet an issue
         sorted_pricepoints = cls._sort_pricepoints(unique_pricepoints)
         validators.equal(unique_pricepoints, sorted_pricepoints)
 
     @staticmethod
-    def _sort_pricepoints(pricepoints: Sequence[Pricepoint]) -> tuple[Pricepoint]:
+    def _sort_pricepoints(pricepoints: Sequence[Pricepoint]) -> tuple[Pricepoint, ...]:
         return tuple(sorted(pricepoints, key=lambda p: p.timestamp))
 
     @staticmethod
-    def _make_pricepoints_unique(pricepoints: Sequence[Pricepoint]) -> tuple[Pricepoint]:
-        lookup = {}
+    def _make_pricepoints_unique(pricepoints: Sequence[Pricepoint]) -> tuple[Pricepoint, ...]:
+        lookup: dict[ScriptTimestamp, Pricepoint] = {}
         for p in pricepoints:
             existing = lookup.get(p.timestamp)
             if existing is None:
                 lookup[p.timestamp] = p
             else:
                 if p == existing:
                     # it's an equal duplicate so just ignore it
```

### Comparing `anyhedge-2.1.4/anyhedge/tests/test_bch_primitives.py` & `anyhedge-3.0.0/anyhedge/tests/test_bch_primitives.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.4/anyhedge/tests/test_contract.py` & `anyhedge-3.0.0/anyhedge/tests/test_contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 from ..bch_primitives import (
     SATS_PER_BCH,
     Sats,
     ScriptTimestamp,
     UtxoSats,
 )
 from ..contract import (
+    ContractFromInputSatsAndLeverages,
+    ContractFromNominalHedgeAndLeverages,
     ContractFunding,
     ContractProposal,
     ContractRedemption,
+    RedemptionType,
+    UnredeemableError,
+)
+from ..contract_primitives import (
     LongLeverage,
     NominalOracleUnitsXSatsPerBch,
-    RedemptionType,
+    Role,
     ShortLeverage,
     Side,
-    UnredeemableError,
 )
 from ..fee import FeeAgreement
 from ..oracle import (
     OracleUnit,
     ScriptPriceInOracleUnitsPerBch,
     UsdEM2Beta,
 )
-from ..role import Role
 
 
 ###################
 # Contract Tests
 ###################
 # Generic intent values, not always perfectly reproducible from the contract
 START_TIMESTAMP = ScriptTimestamp(Arrow(year=2021, month=10, day=21).int_timestamp)
@@ -123,23 +127,24 @@
     maturity_timestamp: ScriptTimestamp = MATURITY_TIMESTAMP,
     nominal_oracleUnits: OracleUnit = NOMINAL_VALUE_USDEM2,
     long_leverage: LongLeverage = LONG_LEVERAGE,
     start_price_oracleUnits_per_bch: ScriptPriceInOracleUnitsPerBch = START_PRICE_USDEM2_PER_BCH,
     maker_side: Side = Side.SHORT,
     short_leverage: ShortLeverage = SHORT_LEVERAGE_1_AS_HEDGE,
 ) -> ContractProposal:
-    return ContractProposal.new_from_intent(
+    intent = ContractFromNominalHedgeAndLeverages(
         start_timestamp=start_timestamp,
         maturity_timestamp=maturity_timestamp,
         nominal_oracleUnits=nominal_oracleUnits,
+        short_leverage=short_leverage,
         long_leverage=long_leverage,
         start_price_oracleUnits_per_bch=start_price_oracleUnits_per_bch,
         maker_side=maker_side,
-        short_leverage=short_leverage,
     )
+    return intent.proposal
 
 
 class TestContractProposalDerivedValues(unittest.TestCase):
     ######################
     # Exact contract parameters, some root values, some derived from root values
     ######################
     def test_nominal_oracleUnits_x_satsPerBch(self):
@@ -237,24 +242,24 @@
 
 
 class TestContractProposalNeutralize(unittest.TestCase):
     def test_neutralize_creates_an_opposite_virtual_hedge_at_current_price(self):
         # Use a base case and hand-constructed neutralizing contract to confirm actual result
 
         # Construct the base case
-        base_proposal = ContractProposal.new_from_intent(
+        base_intent = ContractFromNominalHedgeAndLeverages(
             start_timestamp=START_TIMESTAMP,
             maturity_timestamp=MATURITY_TIMESTAMP,
             nominal_oracleUnits=NOMINAL_VALUE_USDEM2,
+            short_leverage=ShortLeverage(1.0),
             long_leverage=LongLeverage(5.0),
             start_price_oracleUnits_per_bch=START_PRICE_USDEM2_PER_BCH,
             maker_side=Side.SHORT,
-            short_leverage=ShortLeverage(1.0),
-            address='',
         )
+        base_proposal = base_intent.proposal
 
         # Manually construct the neutralizing contract
         neutralizing_price = ScriptPriceInOracleUnitsPerBch(190_00)
         neutralizing_timestamp = ScriptTimestamp(round((START_TIMESTAMP + MATURITY_TIMESTAMP) / 2))
         expected_neutralizing_contract = ContractProposal(
             address='',
             short_mutual_redeem_public_key='',
@@ -764,16 +769,84 @@
         self.assertEqual(hedge_redemption.cost_sats_for_nominal_value_at_redemption, hedge_redemption.short_payout_sats)
 
         # leveraged short redemption is different from short payout
         self.assertNotEqual(leveraged_short_redemption.cost_sats_for_nominal_value_at_redemption, leveraged_short_redemption.short_payout_sats)
         self.assertEqual(leveraged_short_redemption.cost_sats_for_nominal_value_at_redemption, COST_SATS_FOR_NOMINAL_VALUE_AT_REDEMPTION)
 
 
-class TestContractSide(unittest.TestCase):
-    def test_from_string_works_for_known_api_values(self):
-        self.assertEqual(Side.from_string('short'), Side.SHORT)
-        self.assertEqual(Side.from_string('hedge'), Side.SHORT)
-        self.assertEqual(Side.from_string('long'), Side.LONG)
+class TestIntent(unittest.TestCase):
+    def test_round_trip_from_canonical_intent_to_contract_then_to_bch_input_intent_results_in_identical_contract(self):
+        # start with standard proposals
+        hedge = standard_contract_proposal(short_leverage=ShortLeverage(1.0))
+        short = standard_contract_proposal(short_leverage=ShortLeverage(3.0))
+
+        # create new contracts based on some original values + effective values using the bch input intent
+        hedge_by_short_input = ContractFromInputSatsAndLeverages(
+            start_timestamp=hedge.start_timestamp,
+            maturity_timestamp=hedge.maturity_timestamp,
+            fixed_input_sats=hedge.short_input_sats,
+            fixed_input_side=Side.SHORT,
+            oracle=hedge.oracle_unit_cls,
+            short_leverage=hedge.effective_short_leverage,
+            long_leverage=hedge.effective_long_leverage,
+            start_price_oracleUnits_per_bch=hedge.start_price_oracleUnits_per_bch,
+            maker_side=hedge.maker_side,
+        ).proposal
+        hedge_by_long_input = ContractFromInputSatsAndLeverages(
+            start_timestamp=hedge.start_timestamp,
+            maturity_timestamp=hedge.maturity_timestamp,
+            fixed_input_sats=hedge.long_input_sats,
+            fixed_input_side=Side.LONG,
+            oracle=hedge.oracle_unit_cls,
+            short_leverage=hedge.effective_short_leverage,
+            long_leverage=hedge.effective_long_leverage,
+            start_price_oracleUnits_per_bch=hedge.start_price_oracleUnits_per_bch,
+            maker_side=hedge.maker_side,
+        ).proposal
+        short_by_short_input = ContractFromInputSatsAndLeverages(
+            start_timestamp=short.start_timestamp,
+            maturity_timestamp=short.maturity_timestamp,
+            fixed_input_sats=short.short_input_sats,
+            fixed_input_side=Side.SHORT,
+            oracle=short.oracle_unit_cls,
+            short_leverage=short.effective_short_leverage,
+            long_leverage=short.effective_long_leverage,
+            start_price_oracleUnits_per_bch=short.start_price_oracleUnits_per_bch,
+            maker_side=short.maker_side,
+        ).proposal
+        short_by_long_input = ContractFromInputSatsAndLeverages(
+            start_timestamp=short.start_timestamp,
+            maturity_timestamp=short.maturity_timestamp,
+            fixed_input_sats=short.long_input_sats,
+            fixed_input_side=Side.LONG,
+            oracle=short.oracle_unit_cls,
+            short_leverage=short.effective_short_leverage,
+            long_leverage=short.effective_long_leverage,
+            start_price_oracleUnits_per_bch=short.start_price_oracleUnits_per_bch,
+            maker_side=short.maker_side,
+        ).proposal
+
+        # confirm that the remade contracts exactly match the original contracts
+        # There are possibly unresolvable off-by-one type differences in the final results. Therefore, we can't use simple assertEqual.
+        # Instead we compare the most relevant values and confirm they are very close in % terms.
+        for i, (original, recreated) in enumerate((
+            (hedge, hedge_by_short_input),
+            (hedge, hedge_by_long_input),
+            (short, short_by_short_input),
+            (short, short_by_long_input),
+        )):
+            # Failure message for group:
+            error_msg = f'failed on index {i}'
+
+            # Confirm that some values are exactly equal
+            self.assertEqual(recreated.low_liquidation_price_oracleUnits_per_bch, original.low_liquidation_price_oracleUnits_per_bch, msg=error_msg)
+
+            # Confirm that downstream values are very close. Use BCH since that allows almostEqual to work on standard decimal places
+            self.assertAlmostEqual(recreated.nominal_oracleUnits_x_satsPerBch / SATS_PER_BCH, original.nominal_oracleUnits_x_satsPerBch / SATS_PER_BCH, places=3, msg=error_msg)
+            self.assertAlmostEqual(recreated.total_input_sats.bch, original.total_input_sats.bch, msg=error_msg)
+            self.assertAlmostEqual(recreated.cost_sats_for_nominal_value_at_high_liquidation.bch, original.cost_sats_for_nominal_value_at_high_liquidation.bch, msg=error_msg)
+            self.assertAlmostEqual(recreated.short_input_sats.bch / SATS_PER_BCH, original.short_input_sats.bch / SATS_PER_BCH, msg=error_msg)
+            self.assertAlmostEqual(recreated.long_input_sats.bch / SATS_PER_BCH, original.long_input_sats.bch / SATS_PER_BCH, msg=error_msg)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `anyhedge-2.1.4/anyhedge/tests/test_fee.py` & `anyhedge-3.0.0/anyhedge/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.4/anyhedge/tests/test_oracle.py` & `anyhedge-3.0.0/anyhedge/tests/test_oracle.py`

 * *Files identical despite different names*

### Comparing `anyhedge-2.1.4/anyhedge.egg-info/PKG-INFO` & `anyhedge-3.0.0/anyhedge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyhedge
-Version: 2.1.4
+Version: 3.0.0
 Summary: Basic components of AnyHedge contracts
 Author-email: emergent_reasons <emergent_reasons@gmail.com>
 License: Copyright (c) 2022 emergent_reasons
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `anyhedge-2.1.4/pyproject.toml` & `anyhedge-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'anyhedge'
-version = '2.1.4'
+version = '3.0.0'
 authors = [
   { name='emergent_reasons', email='emergent_reasons@gmail.com' },
 ]
 license = { file = "LICENSE" }
 description = 'Basic components of AnyHedge contracts'
 readme = 'README.md'
 requires-python = '>=3.10'
```

