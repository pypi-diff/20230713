# Comparing `tmp/pynverse-0.1.4.4_v2.tar.gz` & `tmp/pynverse-0.1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pynverse-0.1.4.4.tar", last modified: Sun Nov  6 14:48:11 2016, max compression
+gzip compressed data, was "pynverse-0.1.4.6.tar", last modified: Thu Jul 13 21:09:55 2023, max compression
```

## Comparing `pynverse-0.1.4.4_v2.tar` & `pynverse-0.1.4.6.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/
--rw-rw-rw-   0        0        0     1072 2016-10-30 23:26:06.000000 pynverse-0.1.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0       54 2016-10-30 23:26:32.000000 pynverse-0.1.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0      920 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/pynverse/
--rw-rw-rw-   0        0        0    11987 2016-10-30 23:26:53.000000 pynverse-0.1.4.4/pynverse/inverse.py
--rw-rw-rw-   0        0        0      307 2016-10-29 12:56:07.000000 pynverse-0.1.4.4/pynverse/utils.py
--rw-rw-rw-   0        0        0       24 2016-10-31 21:16:19.000000 pynverse-0.1.4.4/pynverse/version.py
--rw-rw-rw-   0        0        0      313 2016-10-31 21:16:19.000000 pynverse-0.1.4.4/pynverse/__init__.py
-drwxrwxrwx   0        0        0        0 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/pynverse.egg-info/
--rw-rw-rw-   0        0        0        1 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/pynverse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      920 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/pynverse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       23 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/pynverse.egg-info/requires.txt
--rw-rw-rw-   0        0        0      297 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/pynverse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/pynverse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7686 2016-11-06 14:46:02.000000 pynverse-0.1.4.4/README
--rw-rw-rw-   0        0        0     7160 2016-11-06 14:45:19.000000 pynverse-0.1.4.4/README.md
--rw-rw-rw-   0        0        0      105 2016-11-06 14:48:11.000000 pynverse-0.1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1381 2016-10-31 21:16:19.000000 pynverse-0.1.4.4/setup.py
+drwxr-xr-x   0 alvarosg (466040) primarygroup (89939)        0 2023-07-13 21:09:55.065101 pynverse-0.1.4.6/
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)     1066 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/LICENSE.txt
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)       52 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/MANIFEST.in
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)      885 2023-07-13 21:09:55.065163 pynverse-0.1.4.6/PKG-INFO
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)     7125 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/README.md
+drwxr-xr-x   0 alvarosg (466040) primarygroup (89939)        0 2023-07-13 21:09:55.063776 pynverse-0.1.4.6/pynverse/
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)      313 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/pynverse/__init__.py
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)    11678 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/pynverse/inverse.py
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)      307 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/pynverse/utils.py
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)       25 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/pynverse/version.py
+drwxr-xr-x   0 alvarosg (466040) primarygroup (89939)        0 2023-07-13 21:09:55.064733 pynverse-0.1.4.6/pynverse.egg-info/
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)      885 2023-07-13 21:09:55.000000 pynverse-0.1.4.6/pynverse.egg-info/PKG-INFO
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)      290 2023-07-13 21:09:55.000000 pynverse-0.1.4.6/pynverse.egg-info/SOURCES.txt
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)        1 2023-07-13 21:09:55.000000 pynverse-0.1.4.6/pynverse.egg-info/dependency_links.txt
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)       23 2023-07-13 21:09:55.000000 pynverse-0.1.4.6/pynverse.egg-info/requires.txt
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)        9 2023-07-13 21:09:55.000000 pynverse-0.1.4.6/pynverse.egg-info/top_level.txt
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)       76 2023-07-13 21:09:55.065413 pynverse-0.1.4.6/setup.cfg
+-rw-r--r--   0 alvarosg (466040) primarygroup (89939)     1347 2023-07-13 21:01:48.000000 pynverse-0.1.4.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pynverse-0.1.4.4/LICENSE.txt` & `pynverse-0.1.4.6/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2016 Alvaro Sanchez-Gonzalez
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright (c) 2016 Alvaro Sanchez-Gonzalez
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `pynverse-0.1.4.4/pynverse/inverse.py` & `pynverse-0.1.4.6/pynverse/inverse.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,306 +1,306 @@
-import numpy as np
-import warnings
-
-from scipy.optimize import minimize_scalar
-
-__all__ = ['inversefunc']
-
-
-def inversefunc(func,
-                y_values=None,
-                domain=None,
-                image=None,
-                open_domain=None,
-                args=(),
-                accuracy=2):
-    r"""Obtain the inverse of a function.
-
-    Returns the numerical inverse of the function `f`. It may return a callable
-    that can be used to calculate the inverse, or the inverse of certain points
-    depending on the `y_values` argument.
-    In order for the numerical inverse to exist in its domain, the
-    input function must have, continuous, strictly monotonic behavior i.e. be
-    purely decreasing or purely increasing in that domain. By default the
-    domain interval spans all the real numbers, however it can be restricted
-    with the `domain` and `open_domain` arguments. The image of the function
-    in the interval may be provided, for cases where the function is non
-    continuous right at the end of an open interval.
-
-    Parameters
-    ----------
-    func : callable
-        Callable representing the function to be inverted, able to take a
-        ndarray or an scalar and return an object of the same kind with the
-        evaluation of the function.  If `func` takes many arguments, it is
-        inverted along the axis corresponding to the first argument.
-        The function must not diverge and have a continuous strictly monotonic
-        behavior in the chosen interval.
-    y_values : float, ndarray, optional
-        Values for which calculate the inverse function. If set to None, then
-        a callable that can be used to calculate the inverse of values is
-        returned. Default None.
-    domain : float, ndarray, optional
-        Boundaries of the domain (`domain[0]`, `domain[1]`).
-        `domain[1]` must be larger than `domain[0]`.
-        None values are assumed to be no boundary in that direction.
-        A single scalar value will set it to [`domain`, None].
-        Default None (-Inf, Inf).
-    open_domain : bool, ndarray, optional
-        Whether the domain is an open interval at each of the ends.
-        A single scalar boolean will set it to [`open_domain`, `open_domain`].
-        Default None [False, False].
-    image : float, ndarray, optional
-        Image of the function in the domain (`image[0]`, `image[1]`).
-        `image[1]` must be larger than `image[0]`.
-        None values are assumed to be no boundary in that direction.
-        Default None, this is (-Inf, Inf) if domain is None, or the limits
-        set by func(domain[0]) and func(domain[1]).
-    args : tuple, optional
-        Extra arguments to pass to `func`. Default ().
-    accuracy : int, optional
-        Number of digits for the desired accuracy. It will give a warning
-        if the accuracy is worse than this.
-        Default 2.
-
-    Returns
-    -------
-    callable or ndarray
-        Inverse function of `func`. It can take scalars or ndarrays, and return
-        objects of the same kind with the calculated inverse values.
-
-    Notes
-    -----
-
-    .. versionadded:: 0.19.0
-
-    Examples
-    --------
-    >>> from pynverse import inversefunc
-    >>> import numpy as np
-    >>> cube = (lambda x: x**3)
-    >>> invcube = inversefunc(cube)
-    >>> invcube(27) # Should give 3
-    array(3.0000000063797567)
-    >>> invsquare = inversefunc(np.power, args=(2), domain=0)
-    >>> invsquare([4, 16, 64]) # Should give [2, 4, 8]
-    array([ 2.,  4.,  8.])
-    >>> inversefunc(np.log10, y_values=-2, # Should give 0.01
-    ...             domain=0, open_domain=True)
-    array(0.0099999999882423)
-    >>> inversefunc(np.cos, y_values=[1, 0, -1], # Should give [0, pi / 2, pi]
-    ...             domain=[0, np.pi])
-    array([ 0.        ,  1.57079632,  3.14159265])
-    >>> invtan = inversefunc(np.tan,
-    ...                      domain=[-np.pi / 2, np.pi / 2],
-    ...                      open_domain=True)
-    >>> invtan([1, 0, -1]) # Should give [pi / 4, 0, -pi / 4]
-    array([  7.85398163e-01,   1.29246971e-26,  -7.85398163e-01])
-
-    """
-
-    domain, image, open_domain, args = _normparams_inversefunc(domain,
-                                                               image,
-                                                               open_domain,
-                                                               args)
-
-    ymin, ymax = image
-    xmin, xmax = domain
-    xmin_open, xmax_open = open_domain
-
-    # Calculating if the function is increasing or decreasing, using ref points
-    # anywhere in the valid range (Function has to be strictly monotonic)
-    ref1, ref2 = _get_valid_refpoints(xmin, xmax)
-    trend = np.sign(func(ref2, *args) - func(ref1, *args))
-
-    if trend == 0:
-        raise ValueError("Function is not strictly monotonic")
-
-    # Calculating the image by default
-    if ymin is None:
-        ymin = _auto_ymin(func, args, xmin, xmax, trend)
-    if ymax is None:
-        ymax = _auto_ymax(func, args, xmin, xmax, trend)
-
-    # Creating bounded function
-    def bounded_f(x):
-        if xmin is not None and (x < xmin or (x == xmin and xmin_open)):
-                val = -1 * np.inf * trend
-        elif xmax is not None and (x > xmax or (x == xmax and xmax_open)):
-                val = np.inf * trend
-        else:
-            val = func(x, *args)
-        return val
-
-    min_kwargs = {}
-    min_kwargs['bracket'] = (ref1, ref2)
-    min_kwargs['tol'] = 1.48e-08
-    min_kwargs['method'] = 'Brent'
-
-    def inv(yin):
-        yin = np.asarray(yin, dtype=np.float64)
-        shapein = yin.shape
-        yin = yin.flatten()
-        if ymin is not None:
-            if (xmin_open and trend == 1) or (xmax_open and trend == -1):
-                mask = yin <= ymin
-            else:
-                mask = yin < ymin
-            if yin[mask].size > 0:
-                raise ValueError("Requested values %s lower than the"
-                                 " lower limit %g of the image" %
-                                 (yin[mask], ymin))
-        if ymax is not None:
-            if (xmax_open and trend == 1) or (xmin_open and trend == -1):
-                mask = yin >= ymax
-            else:
-                mask = yin > ymax
-            if yin[mask].size > 0:
-                raise ValueError("Requested values %s higher than the"
-                                 " higher limit %g of the image" %
-                                 (yin[mask], ymax))
-
-        results = yin.copy() * np.nan
-        resultsmask = np.zeros(yin.shape, dtype=np.bool)
-
-        for j in range(yin.size):
-            if xmax is not None:
-                if bounded_f(xmax) == yin[j]:
-                    results[j] = xmax
-                    resultsmask[j] = True
-                    continue
-            if xmin is not None:
-                if bounded_f(xmin) == yin[j]:
-                    results[j] = xmin
-                    resultsmask[j] = True
-                    continue
-
-            optimizer = (lambda x, j=j,
-                         bounded_f=bounded_f: (((bounded_f(x) - yin[j]))**2))
-            try:
-                with warnings.catch_warnings(record=True):
-                    result = minimize_scalar(optimizer, **min_kwargs)
-                results[j] = result.x
-                resultsmask[j] = result.success
-            except:
-                resultsmask[j] = False
-        if any(~resultsmask):
-            warnings.warn("Trouble calculating inverse for values: "
-                          "%s" % str(yin[~resultsmask]), RuntimeWarning)
-
-        try:
-            np.testing.assert_array_almost_equal(yin, func(results, *args),
-                                                 decimal=accuracy)
-        except AssertionError:
-            warnings.warn("Results obtained with less than %g "
-                          "decimal digits of accuracy"
-                          % accuracy, RuntimeWarning)
-
-        return results.reshape(shapein)
-
-    if y_values is None:
-        return inv
-    else:
-        return inv(y_values)
-
-
-def _normparams_inversefunc(domain, image, open_domain, args):
-
-    if not isinstance(args, tuple):
-        args = (args,)
-
-    error_domain = ("domain must be a single scalar, or a have two "
-                    "elements [xmin, xmax]. Set None, to leave it "
-                    "unlimited on one side.")
-    if domain is None:
-        domain = (None, None)
-    else:
-        domain = np.asarray(domain)
-        if domain.ndim == 0:
-            domain = (float(domain), None)
-        elif domain.ndim == 1 and domain.size != 2:
-            raise ValueError(error_domain)
-        elif domain.ndim > 1:
-            raise ValueError(error_domain)
-        else:
-            domain = ((float(domain[0]) if domain[0] is not None else None),
-                      (float(domain[1]) if domain[1] is not None else None))
-
-    error_open_domain = ("open_domain must be a single scalar, or a have two "
-                         "bool elements [open_xmin, open_xmax].")
-    if open_domain is None:
-        open_domain = (False, False)
-    else:
-        open_domain = np.asarray(open_domain)
-        if open_domain.ndim == 0:
-            open_domain = (bool(open_domain), bool(open_domain))
-        elif open_domain.ndim == 1 and open_domain.size != 2:
-            raise ValueError(error_open_domain)
-        elif open_domain.ndim > 1:
-            raise ValueError(error_open_domain)
-        else:
-            open_domain = (bool(open_domain[0]), bool(open_domain[1]))
-
-    error_image = ("image must be a single scalar, or a have two "
-                   "bool elements [ymin, ymax].")
-    if image is None:
-        image = (None, None)
-    else:
-        image = np.asarray(image)
-        if image.ndim != 1 or image.size != 2:
-            raise ValueError(error_image)
-        else:
-            image = ((float(image[0]) if image[0] is not None else None),
-                     (float(image[1]) if image[1] is not None else None))
-
-    if domain[0] is not None and domain[1] is not None:
-        if domain[0] >= domain[1]:
-            raise ValueError("domain[0] min must be less than domain[1]")
-
-    if image[0] is not None and image[1] is not None:
-        if image[0] >= image[1]:
-            raise ValueError("image[0] min must be less than image[1]")
-
-    return domain, image, open_domain, args
-
-
-def _get_valid_refpoints(xmin, xmax):
-    if xmin is not None and xmax is not None:
-        d = xmax - xmin
-        ref1 = xmin + d / 4.
-        ref2 = xmax - d / 4.
-    elif xmin is not None:
-        ref1 = xmin + 1.
-        ref2 = xmin + 2.
-    elif xmax is not None:
-        ref1 = xmax - 2.
-        ref2 = xmax - 1.
-    else:
-        ref1 = 0.
-        ref2 = 1.
-    return ref1, ref2
-
-
-def _auto_ymin(func, args, xmin, xmax, trend):
-    ymin = None
-    if ((xmin is not None and trend == 1) or
-       (xmax is not None and trend == -1)):
-        try:
-            with warnings.catch_warnings(record=True):
-                ymin = func(xmin, *args) if trend == 1 else func(xmax, *args)
-        except:
-            raise ValueError("Cannot automatically calculate the lower limit "
-                             "of the image please inclue it as a parameter")
-    return ymin
-
-
-def _auto_ymax(func, args, xmin, xmax, trend):
-    ymax = None
-    if ((xmax is not None and trend == 1) or
-       (xmin is not None and trend == -1)):
-        try:
-            with warnings.catch_warnings(record=True):
-                ymax = func(xmax, *args) if trend == 1 else func(xmin, *args)
-        except:
-            raise ValueError("Cannot automatically calculate the upper limit "
-                             "of the image please include it as a parameter")
-    return ymax
+import numpy as np
+import warnings
+
+from scipy.optimize import minimize_scalar
+
+__all__ = ['inversefunc']
+
+
+def inversefunc(func,
+                y_values=None,
+                domain=None,
+                image=None,
+                open_domain=None,
+                args=(),
+                accuracy=2):
+    r"""Obtain the inverse of a function.
+
+    Returns the numerical inverse of the function `f`. It may return a callable
+    that can be used to calculate the inverse, or the inverse of certain points
+    depending on the `y_values` argument.
+    In order for the numerical inverse to exist in its domain, the
+    input function must have, continuous, strictly monotonic behavior i.e. be
+    purely decreasing or purely increasing in that domain. By default the
+    domain interval spans all the real numbers, however it can be restricted
+    with the `domain` and `open_domain` arguments. The image of the function
+    in the interval may be provided, for cases where the function is non
+    continuous right at the end of an open interval.
+
+    Parameters
+    ----------
+    func : callable
+        Callable representing the function to be inverted, able to take a
+        ndarray or an scalar and return an object of the same kind with the
+        evaluation of the function.  If `func` takes many arguments, it is
+        inverted along the axis corresponding to the first argument.
+        The function must not diverge and have a continuous strictly monotonic
+        behavior in the chosen interval.
+    y_values : float, ndarray, optional
+        Values for which calculate the inverse function. If set to None, then
+        a callable that can be used to calculate the inverse of values is
+        returned. Default None.
+    domain : float, ndarray, optional
+        Boundaries of the domain (`domain[0]`, `domain[1]`).
+        `domain[1]` must be larger than `domain[0]`.
+        None values are assumed to be no boundary in that direction.
+        A single scalar value will set it to [`domain`, None].
+        Default None (-Inf, Inf).
+    open_domain : bool, ndarray, optional
+        Whether the domain is an open interval at each of the ends.
+        A single scalar boolean will set it to [`open_domain`, `open_domain`].
+        Default None [False, False].
+    image : float, ndarray, optional
+        Image of the function in the domain (`image[0]`, `image[1]`).
+        `image[1]` must be larger than `image[0]`.
+        None values are assumed to be no boundary in that direction.
+        Default None, this is (-Inf, Inf) if domain is None, or the limits
+        set by func(domain[0]) and func(domain[1]).
+    args : tuple, optional
+        Extra arguments to pass to `func`. Default ().
+    accuracy : int, optional
+        Number of digits for the desired accuracy. It will give a warning
+        if the accuracy is worse than this.
+        Default 2.
+
+    Returns
+    -------
+    callable or ndarray
+        Inverse function of `func`. It can take scalars or ndarrays, and return
+        objects of the same kind with the calculated inverse values.
+
+    Notes
+    -----
+
+    .. versionadded:: 0.19.0
+
+    Examples
+    --------
+    >>> from pynverse import inversefunc
+    >>> import numpy as np
+    >>> cube = (lambda x: x**3)
+    >>> invcube = inversefunc(cube)
+    >>> invcube(27) # Should give 3
+    array(3.0000000063797567)
+    >>> invsquare = inversefunc(np.power, args=(2), domain=0)
+    >>> invsquare([4, 16, 64]) # Should give [2, 4, 8]
+    array([ 2.,  4.,  8.])
+    >>> inversefunc(np.log10, y_values=-2, # Should give 0.01
+    ...             domain=0, open_domain=True)
+    array(0.0099999999882423)
+    >>> inversefunc(np.cos, y_values=[1, 0, -1], # Should give [0, pi / 2, pi]
+    ...             domain=[0, np.pi])
+    array([ 0.        ,  1.57079632,  3.14159265])
+    >>> invtan = inversefunc(np.tan,
+    ...                      domain=[-np.pi / 2, np.pi / 2],
+    ...                      open_domain=True)
+    >>> invtan([1, 0, -1]) # Should give [pi / 4, 0, -pi / 4]
+    array([  7.85398163e-01,   1.29246971e-26,  -7.85398163e-01])
+
+    """
+
+    domain, image, open_domain, args = _normparams_inversefunc(domain,
+                                                               image,
+                                                               open_domain,
+                                                               args)
+
+    ymin, ymax = image
+    xmin, xmax = domain
+    xmin_open, xmax_open = open_domain
+
+    # Calculating if the function is increasing or decreasing, using ref points
+    # anywhere in the valid range (Function has to be strictly monotonic)
+    ref1, ref2 = _get_valid_refpoints(xmin, xmax)
+    trend = np.sign(func(ref2, *args) - func(ref1, *args))
+
+    if trend == 0:
+        raise ValueError("Function is not strictly monotonic")
+
+    # Calculating the image by default
+    if ymin is None:
+        ymin = _auto_ymin(func, args, xmin, xmax, trend)
+    if ymax is None:
+        ymax = _auto_ymax(func, args, xmin, xmax, trend)
+
+    # Creating bounded function
+    def bounded_f(x):
+        if xmin is not None and (x < xmin or (x == xmin and xmin_open)):
+                val = -1 * np.inf * trend
+        elif xmax is not None and (x > xmax or (x == xmax and xmax_open)):
+                val = np.inf * trend
+        else:
+            val = func(x, *args)
+        return val
+
+    min_kwargs = {}
+    min_kwargs['bracket'] = (ref1, ref2)
+    min_kwargs['tol'] = 1.48e-08
+    min_kwargs['method'] = 'Brent'
+
+    def inv(yin):
+        yin = np.asarray(yin, dtype=np.float64)
+        shapein = yin.shape
+        yin = yin.flatten()
+        if ymin is not None:
+            if (xmin_open and trend == 1) or (xmax_open and trend == -1):
+                mask = yin <= ymin
+            else:
+                mask = yin < ymin
+            if yin[mask].size > 0:
+                raise ValueError("Requested values %s lower than the"
+                                 " lower limit %g of the image" %
+                                 (yin[mask], ymin))
+        if ymax is not None:
+            if (xmax_open and trend == 1) or (xmin_open and trend == -1):
+                mask = yin >= ymax
+            else:
+                mask = yin > ymax
+            if yin[mask].size > 0:
+                raise ValueError("Requested values %s higher than the"
+                                 " higher limit %g of the image" %
+                                 (yin[mask], ymax))
+
+        results = yin.copy() * np.nan
+        resultsmask = np.zeros(yin.shape, dtype=bool)
+
+        for j in range(yin.size):
+            if xmax is not None:
+                if bounded_f(xmax) == yin[j]:
+                    results[j] = xmax
+                    resultsmask[j] = True
+                    continue
+            if xmin is not None:
+                if bounded_f(xmin) == yin[j]:
+                    results[j] = xmin
+                    resultsmask[j] = True
+                    continue
+
+            optimizer = (lambda x, j=j,
+                         bounded_f=bounded_f: (((bounded_f(x) - yin[j]))**2))
+            try:
+                with warnings.catch_warnings(record=True):
+                    result = minimize_scalar(optimizer, **min_kwargs)
+                results[j] = result.x
+                resultsmask[j] = result.success
+            except:
+                resultsmask[j] = False
+        if any(~resultsmask):
+            warnings.warn("Trouble calculating inverse for values: "
+                          "%s" % str(yin[~resultsmask]), RuntimeWarning)
+
+        try:
+            np.testing.assert_array_almost_equal(yin, func(results, *args),
+                                                 decimal=accuracy)
+        except AssertionError:
+            warnings.warn("Results obtained with less than %g "
+                          "decimal digits of accuracy"
+                          % accuracy, RuntimeWarning)
+
+        return results.reshape(shapein)
+
+    if y_values is None:
+        return inv
+    else:
+        return inv(y_values)
+
+
+def _normparams_inversefunc(domain, image, open_domain, args):
+
+    if not isinstance(args, tuple):
+        args = (args,)
+
+    error_domain = ("domain must be a single scalar, or a have two "
+                    "elements [xmin, xmax]. Set None, to leave it "
+                    "unlimited on one side.")
+    if domain is None:
+        domain = (None, None)
+    else:
+        domain = np.asarray(domain)
+        if domain.ndim == 0:
+            domain = (float(domain), None)
+        elif domain.ndim == 1 and domain.size != 2:
+            raise ValueError(error_domain)
+        elif domain.ndim > 1:
+            raise ValueError(error_domain)
+        else:
+            domain = ((float(domain[0]) if domain[0] is not None else None),
+                      (float(domain[1]) if domain[1] is not None else None))
+
+    error_open_domain = ("open_domain must be a single scalar, or a have two "
+                         "bool elements [open_xmin, open_xmax].")
+    if open_domain is None:
+        open_domain = (False, False)
+    else:
+        open_domain = np.asarray(open_domain)
+        if open_domain.ndim == 0:
+            open_domain = (bool(open_domain), bool(open_domain))
+        elif open_domain.ndim == 1 and open_domain.size != 2:
+            raise ValueError(error_open_domain)
+        elif open_domain.ndim > 1:
+            raise ValueError(error_open_domain)
+        else:
+            open_domain = (bool(open_domain[0]), bool(open_domain[1]))
+
+    error_image = ("image must be a single scalar, or a have two "
+                   "bool elements [ymin, ymax].")
+    if image is None:
+        image = (None, None)
+    else:
+        image = np.asarray(image)
+        if image.ndim != 1 or image.size != 2:
+            raise ValueError(error_image)
+        else:
+            image = ((float(image[0]) if image[0] is not None else None),
+                     (float(image[1]) if image[1] is not None else None))
+
+    if domain[0] is not None and domain[1] is not None:
+        if domain[0] >= domain[1]:
+            raise ValueError("domain[0] min must be less than domain[1]")
+
+    if image[0] is not None and image[1] is not None:
+        if image[0] >= image[1]:
+            raise ValueError("image[0] min must be less than image[1]")
+
+    return domain, image, open_domain, args
+
+
+def _get_valid_refpoints(xmin, xmax):
+    if xmin is not None and xmax is not None:
+        d = xmax - xmin
+        ref1 = xmin + d / 4.
+        ref2 = xmax - d / 4.
+    elif xmin is not None:
+        ref1 = xmin + 1.
+        ref2 = xmin + 2.
+    elif xmax is not None:
+        ref1 = xmax - 2.
+        ref2 = xmax - 1.
+    else:
+        ref1 = 0.
+        ref2 = 1.
+    return ref1, ref2
+
+
+def _auto_ymin(func, args, xmin, xmax, trend):
+    ymin = None
+    if ((xmin is not None and trend == 1) or
+       (xmax is not None and trend == -1)):
+        try:
+            with warnings.catch_warnings(record=True):
+                ymin = func(xmin, *args) if trend == 1 else func(xmax, *args)
+        except:
+            raise ValueError("Cannot automatically calculate the lower limit "
+                             "of the image please inclue it as a parameter")
+    return ymin
+
+
+def _auto_ymax(func, args, xmin, xmax, trend):
+    ymax = None
+    if ((xmax is not None and trend == 1) or
+       (xmin is not None and trend == -1)):
+        try:
+            with warnings.catch_warnings(record=True):
+                ymax = func(xmax, *args) if trend == 1 else func(xmin, *args)
+        except:
+            raise ValueError("Cannot automatically calculate the upper limit "
+                             "of the image please include it as a parameter")
+    return ymax
```

