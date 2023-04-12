# Comparing `tmp/infinitesimals-0.0.6.tar.gz` & `tmp/infinitesimals-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinitesimals-0.0.6.tar", last modified: Mon Apr 10 22:23:20 2023, max compression
+gzip compressed data, was "infinitesimals-0.1.0.tar", last modified: Wed Apr 12 20:38:22 2023, max compression
```

## Comparing `infinitesimals-0.0.6.tar` & `infinitesimals-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 22:23:20.605577 infinitesimals-0.0.6/
--rw-rw-rw-   0        0        0      152 2023-04-10 22:22:53.000000 infinitesimals-0.0.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      897 2023-04-10 22:23:20.604579 infinitesimals-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-04-10 19:05:04.000000 infinitesimals-0.0.6/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-10 22:23:20.584632 infinitesimals-0.0.6/infinitesimals/
--rw-rw-rw-   0        0        0    10188 2023-04-10 22:21:37.000000 infinitesimals-0.0.6/infinitesimals/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-04-10 22:22:37.000000 infinitesimals-0.0.6/infinitesimals/example.py
-drwxrwxrwx   0        0        0        0 2023-04-10 22:23:20.603582 infinitesimals-0.0.6/infinitesimals.egg-info/
--rw-rw-rw-   0        0        0      897 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-10 22:23:20.000000 infinitesimals-0.0.6/infinitesimals.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 22:23:20.605577 infinitesimals-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      893 2023-04-10 22:23:16.000000 infinitesimals-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:38:22.194996 infinitesimals-0.1.0/
+-rw-rw-rw-   0        0        0      419 2023-04-12 20:38:12.000000 infinitesimals-0.1.0/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 infinitesimals-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-10 19:18:21.000000 infinitesimals-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1208 2023-04-12 20:38:22.193999 infinitesimals-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2023-04-12 20:32:04.000000 infinitesimals-0.1.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-12 20:38:22.163081 infinitesimals-0.1.0/infinitesimals/
+-rw-rw-rw-   0        0        0    10958 2023-04-12 20:36:04.000000 infinitesimals-0.1.0/infinitesimals/__init__.py
+-rw-rw-rw-   0        0        0     3670 2023-04-12 20:20:19.000000 infinitesimals-0.1.0/infinitesimals/example.py
+drwxrwxrwx   0        0        0        0 2023-04-12 20:38:22.193002 infinitesimals-0.1.0/infinitesimals.egg-info/
+-rw-rw-rw-   0        0        0     1208 2023-04-12 20:38:22.000000 infinitesimals-0.1.0/infinitesimals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-12 20:38:22.000000 infinitesimals-0.1.0/infinitesimals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-12 20:38:22.000000 infinitesimals-0.1.0/infinitesimals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-04-12 20:38:22.000000 infinitesimals-0.1.0/infinitesimals.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-12 20:38:22.000000 infinitesimals-0.1.0/infinitesimals.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-12 20:38:22.194996 infinitesimals-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      947 2023-04-12 20:32:16.000000 infinitesimals-0.1.0/setup.py
```

### Comparing `infinitesimals-0.0.6/LICENSE.txt` & `infinitesimals-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `infinitesimals-0.0.6/infinitesimals/__init__.py` & `infinitesimals-0.1.0/infinitesimals/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,251 @@
+import itertools as it
+import more_itertools as mit
+import numpy as np
 import math
-from warnings import simplefilter
-from itertools import zip_longest
-from numpy import convolve, matrix, array
-from numpy.linalg import LinAlgError
-from numpy.linalg import matrix_power
-from numpy.polynomial.polynomial import polypow
 from scipy.special import binom
-from scipy.linalg import fractional_matrix_power, expm, logm, sqrtm
-from scipy.linalg._matfuncs_inv_ssq import LogmExactlySingularWarning
 
-simplefilter('error', LogmExactlySingularWarning)
 
 PRECISION = 32
 
 
-def sqrt(x):
-    if is_real(x):
-        return HyperReal(sqrt(x))
-    if isinstance(x, HyperReal):
-        k = 0
-        while not any(x[:2]):
-            x <<= 2
-            k += 1
-        result = HyperReal.from_matrix(sqrtm(x.to_matrix(PRECISION))) >> k
-        if 'nan' in str(result):
-            raise ValueError
-        return result
-
-
-def sin(x):
-    """calculates the sine of a hyperreal through the taylor series"""
-    if isinstance(x, HyperReal) and x.st:
-        _st, _inf = x.split()
-        return math.sin(_st) * cos(_inf) + math.cos(_st) * sin(_inf)
-    return sum((-1 if n % 2 else 1) * (x ** (2 * n + 1)) / math.factorial(2 * n + 1) for n in range(PRECISION))
-
+def convolution_power(a, n):
+    """De Pril, N. (1985). Recursions for Convolutions of Arithmetic Distributions"""
+    b = [a[0] ** n]
+    for k in range(1, len(a)):
+        b.append(sum((((n + 1) * j - k) * a[j] * b[k - j]) / k for j in range(1, k + 1) if a[j] and b[k - j]) / a[0])
+    return b
+
+
+def superscript(n):
+    """converts numbers to superscript strings. useful for exponents."""
+    _superscript = {
+        '-': '⁻',
+        '.': '⋅',
+        '0': '⁰',
+        '1': '¹',
+        '2': '²',
+        '3': '³',
+        '4': '⁴',
+        '5': '⁵',
+        '6': '⁶',
+        '7': '⁷',
+        '8': '⁸',
+        '9': '⁹',
+    }
+    return ''.join(_superscript[character] for character in str(n))
 
-def cos(x):
-    """calculates the cosine of a hyperreal through the taylor series"""
-    if isinstance(x, HyperReal) and x.st:
-        _st, _inf = x.split()
-        return math.cos(_st) * cos(_inf) - math.sin(_st) * sin(_inf)
-    return sum((-1 if n % 2 else 1) * (x ** (2 * n)) / math.factorial(2 * n) for n in range(PRECISION))
-
-
-def tan(x):
-    return sin(x) / cos(x)
 
+def hyperrealify(function):
+    """decorator to automatically convert arguments into type HyperReal"""
+    def inner(*args):
+        return function(*(HyperReal(arg) if isinstance(arg, int) or isinstance(arg, float) else arg for arg in args))
+    return inner
 
-def superscript_int(n, enclose=False):
-    if enclose:
-        return f'⁽{superscript_int(n)}⁾'
-    return ''.join('⁰¹²³⁴⁵⁶⁷⁸⁹'[int(digit)] for digit in str(n))
 
+def sqrt(x):
+    return x ** .5
 
-def matrix_to_matrix(M, N):
-    """calculates a matrix to the power of another matrix through the exponential series"""
-    return expm(logm(M) * N)
 
+def log(x, base=None):
+    """calculates the logarithm based on a series expansion from https://en.wikipedia.org/wiki/Natural_logarithm"""
+    if base:
+        return log(x) / log(base)
+    _x = ((x - 1) / (x + 1))
+    _x2 = _x * _x
+    return 2 * _x * sum((_x2 ** n) / (2 * n + 1) for n in range(PRECISION))
 
-def hyperrealify(function):
-    """decorator to parse all real number arguments into hyperreals"""
 
-    def inner(*args):
-        return function(*(HyperReal(arg) if is_real(arg) else arg for arg in args))
+def exp(x):
+    """calculates the exponential function from its series expansion"""
+    return 1 + x + sum((x ** n) / math.factorial(n) for n in range(2, PRECISION))
 
-    return inner
 
+def sin(x):
+    """calculates the sine through the taylor series"""
+    return sum((-1 if n % 2 else 1) * (x ** (2 * n + 1)) / math.factorial(2 * n + 1) for n in range(PRECISION))
 
-def is_real(x):
-    return isinstance(x, bool) or isinstance(x, int) or isinstance(x, float)
 
+def cos(x):
+    """calculates the cosine through the taylor series"""
+    return sum((-1 if n % 2 else 1) * (x ** (2 * n)) / math.factorial(2 * n) for n in range(PRECISION))
 
-def exp(x):
-    if is_real(x):
-        return HyperReal(math.exp(x))
-    if isinstance(x, HyperReal):
-        return HyperReal.from_matrix(expm(x.to_matrix(PRECISION)))
 
+def tan(x):
+    return sin(x) / cos(x)
 
-def log(x, base=None):
-    if base:
-        return log(x) / log(base)
-    if is_real(x):
-        return HyperReal(math.log(x))
-    if isinstance(x, HyperReal):
-        return HyperReal.from_matrix(logm(x.to_matrix(PRECISION)))
-
-
-def repr_polynomial(coefficients, variable, mode):
-    """makes a nice looking representation of polynomial. useful for polynomials of infinitesimals"""
-
-    def enclose(text, condition):
-        return f'({text})' if condition else text
-
-    p = ['unicode', 'pythonic'].index(mode)
-    s = ''
-    c = 0
-    for i, v in enumerate(coefficients):
-        if not v:
-            continue
-        s += ('-' if v < 0 else '+') if c else ''
-        s += (str(abs(v)) if i == 0 or v != 1 else '') + ('*' if v != 1 and i > 0 and p else '')
-        s += enclose(variable + ((superscript_int(i) if not p else f'**{i}') if i > 1 else ''), p and i > 1) if i else ''
-        c += 1
-    return enclose(s, c > 1) if c else '0'
 
+class HyperReal:
+    """A number class capable of representing infinitesimals and infinities"""
+    def __init__(self, *coefficients, max_power=0):
+        coefficients = list(coefficients)
+        while any(coefficients) and not coefficients[0]:
+            del coefficients[0]
+            max_power -= 1
+        self.coefficients = np.array(list(mit.padded(coefficients[:PRECISION], 0, PRECISION)), dtype=np.float64)
+        self._max_power = max_power
 
-class HyperReal(tuple):
-    def __new__(cls, *args):
-        if not args:
-            return tuple.__new__(cls, (0,))
-        if not all(is_real(arg) for arg in args):
-            raise ValueError('arguments must be real')
-        return tuple.__new__(cls, args)
+    @property
+    def max_power(self):
+        return int(self._max_power) if int(self._max_power) == self._max_power else self._max_power
 
     def __repr__(self):
-        return repr_polynomial(self, 'ε', 'pythonic')
+        if not self:
+            return '0'
 
-    def __str__(self):
-        return repr_polynomial(self, 'ε', 'unicode')
+        def _str(x):
+            s = str(x)
+            if 'e' in s:
+                i = s.index('e')
+                s = s[:i] + '·10' + superscript(s[i+1:])
+            return s
+
+        string = ''
+        terms = 0
+        for i, coefficient in enumerate(self.coefficients):
+            if not coefficient:
+                continue
+            power = i - self.max_power
+            if int(power) == power:
+                power = int(power)
+            sign = '-' if coefficient < 0 else '+' if terms else ''
+            mag = _str(abs(coefficient)) if power == 0 or abs(coefficient) != 1 else ''
+            variable = 'ε' if power > 0 else 'ω' if power else ''
+            power = superscript(abs(power)) if 0 != abs(power) != 1 else ''
+            string += sign + mag + variable + power
+            terms += 1
+        return string if terms == 1 else '(%s)' % string
+
+    def __getitem__(self, power):
+        """returns the corresponding term with the same omega-power"""
+        index = self.max_power - power
+        if 0 <= index < len(self.coefficients):
+            if int(index) == index:
+                index = int(index)
+            return self.coefficients[index]
+        return 0
 
     @hyperrealify
     def __eq__(self, other):
-        return all(x == y for x, y in zip_longest(self, other, fillvalue=0))
+        if not other:
+            return not self
+        if self.max_power != other.max_power:
+            return False
+        for x, y in it.zip_longest(self.coefficients, other.coefficients, fillvalue=0):
+            if x != y:
+                return False
+        return True
 
     @hyperrealify
     def __lt__(self, other):
-        for x, y in zip_longest(self, other, fillvalue=0):
+        if not other:
+            return self[self.max_power] < 0
+        if self.max_power < other.max_power:
+            return True
+        if self.max_power > other.max_power:
+            return False
+        for x, y in it.zip_longest(self.coefficients, other.coefficients, fillvalue=0):
             if x < y:
                 return True
             elif x > y:
                 return False
         return False
 
-    @hyperrealify
     def __le__(self, other):
-        return (self < other) or (self == other)
+        return self < other or self == other
 
-    @hyperrealify
     def __gt__(self, other):
-        return not (self <= 0)
+        return not (self <= other)
 
-    @hyperrealify
     def __ge__(self, other):
         return not (self < other)
 
-    def __neg__(self):
-        return HyperReal(*(-x for x in self))
+    def __abs__(self):
+        return -self if self < 0 else self
 
     @hyperrealify
-    def __sub__(self, other):
-        return self.__add__(-other)
-
-    @hyperrealify
-    def __rsub__(self, other):
-        return -self.__sub__(other)
+    def __neg__(self):
+        return HyperReal(*(-x for x in self.coefficients), max_power=self.max_power)
 
     @hyperrealify
     def __add__(self, other):
-        return HyperReal(*(x + y for x, y in zip_longest(self, other, fillvalue=0)))
+        max_power_dif = other.max_power - self.max_power
+        if max_power_dif % 1:
+            raise ValueError('cannot add power series with non-integer power differences')
+        max_power_dif = int(max_power_dif)
+        return HyperReal(*(a + b
+                           for a, b in it.zip_longest(it.chain(it.repeat(0, max_power_dif), self.coefficients),
+                                                      it.chain(it.repeat(0, -max_power_dif), other.coefficients),
+                                                      fillvalue=0)),
+                         max_power=max(self.max_power, other.max_power))
 
     @hyperrealify
-    def __rand__(self, other):
-        """Returns the dot product (element-wise multiplication)"""
-        return other.__and__(self)
+    def __radd__(self, other):
+        return other.__add__(self)
 
     @hyperrealify
-    def __and__(self, other):
-        """Returns the dot product (element-wise multiplication)"""
-        return HyperReal(*(x * y for x, y in zip_longest(self, other, fillvalue=0)))
+    def __sub__(self, other):
+        return self.__add__(-other)
 
     @hyperrealify
-    def __radd__(self, other):
-        return other.__add__(self)
+    def __rsub__(self, other):
+        return other.__sub__(self)
 
     @hyperrealify
     def __mul__(self, other):
-        return HyperReal(*convolve(self, other).tolist())
+        return HyperReal(*np.convolve(self.coefficients, other.coefficients),
+                         max_power=self.max_power + other.max_power)
 
     @hyperrealify
     def __rmul__(self, other):
         return other.__mul__(self)
 
+    @hyperrealify
     def __truediv__(self, other):
-        try:
-            if is_real(other):
-                return HyperReal(*(x / other for x in self))
-            if isinstance(other, HyperReal):
-                _self, _other = self, other
-                while _other.inf and not _self.st and not _other.st:
-                    _self <<= 1
-                    _other <<= 1
-                return _self * (_other ** -1)
-        except ZeroDivisionError:
-            raise ZeroDivisionError(f'division by infinitesimal')
+        return self * (other ** -1)
 
     @hyperrealify
     def __rtruediv__(self, other):
         return other.__truediv__(self)
 
+    @hyperrealify
+    def __pow__(self, power, modulo=None):
+        if modulo:
+            return self.__pow__(power) % modulo
+        if power == 0:
+            return HyperReal(1)
+        if is_real(power):
+            power = power.real
+            return HyperReal(*convolution_power(list(mit.padded(self.coefficients, 0, PRECISION)), power),
+                             max_power=self.max_power * power)
+        return (self ** st(power)) * exp(inf(power) * log(self))
+
+    @hyperrealify
+    def __rpow__(self, other):
+        return other.__pow__(self)
+
     def __floor__(self):
-        _st, _inf = self.split()
-        return math.floor(_st) - int(_st % 1 == 0 and _inf < 0)
+        if self.max_power % 1:
+            raise ValueError('non-integer infinite or infinitesimal powers cannot be floored')
+        _sum = 0
+        for power in range(0, self.max_power + 1):
+            large_part = self[power]
+            small_part = HyperReal(*self.coefficients[self.max_power + 1 - power:], max_power=power - 1)
+            _sum += math.floor(large_part) * (omega ** power) - int(large_part % 1 == 0 and small_part < 0)
+        return _sum
 
     def __ceil__(self):
-        _st, _inf = self.split()
-        return math.ceil(_st) + int(_st % 1 == 0 and _inf > 0)
+        if self.max_power % 1:
+            raise ValueError('non-integer infinite or infinitesimal powers cannot be ceiled')
+        _sum = 0
+        for power in range(0, self.max_power + 1):
+            large_part = self[power]
+            small_part = HyperReal(*self.coefficients[self.max_power + 1 - power:], max_power=power - 1)
+            _sum += math.ceil(large_part) * (omega ** power) + int(large_part % 1 == 0 and small_part > 0)
+        return _sum
 
     def __mod__(self, other):
         return self - other * (self // other)
 
     @hyperrealify
     def __rmod__(self, other):
         return other.__mod__(self)
@@ -219,118 +254,87 @@
     def __floordiv__(self, other):
         return (self / other).__floor__()
 
     @hyperrealify
     def __rfloordiv__(self, other):
         return other.__floordiv__(self)
 
-    @hyperrealify
-    def __rpow__(self, other):
-        return other.__pow__(self)
+    def __round__(self, n=0):
+        if self.max_power % 1:
+            raise ValueError('non-integer infinite or infinitesimal powers cannot be rounded')
+        _sum = 0
+        for power in range(0, self.max_power + 1):
+            large_part = self[power]
+            small_part = HyperReal(*self.coefficients[self.max_power + 1 - power:], max_power=power - 1)
+            last_digit = round(large_part * (10 ** (n + 1))) % 10
+            first_digits = math.floor(large_part * (10 ** n)) + int(last_digit > 5 or (last_digit == 5 and small_part > 0))
+            _sum += round(first_digits * (10 ** - n), n) * (omega ** power)
+        return _sum
 
-    def __pow__(self, power, modulo=None):
-        if modulo:
-            return self.__pow__(power) % modulo
-        if isinstance(power, int) and power >= 0:
-            return HyperReal(*polypow(self, power))
-        try:
-            if isinstance(power, int):
-                return HyperReal.from_matrix(matrix_power(self.to_matrix(PRECISION), power))
-            if isinstance(power, float):
-                return HyperReal.from_matrix(fractional_matrix_power(self.to_matrix(PRECISION), power))
-            if isinstance(power, HyperReal):
-                return HyperReal.from_matrix(
-                    matrix_to_matrix(self.to_matrix(PRECISION), power.to_matrix(PRECISION)))
-        except LinAlgError:
-            raise ZeroDivisionError(f'{self} cannot be raised to a negative power')
-        except LogmExactlySingularWarning:
-            raise ZeroDivisionError(f'{self} cannot be raised to an infinitesimal power')
+    def __int__(self):
+        if not self - self[0]:
+            return self[0]
+        raise ValueError(f'cannot convert {self} to integer')
 
     def __bool__(self):
-        return any(self)
-
-    def __round__(self, n=0):
-        last_digit = round(self.st * (10 ** (n + 1))) % 10
-        first_digits = math.floor(self.st * (10 ** n)) + int(last_digit == 5 and self.inf > 0)
-        return round(first_digits * (10 ** - n), n)
-
-    @staticmethod
-    def from_matrix(M):
-        """inverse of to_matrix"""
-        return HyperReal(*(x for x in array(M[0, :]).flatten()))
-
-    def to_matrix(self, terms=None):
-        """converts hyperreal to an equivalently-behaving real matrix of dimension `terms`"""
-        if terms is None:
-            terms = len(self)
-        return matrix([[self[x - y] if 0 <= x - y < len(self) else 0 for x in range(terms)] for y in range(terms)])
+        return any(self.coefficients)
 
     @property
     def st(self):
         return self[0]
 
     @property
-    def real(self):
-        return self.st
-
-    @property
     def inf(self):
-        return HyperReal(0, *self[1:])
-
-    def split(self):
-        """splits hyperreal into standard and infinitesimal part"""
-        return self.st, self.inf
+        return self - self.st
 
-    def __float__(self):
-        return float(self.st)
-
-    def __int__(self):
-        return int(self.st)
+    @property
+    def real(self):
+        return self.st.real
 
-    def __lshift__(self, other):
-        """division by (ε ** other). truncates infinite part"""
-        return HyperReal(*self[other:])
 
-    def __rshift__(self, other):
-        """multiplication by (ε ** other)"""
-        return HyperReal(*([0] * other), *self)
+epsilon = ε = HyperReal(1, max_power=-1)
+omega = ω = HyperReal(1, max_power=1)
 
-    def is_integer(self):
-        return self.st.is_integer()
 
-    def is_real(self):
-        return not self.inf
+def is_real(x):
+    return x.real == x
 
 
-st = float
+def st(x):
+    return x.st if isinstance(x, HyperReal) else x
 
 
 def inf(x):
-    return x - float(x)
-
-
-epsilon = ε = HyperReal(0, 1)
-
-
-def auto_derivative(f, x, n=1):
-    return sum((-1 if k % 2 else 1) * binom(n, k) * f(x + (n - k) * ε) for k in range(n))[n]
+    return x - st(x)
 
 
 def limit(f, x):
+    """calculates the limit of f(a) as a approaches x using the standard part"""
     if st(x) == x:
         left_limit, right_limit = limit(f, x - ε), limit(f, x + ε)
         if left_limit != right_limit:
             raise ValueError('left-hand and right-hand limits don\'t match')
         return right_limit
     try:
         return st(f(x))
     except Exception as e:
         raise ValueError(f'{e}\nlimit does not exist')
 
 
 def continuous(function):
-    """decorator to fill in point-discontinuities using the `limit` method"""
+    """decorator to fill-in point-discontinuities using the `limit` method"""
 
     def inner(x):
         return limit(function, x)
 
     return inner
+
+
+def auto_derivative(f, x, n=1):
+    """automatically calculates the n'th derivative of f(x) via f'(x)=st((f(x+ε)-f(x))/ε)"""
+    _sum = 0
+    for k in range(1, n + 1):
+        _f = f(x + k * ε)
+        if n > 0 and not isinstance(_f, HyperReal):
+            continue
+        _sum += (-1 if (k + n) % 2 else 1) * binom(n, k) * _f[-n]
+    return _sum
```

