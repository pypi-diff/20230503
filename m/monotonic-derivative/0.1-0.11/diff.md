# Comparing `tmp/monotonic derivative-0.1.tar.gz` & `tmp/monotonic derivative-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monotonic derivative-0.1.tar", last modified: Wed May  3 14:18:07 2023, max compression
+gzip compressed data, was "monotonic derivative-0.11.tar", last modified: Wed May  3 15:25:42 2023, max compression
```

## Comparing `monotonic derivative-0.1.tar` & `monotonic derivative-0.11.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:18:07.836639 monotonic derivative-0.1/
--rw-rw-rw-   0        0        0     1089 2023-05-03 14:05:15.000000 monotonic derivative-0.1/LICENSE
--rw-rw-rw-   0        0        0      514 2023-05-03 14:18:07.830445 monotonic derivative-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3135 2023-05-03 14:05:15.000000 monotonic derivative-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 14:18:07.719409 monotonic derivative-0.1/monotonic_derivative/
--rw-rw-rw-   0        0        0     4915 2023-05-03 14:05:15.000000 monotonic derivative-0.1/monotonic_derivative/monotonic_derivative.py
-drwxrwxrwx   0        0        0        0 2023-05-03 14:18:07.825181 monotonic derivative-0.1/monotonic_derivative.egg-info/
--rw-rw-rw-   0        0        0      514 2023-05-03 14:18:06.000000 monotonic derivative-0.1/monotonic_derivative.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-05-03 14:18:06.000000 monotonic derivative-0.1/monotonic_derivative.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:18:06.000000 monotonic derivative-0.1/monotonic_derivative.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-03 14:18:06.000000 monotonic derivative-0.1/monotonic_derivative.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-03 14:18:06.000000 monotonic derivative-0.1/monotonic_derivative.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 14:18:07.839326 monotonic derivative-0.1/setup.cfg
--rw-rw-rw-   0        0        0      644 2023-05-03 14:17:27.000000 monotonic derivative-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:25:42.763061 monotonic derivative-0.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-03 15:25:31.000000 monotonic derivative-0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 15:25:42.763061 monotonic derivative-0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-03 15:25:31.000000 monotonic derivative-0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:25:42.763061 monotonic derivative-0.11/monotonic_derivative/
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-03 15:25:31.000000 monotonic derivative-0.11/monotonic_derivative/monotonic_derivative.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:25:42.763061 monotonic derivative-0.11/monotonic_derivative.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 15:25:42.000000 monotonic derivative-0.11/monotonic_derivative.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:25:42.763061 monotonic derivative-0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-03 15:25:31.000000 monotonic derivative-0.11/setup.py
```

### Comparing `monotonic derivative-0.1/README.md` & `monotonic derivative-0.11/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-## Monotonic Derivative - A Python Library
-
-Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
-
-### Table of Contents
-
-- [Installation](#installation)
-- [Usage](#usage)
-- [Example](#example)
-- [Real-life Applications](#real-life-applications)
-- [Contributing](#contributing)
-- [License](#license)
-
-### Installation
-
-To install the Monotonic Derivative library, cloent he repo (soon use pip:)
-
-```
-       git clone https://github.com/A-Wpro/monotonic_derivative.git
-(soon) pip install monotonic-derivative
-```
-
-### Usage
-
-First, import the `ensure_monotonic_derivative` function from the `monotonic_derivative` module:
-
-```python
-from monotonic_derivative import ensure_monotonic_derivative
-```
-
-The primary function of the library, `ensure_monotonic_derivative`, takes the following arguments:
-
-- `x`: numpy array, the independent variable data points
-- `y`: numpy array, the dependent variable data points
-- `degree`: int, the degree of the derivative to check for monotonicity (default: 2)
-- `force_negative_derivative`: bool, force the specified degree derivative to be monotonically decreasing if True (default: False)
-- `verbose`: bool, print additional information if True (default: False)
-- `save_plot`: bool, save the plots as PNG images if True (default: False)
-
-The function returns a modified numpy array of dependent variable data points (`modified_y`) that satisfy the specified monotonicity constraints.
-
-### Example
-
-```python
-import numpy as np
-from monotonic_derivative import ensure_monotonic_derivative
-
-x = np.array([0, 1, 2, 3, 4, 5])
-y = np.array([100, 55, 53, 40, 35, 5])
-
-modified_y_positive = ensure_monotonic_derivative(x, y, degree=2, force_negative_derivative=False, verbose=True, save_plot=True)
-```
-
-### Real-life Applications
-
-In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
-
-The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
-
-### Contributing
-
-We welcome contributions to the Monotonic Derivative library! Please feel free to submit pull requests for bug fixes, new features, or improvements to the code or documentation.
-
-### License
-
-This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
+## Monotonic Derivative - A Python Library
+
+Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.
+
+### Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Example](#example)
+- [Real-life Applications](#real-life-applications)
+- [Contributing](#contributing)
+- [License](#license)
+
+### Installation
+
+To install the Monotonic Derivative library, cloent he repo (soon use pip:)
+
+```
+       git clone https://github.com/A-Wpro/monotonic_derivative.git
+(soon) pip install monotonic-derivative
+```
+
+### Usage
+
+First, import the `ensure_monotonic_derivative` function from the `monotonic_derivative` module:
+
+```python
+from monotonic_derivative import ensure_monotonic_derivative
+```
+
+The primary function of the library, `ensure_monotonic_derivative`, takes the following arguments:
+
+- `x`: numpy array, the independent variable data points
+- `y`: numpy array, the dependent variable data points
+- `degree`: int, the degree of the derivative to check for monotonicity (default: 2)
+- `force_negative_derivative`: bool, force the specified degree derivative to be monotonically decreasing if True (default: False)
+- `verbose`: bool, print additional information if True (default: False)
+- `save_plot`: bool, save the plots as PNG images if True (default: False)
+
+The function returns a modified numpy array of dependent variable data points (`modified_y`) that satisfy the specified monotonicity constraints.
+
+### Example
+
+```python
+import numpy as np
+from monotonic_derivative import ensure_monotonic_derivative
+
+x = np.array([0, 1, 2, 3, 4, 5])
+y = np.array([100, 55, 53, 40, 35, 5])
+
+modified_y_positive = ensure_monotonic_derivative(x, y, degree=2, force_negative_derivative=False, verbose=True, save_plot=True)
+```
+
+### Real-life Applications
+
+In many real-life scenarios, the collected data may produce curves that are not logical or do not follow the expected constraints. For example, the data representing the velocity of a car over time should show an increasing or decreasing acceleration, but due to measurement errors or other factors, the collected data points may not reflect this.
+
+The Monotonic Derivative library offers an easy solution to slightly modify the data to respect these constraints. By using this library, you can ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing, making your data analysis more accurate and reliable.
+
+### Contributing
+
+We welcome contributions to the Monotonic Derivative library! Please feel free to submit pull requests for bug fixes, new features, or improvements to the code or documentation.
+
+### License
+
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

### Comparing `monotonic derivative-0.1/monotonic_derivative/monotonic_derivative.py` & `monotonic derivative-0.11/monotonic_derivative/monotonic_derivative.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import numpy as np
-from scipy.interpolate import CubicSpline
-from scipy.optimize import minimize
-import matplotlib.pyplot as plt
-from io import BytesIO
-import imageio
-
-def ensure_monotonic_derivative(x, y, degree=2, force_negative_derivative=False, verbose=False, save_plot=False):
-    """
-    Modify the given data points to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing.
-
-    Parameters:
-    x: numpy array, the independent variable data points
-    y: numpy array, the dependent variable data points
-    degree: int, the degree of the derivative to check for monotonicity
-    force_negative_derivative: bool, force the specified degree derivative to be monotonically decreasing if True
-    verbose: bool, print additional information if True
-    save_plot: bool, save the plots as GIF images if True
-
-    Returns:
-    modified_y: numpy array, the modified dependent variable data points
-    """
-    
-    def objective_function(y, x, y_original):
-        return np.sum((y - y_original) ** 2)
-
-
-    def constraint_second_derivative_increasing(y, x):
-        """
-        Function to create a constraint function to be used in the optimization problem.
-        The constraint function calculates the minimum difference between consecutive second derivatives.
-
-        Parameters:
-        y: numpy array, the dependent variable data points
-        x: numpy array, the independent variable data points
-
-        Returns:
-        constraint: function, the constraint function for the optimization problem
-        """
-
-        def constraint(y):
-            cs = CubicSpline(x, y)
-            y_2nd_derivative = cs(x, 2)
-            return np.min(np.diff(y_2nd_derivative))
-
-        return constraint
-
-
-    def constraint_second_derivative_decreasing(y, x):
-        """
-        Function to create a constraint function to be used in the optimization problem.
-        The constraint function calculates the maximum difference between consecutive second derivatives.
-
-        Parameters:
-        y: numpy array, the dependent variable data points
-        x: numpy array, the independent variable data points
-
-        Returns:
-        constraint: function, the constraint function for the optimization problem
-        """
-
-        def constraint(y):
-            cs = CubicSpline(x, y)
-            y_2nd_derivative = cs(x, 2)
-            return np.min(-np.diff(y_2nd_derivative))
-
-        return constraint
-    
-    # Check if x and y have the same length
-    if len(x) != len(y):
-        raise ValueError("x and y must have the same length")
-    # Check if the specified degree is valid
-    if degree >= len(y) - 1:
-        raise ValueError("Degree must be less than the length of the data minus 1, since we lose one data point for each derivative and need at least two data points")
-
-    # Define the constraint for the optimization problem
-    if force_negative_derivative:
-        cons = {'type': 'ineq', 'fun': constraint_second_derivative_decreasing(y, x)}
-    else:
-        cons = {'type': 'ineq', 'fun': constraint_second_derivative_increasing(y, x)}
-    
-    # Solve the optimization problem
-    res = minimize(objective_function, y, args=(x, y), constraints=cons)
-    modified_y = res.x
-
-    if verbose:
-        print("Original y    :", y)
-        print("Modified y    :", modified_y)
-        print("Optimization success:", res.success)
-        print("Optimization message:", res.message)
-
-    # Save and display plots of original and modified data and their derivatives if save_plot is True
-    if save_plot:
-        fig, ax = plt.subplots(degree + 1, 1, figsize=(8, 3 * (degree + 1)))
-
-        # Plot the original and modified data points
-        ax[0].plot(x, y, "o--", label="Original data points")
-        ax[0].plot(x, modified_y, "o--", label="Modified data points")
-        ax[0].set_xlabel("x")
-        ax[0].set_ylabel("y")
-        ax[0].legend()
-
-        cs_original = CubicSpline(x, y)
-        cs_modified = CubicSpline(x, modified_y)
-
-        # Plot derivatives from 1st to the specified degree
-        for d, ax_i in enumerate(ax[1:], start=1):
-            ax_i.plot(x[:-d], np.diff(y, n=d) / np.prod([np.diff(x) for _ in range(d)]), "o--", label=f"{d}th derivative (original)")
-            ax_i.plot(x[:-d], np.diff(modified_y, n=d) / np.prod([np.diff(x) for _ in range(d)]), "o--", label=f"{d}th derivative (modified)")
-            ax_i.set_xlabel("x")
-            ax_i.set_ylabel(f"{d}th derivative")
-            ax_i.legend()
-
-        plt.tight_layout()
-
-        buf = BytesIO()
-        plt.savefig(buf, format="png")
-        buf.seek(0)
-        image = imageio.imread(buf)
-        plt.close(fig)
-
-        # Save the image as a png
-        imageio.imwrite("derivative.png", image)
-
-
-    return modified_y
+import numpy as np
+from scipy.interpolate import CubicSpline
+from scipy.optimize import minimize
+import matplotlib.pyplot as plt
+from io import BytesIO
+import imageio
+
+def ensure_monotonic_derivative(x, y, degree=2, force_negative_derivative=False, verbose=False, save_plot=False):
+    """
+    Modify the given data points to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing.
+
+    Parameters:
+    x: numpy array, the independent variable data points
+    y: numpy array, the dependent variable data points
+    degree: int, the degree of the derivative to check for monotonicity
+    force_negative_derivative: bool, force the specified degree derivative to be monotonically decreasing if True
+    verbose: bool, print additional information if True
+    save_plot: bool, save the plots as GIF images if True
+
+    Returns:
+    modified_y: numpy array, the modified dependent variable data points
+    """
+    
+    def objective_function(y, x, y_original):
+        return np.sum((y - y_original) ** 2)
+
+
+    def constraint_second_derivative_increasing(y, x):
+        """
+        Function to create a constraint function to be used in the optimization problem.
+        The constraint function calculates the minimum difference between consecutive second derivatives.
+
+        Parameters:
+        y: numpy array, the dependent variable data points
+        x: numpy array, the independent variable data points
+
+        Returns:
+        constraint: function, the constraint function for the optimization problem
+        """
+
+        def constraint(y):
+            cs = CubicSpline(x, y)
+            y_2nd_derivative = cs(x, 2)
+            return np.min(np.diff(y_2nd_derivative))
+
+        return constraint
+
+
+    def constraint_second_derivative_decreasing(y, x):
+        """
+        Function to create a constraint function to be used in the optimization problem.
+        The constraint function calculates the maximum difference between consecutive second derivatives.
+
+        Parameters:
+        y: numpy array, the dependent variable data points
+        x: numpy array, the independent variable data points
+
+        Returns:
+        constraint: function, the constraint function for the optimization problem
+        """
+
+        def constraint(y):
+            cs = CubicSpline(x, y)
+            y_2nd_derivative = cs(x, 2)
+            return np.min(-np.diff(y_2nd_derivative))
+
+        return constraint
+    
+    # Check if x and y have the same length
+    if len(x) != len(y):
+        raise ValueError("x and y must have the same length")
+    # Check if the specified degree is valid
+    if degree >= len(y) - 1:
+        raise ValueError("Degree must be less than the length of the data minus 1, since we lose one data point for each derivative and need at least two data points")
+
+    # Define the constraint for the optimization problem
+    if force_negative_derivative:
+        cons = {'type': 'ineq', 'fun': constraint_second_derivative_decreasing(y, x)}
+    else:
+        cons = {'type': 'ineq', 'fun': constraint_second_derivative_increasing(y, x)}
+    
+    # Solve the optimization problem
+    res = minimize(objective_function, y, args=(x, y), constraints=cons)
+    modified_y = res.x
+
+    if verbose:
+        print("Original y    :", y)
+        print("Modified y    :", modified_y)
+        print("Optimization success:", res.success)
+        print("Optimization message:", res.message)
+
+    # Save and display plots of original and modified data and their derivatives if save_plot is True
+    if save_plot:
+        fig, ax = plt.subplots(degree + 1, 1, figsize=(8, 3 * (degree + 1)))
+
+        # Plot the original and modified data points
+        ax[0].plot(x, y, "o--", label="Original data points")
+        ax[0].plot(x, modified_y, "o--", label="Modified data points")
+        ax[0].set_xlabel("x")
+        ax[0].set_ylabel("y")
+        ax[0].legend()
+
+        cs_original = CubicSpline(x, y)
+        cs_modified = CubicSpline(x, modified_y)
+
+        # Plot derivatives from 1st to the specified degree
+        for d, ax_i in enumerate(ax[1:], start=1):
+            ax_i.plot(x[:-d], np.diff(y, n=d) / np.prod([np.diff(x) for _ in range(d)]), "o--", label=f"{d}th derivative (original)")
+            ax_i.plot(x[:-d], np.diff(modified_y, n=d) / np.prod([np.diff(x) for _ in range(d)]), "o--", label=f"{d}th derivative (modified)")
+            ax_i.set_xlabel("x")
+            ax_i.set_ylabel(f"{d}th derivative")
+            ax_i.legend()
+
+        plt.tight_layout()
+
+        buf = BytesIO()
+        plt.savefig(buf, format="png")
+        buf.seek(0)
+        image = imageio.imread(buf)
+        plt.close(fig)
+
+        # Save the image as a png
+        imageio.imwrite("derivative.png", image)
+
+
+    return modified_y
```

### Comparing `monotonic derivative-0.1/setup.py` & `monotonic derivative-0.11/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from setuptools import setup
-
-setup(
-    name='monotonic derivative',
-    version='0.1',
-    description='Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.',
-    author='Adam Wecker',
-    packages=['monotonic_derivative'],
-    install_requires=['numpy', 'scipy', 'matplotlib', 'imageio'],
-)
+from setuptools import setup
+
+setup(
+    name="monotonic derivative",
+    version="0.11",
+    description="Monotonic Derivative is a Python library designed to modify real-life data to ensure that the specified degree derivative of the cubic spline is always monotonically increasing or decreasing. This library can be particularly useful in applications where the derivatives of the given data must follow specific monotonicity constraints, such as in scientific modeling or engineering applications.",
+    author="Adam Wecker",
+    packages=["monotonic_derivative"],
+    install_requires=["numpy", "scipy", "matplotlib", "imageio"],
+)
```