### Comparing `pynverse-0.1.4.4/README` & `pynverse-0.1.4.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,210 +1,141 @@
-pynverse |PyPI version|
-=======================
-
-A module specialized on calculating the numerical inverse of any
-invertible continuous function.
-
-Requirements
-------------
-
-|Scipy| |Numpy|
-
-Install
--------
-
-In order to install this tool you'll need ``pip``:
-
-::
-
-    pip install pynverse
-
-Usage
------
-
-Pynverse provides a main function ``inversefunc`` that calculates the
-numerical inverse of a function ``f`` passed as the first argument in
-the form of a callable.
-
-.. code:: python
-
-        >>> from pynverse import inversefunc
-
-It can be used to calculate the inverse function at certain ``y_values``
-points:
-
-.. code:: python
-
-        >>> cube = (lambda x: x**3)
-        >>> invcube = inversefunc(cube, y_values=3)
-        array(3.0000000063797567)
-
-Or to obtain a callable that will calculate the inverse values at any
-other points if ``y_values`` is not provided:
-
-.. code:: python
-
-        >>> invcube = inversefunc(cube)
-        >>> invcube(27)
-        array(3.0000000063797567)
-
-It requires the function to be continuous and strictly monotonic (i.e.
-purely decreasing or purely increasing) within the domain of the
-function. By default, the domain includes all real numbers, but it can
-be restricted to an inverval using the ``domain`` argument:
-
-.. code:: python
-
-        >>> import numpy as np
-        >>> inversefunc(np.cos, y_values=[1, 0, -1], # Should give [0, pi / 2, pi]
-        ...             domain=[0, np.pi])
-        array([ 0.        ,  1.57079632,  3.14159265])
-
-Additionally, the argument ``open_domain`` can be used to specify the
-open/closed character of each of the ends of the domain interval:
-
-.. code:: python
-
-        >>> inversefunc(np.log10, y_values=-2, # Should give 0.01
-        ...             domain=0, open_domain=[True, False])
-        array(0.0099999999882423)
-
-Or on both ends simultaneously:
-
-.. code:: python
-
-        >>> invtan = inversefunc(np.tan,
-        ...                      domain=[-np.pi / 2, np.pi / 2],
-        ...                      open_domain=True)
-        >>> invtan([1, 0, -1]) # Should give [pi / 4, 0, -pi / 4]
-        array([  7.85398163e-01,   1.29246971e-26,  -7.85398163e-01])
-
-Additional parameters may be passed to the function for easier
-reusability of callables using the ``args`` argument:
-
-.. code:: python
-
-        >>> invsquare = inversefunc(np.power, args=(2), domain=0)
-        >>> invsquare([4, 16, 64])
-        array([ 2.,  4.,  8.])
-
-The image of the function in the interval may be also provided for cases
-where the function is non continuous right at the end of an open
-interval with the ``image`` argument:
-
-.. code:: python
-
-        >>> invmod = inversefunc(np.mod, args=(1), domain=[5,6], 
-        ...                      open_domain=[False,True], image=[0,1])
-        >>> invmod([0.,0.3,0.5])
-        array([ 5. ,  5.3,  5.5])
-
-Additionally an argument can be used to check for the number of digits
-of accuracy in the results, giving a warning in case this is not meet:
-
-.. code:: python
-
-        >>> inversefunc(np.log10, y_values=-8, # Should give 0.01
-        ...             domain=0, open_domain=True, accuracy=6)
-        pynverse\inverse.py:195: RuntimeWarning: Results obtained with less than 6 decimal digits of accuracy
-        array(9.999514710830838e-09)
-
-As it is compatible with arrays, it can very easily used to obtain the
-inverse for broad ranges. These are some examples of using the returned
-numerical inverse callables with arrays to make plots, and compare them
-to the analytical inverse, each of them calculated as simply as:
-
-.. code:: python
-
-    log = lambda x: np.log10(x)
-    invlog = inversefunc(log, domain=0, open_domain=True)
-    x1=np.linspace(0.00001,10,100)
-    x2=np.linspace(-5,1,100)
-    ax1.plot(x1,log(y1),'b-')
-    ax2.plot(x2,invlog(x2),'b-')
-
-    invlog_a = lambda x: 10**x
-    ax2.plot(x2,invlog_a(x2),'r--')
-
-.. figure:: https://cloud.githubusercontent.com/assets/12649253/19738042/cf22460a-9bad-11e6-9c17-6fdd6cda0991.png
-   :alt: 
-
-In particular, for the definition of piecewise functions, there is a
-``piecewise`` utility function provided that solves the issues of
-np.piecewise when working with both scalars and arrays. For example, the
-inverse for the last plot was obtained as:
-
-.. code:: python
-
-    from pynverse import inversefunc, piecewise
-
-    pw=lambda x: piecewise(x,[x<1,(x>=1)*(x<3),x>=3],
-                           [lambda x: x, lambda x: x**2, lambda x: x+6])
-    invpw =inversefunc(pw) 
-
-Disclaimer
-----------
-
-The problem of calculating the numerical inverse of an arbitrary
-function in unlimited or open intervals is still an open question in
-applied mathematics. The main purpose of this package is not to be fast,
-or as accurate as it could be if the inverse was calculated specifically
-for a known function, using more specialised techniques. The current
-implementation essentially uses the existing tools in scipy to solve the
-particular problem of finding the inverse of a function meeting the
-continuity and monotonicity conditions, but while it performs really
-well it may fail under certain conditions. For example when inverting a
-``log10`` it is known to start giving inccacurate values when being
-asked to invert -10, which should correspond to 0.0000000001 (1e-10),
-but gives instead 0.0000000000978 (0.978e-10).
-
-The advantage about estimating the inverse function is that the accuracy
-can always be verified by checking if f(finv(x))==x.
-
-Details about the implementation
---------------------------------
-
-The summarized internal strategy is the following:
-
-1. Figure out if the function is increasing or decreasing. For this two
-   reference points ref1 and ref2 are needed:
-
-   -  In case of a finite interval, the points ref points are 1/4 and
-      3/4 through the interval.
-   -  In an infinite interval any two values work really.
-   -  If f(ref1)<f(ref2), the function is increasing, otherwise is
-      decreasing.
-
-2. Figure out the image of the function in the interval.
-
-   -  If values are provided, then those are used.
-   -  In a closed interval just calculate f(a) and f(b), where a and b
-      are the ends of the interval.
-   -  In an open interval try to calculate f(a) and f(b), if this works
-      those are used, otherwise it will be assume to be (-Inf, Inf).
-
-3. Built a bounded function with the following conditions:
-
-   -  bounded\_f(x):
-
-      -  return -Inf if x below interval, and f is increasing.
-      -  return +Inf if x below interval, and f is decreasing.
-      -  return +Inf if x above interval, and f is increasing.
-      -  return -Inf if x above interval, and f is decreasing.
-      -  return f(x) otherwise
-
-4. If the required number y0 for the inverse is outside the image, raise
-   an exception.
-5. Find roots for bounded\_f(x)-y0, by minimizing
-   (bounded\_f(x)-y0)\*\*2, using the ``Brent`` method, making sure that
-   the algorithm for minimising starts in a point inside the original
-   interval by setting ref1, ref2 as brackets. As soon as if goes
-   outside the allowed intervals, bounded\_f returns infinite, forcing
-   the algorithm to go back to search inside the interval.
-6. Check that the solutions are accurate and they meet f(x0)=y0 to some
-   desired precision, raising a warning otherwise.
-
-.. |PyPI version| image:: https://badge.fury.io/py/pynverse.svg
-   :target: https://badge.fury.io/py/pynverse
-.. |Scipy| image:: https://img.shields.io/badge/scipy-%3E=0.11-blue.svg
-.. |Numpy| image:: https://img.shields.io/badge/numpy-%3E=1.6-blue.svg
-
+# pynverse [![PyPI version](https://badge.fury.io/py/pynverse.svg)](https://badge.fury.io/py/pynverse)
+
+A module specialized on calculating the numerical inverse of any invertible continuous function.
+
+
+## Requirements
+
+  ![Scipy](https://img.shields.io/badge/scipy-%3E=0.11-blue.svg)
+  ![Numpy](https://img.shields.io/badge/numpy-%3E=1.6-blue.svg)
+
+## Install
+
+In order to install this tool you'll need `pip`:
+
+    pip install git+git://github.com/alvarosg/pynverse.git
+    
+Note installing from PyPI is not longer supported / maintained.
+    
+## Usage
+
+Pynverse provides a main function `inversefunc` that calculates the numerical inverse of a function `f` passed as the first argument in the form of a callable. 
+```python
+    >>> from pynverse import inversefunc
+```
+
+It can be used to calculate the inverse function at certain `y_values` points:
+```python
+    >>> cube = (lambda x: x**3)
+    >>> invcube = inversefunc(cube, y_values=27)
+    array(3.0000000063797567)
+```
+
+Or to obtain a callable that will calculate the inverse values at any other points if `y_values` is not provided:
+```python
+    >>> invcube = inversefunc(cube)
+    >>> invcube(27)
+    array(3.0000000063797567)
+```
+
+It requires the function to be continuous and strictly monotonic (i.e. purely decreasing or purely increasing) within the domain of the function. By default, the domain includes all real numbers, but it can be restricted to an inverval using the `domain` argument:
+```python
+    >>> import numpy as np
+    >>> inversefunc(np.cos, y_values=[1, 0, -1], # Should give [0, pi / 2, pi]
+    ...             domain=[0, np.pi])
+    array([ 0.        ,  1.57079632,  3.14159265])
+```
+
+Additionally, the argument `open_domain` can be used to specify the open/closed character of each of the ends of the domain interval:
+```python
+    >>> inversefunc(np.log10, y_values=-2, # Should give 0.01
+    ...             domain=0, open_domain=[True, False])
+    array(0.0099999999882423)
+```
+
+Or on both ends simultaneously:
+```python
+    >>> invtan = inversefunc(np.tan,
+    ...                      domain=[-np.pi / 2, np.pi / 2],
+    ...                      open_domain=True)
+    >>> invtan([1, 0, -1]) # Should give [pi / 4, 0, -pi / 4]
+    array([  7.85398163e-01,   1.29246971e-26,  -7.85398163e-01])
+```
+
+Additional parameters may be passed to the function for easier reusability of callables using the `args` argument:
+
+```python
+    >>> invsquare = inversefunc(np.power, args=(2), domain=0)
+    >>> invsquare([4, 16, 64])
+    array([ 2.,  4.,  8.])
+```
+
+The image of the function in the interval may be also provided for cases where the function is non continuous right at the end of an open interval with the `image` argument:
+
+```python
+    >>> invmod = inversefunc(np.mod, args=(1), domain=[5,6], 
+    ...                      open_domain=[False,True], image=[0,1])
+    >>> invmod([0.,0.3,0.5])
+    array([ 5. ,  5.3,  5.5])
+```
+
+Additionally an argument can be used to check for the number of digits of accuracy in the results, giving a warning in case this is not meet:
+```python
+    >>> inversefunc(np.log10, y_values=-8, # Should give 0.01
+    ...             domain=0, open_domain=True, accuracy=6)
+    pynverse\inverse.py:195: RuntimeWarning: Results obtained with less than 6 decimal digits of accuracy
+    array(9.999514710830838e-09)
+```
+
+As it is compatible with arrays, it can very easily used to obtain the inverse for broad ranges. These are some examples of using the returned numerical inverse callables with arrays to make plots, and compare them to the analytical inverse, each of them calculated as simply as:
+```python
+log = lambda x: np.log10(x)
+invlog = inversefunc(log, domain=0, open_domain=True)
+x1=np.linspace(0.00001,10,100)
+x2=np.linspace(-5,1,100)
+ax1.plot(x1,log(y1),'b-')
+ax2.plot(x2,invlog(x2),'b-')
+
+invlog_a = lambda x: 10**x
+ax2.plot(x2,invlog_a(x2),'r--')
+```
+
+![](https://cloud.githubusercontent.com/assets/12649253/19738042/cf22460a-9bad-11e6-9c17-6fdd6cda0991.png)
+
+In particular, for the definition of piecewise functions, there is a `piecewise` utility function provided that solves the issues of np.piecewise when working with both scalars and arrays. For example, the inverse for the last plot was obtained as:
+
+```python
+from pynverse import inversefunc, piecewise
+
+pw=lambda x: piecewise(x,[x<1,(x>=1)*(x<3),x>=3],
+                       [lambda x: x, lambda x: x**2, lambda x: x+6])
+invpw =inversefunc(pw) 
+```
+
+## Disclaimer
+
+The problem of calculating the numerical inverse of an arbitrary function in unlimited or open intervals is still an open question in applied mathematics. The main purpose of this package is not to be fast, or as accurate as it could be if the inverse was calculated specifically for a known function, using more specialised techniques. The current implementation essentially uses the existing tools in scipy to solve the particular problem of finding the inverse of a function meeting the continuity and monotonicity conditions, but while it performs really well it may fail under certain conditions. For example when inverting a `log10` it is known to start giving inccacurate values when being asked to invert -10, which should correspond to 0.0000000001 (1e-10), but gives instead 0.0000000000978 (0.978e-10). 
+
+The advantage about estimating the inverse function is that the accuracy can always be verified by checking if f(finv(x))==x.
+
+## Details about the implementation
+
+The summarized internal strategy is the following:
+
+1. Figure out if the function is increasing or decreasing. For this two reference points ref1 and ref2 are needed:
+    * In case of a finite interval, the points ref points are 1/4 and 3/4 through the interval.
+    * In an infinite interval any two values work really.
+    * If f(ref1)<f(ref2), the function is increasing, otherwise is decreasing.
+2. Figure out the image of the function in the interval. 
+    * If values are provided, then those are used.
+    * In a closed interval just calculate f(a) and f(b), where a and b are the ends of the interval.
+    * In an open interval try to calculate f(a) and f(b), if this works those are used, otherwise it will be assume to be (-Inf, Inf).
+3. Built a bounded function with the following conditions:
+    * bounded_f(x):
+        * return -Inf if x below interval, and f is increasing.
+        * return +Inf if x below interval, and f is decreasing.
+        * return +Inf if x above interval, and f is increasing.
+        * return -Inf if x above interval, and f is decreasing.
+        * return f(x) otherwise
+4. If the required number y0 for the inverse is outside the image, raise an exception.
+5. Find roots for bounded_f(x)-y0, by minimizing (bounded_f(x)-y0)**2, using the `Brent` method, making sure that the algorithm for minimising starts in a point inside the original interval by setting ref1, ref2 as brackets. As soon as if goes outside the allowed intervals, bounded_f returns infinite, forcing the algorithm to go back to search inside the interval.
+6. Check that the solutions are accurate and they meet f(x0)=y0 to some desired precision, raising a warning otherwise.
```

### Comparing `pynverse-0.1.4.4/setup.py` & `pynverse-0.1.4.6/setup.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-
-from setuptools import setup, find_packages
-import imp
-
-version = imp.load_source('pynverse.version', 'pynverse/version.py')
-rev = version.git_revision
-
-setup(
-    name='pynverse',
-    packages=find_packages(),
-    version=rev,
-    description='A library for calculating the numerical inverse of a function',
-    author='Alvaro Sanchez-Gonzalez',
-    author_email='sanchezgnzlz.alvaro@gmail.com',
-    url='https://github.com/alvarosg/pynverse',
-    download_url='https://github.com/alvarosg/pynverse/tarball/' + rev,
-    keywords=['inverse', 'function', 'numerical'],
-    license='MIT',
-    classifiers=[
-            'Development Status :: 4 - Beta',
-            'Intended Audience :: Developers',
-            'Topic :: Software Development :: Build Tools',
-            'License :: OSI Approved :: MIT License',
-            'Programming Language :: Python :: 2.7',
-            'Programming Language :: Python :: 3',
-            'Programming Language :: Python :: 3.2',
-            'Programming Language :: Python :: 3.3',
-            'Programming Language :: Python :: 3.4',
-            'Programming Language :: Python :: 3.5',
-    ],
-    test_suite='nose.collector',
-    install_requires=['scipy>=0.11', 'numpy>=1.6'],
-    setup_requires=['nose>=1.0', 'scipy>=0.11', 'numpy>=1.6'],
-    tests_require=['nose>=1.0', 'scipy>=0.11', 'numpy>=1.6'],
+
+from setuptools import setup, find_packages
+import imp
+
+version = imp.load_source('pynverse.version', 'pynverse/version.py')
+rev = version.git_revision
+
+setup(
+    name='pynverse',
+    packages=find_packages(),
+    version=rev,
+    description='A library for calculating the numerical inverse of a function',
+    author='Alvaro Sanchez-Gonzalez',
+    author_email='sanchezgnzlz.alvaro@gmail.com',
+    url='https://github.com/alvarosg/pynverse',
+    download_url='https://github.com/alvarosg/pynverse/tarball/' + rev,
+    keywords=['inverse', 'function', 'numerical'],
+    license='MIT',
+    classifiers=[
+            'Development Status :: 4 - Beta',
+            'Intended Audience :: Developers',
+            'Topic :: Software Development :: Build Tools',
+            'License :: OSI Approved :: MIT License',
+            'Programming Language :: Python :: 2.7',
+            'Programming Language :: Python :: 3',
+            'Programming Language :: Python :: 3.2',
+            'Programming Language :: Python :: 3.3',
+            'Programming Language :: Python :: 3.4',
+            'Programming Language :: Python :: 3.5',
+    ],
+    test_suite='nose.collector',
+    install_requires=['scipy>=0.11', 'numpy>=1.6'],
+    setup_requires=['nose>=1.0', 'scipy>=0.11', 'numpy>=1.6'],
+    tests_require=['nose>=1.0', 'scipy>=0.11', 'numpy>=1.6'],
 )
```