### Comparing `infinitesimals-0.0.6/infinitesimals/example.py` & `infinitesimals-0.1.0/infinitesimals/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,94 +3,99 @@
 from math import floor, ceil
 from sys import float_info
 
 """Example program for demonstrating the capabilities of the infinitesimal library"""
 
 
 def main():
-    print('initializing hyperreals is easy')
-    x = HyperReal(1, 2, 1)  # also try "x = 1.0 + 2.0 * ε + (ε ** 2)" or "1.0 + 2.0 * epsilon + (epsilon ** 2)"
-    print(x == (1.0 + 2.0 * ε + (ε ** 2)) == (1.0 + 2.0 * epsilon + (epsilon ** 2)), '\n')
+    print('Initializing hyperreals is easy.')
+    x = 1 + 2 * ε + (ε ** 2)  # also try "x = 1.0 + 2.0 * epsilon + (epsilon ** 2)"
+    print(f'x = {x}', '\n')
 
-    print('ε really is an infinitesimal, and not just a really small number')
+    print('ε really is an infinitesimal, and not just a really small number!')
     smallest_float = float_info.min  # 2.2250738585072014e-308
     print(0 < ε < smallest_float)
     largest_float = float_info.max  # 1.7976931348623157e+308
     print((ε ** 2) * largest_float < ε * smallest_float, '\n')
 
