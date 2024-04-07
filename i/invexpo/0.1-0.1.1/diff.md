# Comparing `tmp/invexpo-0.1.tar.gz` & `tmp/invexpo-0.1.1.tar.gz`

## Comparing `invexpo-0.1.tar` & `invexpo-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 invexpo-0.1/README.md
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 invexpo-0.1/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 invexpo-0.1/src/invexpo/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 invexpo-0.1/src/invexpo/exceptions.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 invexpo-0.1/src/invexpo/inverse_exponential.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 invexpo-0.1/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 invexpo-0.1/LICENSE
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 invexpo-0.1/pyproject.toml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 invexpo-0.1/PKG-INFO
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 invexpo-0.1.1/README.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 invexpo-0.1.1/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 invexpo-0.1.1/src/invexpo/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 invexpo-0.1.1/src/invexpo/exceptions.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 invexpo-0.1.1/src/invexpo/inverse_exponential.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 invexpo-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 invexpo-0.1.1/LICENSE
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 invexpo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 invexpo-0.1.1/PKG-INFO
```

### Comparing `invexpo-0.1/README.md` & `invexpo-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-# Inverse Exponential Distribution
-This is a custom probability density function I created to solve a particular problem I had at work, however it could also be useful to others.
-
-This distribution aims to fit exponentially *ascending* data on a continuous interval [a, b]. That is, it's not bound to zero like the regular exponential distribution and can be defined for any interval.
-
-With this module, I aim to mimic the `scipy` API it has for its distributions (although not *everything* is implemented.)
-
-## Dependencies
-This module uses [scipy](https://github.com/scipy/scipy/blob/main/LICENSE.txt) for a lot of the backend which (at the time of writing) is licensed under BSD-3.
-
-## Warnings
-* When fitting your data, the lower and upper bounds are determined by the min/max of the data; this will severely impact the results if you have very low/high extremes. It's recommended to treat your data and ensure the sample you're fitting is a "natural"-looking exponentially ascending shape.
-
-* Drawing samples (with `rvs()`) is very slow when exceeding ~1000 samples. It's currently using optimization and numerical integration to evaluate the inverse CDF each time you want to draw a sample. In the future this may be improved if required.
-
-## Example Data
-This is an example of exponentially ascending data on the interval `[600, 800]`
-
-* NOTE: this distribution can capture various shapes whether it's a slow rise or sharper rise. This example used a fairly linear rise as a demonstration.
-
-<img width="580" alt="image" src="https://github.com/Kiyoshika/inverse-exponential/assets/49159969/e3b89740-747c-4ccb-8b63-b3c21313da18">
-
-## Mathematical Details
-If you're interested in the actual derivation, see the [whitepaper](whitepaper.pdf) in this repo.
-
-## Installation
-TODO:
-
-## Usage
-Initialize an "empty" distribution:
-```python
-from invexpo.inverse_exponential import InverseExponential
-
-invex = InverseExponential()
-```
-
-You can either fit the distribution to data or create a theoretical distribution.
-
-Note that `fit()` only accepts python lists as of now:
-```python
-# sample data that mimics an "exponentially increasing" function bounded by [600, 800]
-data = [600, 625, 650, 675, 700, 710, 720, 730, 740, 750, 760, 770, 780, 790, 800]
-
-invex = InverseExponential()
-
-# fit to data
-invex.fit(data)
-
-# create theoretical distribution
-# NOTE: the 'a' (shape) parameter is usually very small, large numbers can cause overflows.
-# Larger values of 'a' will create sharper peaks. Smaller values will more smoothly
-# transition over the interval.
-invex.create(a = 0.007, lower_bound = 300, upper_bound = 900)
-```
-
-### Methods
-After fitting/creating a distribution you can use the following methods:
-
-* `get_parameter() -> float`
-  * Returns the value of `a`, the shape parameter
-* `pdf(x: float) -> float`
-  * Evaluates the probability density function at `x` (i.e., `P(x)`)
-* `cdf(x: float) -> float`
-  * Evaluate the cumulative density function at `x`, (i.e., `P(X <= x)`)
-* `icdf(p: float) -> float`
-  * Evaluate the inverse CDF to get a percentile `p` for `0 <= p <= 1`
-* `ppf(p: float) -> float`
-  * Same as `icdf` just a different name (percentile point function)
-* `integrate(lower_bound: float, upper_bound: float) -> float`
-  * Integrates the pdf over the interval `[lower_bound, upper_bound]`
-* `rvs(size: int = 1) -> list[float]`
-  * Generate `size` random variables from the distribution
-  * WARNING: this is unoptimized and slows down heavily after ~1000 samples
-* `moment(n: int) -> float`
-  * Obtain the `n`-th moment of the distribution
-* `mean() -> float`
-  * Obtain the mean of the distribution (equivalent to `moment(1)`)
-* `median() -> float`
-  * Obtain the median of the distribution
-* `var() -> float`
-  * Obtain the variance of the distribution (equivalent to `moment(2) - moment(1)**2`)
-* `std() -> float`
-  * Obtain the standard deviation of the distribution (equivalent to `np.sqrt(var())`)
+# Inverse Exponential Distribution
+This is a custom probability density function I created to solve a particular problem I had at work, however it could also be useful to others.
+
+This distribution aims to fit exponentially *ascending* data on a continuous interval [a, b]. That is, it's not bound to zero like the regular exponential distribution and can be defined for any interval.
+
+With this module, I aim to mimic the `scipy` API it has for its distributions (although not *everything* is implemented.)
+
+## Dependencies
+This module uses [scipy](https://github.com/scipy/scipy/blob/main/LICENSE.txt) for a lot of the backend which (at the time of writing) is licensed under BSD-3.
+
+## Warnings
+* When fitting your data, the lower and upper bounds are determined by the min/max of the data; this will severely impact the results if you have very low/high extremes. It's recommended to treat your data and ensure the sample you're fitting is a "natural"-looking exponentially ascending shape.
+
+* Drawing samples (with `rvs()`) is very slow when exceeding ~1000 samples. It's currently using optimization and numerical integration to evaluate the inverse CDF each time you want to draw a sample. In the future this may be improved if required.
+
+## Example Data
+This is an example of exponentially ascending data on the interval `[600, 800]`
+
+* NOTE: this distribution can capture various shapes whether it's a slow rise or sharper rise. This example used a fairly linear rise as a demonstration.
+
+<img width="580" alt="image" src="https://github.com/Kiyoshika/inverse-exponential/assets/49159969/e3b89740-747c-4ccb-8b63-b3c21313da18">
+
+## Mathematical Details
+If you're interested in the actual derivation, see the [whitepaper](whitepaper.pdf) in this repo.
+
+## Installation
+Install with `pip3 install invexpo` or download from the [releases](https://github.com/Kiyoshika/inverse-exponential/releases) and install locally.
+
+## Usage
+Initialize an "empty" distribution:
+```python
+from invexpo.inverse_exponential import InverseExponential
+
+invex = InverseExponential()
+```
+
+You can either fit the distribution to data or create a theoretical distribution.
+
+Note that `fit()` only accepts python lists as of now:
+```python
+# sample data that mimics an "exponentially increasing" function bounded by [600, 800]
+data = [600, 625, 650, 675, 700, 710, 720, 730, 740, 750, 760, 770, 780, 790, 800]
+
+invex = InverseExponential()
+
+# fit to data
+invex.fit(data)
+
+# create theoretical distribution
+# NOTE: the 'a' (shape) parameter is usually very small, large numbers can cause overflows.
+# Larger values of 'a' will create sharper peaks. Smaller values will more smoothly
+# transition over the interval.
+invex.create(a = 0.007, lower_bound = 300, upper_bound = 900)
+```
+
+### Methods
+After fitting/creating a distribution you can use the following methods:
+
+* `get_parameter() -> float`
+  * Returns the value of `a`, the shape parameter
+* `pdf(x: float) -> float`
+  * Evaluates the probability density function at `x` (i.e., `P(x)`)
+* `cdf(x: float) -> float`
+  * Evaluate the cumulative density function at `x`, (i.e., `P(X <= x)`)
+* `icdf(p: float) -> float`
+  * Evaluate the inverse CDF to get a percentile `p` for `0 <= p <= 1`
+* `ppf(p: float) -> float`
+  * Same as `icdf` just a different name (percentile point function)
+* `integrate(lower_bound: float, upper_bound: float) -> float`
+  * Integrates the pdf over the interval `[lower_bound, upper_bound]`
+* `rvs(size: int = 1) -> list[float]`
+  * Generate `size` random variables from the distribution
+  * WARNING: this is unoptimized and slows down heavily after ~1000 samples
+* `moment(n: int) -> float`
+  * Obtain the `n`-th moment of the distribution
+* `mean() -> float`
+  * Obtain the mean of the distribution (equivalent to `moment(1)`)
+* `median() -> float`
+  * Obtain the median of the distribution
+* `var() -> float`
+  * Obtain the variance of the distribution (equivalent to `moment(2) - moment(1)**2`)
+* `std() -> float`
+  * Obtain the standard deviation of the distribution (equivalent to `np.sqrt(var())`)
```

### Comparing `invexpo-0.1/example.py` & `invexpo-0.1.1/example.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from invexpo.inverse_exponential import InverseExponential
-import matplotlib.pyplot as plt
-
-# sample data that mimics an "exponentially increasing" function bounded by [600, 800]
-data = [600, 625, 650, 675, 700, 710, 720, 730, 740, 750, 760, 770, 780, 790, 800]
-
-invex = InverseExponential()
-invex.fit(data)
-
-print("Integral from [600, 700]:\t", invex.integrate(600, 700))
-print("CDF of x = 750:\t\t\t", invex.cdf(750))
-print("80th percentile:\t\t", invex.icdf(0.8)) # or invex.ppf(0.8), icdf is an alias
-print("Mean:\t\t\t\t", invex.mean())
-print("Median:\t\t\t\t", invex.median())
-print("Variance:\t\t\t", invex.var())
-print("Std. Dev:\t\t\t", invex.std())
-print("2nd moment:\t\t\t", invex.moment(2))
-print("5 new samples:\t\t\t", invex.rvs(5))
+from invexpo.inverse_exponential import InverseExponential
+import matplotlib.pyplot as plt
+
+# sample data that mimics an "exponentially increasing" function bounded by [600, 800]
+data = [600, 625, 650, 675, 700, 710, 720, 730, 740, 750, 760, 770, 780, 790, 800]
+
+invex = InverseExponential()
+invex.fit(data)
+
+print("Integral from [600, 700]:\t", invex.integrate(600, 700))
+print("CDF of x = 750:\t\t\t", invex.cdf(750))
+print("80th percentile:\t\t", invex.icdf(0.8)) # or invex.ppf(0.8), icdf is an alias
+print("Mean:\t\t\t\t", invex.mean())
+print("Median:\t\t\t\t", invex.median())
+print("Variance:\t\t\t", invex.var())
+print("Std. Dev:\t\t\t", invex.std())
+print("2nd moment:\t\t\t", invex.moment(2))
+print("5 new samples:\t\t\t", invex.rvs(5))
```

### Comparing `invexpo-0.1/src/invexpo/inverse_exponential.py` & `invexpo-0.1.1/src/invexpo/inverse_exponential.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-from scipy.optimize import root_scalar, minimize
-from scipy import integrate 
-from scipy.stats import uniform
-import numpy as np
-
-from .exceptions import ArgumentError, NotFittedError
-
-class InverseExponential:
-    def __init__(self) -> None:
-        self.__param_a: float = 0.001
-        self.__fitted: bool = False
-    
-    def fit(self, data: list[float], maxiter: int = 1000) -> None:
-        if len(data) < 1:
-            raise ArgumentError("Need more than one sample to fit data.")
-
-        self.__data: list[float] = data.copy()
-        self.__lower_bound: float = min(data)
-        self.__upper_bound: float = max(data)
-        if self.__upper_bound == self.__lower_bound:
-            raise ArgumentError("Lower bound and upper bound must be different.")
-
-        self.__range: float = self.__upper_bound - self.__lower_bound
-
-        self.__find_root_of_likelihood(maxiter)
-        self.__fitted = True
-
-    def get_parameter(self) -> float:
-        return self.__param_a
-
-    # create a theoretical distribution
-    def create(self, a: float, lower_bound: float, upper_bound) -> None:
-        if lower_bound >= upper_bound:
-            raise ArgumentError("Lower bound must be less than upper bound.")
-
-        self.__param_a = a
-        self.__lower_bound = lower_bound
-        self.__upper_bound = upper_bound
-        self.__range = upper_bound - lower_bound
-        self.__fitted = True
-
-    def pdf(self, x: float) -> float:
-        if not self.__fitted:
-            raise NotFittedError("pdf")
-
-        _a: float = self.__param_a
-        _numerator: float = _a * np.exp(_a * (x - self.__lower_bound))
-        _denominator: float = np.exp(_a * self.__range) - 1
-
-        return _numerator / _denominator
-
-    def cdf(self, x: float) -> float:
-        if not self.__fitted:
-            raise NotFittedError("cdf")
-
-        if x <= self.__lower_bound:
-            return 0.0
-
-        if x >= self.__upper_bound:
-            return 1.0
-
-        return integrate.quad(self.pdf, self.__lower_bound, x)[0]
-
-    def ppf(self, p: float) -> float:
-        if not self.__fitted:
-            raise NotFittedError("ppf")
-
-        if p < 0.0 or p > 1.0:
-            raise ArgumentError("p must be 0.0 <= p <= 1.0")
-
-        return self.__find_ppf(p)
-
-    def icdf(self, p: float) -> float:
-        return self.ppf(p)
-
-    def integrate(self, lower_bound: float, upper_bound: float) -> float:
-        if lower_bound >= upper_bound:
-            raise ArgumentError("lower_bound must be less than upper_bound.")
-
-        return integrate.quad(self.pdf, lower_bound, upper_bound)[0]
-
-    def rvs(self, size = 1) -> list[float]:
-        if size < 1:
-            raise ArgumentError("size must be >= 1.")
-
-        _uniform_dist = uniform()
-
-        samples: list[float] = []
-        for i in range(size):
-            _u: float = _uniform_dist.rvs()
-            _sample = self.ppf(_u)
-            if _sample < self.__lower_bound:
-                samples.append(self.__lower_bound)
-            elif _sample > self.__upper_bound:
-                samples.append(self.__upper_bound)
-            else:
-                samples.append(_sample)
-
-        return samples
-
-    def moment(self, n: int) -> float:
-        if not self.__fitted:
-            raise NotFittedError("moment")
-
-        return integrate.quad(lambda x: pow(x, n) * self.pdf(x), self.__lower_bound, self.__upper_bound)[0]
-
-    def median(self) -> float:
-        if not self.__fitted:
-            raise NotFittedError("median")
-
-        return self.icdf(0.5)
-
-    def mean(self) -> float:
-        return self.moment(1)
-
-    def var(self) -> float:
-        return self.moment(2) - self.moment(1)**2
-
-    def std(self) -> float:
-        return np.sqrt(self.var())
-
-    def sf(self, x: float) -> float:
-        raise NotImplementedError()
-
-    def isf(self, p: float) -> float:
-        raise NotImplementedError()
-
-    def __log_likelihood(self, _a: float) -> float:
-        _sum: float = 0.0
-        for _x in self.__data:
-            _sum += (_x - self.__lower_bound)
-        _n: int = len(self.__data)
-
-        return _n/_a + _sum - (self.__range * _n * np.exp(self.__range * _a))/(np.exp(self.__range * _a) - 1.0)
-
-    def __find_root_of_likelihood(self, maxiter: int) -> None:
-        result = root_scalar(self.__log_likelihood, method = 'newton', x0 = 0.01, maxiter = maxiter)
-        if not result.converged:
-            raise Exception("Optimizer could not converge. Try increasing maxiter?")
-        self.__param_a = result.root
-
-    def __find_ppf(self, p: float) -> float:
-        # start the initial guess in the middle of the range
-        x0: float = (self.__lower_bound + self.__upper_bound) / 2.0
-        result = minimize(lambda x: (self.cdf(x) - p)**2, x0 = [x0])
-        if not result.success:
-            raise Exception("ppf optimizer was not successful in finding an appropriate value.")
-
-        return result.x[0]
+from scipy.optimize import root_scalar, minimize
+from scipy import integrate 
+from scipy.stats import uniform
+import numpy as np
+
+from .exceptions import ArgumentError, NotFittedError
+
+class InverseExponential:
+    def __init__(self) -> None:
+        self.__param_a: float = 0.001
+        self.__fitted: bool = False
+    
+    def fit(self, data: list[float], maxiter: int = 1000) -> None:
+        if len(data) < 1:
+            raise ArgumentError("Need more than one sample to fit data.")
+
+        self.__data: list[float] = data.copy()
+        self.__lower_bound: float = min(data)
+        self.__upper_bound: float = max(data)
+        if self.__upper_bound == self.__lower_bound:
+            raise ArgumentError("Lower bound and upper bound must be different.")
+
+        self.__range: float = self.__upper_bound - self.__lower_bound
+
+        self.__find_root_of_likelihood(maxiter)
+        self.__fitted = True
+
+    def get_parameter(self) -> float:
+        return self.__param_a
+
+    # create a theoretical distribution
+    def create(self, a: float, lower_bound: float, upper_bound) -> None:
+        if lower_bound >= upper_bound:
+            raise ArgumentError("Lower bound must be less than upper bound.")
+
+        self.__param_a = a
+        self.__lower_bound = lower_bound
+        self.__upper_bound = upper_bound
+        self.__range = upper_bound - lower_bound
+        self.__fitted = True
+
+    def pdf(self, x: float) -> float:
+        if not self.__fitted:
+            raise NotFittedError("pdf")
+
+        _a: float = self.__param_a
+        _numerator: float = _a * np.exp(_a * (x - self.__lower_bound))
+        _denominator: float = np.exp(_a * self.__range) - 1
+
+        return _numerator / _denominator
+
+    def cdf(self, x: float) -> float:
+        if not self.__fitted:
+            raise NotFittedError("cdf")
+
+        if x <= self.__lower_bound:
+            return 0.0
+
+        if x >= self.__upper_bound:
+            return 1.0
+
+        return integrate.quad(self.pdf, self.__lower_bound, x)[0]
+
+    def ppf(self, p: float) -> float:
+        if not self.__fitted:
+            raise NotFittedError("ppf")
+
+        if p < 0.0 or p > 1.0:
+            raise ArgumentError("p must be 0.0 <= p <= 1.0")
+
+        return self.__find_ppf(p)
+
+    def icdf(self, p: float) -> float:
+        return self.ppf(p)
+
+    def integrate(self, lower_bound: float, upper_bound: float) -> float:
+        if lower_bound >= upper_bound:
+            raise ArgumentError("lower_bound must be less than upper_bound.")
+
+        return integrate.quad(self.pdf, lower_bound, upper_bound)[0]
+
+    def rvs(self, size = 1) -> list[float]:
+        if size < 1:
+            raise ArgumentError("size must be >= 1.")
+
+        _uniform_dist = uniform()
+
+        samples: list[float] = []
+        for i in range(size):
+            # sometimes the icdf is slightly inaccurate and generates values outside the bounds
+            # so we repeatedly sample until we obtain valid values
+            while True:
+                _u: float = _uniform_dist.rvs()
+                _sample = self.ppf(_u)
+                if _sample >= self.__lower_bound and _sample <= self.__upper_bound:
+                    samples.append(_sample)
+                    break
+
+        return samples
+
+    def moment(self, n: int) -> float:
+        if not self.__fitted:
+            raise NotFittedError("moment")
+
+        return integrate.quad(lambda x: pow(x, n) * self.pdf(x), self.__lower_bound, self.__upper_bound)[0]
+
+    def median(self) -> float:
+        if not self.__fitted:
+            raise NotFittedError("median")
+
+        return self.icdf(0.5)
+
+    def mean(self) -> float:
+        return self.moment(1)
+
+    def var(self) -> float:
+        return self.moment(2) - self.moment(1)**2
+
+    def std(self) -> float:
+        return np.sqrt(self.var())
+
+    def sf(self, x: float) -> float:
+        raise NotImplementedError()
+
+    def isf(self, p: float) -> float:
+        raise NotImplementedError()
+
+    def __log_likelihood(self, _a: float) -> float:
+        _sum: float = 0.0
+        for _x in self.__data:
+            _sum += (_x - self.__lower_bound)
+        _n: int = len(self.__data)
+
+        return _n/_a + _sum - (self.__range * _n * np.exp(self.__range * _a))/(np.exp(self.__range * _a) - 1.0)
+
+    def __find_root_of_likelihood(self, maxiter: int) -> None:
+        result = root_scalar(self.__log_likelihood, method = 'newton', x0 = 0.01, maxiter = maxiter)
+        if not result.converged:
+            raise Exception("Optimizer could not converge. Try increasing maxiter?")
+        self.__param_a = result.root
+
+    def __find_ppf(self, p: float) -> float:
+        # start the initial guess in the middle of the range
+        x0: float = (self.__lower_bound + self.__upper_bound) / 2.0
+        result = minimize(lambda x: (self.cdf(x) - p)**2, x0 = [x0])
+        if not result.success:
+            raise Exception("ppf optimizer was not successful in finding an appropriate value.")
+
+        return result.x[0]
```

### Comparing `invexpo-0.1/LICENSE` & `invexpo-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2024, Zach Weaver
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2024, Zach Weaver
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `invexpo-0.1/pyproject.toml` & `invexpo-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-[build-system]
-requires = ["hatchling", "scipy"]
-build-backend = "hatchling.build"
-
-[project]
-name = "invexpo"
-version = "0.1"
-authors = [
-    { name="Zachary Weaver", email="zacharylweaver00@gmail.com" }
-]
-description = "An implementation of an inverse exponential distribution to fit exponentially ascending data on any continuous interval"
-requires-python = ">=3.8"
-assifiers = [
-    "Topic :: Scientific/Engineering :: Mathematics",
-    "License :: OSI Approved :: BSD License",
-    "Operating System :: OS Independent"
-]
-dependencies = [
-    "scipy~=1.13.0"
-]
-
-[project.urls]
-Homepage = "https://github.com/Kiyoshika/inverse-exponential"
-Issues = "https://github.com/Kiyoshika/inverse-exponential/issues"
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/invexpo"]
+[build-system]
+requires = ["hatchling", "scipy"]
+build-backend = "hatchling.build"
+
+[project]
+name = "invexpo"
+version = "0.1.1"
+authors = [
+    { name="Zachary Weaver", email="zacharylweaver00@gmail.com" }
+]
+description = "An implementation of an inverse exponential distribution to fit exponentially ascending data on any continuous interval"
+requires-python = ">=3.8"
+assifiers = [
+    "Topic :: Scientific/Engineering :: Mathematics",
+    "License :: OSI Approved :: BSD License",
+    "Operating System :: OS Independent"
+]
+dependencies = [
+    "scipy~=1.13.0"
+]
+
+[project.urls]
+Homepage = "https://github.com/Kiyoshika/inverse-exponential"
+Issues = "https://github.com/Kiyoshika/inverse-exponential/issues"
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/invexpo"]
```