-    print('hypereals have many built-in capabilities')
+    print('HyperReals have many built-in capabilities.')
     print(dir(HyperReal), '\n')
 
-    print('every hyperreal, x, has a standard part st(x)==x.st, and infinitesimal part inf(x)==x.inf')
-    print(f'{x=}, st(x)={x.st}, inf(x)={x.inf}', '\n')
+    print('Every HyperReal, x, has a standard part st(x)==x.st, and infinite(simal) part inf(x)==x.inf.')
+    print(f'x = {x}, st(x) = {x.st}, inf(x) = {x.inf}.', '\n')
 
-    print('pythonic alternative for displaying hyperreals')
-    print(repr(x), '\n')
-
-    print('you can set how many terms will be used in calculations\n')
+    print('You can set how many terms will be used in calculations.\n')
     infinitesimals.PRECISION = 10
 
-    print('they support all elementary operations')
-    print(f'1 / x = {1 / x}')
-    print(f'x % 1 = {x % 1}')
-    print(f'2 ** x = {2 ** x}\n')
-
-    print('and common elementary operations')
-    print(f'exp(x) = {exp(x)}')
-    print(f'log(x) = {log(x)}')
-    print(f'sin(x) = {sin(x)}\n')
+    print('They support all arithmetical operations:')
+    print(f'1 / x = {1 / x},')
+    print(f'x % 1 = {x % 1},')
+    print(f'2 ** x = {2 ** x},\n')
+
+    print('and common elementary functions:')
+    print(f'exp(x) = {exp(x)},')
+    print(f'log(x) = {log(x)},')
+    print(f'sin(x) = {sin(x)}.\n')
 
     infinitesimals.PRECISION = 32  # default precision
 
-    print('their rounding behaviour is also consistent')
-    print(f'floor(1 - ε) = {floor(1 - ε)}')
-    print(f'ceil(10 + ε) = {ceil(10 + ε)}')
-    print(f'round(0.5 + ε) = {round(0.5 + ε)}')
-    print(f'round(0.5 - ε) = {round(0.5 - ε)}\n')
+    print('Their rounding behaviour is also consistent.')
+    print(f'floor(1 - ε) = {floor(1 - ε)},')
+    print(f'ceil(10 + ε) = {ceil(10 + ε)},')
+    print(f'round(0.5 + ε) = {round(0.5 + ε)},')
+    print(f'round(0.5 - ε) = {round(0.5 - ε)}.\n')
 
-    print('but most excitingly, they work as an efficient alternative to symbolic or numeric analysis')
-    print('for example, limits involving point discontinuities become trivial')
+    print('But perhaps most excitingly, they work as an efficient alternative to symbolic or numeric analysis.')
+    print('For example, limits involving point discontinuities become trivial.')
 
     def f(x):
         return (2 ** x - 3 ** x) / x
 
-    print(f'st(f(ε)) = {st(f(ε))}\n')
+    print(f'limit of f(x) as x -> 0+ = {st(f(ε))}.\n')
 
-    print('which is employed in the `limit` method')
+    print('Which is employed in the `limit` method:')
 
     def g(x):
         return x * x / (1 - cos(x))
 
-    print(f'limit of g(x) as x -> 0 = {limit(g, 0)}\n')
+    print(f'limit of g(x) as x -> 0 = {limit(g, 0)}.\n')
 
-    print(f'and is further used in the `continuous` decorator')
+    print(f'The `limit` method is further used in the `continuous` decorator:')
 
     @continuous
     def sinc(x):
         return sin(x) / x
 
-    print(f'sinc(0) = {sinc(0)}\n')
+    print(f'sinc(0) = {sinc(0)}.\n')
 
-    print('automatic derivation is also made easy')
+    print('Automatic derivation is also made easy:')
 
     def h(x):
         return x ** x
 
     def h_prime(x):
-        return st((f(x + ε) - f(x)) / ε)
+        return st((h(x + ε) - h(x)) / ε)
+
+    print(f'h\'(1) = {h_prime(1)},\n')
+    print('which is conveniently used in the `auto_derivative` method:')
+    print(f'10th derivative of h at x=1 is {auto_derivative(h, 1, 10)}.\n')
+
+    print('Note: Errors are likely due to too low PRECISION or floating-point errors.')
+    print('However, any float-like-class which behave like floats should be compatible coefficients for HyperReals.\n')
+
+    print('The inverse of an infinitesimal is an infinity,')
+    print(f'1 / ε = {1 / ε}.\n')
+
+    print('Again, ω really is an infinity, and not just a really big number.')
+    print(0 < ε < smallest_float < 1 < largest_float < ω, '\n')
+
+    print('You can perform arithmetic with infinities just like you would infinitesimals.\n')
 
-    print(f'h\'(1) = {h_prime(x)}\n')
-    print('which is conveniently used in the `auto_derivative` method')
-    print(f'h{superscript_int(10, enclose=True)}(1) = {auto_derivative(h, 1, 10)}\n')
-
-    try:
-        print(f'1 / ε = {1 / ε}')
-    except ZeroDivisionError as e:
-        print(f'ZeroDivisionError: {e}')
-        print('at the moment, infinities are not supported, but plan on being in a future version\n')
+    print('But again, perhaps most interestingly, is its convenience in non-standard analysis:')
+    print(f'limit of sinc(x) as x -> ∞ = {limit(sinc, ω)}.\n')
 
-    print('hope you enjoy the infinitesimals library!')
-    print('try commenting out various pieces code to play around with different features and limitations')
+    print('Hope you enjoy the infinitesimals library!')
+    print('Try commenting out various pieces code to play around with different features and limitations.\n')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `infinitesimals-0.0.6/setup.py` & `infinitesimals-0.1.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 classifiers = [
-    'Development Status :: 2 - Pre-Alpha',
+    'Development Status :: 3 - Alpha',
     'Intended Audience :: Science/Research',
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='infinitesimals',
-    version='0.0.6',
-    description='A capable HyperReal class and related methods for work with infinitesimals and nonstandard analysis.',
+    version='0.1.0',
+    description='A capable HyperReal class and related methods for work with infinitesimals and infinities in nonstandard analysis.',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
-    keywords=['math', 'infinitesimal', 'infinitesimals', 'hyperreal', 'analysis', 'nonstandard analysis'],
+    keywords=['math', 'infinitesimal', 'infinitesimals', 'infinity', 'infinities', 'hyperreal', 'analysis', 'nonstandard analysis'],
     classifiers=classifiers,
     packages=find_packages(),
-    install_requires=['numpy', 'scipy']
+    install_requires=['numpy', 'scipy', 'more_itertools']
 )
```

