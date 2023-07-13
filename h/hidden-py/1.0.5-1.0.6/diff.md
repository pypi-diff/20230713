# Comparing `tmp/hidden-py-1.0.5.tar.gz` & `tmp/hidden-py-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidden-py-1.0.5.tar", last modified: Wed Jul 12 16:50:23 2023, max compression
+gzip compressed data, was "hidden-py-1.0.6.tar", last modified: Thu Jul 13 17:44:12 2023, max compression
```

## Comparing `hidden-py-1.0.5.tar` & `hidden-py-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:23.067329 hidden-py-1.0.5/
--rw-rw-rw-   0        0        0     1088 2023-04-19 15:14:57.000000 hidden-py-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0    13267 2023-07-12 16:50:23.067329 hidden-py-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    12562 2023-07-12 16:36:28.000000 hidden-py-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:23.040326 hidden-py-1.0.5/hidden_py/
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/__init__.py
--rw-rw-rw-   0        0        0     5692 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/dynamics.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:23.048326 hidden-py-1.0.5/hidden_py/filters/
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/filters/__init__.py
--rw-rw-rw-   0        0        0     9542 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/filters/bayesian.py
--rw-rw-rw-   0        0        0    11766 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/infer.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:23.058330 hidden-py-1.0.5/hidden_py/optimize/
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/optimize/__init__.py
--rw-rw-rw-   0        0        0    11671 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/optimize/base.py
--rw-rw-rw-   0        0        0      183 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/optimize/config.py
--rw-rw-rw-   0        0        0    19955 2023-07-12 16:44:04.000000 hidden-py-1.0.5/hidden_py/optimize/optimization.py
--rw-rw-rw-   0        0        0      289 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/optimize/registry.py
--rw-rw-rw-   0        0        0     2395 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/optimize/results.py
--rw-rw-rw-   0        0        0        0 2023-06-20 18:29:03.000000 hidden-py-1.0.5/hidden_py/optimize/types.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:23.046327 hidden-py-1.0.5/hidden_py.egg-info/
--rw-rw-rw-   0        0        0    13267 2023-07-12 16:50:22.000000 hidden-py-1.0.5/hidden_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-07-12 16:50:22.000000 hidden-py-1.0.5/hidden_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:50:22.000000 hidden-py-1.0.5/hidden_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-12 16:50:22.000000 hidden-py-1.0.5/hidden_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-12 16:50:22.000000 hidden-py-1.0.5/hidden_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 16:50:23.068329 hidden-py-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1162 2023-07-12 16:48:33.000000 hidden-py-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:50:23.064329 hidden-py-1.0.5/tests/
--rw-rw-rw-   0        0        0     3808 2023-06-20 18:29:03.000000 hidden-py-1.0.5/tests/test_dynamics.py
--rw-rw-rw-   0        0        0    11048 2023-06-20 18:29:03.000000 hidden-py-1.0.5/tests/test_filters.py
--rw-rw-rw-   0        0        0     5943 2023-06-20 18:29:03.000000 hidden-py-1.0.5/tests/test_inferrence.py
--rw-rw-rw-   0        0        0     7823 2023-06-20 18:29:03.000000 hidden-py-1.0.5/tests/test_optimizers.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.843456 hidden-py-1.0.6/
+-rw-r--r--   0 stevelarge   (501) staff       (20)     1068 2022-03-05 13:45:02.000000 hidden-py-1.0.6/LICENSE.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)    13053 2023-07-13 17:44:12.843218 hidden-py-1.0.6/PKG-INFO
+-rw-r--r--   0 stevelarge   (501) staff       (20)    12366 2023-06-21 04:36:21.000000 hidden-py-1.0.6/README.md
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.839360 hidden-py-1.0.6/hidden_py/
+-rw-r--r--   0 stevelarge   (501) staff       (20)       66 2023-07-13 16:20:17.000000 hidden-py-1.0.6/hidden_py/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     5515 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/dynamics.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.840561 hidden-py-1.0.6/hidden_py/filters/
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/filters/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     9293 2023-07-13 17:43:37.000000 hidden-py-1.0.6/hidden_py/filters/bayesian.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    11471 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/infer.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.842134 hidden-py-1.0.6/hidden_py/optimize/
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/__init__.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    11349 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/base.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)      170 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/config.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    19445 2023-07-13 17:42:41.000000 hidden-py-1.0.6/hidden_py/optimize/optimization.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)      281 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/registry.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     2318 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/results.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)        0 2023-06-18 01:27:25.000000 hidden-py-1.0.6/hidden_py/optimize/types.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.840226 hidden-py-1.0.6/hidden_py.egg-info/
+-rw-r--r--   0 stevelarge   (501) staff       (20)    13053 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/PKG-INFO
+-rw-r--r--   0 stevelarge   (501) staff       (20)      623 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/SOURCES.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)        1 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/dependency_links.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       52 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/requires.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       10 2023-07-13 17:44:12.000000 hidden-py-1.0.6/hidden_py.egg-info/top_level.txt
+-rw-r--r--   0 stevelarge   (501) staff       (20)       38 2023-07-13 17:44:12.843505 hidden-py-1.0.6/setup.cfg
+-rw-r--r--   0 stevelarge   (501) staff       (20)     1123 2023-07-13 17:43:53.000000 hidden-py-1.0.6/setup.py
+drwxr-xr-x   0 stevelarge   (501) staff       (20)        0 2023-07-13 17:44:12.842895 hidden-py-1.0.6/tests/
+-rw-r--r--   0 stevelarge   (501) staff       (20)     3644 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_dynamics.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)    10667 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_filters.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     5702 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_inferrence.py
+-rw-r--r--   0 stevelarge   (501) staff       (20)     7563 2023-06-18 01:27:25.000000 hidden-py-1.0.6/tests/test_optimizers.py
```

### Comparing `hidden-py-1.0.5/LICENSE.txt` & `hidden-py-1.0.6/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Steven Large
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2020 Steven Large
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `hidden-py-1.0.5/PKG-INFO` & `hidden-py-1.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-Metadata-Version: 2.1
-Name: hidden-py
-Version: 1.0.5
-Summary: A python package for discrete-output hidden Markov models
-Author: Steven Large
-Author-email: stevelarge7@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/StevenJLarge/hmm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# **A Hidden Markov Model package for python**
-
-### Installation
-
-To install this package simply run the command:
-
-`pip install hidden-py`
-
-<br />
-
-## Table of Contents
-
-- [Overview](#overview)
-  - [Dynamics/Simulation](#dynamicssimulation)
-  - [System Identification](#system-identification)
-  - [Signal Processing](#signal-processing)
-- [Roadmap](#roadmap)
-- [References](#references)
-
----
-
-## Overview
-
-This package contains logic for inferring, simulating, and fitting Hidden Markov Models with discrete states and observations. This poackage serves as a complement to several common HMM packages that deal primarily with _mixture models_, where output symbols are continuous, and drawn from a distriubtion of values that is somehow conditional on the hidden state.
-
-Here, we have considered primarily scenarios where the observation value is an integer, and one of the possible hidden states, although this is not required, there could be more hidden states than possible observations, or vice-versa, all that really matters is that the observation values (and hidden state values) are discrete. There are three major use-cases for this codebase: dynamics/simulation, system identification/parameter fitting, and signal processing. In all cases, these functionalities are outlined in several tutorial notebooks in the `notebooks/tutorials` location of the [github repository](https://github.com/StevenJLarge/hmm)
-
-<br />
-
-## Hidden Markov Models
-
-Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
-
-Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
-
-<p align='center'>
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true" width="75%" vspace="30px"/>
-</p>
-
-Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step. For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
-
-$$ p_T = A^T \cdot p_0 $$
-
-A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
-
-<p align="center">
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true" width="75%" vspace="30px" />
-</p>
-
-Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
-
----
-
-As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
-
-### Dynamics/Simulation
-
-The `hidden.dynamics` submodule contains the code necessary to simulate the hidden state and observation dynamics as specified by a state transition matrix $A$ (with elements that quantify the rate of transitions between states) and an observation matrix $B$, with elements that quantify the probability of observing a given output symbol, given the current hidden state.
-
-For instance, the code necessary to initialize a hidden Markov model, run the dyanamics, and extract the observation and state time-series
-
-```python
-from hidden_py import dynamics
-
-# 2 hidden states, 2 possible observation values
-hmm = dynamics.HMM(2, 2)
-
-# Helper routine to initialize A and B matrices
-hmm.init_uniform_cycle()
-
-# Run dynamics for 100 time steps
-hmm.run_dynamics(100)
-
-# Pull out the observations, and true (simulated) hidden state values
-observations = hmm.get_obs_ts()
-hidden_states = hmm.get_state_ts()
-```
-
-As an example, the schematic below shows a possible trajectory for a HMM with 2 hidden states and 2 possible observation values.
-
-<p align="center">
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/sample_trajectory.png?raw=true" width="75%" vspace="30px" />
-</p>
-
-Here the red dots represent the state of the hidden system over time, while the black dots indicate the observed value at that point in time. So, at time point 3, for instance, the observed value differs from the hidden state. See the `notebooks/tutorials/02-hidden-markov-model.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) for a more in-depth review of this process.
-
-<br />
-
----
-
-### System Identification
-
-The `infer` submodule contains the code that wraps lower-level functionality (primarily in the `filters/bayesian.py` and `optimize/optimization.py` files) for both signal processing and system identification/parameter fitting.
-
-There are two separate means of performing system identification: Local/Global partial likelihood optimization, and complete-data likelihood optimization. While more comprehensive details are contained in the github notebooks, broadly speaking partial data likelihood optimization performs relatively standard optimizations on the likelihood function $\mathcal{L}(\theta | Y)$ which considers only the observations as the _data_. Effectively, these optimizers wrap the `scipy.opt.minimize` functions by encoding and decoding the $A$ and $B$ matrices into a parameter vector (ensuring that their column-normalization is preserved) and calculating the negative log-likelihood of a particular parameter vector. In practice, given a set of observations, we can initialize an `analyzer` and run either local (using, by default, the `scipy.opt.minimize` function with the `L-BFGS-B` algorithm) or global (using the `scipy` SHGO algorithm) as:
-
-```python
-from hidden_py import infer
-
-# Input the dimensions of the HMM and observations
-analyzer = infer.MarkovInfer(2, 2)
-
-# Initial estimates of the A and B matrices
-A_est = np.array([
-    [0.8, 0.1],
-    [0.2, 0.9]
-])
-
-B_est = np.array([
-    [0.9, 0.05],
-    [0.1, 0.95]
-])
-
-# Run local partial-data likelihood optimization (default behaviour), the symmetric keyword can be used to specify whether or not the A and B matrices are assumed to be symmetric
-opt_local = analyzer.optimize(observations, A_est, B_est, symmetric=False)
-
-# And the partial-data global likelihood optimization, the A and B initial matrices are not used in the optimizer, aside from providing a way of specifying the dimension of the parameter vectors
-opt_global = analyzer.optimize(observations, A_est, B_est, symmetric=False, opt_type=OptClass.Global)
-
-```
-
-Now, for the complete-data likeihood optimization, the interface is very similar, but behind the scenes the code will implement an implementation of the Baum-Welch reparameterization algorithm (an instance of an Expectation-Maximization algorithm) to find the optimal parameter values. In practice, this can be done as:
-
-```python
-from hidden_py import infer
-from hidden_py.optimize.base import OptClass
-
-analyzer = infer.MarkovInfer(2, 2)
-
-res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax)
-
-```
-
-In all cases, there is also an option to add algorithm options to customize the specifics of the optinization. Most relevant is for the expectation-maximization where you can specify a maximum number of iterations for the algorithm, as well as a threshold on the size of parameter changes (quantified by the matrix norm of pre- and post-update $A$ and $B$ matrices). This can be accessed through the `algo_opts` dictionary. For instance, if we wanted to change the maximum iterations in the BW algorithm to 1000 and set the termination threshold at `1e-10`, we would perform the previous call as
-
-```python
-options = {
-    'maxiter': 1000,
-    "threshold": 1e-10
-}
-
-res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax, algo_opts=options)
-```
-
-In essence, this set of tools allows you to infer the best model given a set of observed data. Under the hood, many of the tools from the signal processing module are used, but the `analyzer.optimize(...)` function calls largely hide that complexity.
-
-<br />
-
----
-
-### Signal Processing
-
-The `infer` submodule can also be used for the purposes of signal processing: given a valid estimate of the model parameters, how can we best estimate the hidden state value, given the observations. There are two distinct domains of application, first would be prediction in real time, where only observations in the past are available for inferring the current hidden state (this would use the so-called forward-filtered estiamte). There is also an _ex post_ approach, which uses the entirety of observations from a given period of time to estimate the hidden state at a particular point within that time period. This is the so-called Bayesian smoothed estiamte of the hidden state.
-
-Mathematically, if we denote $Y^t \equiv \{ y_0, y_1, \cdots, y_t \}$ as the sequence of observations from tie $t=0$ up to time $t$, then for a total trajectory length of $T$, the forward filter and Bayesian smoothed estimate are calculating
-
-$$
-p(x_t | Y^t) \quad \to \qquad \text{\sf Forward-filter} \\
-
-\, \\
-
-p(x_t | Y^T) \quad \to \quad \text{\sf Bayesian smoother}
-$$
-
-where, $x_t$ is the hidden state at time $t$.
-
-Quantitatively the forward filter and Bayesian smoothed estimates of a given HMM sequence of observations can be calculated in the following way:
-
-```python
-from hidden_py import infer
-
-analyzer = infer.MarkovInfer(2, 2)
-
-# Gets the forward algorithm results
-analyzer.forward_algo(observations, A, B)
-
-# Gets the Bayesian-smoothed estimate of the hidden state
-analyzer.bayesian_smooth(observations, A, B)
-
-```
-
-The tutorial notebook `notebooks/tutorials.03-slarge-hmm-filters.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) gives a more comprehensive overview and visualization of this procedure.
-
-<br />
-
----
-
-## References
-
-There is a breadth of research and literatur on HMMs out in the world, but below are a few sources that I found particularly helpful in working on this project
-
-<ol>
-    <li> <a href="https://www.cambridge.org/core/books/control-theory-for-physicists/21AFE5D6C475D1B44BCF9B8536338D98">"Control Theory for Physicists"</a>, J. Bechhoeffer, C
-    Cambridge University Press, 2021</li>
-    <li><a href="http://numerical.recipes/aboutNR3book.html">"Numerical Recipes: The Art of Scientific Computing"</a>, W.H. Press, S.A. Teukolsky, W.T. Vetterling, & B.P. Flannery, Cambridge University Press, 3rd ed., 2007</li>
-</ol>
+Metadata-Version: 2.1
+Name: hidden-py
+Version: 1.0.6
+Summary: A python package for discrete-output hidden Markov models
+Author: Steven Large
+Author-email: stevelarge7@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/StevenJLarge/hmm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# **A Hidden Markov Model package for python**
+
+### Installation
+
+To install this package simply run the command:
+
+`pip install hidden-py`
+
+<br />
+
+## Table of Contents
+
+- [Overview](#overview)
+  - [Dynamics/Simulation](#dynamicssimulation)
+  - [System Identification](#system-identification)
+  - [Signal Processing](#signal-processing)
+- [Roadmap](#roadmap)
+- [References](#references)
+
+---
+
+## Overview
+
+This package contains logic for inferring, simulating, and fitting Hidden Markov Models with discrete states and observations. This poackage serves as a complement to several common HMM packages that deal primarily with _mixture models_, where output symbols are continuous, and drawn from a distriubtion of values that is somehow conditional on the hidden state.
+
+Here, we have considered primarily scenarios where the observation value is an integer, and one of the possible hidden states, although this is not required, there could be more hidden states than possible observations, or vice-versa, all that really matters is that the observation values (and hidden state values) are discrete. There are three major use-cases for this codebase: dynamics/simulation, system identification/parameter fitting, and signal processing. In all cases, these functionalities are outlined in several tutorial notebooks in the `notebooks/tutorials` location of the [github repository](https://github.com/StevenJLarge/hmm)
+
+<br />
+
+## Hidden Markov Models
+
+Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
+
+Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
+
+<p align='center'>
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true" width="75%" vspace="30px"/>
+</p>
+
+Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step. For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
+
+$$ p_T = A^T \cdot p_0 $$
+
+A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
+
+<p align="center">
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true" width="75%" vspace="30px" />
+</p>
+
+Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
+
+---
+
+As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
+
+### Dynamics/Simulation
+
+The `hidden.dynamics` submodule contains the code necessary to simulate the hidden state and observation dynamics as specified by a state transition matrix $A$ (with elements that quantify the rate of transitions between states) and an observation matrix $B$, with elements that quantify the probability of observing a given output symbol, given the current hidden state.
+
+For instance, the code necessary to initialize a hidden Markov model, run the dyanamics, and extract the observation and state time-series
+
+```python
+from hidden_py import dynamics
+
+# 2 hidden states, 2 possible observation values
+hmm = dynamics.HMM(2, 2)
+
+# Helper routine to initialize A and B matrices
+hmm.init_uniform_cycle()
+
+# Run dynamics for 100 time steps
+hmm.run_dynamics(100)
+
+# Pull out the observations, and true (simulated) hidden state values
+observations = hmm.get_obs_ts()
+hidden_states = hmm.get_state_ts()
+```
+
+As an example, the schematic below shows a possible trajectory for a HMM with 2 hidden states and 2 possible observation values.
+
+<p align="center">
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/sample_trajectory.png?raw=true" width="75%" vspace="30px" />
+</p>
+
+Here the red dots represent the state of the hidden system over time, while the black dots indicate the observed value at that point in time. So, at time point 3, for instance, the observed value differs from the hidden state. See the `notebooks/tutorials/02-hidden-markov-model.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) for a more in-depth review of this process.
+
+<br />
+
+---
+
+### System Identification
+
+The `infer` submodule contains the code that wraps lower-level functionality (primarily in the `filters/bayesian.py` and `optimize/optimization.py` files) for both signal processing and system identification/parameter fitting.
+
+There are two separate means of performing system identification: Local/Global partial likelihood optimization, and complete-data likelihood optimization. While more comprehensive details are contained in the github notebooks, broadly speaking partial data likelihood optimization performs relatively standard optimizations on the likelihood function $\mathcal{L}(\theta | Y)$ which considers only the observations as the _data_. Effectively, these optimizers wrap the `scipy.opt.minimize` functions by encoding and decoding the $A$ and $B$ matrices into a parameter vector (ensuring that their column-normalization is preserved) and calculating the negative log-likelihood of a particular parameter vector. In practice, given a set of observations, we can initialize an `analyzer` and run either local (using, by default, the `scipy.opt.minimize` function with the `L-BFGS-B` algorithm) or global (using the `scipy` SHGO algorithm) as:
+
+```python
+from hidden_py import infer
+
+# Input the dimensions of the HMM and observations
+analyzer = infer.MarkovInfer(2, 2)
+
+# Initial estimates of the A and B matrices
+A_est = np.array([
+    [0.8, 0.1],
+    [0.2, 0.9]
+])
+
+B_est = np.array([
+    [0.9, 0.05],
+    [0.1, 0.95]
+])
+
+# Run local partial-data likelihood optimization (default behaviour), the symmetric keyword can be used to specify whether or not the A and B matrices are assumed to be symmetric
+opt_local = analyzer.optimize(observations, A_est, B_est, symmetric=False)
+
+# And the partial-data global likelihood optimization, the A and B initial matrices are not used in the optimizer, aside from providing a way of specifying the dimension of the parameter vectors
+opt_global = analyzer.optimize(observations, A_est, B_est, symmetric=False, opt_type=OptClass.Global)
+
+```
+
+Now, for the complete-data likeihood optimization, the interface is very similar, but behind the scenes the code will implement an implementation of the Baum-Welch reparameterization algorithm (an instance of an Expectation-Maximization algorithm) to find the optimal parameter values. In practice, this can be done as:
+
+```python
+from hidden_py import infer
+from hidden_py.optimize.base import OptClass
+
+analyzer = infer.MarkovInfer(2, 2)
+
+res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax)
+
+```
+
+In all cases, there is also an option to add algorithm options to customize the specifics of the optinization. Most relevant is for the expectation-maximization where you can specify a maximum number of iterations for the algorithm, as well as a threshold on the size of parameter changes (quantified by the matrix norm of pre- and post-update $A$ and $B$ matrices). This can be accessed through the `algo_opts` dictionary. For instance, if we wanted to change the maximum iterations in the BW algorithm to 1000 and set the termination threshold at `1e-10`, we would perform the previous call as
+
+```python
+options = {
+    'maxiter': 1000,
+    "threshold": 1e-10
+}
+
+res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax, algo_opts=options)
+```
+
+In essence, this set of tools allows you to infer the best model given a set of observed data. Under the hood, many of the tools from the signal processing module are used, but the `analyzer.optimize(...)` function calls largely hide that complexity.
+
+<br />
+
+---
+
+### Signal Processing
+
+The `infer` submodule can also be used for the purposes of signal processing: given a valid estimate of the model parameters, how can we best estimate the hidden state value, given the observations. There are two distinct domains of application, first would be prediction in real time, where only observations in the past are available for inferring the current hidden state (this would use the so-called forward-filtered estiamte). There is also an _ex post_ approach, which uses the entirety of observations from a given period of time to estimate the hidden state at a particular point within that time period. This is the so-called Bayesian smoothed estiamte of the hidden state.
+
+Mathematically, if we denote $Y^t \equiv \{ y_0, y_1, \cdots, y_t \}$ as the sequence of observations from tie $t=0$ up to time $t$, then for a total trajectory length of $T$, the forward filter and Bayesian smoothed estimate are calculating
+
+$$
+p(x_t | Y^t) \quad \to \qquad \text{\sf Forward-filter} \\
+
+\, \\
+
+p(x_t | Y^T) \quad \to \quad \text{\sf Bayesian smoother}
+$$
+
+where, $x_t$ is the hidden state at time $t$.
+
+Quantitatively the forward filter and Bayesian smoothed estimates of a given HMM sequence of observations can be calculated in the following way:
+
+```python
+from hidden_py import infer
+
+analyzer = infer.MarkovInfer(2, 2)
+
+# Gets the forward algorithm results
+analyzer.forward_algo(observations, A, B)
+
+# Gets the Bayesian-smoothed estimate of the hidden state
+analyzer.bayesian_smooth(observations, A, B)
+
+```
+
+The tutorial notebook `notebooks/tutorials.03-slarge-hmm-filters.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) gives a more comprehensive overview and visualization of this procedure.
+
+<br />
+
+---
+
+## References
+
+There is a breadth of research and literatur on HMMs out in the world, but below are a few sources that I found particularly helpful in working on this project
+
+<ol>
+    <li> <a href="https://www.cambridge.org/core/books/control-theory-for-physicists/21AFE5D6C475D1B44BCF9B8536338D98">"Control Theory for Physicists"</a>, J. Bechhoeffer, C
+    Cambridge University Press, 2021</li>
+    <li><a href="http://numerical.recipes/aboutNR3book.html">"Numerical Recipes: The Art of Scientific Computing"</a>, W.H. Press, S.A. Teukolsky, W.T. Vetterling, & B.P. Flannery, Cambridge University Press, 3rd ed., 2007</li>
+</ol>
```

### Comparing `hidden-py-1.0.5/README.md` & `hidden-py-1.0.6/hidden_py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,196 +1,214 @@
-# **A Hidden Markov Model package for python**
-
-### Installation
-
-To install this package simply run the command:
-
-`pip install hidden-py`
-
-<br />
-
-## Table of Contents
-
-- [Overview](#overview)
-  - [Dynamics/Simulation](#dynamicssimulation)
-  - [System Identification](#system-identification)
-  - [Signal Processing](#signal-processing)
-- [Roadmap](#roadmap)
-- [References](#references)
-
----
-
-## Overview
-
-This package contains logic for inferring, simulating, and fitting Hidden Markov Models with discrete states and observations. This poackage serves as a complement to several common HMM packages that deal primarily with _mixture models_, where output symbols are continuous, and drawn from a distriubtion of values that is somehow conditional on the hidden state.
-
-Here, we have considered primarily scenarios where the observation value is an integer, and one of the possible hidden states, although this is not required, there could be more hidden states than possible observations, or vice-versa, all that really matters is that the observation values (and hidden state values) are discrete. There are three major use-cases for this codebase: dynamics/simulation, system identification/parameter fitting, and signal processing. In all cases, these functionalities are outlined in several tutorial notebooks in the `notebooks/tutorials` location of the [github repository](https://github.com/StevenJLarge/hmm)
-
-<br />
-
-## Hidden Markov Models
-
-Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
-
-Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
-
-<p align='center'>
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true" width="75%" vspace="30px"/>
-</p>
-
-Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step. For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
-
-$$ p_T = A^T \cdot p_0 $$
-
-A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
-
-<p align="center">
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true" width="75%" vspace="30px" />
-</p>
-
-Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
-
----
-
-As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
-
-### Dynamics/Simulation
-
-The `hidden.dynamics` submodule contains the code necessary to simulate the hidden state and observation dynamics as specified by a state transition matrix $A$ (with elements that quantify the rate of transitions between states) and an observation matrix $B$, with elements that quantify the probability of observing a given output symbol, given the current hidden state.
-
-For instance, the code necessary to initialize a hidden Markov model, run the dyanamics, and extract the observation and state time-series
-
-```python
-from hidden_py import dynamics
-
-# 2 hidden states, 2 possible observation values
-hmm = dynamics.HMM(2, 2)
-
-# Helper routine to initialize A and B matrices
-hmm.init_uniform_cycle()
-
-# Run dynamics for 100 time steps
-hmm.run_dynamics(100)
-
-# Pull out the observations, and true (simulated) hidden state values
-observations = hmm.get_obs_ts()
-hidden_states = hmm.get_state_ts()
-```
-
-As an example, the schematic below shows a possible trajectory for a HMM with 2 hidden states and 2 possible observation values.
-
-<p align="center">
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/sample_trajectory.png?raw=true" width="75%" vspace="30px" />
-</p>
-
-Here the red dots represent the state of the hidden system over time, while the black dots indicate the observed value at that point in time. So, at time point 3, for instance, the observed value differs from the hidden state. See the `notebooks/tutorials/02-hidden-markov-model.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) for a more in-depth review of this process.
-
-<br />
-
----
-
-### System Identification
-
-The `infer` submodule contains the code that wraps lower-level functionality (primarily in the `filters/bayesian.py` and `optimize/optimization.py` files) for both signal processing and system identification/parameter fitting.
-
-There are two separate means of performing system identification: Local/Global partial likelihood optimization, and complete-data likelihood optimization. While more comprehensive details are contained in the github notebooks, broadly speaking partial data likelihood optimization performs relatively standard optimizations on the likelihood function $\mathcal{L}(\theta | Y)$ which considers only the observations as the _data_. Effectively, these optimizers wrap the `scipy.opt.minimize` functions by encoding and decoding the $A$ and $B$ matrices into a parameter vector (ensuring that their column-normalization is preserved) and calculating the negative log-likelihood of a particular parameter vector. In practice, given a set of observations, we can initialize an `analyzer` and run either local (using, by default, the `scipy.opt.minimize` function with the `L-BFGS-B` algorithm) or global (using the `scipy` SHGO algorithm) as:
-
-```python
-from hidden_py import infer
-
-# Input the dimensions of the HMM and observations
-analyzer = infer.MarkovInfer(2, 2)
-
-# Initial estimates of the A and B matrices
-A_est = np.array([
-    [0.8, 0.1],
-    [0.2, 0.9]
-])
-
-B_est = np.array([
-    [0.9, 0.05],
-    [0.1, 0.95]
-])
-
-# Run local partial-data likelihood optimization (default behaviour), the symmetric keyword can be used to specify whether or not the A and B matrices are assumed to be symmetric
-opt_local = analyzer.optimize(observations, A_est, B_est, symmetric=False)
-
-# And the partial-data global likelihood optimization, the A and B initial matrices are not used in the optimizer, aside from providing a way of specifying the dimension of the parameter vectors
-opt_global = analyzer.optimize(observations, A_est, B_est, symmetric=False, opt_type=OptClass.Global)
-
-```
-
-Now, for the complete-data likeihood optimization, the interface is very similar, but behind the scenes the code will implement an implementation of the Baum-Welch reparameterization algorithm (an instance of an Expectation-Maximization algorithm) to find the optimal parameter values. In practice, this can be done as:
-
-```python
-from hidden_py import infer
-from hidden_py.optimize.base import OptClass
-
-analyzer = infer.MarkovInfer(2, 2)
-
-res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax)
-
-```
-
-In all cases, there is also an option to add algorithm options to customize the specifics of the optinization. Most relevant is for the expectation-maximization where you can specify a maximum number of iterations for the algorithm, as well as a threshold on the size of parameter changes (quantified by the matrix norm of pre- and post-update $A$ and $B$ matrices). This can be accessed through the `algo_opts` dictionary. For instance, if we wanted to change the maximum iterations in the BW algorithm to 1000 and set the termination threshold at `1e-10`, we would perform the previous call as
-
-```python
-options = {
-    'maxiter': 1000,
-    "threshold": 1e-10
-}
-
-res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax, algo_opts=options)
-```
-
-In essence, this set of tools allows you to infer the best model given a set of observed data. Under the hood, many of the tools from the signal processing module are used, but the `analyzer.optimize(...)` function calls largely hide that complexity.
-
-<br />
-
----
-
-### Signal Processing
-
-The `infer` submodule can also be used for the purposes of signal processing: given a valid estimate of the model parameters, how can we best estimate the hidden state value, given the observations. There are two distinct domains of application, first would be prediction in real time, where only observations in the past are available for inferring the current hidden state (this would use the so-called forward-filtered estiamte). There is also an _ex post_ approach, which uses the entirety of observations from a given period of time to estimate the hidden state at a particular point within that time period. This is the so-called Bayesian smoothed estiamte of the hidden state.
-
-Mathematically, if we denote $Y^t \equiv \{ y_0, y_1, \cdots, y_t \}$ as the sequence of observations from tie $t=0$ up to time $t$, then for a total trajectory length of $T$, the forward filter and Bayesian smoothed estimate are calculating
-
-$$
-p(x_t | Y^t) \quad \to \qquad \text{\sf Forward-filter} \\
-
-\, \\
-
-p(x_t | Y^T) \quad \to \quad \text{\sf Bayesian smoother}
-$$
-
-where, $x_t$ is the hidden state at time $t$.
-
-Quantitatively the forward filter and Bayesian smoothed estimates of a given HMM sequence of observations can be calculated in the following way:
-
-```python
-from hidden_py import infer
-
-analyzer = infer.MarkovInfer(2, 2)
-
-# Gets the forward algorithm results
-analyzer.forward_algo(observations, A, B)
-
-# Gets the Bayesian-smoothed estimate of the hidden state
-analyzer.bayesian_smooth(observations, A, B)
-
-```
-
-The tutorial notebook `notebooks/tutorials.03-slarge-hmm-filters.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) gives a more comprehensive overview and visualization of this procedure.
-
-<br />
-
----
-
-## References
-
-There is a breadth of research and literatur on HMMs out in the world, but below are a few sources that I found particularly helpful in working on this project
-
-<ol>
-    <li> <a href="https://www.cambridge.org/core/books/control-theory-for-physicists/21AFE5D6C475D1B44BCF9B8536338D98">"Control Theory for Physicists"</a>, J. Bechhoeffer, C
-    Cambridge University Press, 2021</li>
-    <li><a href="http://numerical.recipes/aboutNR3book.html">"Numerical Recipes: The Art of Scientific Computing"</a>, W.H. Press, S.A. Teukolsky, W.T. Vetterling, & B.P. Flannery, Cambridge University Press, 3rd ed., 2007</li>
-</ol>
+Metadata-Version: 2.1
+Name: hidden-py
+Version: 1.0.6
+Summary: A python package for discrete-output hidden Markov models
+Author: Steven Large
+Author-email: stevelarge7@gmail.com
+License: MIT
+Project-URL: Source, https://github.com/StevenJLarge/hmm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# **A Hidden Markov Model package for python**
+
+### Installation
+
+To install this package simply run the command:
+
+`pip install hidden-py`
+
+<br />
+
+## Table of Contents
+
+- [Overview](#overview)
+  - [Dynamics/Simulation](#dynamicssimulation)
+  - [System Identification](#system-identification)
+  - [Signal Processing](#signal-processing)
+- [Roadmap](#roadmap)
+- [References](#references)
+
+---
+
+## Overview
+
+This package contains logic for inferring, simulating, and fitting Hidden Markov Models with discrete states and observations. This poackage serves as a complement to several common HMM packages that deal primarily with _mixture models_, where output symbols are continuous, and drawn from a distriubtion of values that is somehow conditional on the hidden state.
+
+Here, we have considered primarily scenarios where the observation value is an integer, and one of the possible hidden states, although this is not required, there could be more hidden states than possible observations, or vice-versa, all that really matters is that the observation values (and hidden state values) are discrete. There are three major use-cases for this codebase: dynamics/simulation, system identification/parameter fitting, and signal processing. In all cases, these functionalities are outlined in several tutorial notebooks in the `notebooks/tutorials` location of the [github repository](https://github.com/StevenJLarge/hmm)
+
+<br />
+
+## Hidden Markov Models
+
+Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
+
+Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
+
+<p align='center'>
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true" width="75%" vspace="30px"/>
+</p>
+
+Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step. For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
+
+$$ p_T = A^T \cdot p_0 $$
+
+A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
+
+<p align="center">
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true" width="75%" vspace="30px" />
+</p>
+
+Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
+
+---
+
+As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
+
+### Dynamics/Simulation
+
+The `hidden.dynamics` submodule contains the code necessary to simulate the hidden state and observation dynamics as specified by a state transition matrix $A$ (with elements that quantify the rate of transitions between states) and an observation matrix $B$, with elements that quantify the probability of observing a given output symbol, given the current hidden state.
+
+For instance, the code necessary to initialize a hidden Markov model, run the dyanamics, and extract the observation and state time-series
+
+```python
+from hidden_py import dynamics
+
+# 2 hidden states, 2 possible observation values
+hmm = dynamics.HMM(2, 2)
+
+# Helper routine to initialize A and B matrices
+hmm.init_uniform_cycle()
+
+# Run dynamics for 100 time steps
+hmm.run_dynamics(100)
+
+# Pull out the observations, and true (simulated) hidden state values
+observations = hmm.get_obs_ts()
+hidden_states = hmm.get_state_ts()
+```
+
+As an example, the schematic below shows a possible trajectory for a HMM with 2 hidden states and 2 possible observation values.
+
+<p align="center">
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/sample_trajectory.png?raw=true" width="75%" vspace="30px" />
+</p>
+
+Here the red dots represent the state of the hidden system over time, while the black dots indicate the observed value at that point in time. So, at time point 3, for instance, the observed value differs from the hidden state. See the `notebooks/tutorials/02-hidden-markov-model.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) for a more in-depth review of this process.
+
+<br />
+
+---
+
+### System Identification
+
+The `infer` submodule contains the code that wraps lower-level functionality (primarily in the `filters/bayesian.py` and `optimize/optimization.py` files) for both signal processing and system identification/parameter fitting.
+
+There are two separate means of performing system identification: Local/Global partial likelihood optimization, and complete-data likelihood optimization. While more comprehensive details are contained in the github notebooks, broadly speaking partial data likelihood optimization performs relatively standard optimizations on the likelihood function $\mathcal{L}(\theta | Y)$ which considers only the observations as the _data_. Effectively, these optimizers wrap the `scipy.opt.minimize` functions by encoding and decoding the $A$ and $B$ matrices into a parameter vector (ensuring that their column-normalization is preserved) and calculating the negative log-likelihood of a particular parameter vector. In practice, given a set of observations, we can initialize an `analyzer` and run either local (using, by default, the `scipy.opt.minimize` function with the `L-BFGS-B` algorithm) or global (using the `scipy` SHGO algorithm) as:
+
+```python
+from hidden_py import infer
+
+# Input the dimensions of the HMM and observations
+analyzer = infer.MarkovInfer(2, 2)
+
+# Initial estimates of the A and B matrices
+A_est = np.array([
+    [0.8, 0.1],
+    [0.2, 0.9]
+])
+
+B_est = np.array([
+    [0.9, 0.05],
+    [0.1, 0.95]
+])
+
+# Run local partial-data likelihood optimization (default behaviour), the symmetric keyword can be used to specify whether or not the A and B matrices are assumed to be symmetric
+opt_local = analyzer.optimize(observations, A_est, B_est, symmetric=False)
+
+# And the partial-data global likelihood optimization, the A and B initial matrices are not used in the optimizer, aside from providing a way of specifying the dimension of the parameter vectors
+opt_global = analyzer.optimize(observations, A_est, B_est, symmetric=False, opt_type=OptClass.Global)
+
+```
+
+Now, for the complete-data likeihood optimization, the interface is very similar, but behind the scenes the code will implement an implementation of the Baum-Welch reparameterization algorithm (an instance of an Expectation-Maximization algorithm) to find the optimal parameter values. In practice, this can be done as:
+
+```python
+from hidden_py import infer
+from hidden_py.optimize.base import OptClass
+
+analyzer = infer.MarkovInfer(2, 2)
+
+res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax)
+
+```
+
+In all cases, there is also an option to add algorithm options to customize the specifics of the optinization. Most relevant is for the expectation-maximization where you can specify a maximum number of iterations for the algorithm, as well as a threshold on the size of parameter changes (quantified by the matrix norm of pre- and post-update $A$ and $B$ matrices). This can be accessed through the `algo_opts` dictionary. For instance, if we wanted to change the maximum iterations in the BW algorithm to 1000 and set the termination threshold at `1e-10`, we would perform the previous call as
+
+```python
+options = {
+    'maxiter': 1000,
+    "threshold": 1e-10
+}
+
+res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax, algo_opts=options)
+```
+
+In essence, this set of tools allows you to infer the best model given a set of observed data. Under the hood, many of the tools from the signal processing module are used, but the `analyzer.optimize(...)` function calls largely hide that complexity.
+
+<br />
+
+---
+
+### Signal Processing
+
+The `infer` submodule can also be used for the purposes of signal processing: given a valid estimate of the model parameters, how can we best estimate the hidden state value, given the observations. There are two distinct domains of application, first would be prediction in real time, where only observations in the past are available for inferring the current hidden state (this would use the so-called forward-filtered estiamte). There is also an _ex post_ approach, which uses the entirety of observations from a given period of time to estimate the hidden state at a particular point within that time period. This is the so-called Bayesian smoothed estiamte of the hidden state.
+
+Mathematically, if we denote $Y^t \equiv \{ y_0, y_1, \cdots, y_t \}$ as the sequence of observations from tie $t=0$ up to time $t$, then for a total trajectory length of $T$, the forward filter and Bayesian smoothed estimate are calculating
+
+$$
+p(x_t | Y^t) \quad \to \qquad \text{\sf Forward-filter} \\
+
+\, \\
+
+p(x_t | Y^T) \quad \to \quad \text{\sf Bayesian smoother}
+$$
+
+where, $x_t$ is the hidden state at time $t$.
+
+Quantitatively the forward filter and Bayesian smoothed estimates of a given HMM sequence of observations can be calculated in the following way:
+
+```python
+from hidden_py import infer
+
+analyzer = infer.MarkovInfer(2, 2)
+
+# Gets the forward algorithm results
+analyzer.forward_algo(observations, A, B)
+
+# Gets the Bayesian-smoothed estimate of the hidden state
+analyzer.bayesian_smooth(observations, A, B)
+
+```
+
+The tutorial notebook `notebooks/tutorials.03-slarge-hmm-filters.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) gives a more comprehensive overview and visualization of this procedure.
+
+<br />
+
+---
+
+## References
+
+There is a breadth of research and literatur on HMMs out in the world, but below are a few sources that I found particularly helpful in working on this project
+
+<ol>
+    <li> <a href="https://www.cambridge.org/core/books/control-theory-for-physicists/21AFE5D6C475D1B44BCF9B8536338D98">"Control Theory for Physicists"</a>, J. Bechhoeffer, C
+    Cambridge University Press, 2021</li>
+    <li><a href="http://numerical.recipes/aboutNR3book.html">"Numerical Recipes: The Art of Scientific Computing"</a>, W.H. Press, S.A. Teukolsky, W.T. Vetterling, & B.P. Flannery, Cambridge University Press, 3rd ed., 2007</li>
+</ol>
```

### Comparing `hidden-py-1.0.5/hidden_py/dynamics.py` & `hidden-py-1.0.6/hidden_py/dynamics.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-import numpy as np
-from typing import Iterable, Optional
-
-
-class HMM:
-    def __init__(self, dim_sys: int, dim_obs: int):
-        # Initialize the bayesian filter to the initial observation
-        self.n_sys = dim_sys
-        self.n_obs = dim_obs
-
-        self.A = np.zeros((self.n_sys, self.n_sys))
-        self.B = np.zeros((self.n_obs, self.n_sys))
-
-        self.state_tracker = None
-        self.obs_tracker = None
-
-    def _initialize_tracking(self):
-        self.state_tracker = []
-        self.obs_tracker = []
-
-    def initialize_dynamics(self, A: np.ndarray, B: np.ndarray):
-        self.A = A
-        self.B = B
-
-    def init_uniform_cycle(
-        self, trans_rate: Optional[int] = 0.3,
-        error_rate: Optional[int] = 0.1
-    ):
-        # NOTE This routine assumes that the observation matrix dimension
-        # is equal to the transitionmatrix dimension
-        if self.n_sys != self.n_obs:
-            raise NotImplementedError(
-                "Currently, cycle default matrices can only be instantiated "
-                "when `n_sys` = `n_obs`"
-            )
-        self.A = np.zeros((self.n_sys, self.n_sys))
-        self.B = np.zeros((self.n_sys, self.n_sys))
-
-        # NOTE that this assumes a symmetric cycle (fwd rate = back-rate)
-        for i in range(self.n_sys):
-            for j in range(i + 1, self.n_sys):
-                self.A[i, j] = (lambda x: trans_rate if x == 1 else 0)(np.abs(i - j))
-                self.A[j, i] = self.A[i, j]
-            # For PBCs
-            if i == 0: self.A[self.n_sys - 1, i] = trans_rate
-            if i == self.n_sys - 1: self.A[0, i] = trans_rate
-
-            self.A[i, i] = 1 - np.sum(self.A[:, i])
-
-        for i in range(self.n_obs):
-            for j in range(i + 1, self.n_obs):
-                self.B[i, j] = (lambda x: error_rate if x == 1 else 0)(np.abs(i - j))
-                self.B[j, i] = self.B[i, j]
-            # For PBCs
-            if i == 0: self.B[self.n_obs - 1, i] = error_rate
-            if i == self.n_obs - 1: self.B[0, i] = error_rate
-
-            self.B[i, i] = 1 - np.sum(self.B[:, i])
-
-    def _validate_dynamics_matrices(self):
-        A_condition = self.A.sum(axis=0)
-        B_condition = self.B.sum(axis=0)
-
-        if not (A_condition == 1).all():
-            raise ValueError(
-                f"Invalid transition matrix A : {self.A}"
-            )
-        if  not (B_condition == 1).all():
-            raise ValueError(
-                f"Invalid observation matrix B : {self.B}"
-            )
-
-    # Dynamics routines
-    def run_dynamics(
-        self, n_steps: Optional[int] = 100, init_state: Optional[int] = None
-    ):
-        self._validate_dynamics_matrices()
-
-        if init_state is None:
-            self._set_state(np.random.randint(0, self.n_sys))
-        else:
-            self._set_state(init_state)
-
-        self._set_obs(np.argmax(self.state))
-
-        if self.state_tracker is None or self.obs_tracker is None:
-            self._initialize_tracking()
-
-        for _ in range(n_steps):
-            self.state_tracker.append(self.state)
-            self.obs_tracker.append(self.obs)
-            self.step_dynamics()
-
-    def step_dynamics(self):
-        # Kinetic monte-carlo dynamics
-        w_sys = np.random.uniform()
-        w_obs = np.random.uniform()
-
-        trans_prob = self.A[:, np.argmax(self.state)]
-        new_sys = np.argmax(w_sys < np.cumsum(trans_prob))
-        self._set_state(new_sys)
-
-        obs_prob = self.B[:, np.argmax(self.state)]
-        new_obs = np.argmax(w_obs < np.cumsum(obs_prob))
-        self._set_obs(new_obs)
-
-    def _set_state(self, new_state):
-        if new_state < 0 or new_state > self.n_sys:
-            raise IndexError(
-                f"New state `{new_state}` out of bounds for system of "
-                f"dimension `{self.n_sys}`"
-            )
-        self.state = np.zeros(self.n_sys)
-        self.state[new_state] = 1
-
-    def _set_obs(self, new_obs):
-        if new_obs < 0 or new_obs > self.n_obs:
-            raise IndexError(
-                f"New observation `{new_obs}` out of bounds for system with "
-                f"dimension `{self.n_obs}`"
-            )
-        self.obs = np.zeros(self.n_obs)
-        self.obs[new_obs] = 1
-
-    def get_state_ts(self):
-        return [np.argmax(s) for s in self.state_tracker]
-
-    def get_obs_ts(self):
-        return [np.argmax(o) for o in self.obs_tracker]
-
-    @property
-    def current_state(self):
-        return self.state
-
-    @property
-    def current_obs(self):
-        return self.obs
-
-    @property
-    def steady_state(self):
-        e_vals, e_vecs = np.linalg.eig(self.A)
-        ss_idx = np.argmin(np.abs(1 - e_vals))
-        return e_vecs[:, ss_idx] / np.sum(e_vecs[:, ss_idx])
-
-
-def plot_traj(state: Iterable, observation: Iterable):
-    import matplotlib.pyplot as plt
-    import seaborn as sns
-    sns.set(style='darkgrid')
-    Pal = sns.color_palette('hls', 2)
-
-    _, ax = plt.subplots(1, 1, figsize=(6, 3.5))
-
-    ax.plot(state, 'o', markersize=7, color=Pal[0], label='State')
-    ax.plot(observation, 'o', markersize=4, color=Pal[1], label='Observation')
-    ax.set_xlabel(r"Time", fontsize=15)
-    ax.set_ylabel(r"State", fontsize=15)
-    ax.legend(fontsize=12)
-
-    plt.tight_layout()
-    plt.show()
-    plt.close()
-
-
-if __name__ == "__main__":
-
-    # Setup
-    obj = HMM(3, 3)
-    obj.init_uniform_cycle(0.1)
-
-    # Generate synthetic dynamics:
-    obj.run_dynamics(n_steps=25)
-    state = obj.get_state_ts()
-    obs = obj.get_obs_ts()
-
-    plot_traj(state, obs)
-
+import numpy as np
+from typing import Iterable, Optional
+
+
+class HMM:
+    def __init__(self, dim_sys: int, dim_obs: int):
+        # Initialize the bayesian filter to the initial observation
+        self.n_sys = dim_sys
+        self.n_obs = dim_obs
+
+        self.A = np.zeros((self.n_sys, self.n_sys))
+        self.B = np.zeros((self.n_obs, self.n_sys))
+
+        self.state_tracker = None
+        self.obs_tracker = None
+
+    def _initialize_tracking(self):
+        self.state_tracker = []
+        self.obs_tracker = []
+
+    def initialize_dynamics(self, A: np.ndarray, B: np.ndarray):
+        self.A = A
+        self.B = B
+
+    def init_uniform_cycle(
+        self, trans_rate: Optional[int] = 0.3,
+        error_rate: Optional[int] = 0.1
+    ):
+        # NOTE This routine assumes that the observation matrix dimension
+        # is equal to the transitionmatrix dimension
+        if self.n_sys != self.n_obs:
+            raise NotImplementedError(
+                "Currently, cycle default matrices can only be instantiated "
+                "when `n_sys` = `n_obs`"
+            )
+        self.A = np.zeros((self.n_sys, self.n_sys))
+        self.B = np.zeros((self.n_sys, self.n_sys))
+
+        # NOTE that this assumes a symmetric cycle (fwd rate = back-rate)
+        for i in range(self.n_sys):
+            for j in range(i + 1, self.n_sys):
+                self.A[i, j] = (lambda x: trans_rate if x == 1 else 0)(np.abs(i - j))
+                self.A[j, i] = self.A[i, j]
+            # For PBCs
+            if i == 0: self.A[self.n_sys - 1, i] = trans_rate
+            if i == self.n_sys - 1: self.A[0, i] = trans_rate
+
+            self.A[i, i] = 1 - np.sum(self.A[:, i])
+
+        for i in range(self.n_obs):
+            for j in range(i + 1, self.n_obs):
+                self.B[i, j] = (lambda x: error_rate if x == 1 else 0)(np.abs(i - j))
+                self.B[j, i] = self.B[i, j]
+            # For PBCs
+            if i == 0: self.B[self.n_obs - 1, i] = error_rate
+            if i == self.n_obs - 1: self.B[0, i] = error_rate
+
+            self.B[i, i] = 1 - np.sum(self.B[:, i])
+
+    def _validate_dynamics_matrices(self):
+        A_condition = self.A.sum(axis=0)
+        B_condition = self.B.sum(axis=0)
+
+        if not (A_condition == 1).all():
+            raise ValueError(
+                f"Invalid transition matrix A : {self.A}"
+            )
+        if  not (B_condition == 1).all():
+            raise ValueError(
+                f"Invalid observation matrix B : {self.B}"
+            )
+
+    # Dynamics routines
+    def run_dynamics(
+        self, n_steps: Optional[int] = 100, init_state: Optional[int] = None
+    ):
+        self._validate_dynamics_matrices()
+
+        if init_state is None:
+            self._set_state(np.random.randint(0, self.n_sys))
+        else:
+            self._set_state(init_state)
+
+        self._set_obs(np.argmax(self.state))
+
+        if self.state_tracker is None or self.obs_tracker is None:
+            self._initialize_tracking()
+
+        for _ in range(n_steps):
+            self.state_tracker.append(self.state)
+            self.obs_tracker.append(self.obs)
+            self.step_dynamics()
+
+    def step_dynamics(self):
+        # Kinetic monte-carlo dynamics
+        w_sys = np.random.uniform()
+        w_obs = np.random.uniform()
+
+        trans_prob = self.A[:, np.argmax(self.state)]
+        new_sys = np.argmax(w_sys < np.cumsum(trans_prob))
+        self._set_state(new_sys)
+
+        obs_prob = self.B[:, np.argmax(self.state)]
+        new_obs = np.argmax(w_obs < np.cumsum(obs_prob))
+        self._set_obs(new_obs)
+
+    def _set_state(self, new_state):
+        if new_state < 0 or new_state > self.n_sys:
+            raise IndexError(
+                f"New state `{new_state}` out of bounds for system of "
+                f"dimension `{self.n_sys}`"
+            )
+        self.state = np.zeros(self.n_sys)
+        self.state[new_state] = 1
+
+    def _set_obs(self, new_obs):
+        if new_obs < 0 or new_obs > self.n_obs:
+            raise IndexError(
+                f"New observation `{new_obs}` out of bounds for system with "
+                f"dimension `{self.n_obs}`"
+            )
+        self.obs = np.zeros(self.n_obs)
+        self.obs[new_obs] = 1
+
+    def get_state_ts(self):
+        return [np.argmax(s) for s in self.state_tracker]
+
+    def get_obs_ts(self):
+        return [np.argmax(o) for o in self.obs_tracker]
+
+    @property
+    def current_state(self):
+        return self.state
+
+    @property
+    def current_obs(self):
+        return self.obs
+
+    @property
+    def steady_state(self):
+        e_vals, e_vecs = np.linalg.eig(self.A)
+        ss_idx = np.argmin(np.abs(1 - e_vals))
+        return e_vecs[:, ss_idx] / np.sum(e_vecs[:, ss_idx])
+
+
+def plot_traj(state: Iterable, observation: Iterable):
+    import matplotlib.pyplot as plt
+    import seaborn as sns
+    sns.set(style='darkgrid')
+    Pal = sns.color_palette('hls', 2)
+
+    _, ax = plt.subplots(1, 1, figsize=(6, 3.5))
+
+    ax.plot(state, 'o', markersize=7, color=Pal[0], label='State')
+    ax.plot(observation, 'o', markersize=4, color=Pal[1], label='Observation')
+    ax.set_xlabel(r"Time", fontsize=15)
+    ax.set_ylabel(r"State", fontsize=15)
+    ax.legend(fontsize=12)
+
+    plt.tight_layout()
+    plt.show()
+    plt.close()
+
+
+if __name__ == "__main__":
+
+    # Setup
+    obj = HMM(3, 3)
+    obj.init_uniform_cycle(0.1)
+
+    # Generate synthetic dynamics:
+    obj.run_dynamics(n_steps=25)
+    state = obj.get_state_ts()
+    obs = obj.get_obs_ts()
+
+    plot_traj(state, obs)
+
```

### Comparing `hidden-py-1.0.5/hidden_py/filters/bayesian.py` & `hidden-py-1.0.6/hidden_py/filters/bayesian.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,263 +1,263 @@
-# Bayesian filters -- Fowrward, backward, bayesian
-from typing import Iterable, Tuple, Optional
-import numpy as np
-import numba
-
-
-@numba.jit(nopython=True)
-def bayes_estimate(
-    obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray
-) -> np.ndarray:
-    """Implementation of Bayesian 'smoothing' algoithm. This calcualted the
-    probability distribution p(x | Y^T), conditioned on both past and future
-    informaton
-
-    Args:
-        obs_ts (np.ndarray): sequence of observations
-        trans_matrix (np.ndarray): hidden state transition rate matrix
-        obs_matrix (np.ndarray): observation/emmision probability matrix
-
-    Returns:
-        np.ndarray: array with each row representing the inferred probability
-        distribution over individual states
-    """
-    fwd_tracker, pred = forward_algo(obs_ts, trans_matrix, obs_matrix)
-
-    bayes_smooth = np.zeros((len(obs_ts), trans_matrix.shape[1]), dtype=float)
-    bayes_smooth[-1, :] = fwd_tracker[-1, :]
-    ratio = np.zeros(trans_matrix.shape)
-
-    # Iterate backwards through the forward tracker from N-1 -> 1
-    for i in range(fwd_tracker.shape[0] - 1, 0, -1):
-        # Ratio of previous bayesian estimates to forward predictions, shaped
-        # to match trans_matrix shape
-        ratio[:, :] = (bayes_smooth[i, :] / pred[i, :]).reshape(-1, 1)
-        # summation term
-        summand = np.sum(trans_matrix * ratio, axis=0)
-        # Smoothed bayesian estimate
-        bayes_smooth[i - 1, :] = fwd_tracker[i - 1, :] * summand
-
-    return bayes_smooth
-
-
-@numba.jit(nopython=True)
-def forward_algo(
-    observations: Iterable, trans_matrix: np.ndarray, obs_matrix: np.ndarray
-) -> Tuple[np.ndarray, np.ndarray]:
-    """Runs the forward bayesian filter calculations on an input set of
-    bservations (`observations`) based on input transition (`trans_matrix`)
-    and observation (`obs_matrix`) matrices.
-
-    Args:
-        observations (Iterable): Integer sequence of observed states
-        trans_matrix (np.ndarray): Matrix of transition probabilities
-        obs_matrix (np.ndarray): Matrix of observation probabilities
-
-    Returns:
-        Tuple[np.ndarray, np.ndarray]: Bayesian filtered state estimates,
-            Bayesian state predictions (middle-state of recursive Bayesian
-            update equations)
-    """
-    # initialize trackers so that single-observation slices will be
-    # contiguous in memory
-    fwd_track = np.zeros((len(observations), trans_matrix.shape[0]))
-    pred_track = np.zeros((len(observations), trans_matrix.shape[0]))
-    fwd_est = np.ones(trans_matrix.shape[0]) / trans_matrix.shape[0]
-
-    for i, obs in enumerate(observations):
-        fwd_est, pred = _forward_filter(obs, trans_matrix, obs_matrix, fwd_est)
-        fwd_track[i, :] = fwd_est
-        pred_track[i, :] = pred
-
-    return fwd_track, pred_track
-
-
-@numba.jit(nopython=True)
-def backward_algo(
-    observations: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray
-) -> Tuple[np.ndarray, np.ndarray]:
-    """Backwards algorithm, calcualtes the probability P(x | Y^[t: T]), that is,
-    the probability distribution over the current system states, given all of
-    the future observations that will occur.
-
-    Args:
-        observations (np.ndarray): forward-time sequence of opservations
-        trans_matrix (np.ndarray): hidden state transition matrix
-        obs_matrix (np.ndarray): observation/emmision probability matrix
-
-    Returns:
-        Tuple[np.ndarray, np.ndarray]: matrix with each row corresponding to
-        the inferred probability over states of the hidden system, conditioned
-        on all future observations, as well as a matrix of predictions of
-        probabilities
-    """
-    back_track = np.zeros((len(observations), trans_matrix.shape[0]))
-    pred_track = np.zeros((len(observations), trans_matrix.shape[0]))
-    back = np.ones(trans_matrix.shape[0]) / trans_matrix.shape[0]
-
-    for i, obs in enumerate(observations[::-1]):
-        back, pred = _forward_filter(
-            obs, trans_matrix.T, obs_matrix.T, back
-        )
-        back_track[i, :] = back
-        pred_track[i, :] = pred
-
-    return np.flipud(back_track), np.flipud(pred_track)
-
-
-@numba.jit(nopython=True)
-def _forward_filter(
-    obs: int, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
-    fwd_est: np.ndarray
-) -> Tuple[np.ndarray, np.ndarray]:
-    """Implementation of single-step of the Bayesian filter equations, used
-    to prtoduce a recursive/running estimate of the hidden state
-    probability, conditioned on the entire previous history of observations
-
-    Args:
-        obs (int): observation at time t
-        A (np.ndarray): transition probability matrix
-        B (np.ndarray): observation probability matrix
-        bayes_ (np.ndarray): Bayesian filtered estimate
-
-    Returns:
-        Tuple[np.ndarray, np.ndarray]: bayesian filter estimate, prediction
-    """
-    fwd_est = trans_matrix @ fwd_est
-    pred = fwd_est.copy()
-    fwd_est = obs_matrix[obs, :] * fwd_est
-    fwd_est /= np.sum(fwd_est)
-    return fwd_est, pred
-
-
-@numba.jit(nopython=True)
-def _backward_filter(
-    obs: int, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
-    back_est: np.ndarray
-) -> Tuple[np.ndarray, np.ndarray]:
-    """Implementation of single-step of the Bayesian backward filter equations,
-    used to produce a recursive/running estimate of the hidden state
-    probability, conditioned on the entire future history of observations
-
-    Args:
-        obs (int): observation at time t
-        A (np.ndarray): transition probability matrix
-        B (np.ndarray): observation probability matrix
-        back_est_ (np.ndarray): Bayesian filtered backwards estimate
-
-    Returns:
-        Tuple[np.ndarray, np.ndarray]: bayesian filter estimate, prediction
-    """
-    back_est = trans_matrix.T @ back_est
-    pred = back_est.copy()
-    back_est = obs_matrix[:, obs] * back_est
-    back_est /= np.sum(back_est)
-    return back_est, pred
-
-
-@numba.jit(nopython=True)
-def alpha_prob(
-    obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
-    norm: Optional[bool] = False
-) -> np.ndarray:
-    """routine to calculate the alpha function P(y^t | x_t ) for all obserations
-
-    Args:
-        obs_ts (np.ndarray): sequence of observations
-        trans_matrix (np.ndarray): transition rate matrix
-        obs_matrix (np.ndarray): observation/emission probability matrix
-
-    Returns:
-        np.ndarray: Matrix with each column corresponding to the alpha value
-        for each state, and each row representing the estimate at each point
-        in time
-    """
-    alpha_tracker = np.zeros((len(obs_ts), trans_matrix.shape[0]))
-    alpha = obs_matrix[:, obs_ts[0]].copy()
-    alpha_tracker[0, :] = alpha
-    for i, obs in enumerate(obs_ts[1:]):
-        alpha = (trans_matrix @ alpha) * obs_matrix[obs, :]
-        alpha_tracker[i + 1, :] = alpha
-    if norm:
-        alpha_tracker = (
-            alpha_tracker / np.repeat(
-                alpha_tracker
-                .sum(axis=1)
-                .reshape(-1, 1),
-                alpha_tracker.shape[1]
-            ).reshape(alpha_tracker.shape)
-        )
-
-    return alpha_tracker
-
-
-@numba.jit(nopython=True)
-def beta_prob(
-    obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
-    norm: Optional[bool] = False
-) -> np.ndarray:
-    """routine to calculate the beta function P(y^[t: T] | x_t ) for all obserations
-
-    Args:
-        obs_ts (np.ndarray): sequence of observations
-        trans_matrix (np.ndarray): transition rate matrix
-        obs_matrix (np.ndarray): observation/emission probability matrix
-
-    Returns:
-        np.ndarray: Matrix with each column corresponding to the beta value
-        for each state, and each row representing the estimate at each point
-        in time
-    """
-    beta_tracker = np.zeros((len(obs_ts), trans_matrix.shape[0]))
-    beta = np.ones(trans_matrix.shape[0])
-    beta_tracker[0, :] += beta
-    for i, obs in enumerate(obs_ts[-1:0:-1]):
-        beta = trans_matrix.T @ (beta * obs_matrix[:, obs])
-        beta_tracker[i + 1, :] = beta
-    if norm:
-        beta_tracker = (
-            beta_tracker / np.repeat(
-                beta_tracker
-                .sum(axis=1)
-                .reshape(-1, 1),
-                beta_tracker.shape[1]
-            ).reshape(beta_tracker.shape)
-        )
-    return beta_tracker[::-1]
-
-
-if __name__ == "__main__":
-    # test out the routines to make sure they all match
-    from hidden_py.infer import MarkovInfer
-    from hidden_py.dynamics import HMM
-    import time
-
-    hmm = HMM(2, 2)
-    hmm.init_uniform_cycle()
-
-    hmm.run_dynamics(5)
-    obs_ts, state_ts = hmm.get_obs_ts(), hmm.get_state_ts()
-
-    A_perturb = np.array([
-        [-0.05, 0.04],
-        [0.05, -0.04]
-    ])
-
-    A_sample = hmm.A + A_perturb
-    B_sample = hmm.B + A_perturb
-
-    analyzer = MarkovInfer(2, 2)
-
-    start_1 = time.time()
-    est_bayes_1 = bayes_estimate(np.array(obs_ts), A_sample, B_sample)
-    end_1 = time.time()
-
-    start_2 = time.time()
-    est_bayes_1 = bayes_estimate(np.array(obs_ts), A_sample, B_sample)
-    end_2 = time.time()
-
-    print("----- Timer results -----")
-    print(f"First iterations  : {end_1 - start_1}")
-    print(f"Second iterations : {end_2 - start_2}")
-
-    print("\n\t-- DONE --\n")
+# Bayesian filters -- Fowrward, backward, bayesian
+from typing import Iterable, Tuple, Optional
+import numpy as np
+import numba
+
+
+# @numba.jit(nopython=True)
+def bayes_estimate(
+    obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray
+) -> np.ndarray:
+    """Implementation of Bayesian 'smoothing' algoithm. This calcualted the
+    probability distribution p(x | Y^T), conditioned on both past and future
+    informaton
+
+    Args:
+        obs_ts (np.ndarray): sequence of observations
+        trans_matrix (np.ndarray): hidden state transition rate matrix
+        obs_matrix (np.ndarray): observation/emmision probability matrix
+
+    Returns:
+        np.ndarray: array with each row representing the inferred probability
+        distribution over individual states
+    """
+    fwd_tracker, pred = forward_algo(obs_ts, trans_matrix, obs_matrix)
+
+    bayes_smooth = np.zeros((len(obs_ts), trans_matrix.shape[1]), dtype=float)
+    bayes_smooth[-1, :] = fwd_tracker[-1, :]
+    ratio = np.zeros(trans_matrix.shape)
+
+    # Iterate backwards through the forward tracker from N-1 -> 1
+    for i in range(fwd_tracker.shape[0] - 1, 0, -1):
+        # Ratio of previous bayesian estimates to forward predictions, shaped
+        # to match trans_matrix shape
+        ratio[:, :] = (bayes_smooth[i, :] / pred[i, :]).reshape(-1, 1)
+        # summation term
+        summand = np.sum(trans_matrix * ratio, axis=0)
+        # Smoothed bayesian estimate
+        bayes_smooth[i - 1, :] = fwd_tracker[i - 1, :] * summand
+
+    return bayes_smooth
+
+
+# @numba.jit(nopython=True)
+def forward_algo(
+    observations: Iterable, trans_matrix: np.ndarray, obs_matrix: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Runs the forward bayesian filter calculations on an input set of
+    bservations (`observations`) based on input transition (`trans_matrix`)
+    and observation (`obs_matrix`) matrices.
+
+    Args:
+        observations (Iterable): Integer sequence of observed states
+        trans_matrix (np.ndarray): Matrix of transition probabilities
+        obs_matrix (np.ndarray): Matrix of observation probabilities
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: Bayesian filtered state estimates,
+            Bayesian state predictions (middle-state of recursive Bayesian
+            update equations)
+    """
+    # initialize trackers so that single-observation slices will be
+    # contiguous in memory
+    fwd_track = np.zeros((len(observations), trans_matrix.shape[0]))
+    pred_track = np.zeros((len(observations), trans_matrix.shape[0]))
+    fwd_est = np.ones(trans_matrix.shape[0]) / trans_matrix.shape[0]
+
+    for i, obs in enumerate(observations):
+        fwd_est, pred = _forward_filter(obs, trans_matrix, obs_matrix, fwd_est)
+        fwd_track[i, :] = fwd_est
+        pred_track[i, :] = pred
+
+    return fwd_track, pred_track
+
+
+# @numba.jit(nopython=True)
+def backward_algo(
+    observations: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Backwards algorithm, calcualtes the probability P(x | Y^[t: T]), that is,
+    the probability distribution over the current system states, given all of
+    the future observations that will occur.
+
+    Args:
+        observations (np.ndarray): forward-time sequence of opservations
+        trans_matrix (np.ndarray): hidden state transition matrix
+        obs_matrix (np.ndarray): observation/emmision probability matrix
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: matrix with each row corresponding to
+        the inferred probability over states of the hidden system, conditioned
+        on all future observations, as well as a matrix of predictions of
+        probabilities
+    """
+    back_track = np.zeros((len(observations), trans_matrix.shape[0]))
+    pred_track = np.zeros((len(observations), trans_matrix.shape[0]))
+    back = np.ones(trans_matrix.shape[0]) / trans_matrix.shape[0]
+
+    for i, obs in enumerate(observations[::-1]):
+        back, pred = _forward_filter(
+            obs, trans_matrix.T, obs_matrix.T, back
+        )
+        back_track[i, :] = back
+        pred_track[i, :] = pred
+
+    return np.flipud(back_track), np.flipud(pred_track)
+
+
+# @numba.jit(nopython=True)
+def _forward_filter(
+    obs: int, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
+    fwd_est: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Implementation of single-step of the Bayesian filter equations, used
+    to prtoduce a recursive/running estimate of the hidden state
+    probability, conditioned on the entire previous history of observations
+
+    Args:
+        obs (int): observation at time t
+        A (np.ndarray): transition probability matrix
+        B (np.ndarray): observation probability matrix
+        bayes_ (np.ndarray): Bayesian filtered estimate
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: bayesian filter estimate, prediction
+    """
+    fwd_est = trans_matrix @ fwd_est
+    pred = fwd_est.copy()
+    fwd_est = obs_matrix[obs, :] * fwd_est
+    fwd_est /= np.sum(fwd_est)
+    return fwd_est, pred
+
+
+# @numba.jit(nopython=True)
+def _backward_filter(
+    obs: int, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
+    back_est: np.ndarray
+) -> Tuple[np.ndarray, np.ndarray]:
+    """Implementation of single-step of the Bayesian backward filter equations,
+    used to produce a recursive/running estimate of the hidden state
+    probability, conditioned on the entire future history of observations
+
+    Args:
+        obs (int): observation at time t
+        A (np.ndarray): transition probability matrix
+        B (np.ndarray): observation probability matrix
+        back_est_ (np.ndarray): Bayesian filtered backwards estimate
+
+    Returns:
+        Tuple[np.ndarray, np.ndarray]: bayesian filter estimate, prediction
+    """
+    back_est = trans_matrix.T @ back_est
+    pred = back_est.copy()
+    back_est = obs_matrix[:, obs] * back_est
+    back_est /= np.sum(back_est)
+    return back_est, pred
+
+
+# @numba.jit(nopython=True)
+def alpha_prob(
+    obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
+    norm: Optional[bool] = False
+) -> np.ndarray:
+    """routine to calculate the alpha function P(y^t | x_t ) for all obserations
+
+    Args:
+        obs_ts (np.ndarray): sequence of observations
+        trans_matrix (np.ndarray): transition rate matrix
+        obs_matrix (np.ndarray): observation/emission probability matrix
+
+    Returns:
+        np.ndarray: Matrix with each column corresponding to the alpha value
+        for each state, and each row representing the estimate at each point
+        in time
+    """
+    alpha_tracker = np.zeros((len(obs_ts), trans_matrix.shape[0]))
+    alpha = obs_matrix[:, obs_ts[0]].copy()
+    alpha_tracker[0, :] = alpha
+    for i, obs in enumerate(obs_ts[1:]):
+        alpha = (trans_matrix @ alpha) * obs_matrix[obs, :]
+        alpha_tracker[i + 1, :] = alpha
+    if norm:
+        alpha_tracker = (
+            alpha_tracker / np.repeat(
+                alpha_tracker
+                .sum(axis=1)
+                .reshape(-1, 1),
+                alpha_tracker.shape[1]
+            ).reshape(alpha_tracker.shape)
+        )
+
+    return alpha_tracker
+
+
+# @numba.jit(nopython=True)
+def beta_prob(
+    obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
+    norm: Optional[bool] = False
+) -> np.ndarray:
+    """routine to calculate the beta function P(y^[t: T] | x_t ) for all obserations
+
+    Args:
+        obs_ts (np.ndarray): sequence of observations
+        trans_matrix (np.ndarray): transition rate matrix
+        obs_matrix (np.ndarray): observation/emission probability matrix
+
+    Returns:
+        np.ndarray: Matrix with each column corresponding to the beta value
+        for each state, and each row representing the estimate at each point
+        in time
+    """
+    beta_tracker = np.zeros((len(obs_ts), trans_matrix.shape[0]))
+    beta = np.ones(trans_matrix.shape[0])
+    beta_tracker[0, :] += beta
+    for i, obs in enumerate(obs_ts[-1:0:-1]):
+        beta = trans_matrix.T @ (beta * obs_matrix[:, obs])
+        beta_tracker[i + 1, :] = beta
+    if norm:
+        beta_tracker = (
+            beta_tracker / np.repeat(
+                beta_tracker
+                .sum(axis=1)
+                .reshape(-1, 1),
+                beta_tracker.shape[1]
+            ).reshape(beta_tracker.shape)
+        )
+    return beta_tracker[::-1]
+
+
+if __name__ == "__main__":
+    # test out the routines to make sure they all match
+    from hidden_py.infer import MarkovInfer
+    from hidden_py.dynamics import HMM
+    import time
+
+    hmm = HMM(2, 2)
+    hmm.init_uniform_cycle()
+
+    hmm.run_dynamics(5)
+    obs_ts, state_ts = hmm.get_obs_ts(), hmm.get_state_ts()
+
+    A_perturb = np.array([
+        [-0.05, 0.04],
+        [0.05, -0.04]
+    ])
+
+    A_sample = hmm.A + A_perturb
+    B_sample = hmm.B + A_perturb
+
+    analyzer = MarkovInfer(2, 2)
+
+    start_1 = time.time()
+    est_bayes_1 = bayes_estimate(np.array(obs_ts), A_sample, B_sample)
+    end_1 = time.time()
+
+    start_2 = time.time()
+    est_bayes_1 = bayes_estimate(np.array(obs_ts), A_sample, B_sample)
+    end_2 = time.time()
+
+    print("----- Timer results -----")
+    print(f"First iterations  : {end_1 - start_1}")
+    print(f"Second iterations : {end_2 - start_2}")
+
+    print("\n\t-- DONE --\n")
```

### Comparing `hidden-py-1.0.5/hidden_py/infer.py` & `hidden-py-1.0.6/hidden_py/infer.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,295 +1,295 @@
-# File to contain the class definitions and routines for inferring the
-# properties of the HMM
-from typing import Iterable, Optional, Dict
-import numpy as np
-from pandas import DataFrame, Series
-from hidden_py.optimize.registry import OPTIMIZER_REGISTRY
-from hidden_py.optimize.base import OptClass
-from hidden_py.optimize.results import OptimizationResult
-from hidden_py.filters import bayesian
-
-
-class MarkovInfer:
-    # Type hints for instance variables
-    forward_tracker: Iterable
-    backward_tracker: Iterable
-    predictions: Iterable
-    predictions_back: Iterable
-    bayes_smooth: Iterable
-    alpha_tracker: Iterable
-    beta_tracker: Iterable
-    n_sys: int
-    n_obs: int
- 
-    def __init__(self, dim_sys: int, dim_obs: int) -> None:
-        """Constructor for MarkovInfer class, this generally acts as an
-        interface/wrapper for the optimization and filtering routines
-
-        Args:
-            dim_sys (int): Dimension of the number of states in a hidden system
-            dim_obs (int): Number of possible observations
-        """
-        # Tracker lists for forward and backward estimates
-        self.forward_tracker = None
-        self.backward_tracker = None
-        self.predictions = None
-        self.predictions_back = None
-        self.bayes_smooth = None
-        self.alpha_tracker = None
-        self.beta_tracker = None
-
-        # Dimension of target system and observation vector
-        self.n_sys = dim_sys
-        self.n_obs = dim_obs
-
-    @staticmethod
-    def _validate_input(obs_ts: Iterable) -> np.ndarray:
-        """Routine to validate input for observation timeseries. This will cast
-        lists, and pandas Series/DataFrme to a 1-d numpy array, for use in the
-        lower-level (numba-optimized) filter routines
-
-        Args:
-            obs_ts (Iterable): timeseries of observations
-
-        Raises:
-            ValueError: Observations (numpy) cannot be interpreted as 1D
-            ValueError: Observations (pandas) cannot be interpreted as 1D
-            NotImplementedError: Input data type is not supported
-
-        Returns:
-            np.ndarray: npmy-converted observation
-        """
-        # We want this to support input lists as well as pandas Series
-        if isinstance(obs_ts, np.ndarray):
-            if 1 in obs_ts.shape or len(obs_ts.shape) == 1:
-                return obs_ts.flatten()
-            else:
-                raise ValueError("Input observations must be 1-D...")
-
-        if isinstance(obs_ts, list):
-            return np.array(obs_ts)
-        if isinstance(obs_ts, (Series, DataFrame)):
-            if 1 in obs_ts.shape or len(obs_ts.shape) == 1:
-                return obs_ts.to_numpy().flatten()
-            else:
-                raise ValueError("Input observations must be 1-D...")
-
-        else:
-            raise NotImplementedError(
-                "observation timeseries must be list or pandas Series/DataFrame"
-            )
-
-    def forward_algo(
-        self,
-        observations: Iterable[int],
-        trans_matrix: np.ndarray,
-        obs_matrix: np.ndarray,
-    ) -> None:
-        """Wrapper routine to implement the forward filter algorithm, and write
-        results to internal forward_tracker and prediction_tracker variables
-
-        Args:
-            observations (Iterable[int]): observation timeseries
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-        """
-        observations = self._validate_input(observations)
-        self.forward_tracker, self.prediction_tracker = bayesian.forward_algo(
-            observations, trans_matrix, obs_matrix
-        )
-
-    def backward_algo(
-        self,
-        observations: Iterable[int],
-        trans_matrix: np.ndarray,
-        obs_matrix: np.ndarray,
-    ) -> None:
-        """Wrapper routine to implement the backward filter algorithm, and write
-        results to internal backward_tracker and prediction_back variables
-
-        Args:
-            observations (Iterable[int]): observation timeseries
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-        """
-        observations = self._validate_input(observations)
-        self.backward_tracker, self.predictions_back = bayesian.backward_algo(
-            observations, trans_matrix, obs_matrix
-        )
-
-    def alpha(
-        self, observations: np.ndarray, trans_matrix: np.ndarray,
-        obs_matrix: np.ndarray, norm: Optional[bool] = False
-    ) -> None:
-        """Wrapper routine to interface with alpha-calcualtion routine. Sets to
-        internal alpha_tracker instance variable
-
-        Args:
-            observations (np.ndarray): timeseries of observations
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-            norm (Optional[bool], optional): whether or not there we want to
-                use normalized (across states) at each point in time.
-                Defaults to False.
-        """
-        observations = self._validate_input(observations)
-        self.alpha_tracker = bayesian.alpha_prob(
-            observations, trans_matrix, obs_matrix, norm=norm
-        )
-
-    def beta(
-        self, observations: np.ndarray, trans_matrix: np.ndarray,
-        obs_matrix: np.ndarray, norm: Optional[bool] = False
-    ) -> None:
-        """Wrapper routine to interface with beta-calcualtion routine. Sets to
-        internal beta_tracker instance variable
-
-        Args:
-            observations (np.ndarray): timeseries of observations
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-            norm (Optional[bool], optional): whether or not there we want to
-                use normalized (across states) at each point in time.
-                Defaults to False.
-        """
-        observations = self._validate_input(observations)
-        self.beta_tracker = bayesian.beta_prob(
-            observations, trans_matrix, obs_matrix, norm=norm
-        )
-
-    def bayesian_smooth(
-        self, observations: np.ndarray, trans_matrix: np.ndarray,
-        obs_matrix: np.ndarray
-    ) -> None:
-        """Wrapper routine to interface with bayesian smoothing routine. Sets
-        to internal bayes_smooth instance variable
-        
-        Args:
-            observations (np.ndarray): timeseries of observations
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-        """
-        observations = self._validate_input(observations)
-        self.bayes_smooth = bayesian.bayes_estimate(
-            observations, trans_matrix, obs_matrix
-        )
-
-    def discord(self, est_1: Iterable, est_2: Iterable) -> float:
-        """Calculates the discord order parameter for an HMM based on the
-        disagreement between two different estimates. This is the typical
-        `discord` measure for HMMs when one of the estimates is `naive` (equal
-        to observation)
-
-        Args:
-            est_1 (Iterable): first estimate of hidden state
-            est_2 (Iterable): second estimate of hidden state
-
-        Returns:
-            float: Discord order parameter between observations
-        """
-        error = [1 if f == o else -1 for f, o in zip(est_2, est_1)]
-        return 1 - np.mean(error)
-
-    def error_rate(self, pred_ts: Iterable, state_ts: Iterable) -> float:
-        """Calculates the error rate of predictions (pred_ts) as compared to
-        a known sequence of hidden states (state_ts)
-
-        Args:
-            pred_ts (Iterable): state prediction
-            state_ts (Iterable): time series of hidden states
-
-        Returns:
-            float: error rate of predictions
-        """
-        return 1 - np.mean([p == s for p, s in zip(pred_ts, state_ts)])
-
-    def optimize(
-        self, observations: Iterable, trans_init: np.ndarray,
-        obs_init: np.ndarray, symmetric: Optional[bool] = False,
-        opt_type: Optional[OptClass] = OptClass.Local,
-        algo_opts: Optional[Dict] = {}
-    ) -> OptimizationResult:
-        """Main entrypoint for optimizing an internal model
-
-        Args:
-            observations (Iterable): Time series of observations
-            trans_init (np.ndarray): Initial guess at transition rate matrix
-            obs_init (np.ndarray): Initial guess at observation matrix
-            symmetric (Optional[bool], optional): Flag as to whether or not the
-                model is assumed to be symmetric. Only has an impact if Local
-                or Global likelihood optimizer is used. Defaults to False.
-            opt_type (Optional[OptClass], optional): Optimizer class, must be
-                one of the classes contained in the MODEL_REGISTRY.
-                Defaults to OptClass.Local.
-            algo_opts (Optional[Dict], optional): Additional configuration
-                options for the optimization algorithm. Defaults to {}.
-
-        Raises:
-            ValueError: If the provided optimization class is not registerd, or
-                valid.
-
-        Returns:
-            OptimizationResult: Result of optimization
-        """
-        if not isinstance(opt_type, OptClass):
-            raise ValueError(
-                'Invalid `opt_class`, must be a member of OptClass enum...'
-            )
-        observations = self._validate_input(observations)
-        # For the global optimizer, dim_tuple, but no initial guesses
-        optimizer = OPTIMIZER_REGISTRY[opt_type](**algo_opts)
-        if (opt_type is OptClass.Global):
-            print("Running global partial-data likelihood optimization...")
-            dim_tuple = (trans_init.shape, obs_init.shape)
-            return optimizer.optimize(observations, dim_tuple, symmetric)
-
-        # For EM opt, there is no option to input a symmetric constraint
-        elif (opt_type is OptClass.ExpMax):
-            print("Running Baum-Welch (EM) optimization...")
-            return optimizer.optimize(observations, trans_init, obs_init)
-
-        print("Running local partial-data likelihood optimization...")
-        return optimizer.optimize(observations, trans_init, obs_init, symmetric)
-
-
-if __name__ == "__main__":
-    from hidden_py import dynamics
-    import time
-    hmm = dynamics.HMM(2, 2)
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(1000)
-
-    state_ts = hmm.get_state_ts()
-    obs_ts = hmm.get_obs_ts()
-
-    BayesInfer = MarkovInfer(2, 2)
-    param_init = (0.15, 0.15)
-    A_init = np.array([[0.85, 0.15], [0.15, 0.85]])
-    B_init = np.array([[0.85, 0.15], [0.15, 0.85]])
-
-    BayesInfer.forward_algo(obs_ts, hmm.A, hmm.B)
-    BayesInfer.backward_algo(obs_ts, hmm.A, hmm.B)
-    BayesInfer.bayesian_smooth(obs_ts, hmm.A, hmm.B)
-
-    BayesInfer.alpha(obs_ts, hmm.A, hmm.B)
-    BayesInfer.beta(obs_ts, hmm.A, hmm.B)
-
-    res_loc = BayesInfer.optimize(obs_ts, A_init, B_init, symmetric=True)
-    res_glo = BayesInfer.optimize(
-        obs_ts, A_init, B_init, symmetric=True, opt_type=OptClass.Global
-    )
-
-    start_bw = time.time()
-    res_bw = BayesInfer.optimize(
-        obs_ts, A_init, B_init, opt_type=OptClass.ExpMax,
-        algo_opts={
-            "track_optimization": True, "tracking_interval": 10,
-            "maxiter": 200, "testing": "THIS IS A TEST"
-        }
-    )
-    end_bw = time.time()
-    # res_bw = BayesInfer.baum_welch(param_init, obs_ts, maxiter=10)
-
-    print(f"BW Runtime: {round(end_bw - start_bw, 4)}")
-
-    print("--DONE--")
+# File to contain the class definitions and routines for inferring the
+# properties of the HMM
+from typing import Iterable, Optional, Dict
+import numpy as np
+from pandas import DataFrame, Series
+from hidden_py.optimize.registry import OPTIMIZER_REGISTRY
+from hidden_py.optimize.base import OptClass
+from hidden_py.optimize.results import OptimizationResult
+from hidden_py.filters import bayesian
+
+
+class MarkovInfer:
+    # Type hints for instance variables
+    forward_tracker: Iterable
+    backward_tracker: Iterable
+    predictions: Iterable
+    predictions_back: Iterable
+    bayes_smooth: Iterable
+    alpha_tracker: Iterable
+    beta_tracker: Iterable
+    n_sys: int
+    n_obs: int
+ 
+    def __init__(self, dim_sys: int, dim_obs: int) -> None:
+        """Constructor for MarkovInfer class, this generally acts as an
+        interface/wrapper for the optimization and filtering routines
+
+        Args:
+            dim_sys (int): Dimension of the number of states in a hidden system
+            dim_obs (int): Number of possible observations
+        """
+        # Tracker lists for forward and backward estimates
+        self.forward_tracker = None
+        self.backward_tracker = None
+        self.predictions = None
+        self.predictions_back = None
+        self.bayes_smooth = None
+        self.alpha_tracker = None
+        self.beta_tracker = None
+
+        # Dimension of target system and observation vector
+        self.n_sys = dim_sys
+        self.n_obs = dim_obs
+
+    @staticmethod
+    def _validate_input(obs_ts: Iterable) -> np.ndarray:
+        """Routine to validate input for observation timeseries. This will cast
+        lists, and pandas Series/DataFrme to a 1-d numpy array, for use in the
+        lower-level (numba-optimized) filter routines
+
+        Args:
+            obs_ts (Iterable): timeseries of observations
+
+        Raises:
+            ValueError: Observations (numpy) cannot be interpreted as 1D
+            ValueError: Observations (pandas) cannot be interpreted as 1D
+            NotImplementedError: Input data type is not supported
+
+        Returns:
+            np.ndarray: npmy-converted observation
+        """
+        # We want this to support input lists as well as pandas Series
+        if isinstance(obs_ts, np.ndarray):
+            if 1 in obs_ts.shape or len(obs_ts.shape) == 1:
+                return obs_ts.flatten()
+            else:
+                raise ValueError("Input observations must be 1-D...")
+
+        if isinstance(obs_ts, list):
+            return np.array(obs_ts)
+        if isinstance(obs_ts, (Series, DataFrame)):
+            if 1 in obs_ts.shape or len(obs_ts.shape) == 1:
+                return obs_ts.to_numpy().flatten()
+            else:
+                raise ValueError("Input observations must be 1-D...")
+
+        else:
+            raise NotImplementedError(
+                "observation timeseries must be list or pandas Series/DataFrame"
+            )
+
+    def forward_algo(
+        self,
+        observations: Iterable[int],
+        trans_matrix: np.ndarray,
+        obs_matrix: np.ndarray,
+    ) -> None:
+        """Wrapper routine to implement the forward filter algorithm, and write
+        results to internal forward_tracker and prediction_tracker variables
+
+        Args:
+            observations (Iterable[int]): observation timeseries
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+        """
+        observations = self._validate_input(observations)
+        self.forward_tracker, self.prediction_tracker = bayesian.forward_algo(
+            observations, trans_matrix, obs_matrix
+        )
+
+    def backward_algo(
+        self,
+        observations: Iterable[int],
+        trans_matrix: np.ndarray,
+        obs_matrix: np.ndarray,
+    ) -> None:
+        """Wrapper routine to implement the backward filter algorithm, and write
+        results to internal backward_tracker and prediction_back variables
+
+        Args:
+            observations (Iterable[int]): observation timeseries
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+        """
+        observations = self._validate_input(observations)
+        self.backward_tracker, self.predictions_back = bayesian.backward_algo(
+            observations, trans_matrix, obs_matrix
+        )
+
+    def alpha(
+        self, observations: np.ndarray, trans_matrix: np.ndarray,
+        obs_matrix: np.ndarray, norm: Optional[bool] = False
+    ) -> None:
+        """Wrapper routine to interface with alpha-calcualtion routine. Sets to
+        internal alpha_tracker instance variable
+
+        Args:
+            observations (np.ndarray): timeseries of observations
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+            norm (Optional[bool], optional): whether or not there we want to
+                use normalized (across states) at each point in time.
+                Defaults to False.
+        """
+        observations = self._validate_input(observations)
+        self.alpha_tracker = bayesian.alpha_prob(
+            observations, trans_matrix, obs_matrix, norm=norm
+        )
+
+    def beta(
+        self, observations: np.ndarray, trans_matrix: np.ndarray,
+        obs_matrix: np.ndarray, norm: Optional[bool] = False
+    ) -> None:
+        """Wrapper routine to interface with beta-calcualtion routine. Sets to
+        internal beta_tracker instance variable
+
+        Args:
+            observations (np.ndarray): timeseries of observations
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+            norm (Optional[bool], optional): whether or not there we want to
+                use normalized (across states) at each point in time.
+                Defaults to False.
+        """
+        observations = self._validate_input(observations)
+        self.beta_tracker = bayesian.beta_prob(
+            observations, trans_matrix, obs_matrix, norm=norm
+        )
+
+    def bayesian_smooth(
+        self, observations: np.ndarray, trans_matrix: np.ndarray,
+        obs_matrix: np.ndarray
+    ) -> None:
+        """Wrapper routine to interface with bayesian smoothing routine. Sets
+        to internal bayes_smooth instance variable
+        
+        Args:
+            observations (np.ndarray): timeseries of observations
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+        """
+        observations = self._validate_input(observations)
+        self.bayes_smooth = bayesian.bayes_estimate(
+            observations, trans_matrix, obs_matrix
+        )
+
+    def discord(self, est_1: Iterable, est_2: Iterable) -> float:
+        """Calculates the discord order parameter for an HMM based on the
+        disagreement between two different estimates. This is the typical
+        `discord` measure for HMMs when one of the estimates is `naive` (equal
+        to observation)
+
+        Args:
+            est_1 (Iterable): first estimate of hidden state
+            est_2 (Iterable): second estimate of hidden state
+
+        Returns:
+            float: Discord order parameter between observations
+        """
+        error = [1 if f == o else -1 for f, o in zip(est_2, est_1)]
+        return 1 - np.mean(error)
+
+    def error_rate(self, pred_ts: Iterable, state_ts: Iterable) -> float:
+        """Calculates the error rate of predictions (pred_ts) as compared to
+        a known sequence of hidden states (state_ts)
+
+        Args:
+            pred_ts (Iterable): state prediction
+            state_ts (Iterable): time series of hidden states
+
+        Returns:
+            float: error rate of predictions
+        """
+        return 1 - np.mean([p == s for p, s in zip(pred_ts, state_ts)])
+
+    def optimize(
+        self, observations: Iterable, trans_init: np.ndarray,
+        obs_init: np.ndarray, symmetric: Optional[bool] = False,
+        opt_type: Optional[OptClass] = OptClass.Local,
+        algo_opts: Optional[Dict] = {}
+    ) -> OptimizationResult:
+        """Main entrypoint for optimizing an internal model
+
+        Args:
+            observations (Iterable): Time series of observations
+            trans_init (np.ndarray): Initial guess at transition rate matrix
+            obs_init (np.ndarray): Initial guess at observation matrix
+            symmetric (Optional[bool], optional): Flag as to whether or not the
+                model is assumed to be symmetric. Only has an impact if Local
+                or Global likelihood optimizer is used. Defaults to False.
+            opt_type (Optional[OptClass], optional): Optimizer class, must be
+                one of the classes contained in the MODEL_REGISTRY.
+                Defaults to OptClass.Local.
+            algo_opts (Optional[Dict], optional): Additional configuration
+                options for the optimization algorithm. Defaults to {}.
+
+        Raises:
+            ValueError: If the provided optimization class is not registerd, or
+                valid.
+
+        Returns:
+            OptimizationResult: Result of optimization
+        """
+        if not isinstance(opt_type, OptClass):
+            raise ValueError(
+                'Invalid `opt_class`, must be a member of OptClass enum...'
+            )
+        observations = self._validate_input(observations)
+        # For the global optimizer, dim_tuple, but no initial guesses
+        optimizer = OPTIMIZER_REGISTRY[opt_type](**algo_opts)
+        if (opt_type is OptClass.Global):
+            print("Running global partial-data likelihood optimization...")
+            dim_tuple = (trans_init.shape, obs_init.shape)
+            return optimizer.optimize(observations, dim_tuple, symmetric)
+
+        # For EM opt, there is no option to input a symmetric constraint
+        elif (opt_type is OptClass.ExpMax):
+            print("Running Baum-Welch (EM) optimization...")
+            return optimizer.optimize(observations, trans_init, obs_init)
+
+        print("Running local partial-data likelihood optimization...")
+        return optimizer.optimize(observations, trans_init, obs_init, symmetric)
+
+
+if __name__ == "__main__":
+    from hidden_py import dynamics
+    import time
+    hmm = dynamics.HMM(2, 2)
+    hmm.init_uniform_cycle()
+    hmm.run_dynamics(1000)
+
+    state_ts = hmm.get_state_ts()
+    obs_ts = hmm.get_obs_ts()
+
+    BayesInfer = MarkovInfer(2, 2)
+    param_init = (0.15, 0.15)
+    A_init = np.array([[0.85, 0.15], [0.15, 0.85]])
+    B_init = np.array([[0.85, 0.15], [0.15, 0.85]])
+
+    BayesInfer.forward_algo(obs_ts, hmm.A, hmm.B)
+    BayesInfer.backward_algo(obs_ts, hmm.A, hmm.B)
+    BayesInfer.bayesian_smooth(obs_ts, hmm.A, hmm.B)
+
+    BayesInfer.alpha(obs_ts, hmm.A, hmm.B)
+    BayesInfer.beta(obs_ts, hmm.A, hmm.B)
+
+    res_loc = BayesInfer.optimize(obs_ts, A_init, B_init, symmetric=True)
+    res_glo = BayesInfer.optimize(
+        obs_ts, A_init, B_init, symmetric=True, opt_type=OptClass.Global
+    )
+
+    start_bw = time.time()
+    res_bw = BayesInfer.optimize(
+        obs_ts, A_init, B_init, opt_type=OptClass.ExpMax,
+        algo_opts={
+            "track_optimization": True, "tracking_interval": 10,
+            "maxiter": 200, "testing": "THIS IS A TEST"
+        }
+    )
+    end_bw = time.time()
+    # res_bw = BayesInfer.baum_welch(param_init, obs_ts, maxiter=10)
+
+    print(f"BW Runtime: {round(end_bw - start_bw, 4)}")
+
+    print("--DONE--")
```

### Comparing `hidden-py-1.0.5/hidden_py/optimize/base.py` & `hidden-py-1.0.6/hidden_py/optimize/base.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,322 +1,322 @@
-from abc import ABC, abstractmethod
-from enum import Enum, auto
-from typing import Optional, Iterable, Tuple, Union, Iterator
-from operator import mul
-from itertools import islice
-import numpy as np
-import numba
-
-from hidden_py.filters import bayesian
-
-
-class OptClass(Enum):
-    Local = auto()
-    Global = auto()
-    ExpMax = auto()
-
-
-class BaseOptimizer(ABC):
-    def __init__(self):
-        self.status = 0
-        self.result = None
-        self.bayes_filter = None
-        self.predictions = None
-
-    # def __repr__(self):
-    #     return f"{self.name}(status={self.status})"
-
-    @staticmethod
-    def _build_optimization_bounds(
-        n_params: int, lower_lim: Optional[float] = 1e-3,
-        upper_lim: Optional[float] = 1 - 1e-3
-    ) -> Iterable:
-        """Routine to generate a list of optimization bounds for input into an
-        optimization function.
-
-        Args:
-            n_params (int): number of model parameters
-            lower_lim (Optional[float], optional): lower bound on model
-                parameters. Defaults to 1e-3.
-            upper_lim (Optional[float], optional): upper bound on model
-            parameters. Defaults to 1-1e-3.
-
-        Returns:
-            Iterable: Variable-length iterable, with each element containing
-                the same upper and lower bounds on a model parameters.
-        """
-        return [(lower_lim, upper_lim)] * n_params
-
-    @abstractmethod
-    def optimize(self):
-        pass
-
-
-class LikelihoodOptimizer(BaseOptimizer):
-
-    @staticmethod
-    def _encode_parameters_symmetric(
-        A: np.ndarray, B: np.ndarray
-    ) -> Tuple[np.ndarray, Tuple]:
-        """Encoding logic for input HMM transition (A) and abservation (B)
-        matrices. Takes in (symmetric) matrices A and B and encodes them into
-        a parameter array theta = (p1, p2, ...) and also returns a tuple
-        with the dimensions of each input matrix
-
-        Note that because the input matrices are both stochastic matrices, the
-        columns are normalized and so the diagonal entries are not independent
-        parameters, so they do not get included in the encoded vector
-
-        EXAMPLE:
-
-        INPUTS:
-        A = [0.8, 0.2]      B = [0.9, 0.1]
-            [0.2, 0.8]          [0.1, 0.9]
-
-        OUTPUTS:
-        encoded: [0.2, 0.1]
-        dim_tuple: ((2,2), (2,2))
-
-        Args:
-            A (np.ndarray): transition matrix for hidden states
-            B (np.ndarray): matrix for symbol emmissions (observations)
-
-        Raises:
-            ValueError: Input matrix is not square (both must be)
-            ValueError: One of the input matrices is not symmetric
-
-        Returns:
-            Tuple[np.ndarray, Tuple]: encoded param vector,
-                input matrix dimensions
-        """
-        if A.shape[0] != A.shape[1] or B.shape[0] != B.shape[1]:
-            raise ValueError("Input matrix not square...")
-
-        if not np.all(A == A.T) or not np.all(B == B.T):
-            raise ValueError(
-                'Input matrix `A` or `B` is not symmetric...'
-            )
-
-        dim_tuple = (A.shape, B.shape)
-        A_entries = (mul(*A.shape) - A.shape[0]) // 2
-        B_entries = (mul(*B.shape) - B.shape[0]) // 2
-        encoded = np.zeros(A_entries + B_entries)
-
-        encoded[:A_entries] = A[np.triu_indices(A.shape[0], k=1)]
-        encoded[A_entries:] = B[np.triu_indices(B.shape[0], k=1)]
-
-        return encoded, dim_tuple
-
-    @staticmethod
-    def _encode_parameters(
-        A: np.ndarray, B: np.ndarray
-    ) -> Tuple[np.ndarray, Tuple]:
-        """Encodes input (non-symmetric, or not-necessarily symmetric) matrices
-        for transitions (A) and observations (B) into a 1-d parameter vector
-        theta = (p_1, p_2, ...) and also returns a tuple containing the
-        dimensions of the input arrays
-
-        Note that because the input matrices are both stochastic matrices, the
-        columns are normalized and so the diagonal entries are not independent
-        parameters, so they do not get included in the encoded vector
-
-        EXAMPLE
-
-        INPUTS:
-        A = [0.8, 0.3]      B = [0.9, 0.15]
-            [0.2, 0.7]          [0.1, 0.85]
-
-        OUTPUTS:
-        encoded: [0.3, 0.2, 0.15, 0.1]
-        dim_tuple: ((2,2), (2,2))
-
-        Args:
-            A (np.ndarray): transition matrix for hidden states
-            B (np.ndarray): matrix for symbol emmissions (observations)
-
-        Returns:
-            Tuple[np.ndarray, Tuple]: encoded param vector,
-                input matrix dimensions
-        """
-        encoded = np.zeros(mul(*A.shape) + mul(*B.shape) - A.shape[0] - B.shape[0])
-        dim_tuple = (A.shape, B.shape)
-        # Compress the diagonal entries out of A and B
-        A_compressed = np.triu(A, k=1)[:, 1:] + np.tril(A, k=-1)[:, :-1]
-        B_compressed = np.triu(B, k=1)[:, 1:] + np.tril(B, k=-1)[:, :-1]
-        # Encode the off-diagonals into a vector
-        encoded[: mul(*A.shape) - A.shape[0]] = np.ravel(A_compressed)
-        encoded[mul(*A.shape) - A.shape[0]:] = np.ravel(B_compressed)
-        return encoded, dim_tuple
-
-    @staticmethod
-    def _extract_parameters_symmetric(
-        param_arr: Union[np.ndarray, Tuple], A_dim: Tuple, B_dim: Tuple
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """Code to decode/extract (symmetric )HMM model parameters from an
-        input parameter array that has been encoded using
-        `_encode_parameters_symmetric` (i.e. this is the inverse operation)
-
-        EXAMPLE
-
-        INPUTS:
-        param_arr = [0.2, 0.3],  A_dim = (2, 2),  B_dim = (2, 2)
-
-        OUTPUT:
-        A = [0.8, 0.2]      B = [0.7, 0.3]
-            [0.2, 0.8]          [0.3, 0.2]
-
-        Args:
-            param_arr (Union[np.ndarray, Tuple]): encoded parameter array
-            A_dim (Tuple): dimensions of transition matrix
-            B_dim (Tuple): dimenstions of observation matrix
-
-        Returns:
-            Tuple[np.ndarray, np.ndarray]: transition matrix (A),
-                observation matrix (B)
-        """
-
-        def _build_upper_tri(dim: Tuple, param_iter: Iterator):
-            mat_ = np.zeros(dim)
-            for c in range(dim[0] - 1):
-                mat_[c, c+1:] = list(islice(param_iter, dim[0] - 1 - c))
-            return mat_
-
-        A_size = A_dim[0] * A_dim[1] - A_dim[0]
-        A_size //= 2
-
-        param_iter = iter(param_arr)
-        trans_mat = _build_upper_tri(A_dim, param_iter)
-        obs_mat = _build_upper_tri(B_dim, param_iter)
-
-        trans_mat += trans_mat.T
-        obs_mat += obs_mat.T
-        trans_mat += np.diag(1 - trans_mat.sum(axis=1))
-        obs_mat += np.diag(1 - obs_mat.sum(axis=1))
-        return trans_mat, obs_mat
-
-    @staticmethod
-    def _extract_parameters(
-        param_arr: Union[np.ndarray, Tuple], A_dim: Tuple, B_dim: Tuple,
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """Code to decode/extract (non-symmetric or not-necessarily symmetric)
-        HMM model parameters from an input parameter array that has been
-        encoded using `_encode_parameters` (i.e. this is the inverse operation)
-
-        EXAMPLE
-
-        INPUTS:
-        param_arr = [0.2, 0.3, 0.1, 0.15],  A_dim = (2, 2),  B_dim = (2, 2)
-
-        OUTPUT:
-        A = [0.7, 0.2]      B = [0.85, 0.1]
-            [0.3, 0.8]          [0.15, 0.9]
-
-        Args:
-            param_arr (Union[np.ndarray, Tuple]): encoded parameter array
-            A_dim (Tuple): dimensions of transition matrix
-            B_dim (Tuple): dimenstions of observation matrix
-
-        Returns:
-            Tuple[np.ndarray, np.ndarray]: transition matrix (A),
-                observation matrix (B)
-        """
-
-        # If this is passed in as a tuple, cast to numpy array
-        param_arr = np.array(param_arr)
-
-        # Take the dimension to be the 'true' dimension, less the diagonal terms
-        A_size = A_dim[0] * A_dim[1] - A_dim[0]
-
-        # Pull out A, and B specific parameters
-        trans_mat = param_arr[:A_size]
-        obs_mat = param_arr[A_size:]
-
-        trans_mat = trans_mat.reshape(A_dim[0], A_dim[1] - 1)
-        obs_mat = obs_mat.reshape(B_dim[0], B_dim[1] - 1)
-
-        # Now reconstruct the trans matrix diagonal elements: first the
-        # following line will add a diagonal of zeros, note this assumes that
-        # the matrix is condensed along axis 1
-        trans_mat = (
-            np.hstack((np.zeros((A_dim[0], 1)), np.triu(trans_mat)))
-            + np.hstack((np.tril(trans_mat, k=-1), np.zeros((A_dim[0], 1))))
-        )
-
-        obs_mat = (
-            np.hstack((np.zeros((B_dim[0], 1)), np.triu(obs_mat)))
-            + np.hstack((np.tril(obs_mat, k=-1), np.zeros((B_dim[0], 1))))
-        )
-        # Add in diagonal terms so that sum(axis=0) = 1
-        trans_mat += np.eye(trans_mat.shape[0], M=trans_mat.shape[1]) - np.diag(trans_mat.sum(axis=0))
-        obs_mat += np.eye(obs_mat.shape[0], M=obs_mat.shape[1]) - np.diag(obs_mat.sum(axis=0))
-
-        return trans_mat, obs_mat
-
-    @staticmethod
-    @numba.jit(nopython=True)
-    def _likelihood(
-        predictions: np.ndarray, obs_ts: np.ndarray, B: np.ndarray
-    ) -> float:
-        """Calcualte negative log-likelihood value for a particular set of
-        parameters (which produce a specific set of predictions and a B matrix)
-
-        Args:
-            predictions (np.ndarray): Sequence of unnormalized preiction
-                vectors from the bayesian_filter calculation
-            obs_ts (np.ndarray): sequence of discrete-state observations
-            B (np.ndarray): observation matrix
-
-        Returns:
-            float: negative log-likelihood value
-        """
-        likelihood = 0
-        for i, obs in enumerate(obs_ts):
-            inner = predictions[i, :] @ B[obs, :]
-            likelihood -= np.log(inner)
-        return likelihood
-
-    @staticmethod
-    def calc_likelihood(
-        param_arr: Iterable, dim: Tuple, obs_ts: Iterable,
-        symmetric: Optional[bool] = False
-    ) -> float:
-        """Logic to calculate the likelihood values for a given parameter array
-
-        Args:
-            param_arr (Iterable): encoded parameter vector
-            dim (Tuple): tuple of A and B matrix dimensions (dim_tuple from
-                encoding output)
-            obs_ts (Iterable): Time-series sequence of (integer) state
-                observations
-            symmetric (Optional[bool], optional): whether the model
-                (A and B matrices) are assumed to be symmetric.
-                Defaults to False.
-
-        Returns:
-            float: negative log-likeihood of parameter vector, given obs_ts
-        """
-        A_dim, B_dim = dim
-        # Extract parameters
-        if symmetric:
-            A, B = LikelihoodOptimizer._extract_parameters_symmetric(param_arr, A_dim, B_dim)
-        else:
-            A, B = LikelihoodOptimizer._extract_parameters(param_arr, A_dim, B_dim)
-        # Generate predictions vector
-        _, pred = bayesian.forward_algo(obs_ts, A, B)
-        # Return likelihood value
-        return LikelihoodOptimizer._likelihood(pred, np.array(obs_ts), B)
-
-
-class CompleteLikelihoodOptimizer(BaseOptimizer):
-    def __init__(self):
-        pass
-
-    @abstractmethod
-    def optimize(self):
-        pass
-
-
-# Method for runnning tests on abstract class TestLikelihoodOptimizer
-class TestLikelihoodOptimizer(LikelihoodOptimizer):
-    def optimize(self):
-        pass
-
+from abc import ABC, abstractmethod
+from enum import Enum, auto
+from typing import Optional, Iterable, Tuple, Union, Iterator
+from operator import mul
+from itertools import islice
+import numpy as np
+import numba
+
+from hidden_py.filters import bayesian
+
+
+class OptClass(Enum):
+    Local = auto()
+    Global = auto()
+    ExpMax = auto()
+
+
+class BaseOptimizer(ABC):
+    def __init__(self):
+        self.status = 0
+        self.result = None
+        self.bayes_filter = None
+        self.predictions = None
+
+    # def __repr__(self):
+    #     return f"{self.name}(status={self.status})"
+
+    @staticmethod
+    def _build_optimization_bounds(
+        n_params: int, lower_lim: Optional[float] = 1e-3,
+        upper_lim: Optional[float] = 1 - 1e-3
+    ) -> Iterable:
+        """Routine to generate a list of optimization bounds for input into an
+        optimization function.
+
+        Args:
+            n_params (int): number of model parameters
+            lower_lim (Optional[float], optional): lower bound on model
+                parameters. Defaults to 1e-3.
+            upper_lim (Optional[float], optional): upper bound on model
+            parameters. Defaults to 1-1e-3.
+
+        Returns:
+            Iterable: Variable-length iterable, with each element containing
+                the same upper and lower bounds on a model parameters.
+        """
+        return [(lower_lim, upper_lim)] * n_params
+
+    @abstractmethod
+    def optimize(self):
+        pass
+
+
+class LikelihoodOptimizer(BaseOptimizer):
+
+    @staticmethod
+    def _encode_parameters_symmetric(
+        A: np.ndarray, B: np.ndarray
+    ) -> Tuple[np.ndarray, Tuple]:
+        """Encoding logic for input HMM transition (A) and abservation (B)
+        matrices. Takes in (symmetric) matrices A and B and encodes them into
+        a parameter array theta = (p1, p2, ...) and also returns a tuple
+        with the dimensions of each input matrix
+
+        Note that because the input matrices are both stochastic matrices, the
+        columns are normalized and so the diagonal entries are not independent
+        parameters, so they do not get included in the encoded vector
+
+        EXAMPLE:
+
+        INPUTS:
+        A = [0.8, 0.2]      B = [0.9, 0.1]
+            [0.2, 0.8]          [0.1, 0.9]
+
+        OUTPUTS:
+        encoded: [0.2, 0.1]
+        dim_tuple: ((2,2), (2,2))
+
+        Args:
+            A (np.ndarray): transition matrix for hidden states
+            B (np.ndarray): matrix for symbol emmissions (observations)
+
+        Raises:
+            ValueError: Input matrix is not square (both must be)
+            ValueError: One of the input matrices is not symmetric
+
+        Returns:
+            Tuple[np.ndarray, Tuple]: encoded param vector,
+                input matrix dimensions
+        """
+        if A.shape[0] != A.shape[1] or B.shape[0] != B.shape[1]:
+            raise ValueError("Input matrix not square...")
+
+        if not np.all(A == A.T) or not np.all(B == B.T):
+            raise ValueError(
+                'Input matrix `A` or `B` is not symmetric...'
+            )
+
+        dim_tuple = (A.shape, B.shape)
+        A_entries = (mul(*A.shape) - A.shape[0]) // 2
+        B_entries = (mul(*B.shape) - B.shape[0]) // 2
+        encoded = np.zeros(A_entries + B_entries)
+
+        encoded[:A_entries] = A[np.triu_indices(A.shape[0], k=1)]
+        encoded[A_entries:] = B[np.triu_indices(B.shape[0], k=1)]
+
+        return encoded, dim_tuple
+
+    @staticmethod
+    def _encode_parameters(
+        A: np.ndarray, B: np.ndarray
+    ) -> Tuple[np.ndarray, Tuple]:
+        """Encodes input (non-symmetric, or not-necessarily symmetric) matrices
+        for transitions (A) and observations (B) into a 1-d parameter vector
+        theta = (p_1, p_2, ...) and also returns a tuple containing the
+        dimensions of the input arrays
+
+        Note that because the input matrices are both stochastic matrices, the
+        columns are normalized and so the diagonal entries are not independent
+        parameters, so they do not get included in the encoded vector
+
+        EXAMPLE
+
+        INPUTS:
+        A = [0.8, 0.3]      B = [0.9, 0.15]
+            [0.2, 0.7]          [0.1, 0.85]
+
+        OUTPUTS:
+        encoded: [0.3, 0.2, 0.15, 0.1]
+        dim_tuple: ((2,2), (2,2))
+
+        Args:
+            A (np.ndarray): transition matrix for hidden states
+            B (np.ndarray): matrix for symbol emmissions (observations)
+
+        Returns:
+            Tuple[np.ndarray, Tuple]: encoded param vector,
+                input matrix dimensions
+        """
+        encoded = np.zeros(mul(*A.shape) + mul(*B.shape) - A.shape[0] - B.shape[0])
+        dim_tuple = (A.shape, B.shape)
+        # Compress the diagonal entries out of A and B
+        A_compressed = np.triu(A, k=1)[:, 1:] + np.tril(A, k=-1)[:, :-1]
+        B_compressed = np.triu(B, k=1)[:, 1:] + np.tril(B, k=-1)[:, :-1]
+        # Encode the off-diagonals into a vector
+        encoded[: mul(*A.shape) - A.shape[0]] = np.ravel(A_compressed)
+        encoded[mul(*A.shape) - A.shape[0]:] = np.ravel(B_compressed)
+        return encoded, dim_tuple
+
+    @staticmethod
+    def _extract_parameters_symmetric(
+        param_arr: Union[np.ndarray, Tuple], A_dim: Tuple, B_dim: Tuple
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """Code to decode/extract (symmetric )HMM model parameters from an
+        input parameter array that has been encoded using
+        `_encode_parameters_symmetric` (i.e. this is the inverse operation)
+
+        EXAMPLE
+
+        INPUTS:
+        param_arr = [0.2, 0.3],  A_dim = (2, 2),  B_dim = (2, 2)
+
+        OUTPUT:
+        A = [0.8, 0.2]      B = [0.7, 0.3]
+            [0.2, 0.8]          [0.3, 0.2]
+
+        Args:
+            param_arr (Union[np.ndarray, Tuple]): encoded parameter array
+            A_dim (Tuple): dimensions of transition matrix
+            B_dim (Tuple): dimenstions of observation matrix
+
+        Returns:
+            Tuple[np.ndarray, np.ndarray]: transition matrix (A),
+                observation matrix (B)
+        """
+
+        def _build_upper_tri(dim: Tuple, param_iter: Iterator):
+            mat_ = np.zeros(dim)
+            for c in range(dim[0] - 1):
+                mat_[c, c+1:] = list(islice(param_iter, dim[0] - 1 - c))
+            return mat_
+
+        A_size = A_dim[0] * A_dim[1] - A_dim[0]
+        A_size //= 2
+
+        param_iter = iter(param_arr)
+        trans_mat = _build_upper_tri(A_dim, param_iter)
+        obs_mat = _build_upper_tri(B_dim, param_iter)
+
+        trans_mat += trans_mat.T
+        obs_mat += obs_mat.T
+        trans_mat += np.diag(1 - trans_mat.sum(axis=1))
+        obs_mat += np.diag(1 - obs_mat.sum(axis=1))
+        return trans_mat, obs_mat
+
+    @staticmethod
+    def _extract_parameters(
+        param_arr: Union[np.ndarray, Tuple], A_dim: Tuple, B_dim: Tuple,
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """Code to decode/extract (non-symmetric or not-necessarily symmetric)
+        HMM model parameters from an input parameter array that has been
+        encoded using `_encode_parameters` (i.e. this is the inverse operation)
+
+        EXAMPLE
+
+        INPUTS:
+        param_arr = [0.2, 0.3, 0.1, 0.15],  A_dim = (2, 2),  B_dim = (2, 2)
+
+        OUTPUT:
+        A = [0.7, 0.2]      B = [0.85, 0.1]
+            [0.3, 0.8]          [0.15, 0.9]
+
+        Args:
+            param_arr (Union[np.ndarray, Tuple]): encoded parameter array
+            A_dim (Tuple): dimensions of transition matrix
+            B_dim (Tuple): dimenstions of observation matrix
+
+        Returns:
+            Tuple[np.ndarray, np.ndarray]: transition matrix (A),
+                observation matrix (B)
+        """
+
+        # If this is passed in as a tuple, cast to numpy array
+        param_arr = np.array(param_arr)
+
+        # Take the dimension to be the 'true' dimension, less the diagonal terms
+        A_size = A_dim[0] * A_dim[1] - A_dim[0]
+
+        # Pull out A, and B specific parameters
+        trans_mat = param_arr[:A_size]
+        obs_mat = param_arr[A_size:]
+
+        trans_mat = trans_mat.reshape(A_dim[0], A_dim[1] - 1)
+        obs_mat = obs_mat.reshape(B_dim[0], B_dim[1] - 1)
+
+        # Now reconstruct the trans matrix diagonal elements: first the
+        # following line will add a diagonal of zeros, note this assumes that
+        # the matrix is condensed along axis 1
+        trans_mat = (
+            np.hstack((np.zeros((A_dim[0], 1)), np.triu(trans_mat)))
+            + np.hstack((np.tril(trans_mat, k=-1), np.zeros((A_dim[0], 1))))
+        )
+
+        obs_mat = (
+            np.hstack((np.zeros((B_dim[0], 1)), np.triu(obs_mat)))
+            + np.hstack((np.tril(obs_mat, k=-1), np.zeros((B_dim[0], 1))))
+        )
+        # Add in diagonal terms so that sum(axis=0) = 1
+        trans_mat += np.eye(trans_mat.shape[0], M=trans_mat.shape[1]) - np.diag(trans_mat.sum(axis=0))
+        obs_mat += np.eye(obs_mat.shape[0], M=obs_mat.shape[1]) - np.diag(obs_mat.sum(axis=0))
+
+        return trans_mat, obs_mat
+
+    @staticmethod
+    @numba.jit(nopython=True)
+    def _likelihood(
+        predictions: np.ndarray, obs_ts: np.ndarray, B: np.ndarray
+    ) -> float:
+        """Calcualte negative log-likelihood value for a particular set of
+        parameters (which produce a specific set of predictions and a B matrix)
+
+        Args:
+            predictions (np.ndarray): Sequence of unnormalized preiction
+                vectors from the bayesian_filter calculation
+            obs_ts (np.ndarray): sequence of discrete-state observations
+            B (np.ndarray): observation matrix
+
+        Returns:
+            float: negative log-likelihood value
+        """
+        likelihood = 0
+        for i, obs in enumerate(obs_ts):
+            inner = predictions[i, :] @ B[obs, :]
+            likelihood -= np.log(inner)
+        return likelihood
+
+    @staticmethod
+    def calc_likelihood(
+        param_arr: Iterable, dim: Tuple, obs_ts: Iterable,
+        symmetric: Optional[bool] = False
+    ) -> float:
+        """Logic to calculate the likelihood values for a given parameter array
+
+        Args:
+            param_arr (Iterable): encoded parameter vector
+            dim (Tuple): tuple of A and B matrix dimensions (dim_tuple from
+                encoding output)
+            obs_ts (Iterable): Time-series sequence of (integer) state
+                observations
+            symmetric (Optional[bool], optional): whether the model
+                (A and B matrices) are assumed to be symmetric.
+                Defaults to False.
+
+        Returns:
+            float: negative log-likeihood of parameter vector, given obs_ts
+        """
+        A_dim, B_dim = dim
+        # Extract parameters
+        if symmetric:
+            A, B = LikelihoodOptimizer._extract_parameters_symmetric(param_arr, A_dim, B_dim)
+        else:
+            A, B = LikelihoodOptimizer._extract_parameters(param_arr, A_dim, B_dim)
+        # Generate predictions vector
+        _, pred = bayesian.forward_algo(obs_ts, A, B)
+        # Return likelihood value
+        return LikelihoodOptimizer._likelihood(pred, np.array(obs_ts), B)
+
+
+class CompleteLikelihoodOptimizer(BaseOptimizer):
+    def __init__(self):
+        pass
+
+    @abstractmethod
+    def optimize(self):
+        pass
+
+
+# Method for runnning tests on abstract class TestLikelihoodOptimizer
+class TestLikelihoodOptimizer(LikelihoodOptimizer):
+    def optimize(self):
+        pass
+
```

### Comparing `hidden-py-1.0.5/hidden_py/optimize/optimization.py` & `hidden-py-1.0.6/hidden_py/optimize/optimization.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,512 +1,512 @@
-from typing import Iterable, Tuple, Optional, Union
-import warnings
-import numba
-from operator import mul
-import numpy as np
-import scipy.optimize as so
-import scipy.linalg as sl
-
-from hidden_py.optimize.results import LikelihoodOptimizationResult, EMOptimizationResult
-from hidden_py.optimize.base import LikelihoodOptimizer, CompleteLikelihoodOptimizer
-from hidden_py.filters import bayesian
-
-
-class LocalLikelihoodOptimizer(LikelihoodOptimizer):
-    def __init__(
-        self, algorithm: Optional[str] = "L-BFGS-B"
-    ) -> None:
-        """Contructor for LicalLikelihoodOptimizer class
-
-        Args:
-            algorithm (Optional[str], optional): Algorithm to use in numerical
-                optimization. Defaults to "L-BFGS-B" (Limited-Memory
-                Broyden-Fletcher-Goldfarb-Shanno (BFGS) algorithm).
-        """
-        self.algo = algorithm
-        super().__init__()
-
-    def optimize(
-        self, obs_ts: Iterable, A_guess: np.ndarray, B_guess: np.ndarray,
-        symmetric: Optional[bool] = False
-    ) -> LikelihoodOptimizationResult:
-        """Routine to run actual optimization of the model. Passes off the
-        objective function and encoded parameter array to a scipy optimizer
-
-        Args:
-            obs_ts (Iterable): integer sequence of observation values
-            A_guess (np.ndarray): Initial guess at transition matrix
-            B_guess (np.ndarray): Initial guess at observation matrix
-            symmetric (Optional[bool], optional): Whether or not the model
-                (A and B matrices) are assumed to be symmetric.
-                Defaults to False.
-
-        Returns:
-            LikelihoodOptimizationResult: Container object for model results
-        """
-        # Cast observations to numpy array if they are a list
-        obs_ts = np.array(obs_ts)
-
-        # Encode model parameters into parameter vector
-        if symmetric:
-            param_init, dim_tuple = self._encode_parameters_symmetric(A_guess, B_guess)
-        else:
-            param_init, dim_tuple = self._encode_parameters(A_guess, B_guess)
-
-        # Additional arguments to pass into optimizer
-        opt_args = (dim_tuple, obs_ts, symmetric)
-        # Parameter bounds in optimization
-        bnds = self._build_optimization_bounds(len(param_init))
-
-        # run optimizer
-        self.result = so.minimize(
-            fun=LikelihoodOptimizer.calc_likelihood,
-            x0=param_init,
-            args=opt_args,
-            method=self.algo,
-            bounds=bnds
-        )
-
-        # Return results
-        if symmetric:
-            return LikelihoodOptimizationResult(
-                self,
-                *self._extract_parameters_symmetric(self.result.x, *dim_tuple)
-            )
-        return LikelihoodOptimizationResult(
-            self, *self._extract_parameters(self.result.x, *dim_tuple)
-        )
-
-
-class GlobalLikelihoodOptimizer(LikelihoodOptimizer):
-    def __init__(
-        self, sampling_algorithm: Optional[str] = "sobol"
-    ):
-        """Constructor for GlobalLikelihoodOptimizer class
-
-        Args:
-            sampling_algorithm (Optional[str], optional): algorithm to use for
-                sampling initial random points in optimization algorithm.
-                Defaults to "sobol".
-        """
-        self.algo = sampling_algorithm
-        super().__init__()
-
-    def _get_num_params(self, dim_tuple: Tuple, symmetric: bool) -> int:
-        """Utility function to determine the number fo parameters from the input
-        matrix dimensions.
-
-        Args:
-            dim_tuple (Tuple): Tuple containing the size tupled for A and B
-            symmetric (bool): Whether the problem is assumed ot be symmetric
-
-        Returns:
-            int: total number of parametsr in the problem
-        """
-        N_a = mul(*dim_tuple[0])
-        N_b = mul(*dim_tuple[1])
-
-        N_a = N_a - dim_tuple[0][1]
-        N_b = N_b - dim_tuple[1][1]
-
-        if symmetric:
-            N_a //= 2
-            N_b //= 2
-
-        return N_a + N_b
-
-    def optimize(
-        self, obs_ts: Iterable, dim_tuple: Tuple,
-        symmetric: Optional[bool] = False
-    ) -> LikelihoodOptimizationResult:
-        """Routine to run actual optimization of the model. Passes off the
-        objective function and encoded parameter array to a scipy optimizer.
-
-        This global optimizer uses the 'Simplical Homology Global Optimizer'
-        `shgo` algorithm in the scipy library.
-        See https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.shgo.html
-        or Ref[1] for an overview of the method
-
-        REFERENCES:
-            [1] Endres, SC, Sandrock, C, Focke, WW (2018) “A simplicial
-            homology algorithm for lipschitz optimisation”, Journal of Global
-            Optimization.
-
-        Args:
-            obs_ts (Iterable): Integer sequence of observations
-            dim_tuple (Tuple): dimensions of A and B matrices
-            symmetric (Optional[bool], optional): Whether or not the model
-                parameters are assumed to be symmetric.
-                Defaults to False.
-
-        Returns:
-            LikelihoodOptimizationResult: Container object for model results
-        """
-        # Additional arguments
-        obs_ts = np.array(obs_ts)
-        opt_args = (dim_tuple, obs_ts, symmetric)
-        n_params = self._get_num_params(dim_tuple, symmetric)
-        bnds = self._build_optimization_bounds(n_params)
-
-        self.result = so.shgo(
-            func=LikelihoodOptimizer.calc_likelihood,
-            bounds=bnds,
-            args=opt_args,
-            sampling_method=self.algo
-        )
-
-        if symmetric:
-            return LikelihoodOptimizationResult(
-                self,
-                *self._extract_parameters_symmetric(self.result.x, *dim_tuple),
-                metadata={"local_min": self.result.xl}
-            )
-        return LikelihoodOptimizationResult(
-            self, *self._extract_parameters(self.result.x, *dim_tuple),
-            metadata={"local_min": self.result.xl}
-        )
-
-
-class EMOptimizer(CompleteLikelihoodOptimizer):
-    def __init__(
-        self, threshold: Optional[float] = 1e-8, maxiter: Optional[int] = 5000,
-        track_optimization: Optional[Union[bool, int]] = False,
-        tracking_interval: Optional[int] = 100,
-        tracking_norm: Optional[str] = 'fro',
-        **kwargs
-    ) -> None:
-        """Constructor for Expectation-Maximization optimizer
-
-        Args:
-            threshold (Optional[float], optional): update threshold below which
-                the iteration procedure for BW optimization will terminate.
-                Defaults to 1e-8.
-            maxiter (Optional[int], optional): Maximum number of iterations
-                performed before the optimizer terminates. Defaults to 5000.
-            track_optimization (Optional[Union[bool, int]], optional): Flag as
-            to whether or not internal updates to the transition and
-            observation matrices are recorded/tracked. Defaults to False.
-            tracking_interval (Optional[int], optional): Number of steps
-                between recording tracked values, only has an impact if
-                `track_optimization` is set to `True`. Defaults to 100.
-            tracking_norm (Optional[str], optional): Norm used to track matrix
-                update sizes. Can be any of the supported norms used in
-                `scipy.linalg.norm`
-                (https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.norm.html).
-                Defaults to 'fro' (Frobenius).
-        """
-        if len(kwargs) > 0:
-            warnings.warn(
-                f"Unrecognized optimizer options {kwargs}, proceeding without "
-                "using them. See documentation for valid initialization "
-                "options for EM algorithm...", RuntimeWarning
-            )
-
-        super().__init__()
-        self._opt_threshold = threshold
-        self._max_iter = maxiter
-        self._track = track_optimization
-        self._interval = tracking_interval
-        self._update_norm = tracking_norm
-
-    @staticmethod
-    @numba.jit(nopython=True)
-    def xi_matrix(
-        obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
-        alpha_norm: np.ndarray, beta_norm: np.ndarray, bayes: np.ndarray
-    ) -> np.ndarray:
-        """Routine to calculate the `xi` matrix, which represents the joint
-        probability term in the BW algorithm caluclation p(x_t, x_t-1 | Y^T)
-        For a more complete description of the term rationale, see supporting
-        documentation
-
-        Args:
-            obs_ts (np.ndarray): time series of observation values
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-            alpha_norm (np.ndarray): normalized (at point-in-time) alpha values
-                over time (dim: (n_obs, n_hidden_states))
-            beta_norm (np.ndarray): normalized (at point-in-time) beta values
-                over time (dim: (n_obs, n_hidden_states))
-            bayes (np.ndarray): Bayesian smoothed estimate of hidden state
-                probabilities (dim: (n_obs, n_hidden_states))
-
-        Returns:
-            np.ndarray: final xi-matrix, shape will be = shape(trans_matrix)
-        """
-        _shape = trans_matrix.shape
-        # Iniaitalize the xi array with all zeros
-        xi = np.zeros((*_shape, len(obs_ts) - 1))
-
-        for t in range(1, len(obs_ts)):
-            # Stack the column of observation matrix to repeat
-            stacked_obs = np.repeat(obs_matrix[:, obs_ts[t]], obs_matrix.shape[0]).reshape(*_shape)
-
-            # Outer products calculate the beta_i * alpha_j terms in the xi
-            # matrix term equation
-            numer_outer = np.outer(
-                beta_norm[t, :], (alpha_norm[t - 1, :] * bayes[t - 1, :])
-            )
-            outer_denom = np.outer(
-                beta_norm[t, :], alpha_norm[t - 1, :]
-            )
-
-            # Calculate the elements of numerator and denominator
-            numer = trans_matrix * stacked_obs * numer_outer
-            denom = np.repeat(
-                np.sum(trans_matrix * stacked_obs * outer_denom, axis=0),
-                obs_matrix.shape[0]
-            ).reshape(numer.shape).T
-
-            # Set the time-t element of the resulting xi matrix
-            xi[:, :, t - 1] = numer / denom
-
-        # Return the sum over all points in time
-        return xi.sum(axis=2)
-
-    @staticmethod
-    def _gamma_numer(obs: int, t: int, bayes: np.ndarray) -> np.ndarray:
-        """Helper routine to return a matrix with the bayesan estimate in the
-        row corresponding to the time-t observation, and zeros in the other
-
-        Args:
-            obs (int): observation value at time t
-            t (int): time index value
-            bayes (np.ndarray): bayesian state estimate at time t
-
-        Returns:
-            np.ndarray: n_state x n_state array with row `obs` replaced with
-            the bayesian estimate
-        """
-        obs_num = np.zeros((bayes.shape[1], bayes.shape[1]))
-        obs_num[obs, :] = bayes[t, :]
-        return obs_num
-
-    @staticmethod
-    # @numba.jit(nopython=True)
-    def _update_transition_matrix(
-        obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
-        alpha: np.ndarray, beta: np.ndarray, bayes: np.ndarray
-    ) -> np.ndarray:
-        """Baum-Welch update to transition matrix. This routine calls the
-        calculation of the xi-matrix (joint probability term) and divides the
-        result by the summation over all bayesian probability estimates, summed
-        over time (see supporting notebooks/documentation for a mathematical
-        rationale for each of these terms)
-
-        Args:
-            obs_ts (np.ndarray): time-series of HMM observations
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-            alpha (np.ndarray): (normed) alpha value over time
-                (dim: (n_observations, n_hidden_states))
-            beta (np.ndarray): (normed) beta value over time
-                (dim: (n_observations, n_hidden_states))
-            bayes (np.ndarray): bayesian state estimate over time
-                (dim: (n_observations, n_hidden_states))
-
-        Returns:
-            np.ndarray: Updated transition matrix
-                (dim: (n_hidden_states, n_hidden_states))
-        """
-        ratio = EMOptimizer.xi_matrix(
-            obs_ts, trans_matrix, obs_matrix, alpha, beta, bayes
-        )
-
-        bayes_matrix = np.repeat(
-            (1 / bayes[:-1, :].sum(axis=0)).reshape(1, trans_matrix.shape[0]),
-            trans_matrix.shape[1],
-            axis=0
-        )
-
-        trans_matrix_updated = ratio * bayes_matrix
-        return trans_matrix_updated
-
-    @staticmethod
-    def _update_observation_matrix(
-        obs_ts: np.ndarray, bayes: np.ndarray
-    ) -> np.ndarray:
-        """Routine to update the observation matrix, based on recorded
-        observations and the bayesian state estiamtes. See supporting
-        documentation and notebooks for a mathematical description of this term
-
-        Args:
-            obs_ts (np.ndarray): observation time-series
-            bayes (np.ndarray): bayesian state estiamtes
-
-        Returns:
-            np.ndarray: updated observation matrix
-                (dim: (n_possible_observation_values, n_hidden_states))
-        """
-        # This is almost certainly vectorizable, but I cant think of how to do it ATM...
-        gamma_mat = np.zeros((bayes.shape[1], bayes.shape[1], len(obs_ts)))
-
-        for i, obs in enumerate(obs_ts):
-            gamma_mat[:, :, i] = EMOptimizer._gamma_numer(obs, i, bayes)
-        gamma_denom = np.vstack(bayes.shape[1] * [bayes.T]).reshape(gamma_mat.shape)
-
-        return (gamma_mat.sum(axis=2) / gamma_denom.sum(axis=2))
-
-    def baum_welch_step(
-        self, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
-        obs_ts: np.ndarray
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """Single-iteration of the Baum-Welch EM algorithm: Calculate expected
-        quantities first, and then update transition matrix and observation
-        matrix estimates.
-
-        Args:
-            trans_matrix (np.ndarray): current transition matrix estimate
-            obs_matrix (np.ndarray): current observation matrix estimate
-            obs_ts (np.ndarray): observation timeseries
-
-        Returns:
-            Tuple[np.ndarray, np.ndarray]: Updated transition and observation
-                matrices (respectively)
-        """
-        # Expectation step: calculate quantities
-        _alpha = bayesian.alpha_prob(obs_ts, trans_matrix, obs_matrix, norm=True)
-        _beta = bayesian.beta_prob(obs_ts, trans_matrix, obs_matrix, norm=True)
-        _bayes = bayesian.bayes_estimate(obs_ts, trans_matrix, obs_matrix)
-
-        # Maximization step: update matrices
-        trans_matrix_updated = EMOptimizer._update_transition_matrix(
-            obs_ts, trans_matrix, obs_matrix, _alpha, _beta, _bayes
-        )
-        obs_matrix_updated = EMOptimizer._update_observation_matrix(
-            obs_ts, _bayes
-        )
-
-        return trans_matrix_updated, obs_matrix_updated
-
-    def optimize(
-        self, obs_ts: np.ndarray, trans_matrix: np.ndarray,
-        obs_matrix: np.ndarray
-    ) -> EMOptimizationResult:
-        """Main entrypoint for executing on Baum-Welch optimization procedure
-        this routine will iterate updates to the input transition and
-        observation matrices until EITHER the iteration limit is hit OR the
-        maximum change to the A or B matrix during the previous step is below
-        a threshold (both the threshold level and maximum iteration number)
-        are specified in the constructor. Here, update size is quantified by a
-        matrix norm. THe defualt is the Frobenius norm, but can be changes to
-        any of the norms supported by `scipy.linalg.norm`
-        (https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.norm.html)
-
-        Args:
-            obs_ts (np.ndarray): time series of observations
-            trans_matrix (np.ndarray): transition matrix
-            obs_matrix (np.ndarray): observation matrix
-
-        Returns:
-            EMOptimizationResult: Optimization result
-        """
-        iter_count = 0
-        update_size = self._opt_threshold + 1
-        update_tracker = []
-        if self._track:
-            trans_mat_tracker = []
-            obs_mat_tracker = []
-
-        while update_size > self._opt_threshold and iter_count < self._max_iter:
-            prev_trans, prev_obs = trans_matrix, obs_matrix
-
-            # Perform single-step update
-            trans_matrix, obs_matrix = self.baum_welch_step(
-                trans_matrix, obs_matrix, obs_ts
-            )
-
-            # Calculate update 'size'
-            update_size = np.max([
-                sl.norm(prev_trans - trans_matrix, ord=self._update_norm),
-                sl.norm(prev_obs - obs_matrix, ord=self._update_norm)
-            ])
-            update_tracker.append(update_size)
-
-            # Record the transition and observation matrices if tracking is
-            # specified
-            if self._track and (iter_count % self._interval == 0):
-                trans_mat_tracker.append(trans_matrix)
-                obs_mat_tracker.append(obs_matrix)
-            iter_count += 1
-
-        meta_dict = {}
-        if self._track:
-            meta_dict = {
-                "trans_tracker": trans_mat_tracker,
-                "obs_tracker": obs_mat_tracker
-            }
-
-        return EMOptimizationResult(
-            trans_matrix, obs_matrix, update_tracker, iter_count,
-            metadata=meta_dict
-        )
-
-
-if __name__ == "__main__":
-    import time
-    # import os
-    from hidden_py import dynamics, infer
-    from hidden_py.optimize.base import OptClass
-    # testing routines here, lets work with symmetric ''true' matrices
-    A = np.array([
-        [0.7, 0.3],
-        [0.3, 0.7]
-    ])
-
-    B = np.array([
-        [0.9, 0.1],
-        [0.1, 0.9]
-    ])
-
-    hmm = dynamics.HMM(2, 2)
-    hmm.initialize_dynamics(A, B)
-    hmm.run_dynamics(500)
-    obs_ts = hmm.get_obs_ts()
-
-    analyzer = infer.MarkovInfer(2, 2)
-
-    A_test = np.array([
-        [0.75, 0.25],
-        [0.25, 0.75]
-    ])
-
-    A_test_sym = np.array([
-        [0.8, 0.2],
-        [0.2, 0.8]
-    ])
-
-    B_test = np.array([
-        [0.95, 0.20],
-        [0.05, 0.80]
-    ])
-
-    B_test_sym = np.array([
-        [0.95, 0.05],
-        [0.05, 0.95]
-    ])
-
-    param_init_legacy = [0.2, 0.05]
-    start_leg = time.time()
-    # legacy_res = analyzer.max_likelihood(param_init_legacy, obs_ts)
-    end_leg = time.time()
-    opt = LocalLikelihoodOptimizer(algorithm="SLSQP")
-    opt_em = EMOptimizer()
-
-    start_new_nonsym = time.time()
-    # res_nosym = opt.optimize(obs_ts, A_test, B_test)
-    end_new_nonsym = time.time()
-
-    start_new_sym = time.time()
-    # res = opt.optimize(obs_ts, A_test_sym, B_test_sym, symmetric=True)
-    end_new_sym = time.time()
-
-    start_new_em = time.time()
-    res_em = opt_em.optimize(np.array(obs_ts), A_test, B_test)
-    res_em_2 = analyzer.optimize(obs_ts, A_test, B_test, opt_type=OptClass.ExpMax)
-    end_new_em = time.time()
-
-    print(f"Time Leg    : {end_leg - start_leg}")
-    print(f"Time NonSym : {end_new_nonsym - start_new_nonsym}")
-    print(f"Time Sym    : {end_new_sym - start_new_sym}")
-
-    print("--DONE--")
+from typing import Iterable, Tuple, Optional, Union
+import warnings
+import numba
+from operator import mul
+import numpy as np
+import scipy.optimize as so
+import scipy.linalg as sl
+
+from hidden_py.optimize.results import LikelihoodOptimizationResult, EMOptimizationResult
+from hidden_py.optimize.base import LikelihoodOptimizer, CompleteLikelihoodOptimizer
+from hidden_py.filters import bayesian
+
+
+class LocalLikelihoodOptimizer(LikelihoodOptimizer):
+    def __init__(
+        self, algorithm: Optional[str] = "L-BFGS-B"
+    ) -> None:
+        """Contructor for LicalLikelihoodOptimizer class
+
+        Args:
+            algorithm (Optional[str], optional): Algorithm to use in numerical
+                optimization. Defaults to "L-BFGS-B" (Limited-Memory
+                Broyden-Fletcher-Goldfarb-Shanno (BFGS) algorithm).
+        """
+        self.algo = algorithm
+        super().__init__()
+
+    def optimize(
+        self, obs_ts: Iterable, A_guess: np.ndarray, B_guess: np.ndarray,
+        symmetric: Optional[bool] = False
+    ) -> LikelihoodOptimizationResult:
+        """Routine to run actual optimization of the model. Passes off the
+        objective function and encoded parameter array to a scipy optimizer
+
+        Args:
+            obs_ts (Iterable): integer sequence of observation values
+            A_guess (np.ndarray): Initial guess at transition matrix
+            B_guess (np.ndarray): Initial guess at observation matrix
+            symmetric (Optional[bool], optional): Whether or not the model
+                (A and B matrices) are assumed to be symmetric.
+                Defaults to False.
+
+        Returns:
+            LikelihoodOptimizationResult: Container object for model results
+        """
+        # Cast observations to numpy array if they are a list
+        obs_ts = np.array(obs_ts)
+
+        # Encode model parameters into parameter vector
+        if symmetric:
+            param_init, dim_tuple = self._encode_parameters_symmetric(A_guess, B_guess)
+        else:
+            param_init, dim_tuple = self._encode_parameters(A_guess, B_guess)
+
+        # Additional arguments to pass into optimizer
+        opt_args = (dim_tuple, obs_ts, symmetric)
+        # Parameter bounds in optimization
+        bnds = self._build_optimization_bounds(len(param_init))
+
+        # run optimizer
+        self.result = so.minimize(
+            fun=LikelihoodOptimizer.calc_likelihood,
+            x0=param_init,
+            args=opt_args,
+            method=self.algo,
+            bounds=bnds
+        )
+
+        # Return results
+        if symmetric:
+            return LikelihoodOptimizationResult(
+                self,
+                *self._extract_parameters_symmetric(self.result.x, *dim_tuple)
+            )
+        return LikelihoodOptimizationResult(
+            self, *self._extract_parameters(self.result.x, *dim_tuple)
+        )
+
+
+class GlobalLikelihoodOptimizer(LikelihoodOptimizer):
+    def __init__(
+        self, sampling_algorithm: Optional[str] = "sobol"
+    ):
+        """Constructor for GlobalLikelihoodOptimizer class
+
+        Args:
+            sampling_algorithm (Optional[str], optional): algorithm to use for
+                sampling initial random points in optimization algorithm.
+                Defaults to "sobol".
+        """
+        self.algo = sampling_algorithm
+        super().__init__()
+
+    def _get_num_params(self, dim_tuple: Tuple, symmetric: bool) -> int:
+        """Utility function to determine the number fo parameters from the input
+        matrix dimensions.
+
+        Args:
+            dim_tuple (Tuple): Tuple containing the size tupled for A and B
+            symmetric (bool): Whether the problem is assumed ot be symmetric
+
+        Returns:
+            int: total number of parametsr in the problem
+        """
+        N_a = mul(*dim_tuple[0])
+        N_b = mul(*dim_tuple[1])
+
+        N_a = N_a - dim_tuple[0][1]
+        N_b = N_b - dim_tuple[1][1]
+
+        if symmetric:
+            N_a //= 2
+            N_b //= 2
+
+        return N_a + N_b
+
+    def optimize(
+        self, obs_ts: Iterable, dim_tuple: Tuple,
+        symmetric: Optional[bool] = False
+    ) -> LikelihoodOptimizationResult:
+        """Routine to run actual optimization of the model. Passes off the
+        objective function and encoded parameter array to a scipy optimizer.
+
+        This global optimizer uses the 'Simplical Homology Global Optimizer'
+        `shgo` algorithm in the scipy library.
+        See https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.shgo.html
+        or Ref[1] for an overview of the method
+
+        REFERENCES:
+            [1] Endres, SC, Sandrock, C, Focke, WW (2018) “A simplicial
+            homology algorithm for lipschitz optimisation”, Journal of Global
+            Optimization.
+
+        Args:
+            obs_ts (Iterable): Integer sequence of observations
+            dim_tuple (Tuple): dimensions of A and B matrices
+            symmetric (Optional[bool], optional): Whether or not the model
+                parameters are assumed to be symmetric.
+                Defaults to False.
+
+        Returns:
+            LikelihoodOptimizationResult: Container object for model results
+        """
+        # Additional arguments
+        obs_ts = np.array(obs_ts)
+        opt_args = (dim_tuple, obs_ts, symmetric)
+        n_params = self._get_num_params(dim_tuple, symmetric)
+        bnds = self._build_optimization_bounds(n_params)
+
+        self.result = so.shgo(
+            func=LikelihoodOptimizer.calc_likelihood,
+            bounds=bnds,
+            args=opt_args,
+            sampling_method=self.algo
+        )
+
+        if symmetric:
+            return LikelihoodOptimizationResult(
+                self,
+                *self._extract_parameters_symmetric(self.result.x, *dim_tuple),
+                metadata={"local_min": self.result.xl}
+            )
+        return LikelihoodOptimizationResult(
+            self, *self._extract_parameters(self.result.x, *dim_tuple),
+            metadata={"local_min": self.result.xl}
+        )
+
+
+class EMOptimizer(CompleteLikelihoodOptimizer):
+    def __init__(
+        self, threshold: Optional[float] = 1e-8, maxiter: Optional[int] = 5000,
+        track_optimization: Optional[Union[bool, int]] = False,
+        tracking_interval: Optional[int] = 100,
+        tracking_norm: Optional[str] = 'fro',
+        **kwargs
+    ) -> None:
+        """Constructor for Expectation-Maximization optimizer
+
+        Args:
+            threshold (Optional[float], optional): update threshold below which
+                the iteration procedure for BW optimization will terminate.
+                Defaults to 1e-8.
+            maxiter (Optional[int], optional): Maximum number of iterations
+                performed before the optimizer terminates. Defaults to 5000.
+            track_optimization (Optional[Union[bool, int]], optional): Flag as
+            to whether or not internal updates to the transition and
+            observation matrices are recorded/tracked. Defaults to False.
+            tracking_interval (Optional[int], optional): Number of steps
+                between recording tracked values, only has an impact if
+                `track_optimization` is set to `True`. Defaults to 100.
+            tracking_norm (Optional[str], optional): Norm used to track matrix
+                update sizes. Can be any of the supported norms used in
+                `scipy.linalg.norm`
+                (https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.norm.html).
+                Defaults to 'fro' (Frobenius).
+        """
+        if len(kwargs) > 0:
+            warnings.warn(
+                f"Unrecognized optimizer options {kwargs}, proceeding without "
+                "using them. See documentation for valid initialization "
+                "options for EM algorithm...", RuntimeWarning
+            )
+
+        super().__init__()
+        self._opt_threshold = threshold
+        self._max_iter = maxiter
+        self._track = track_optimization
+        self._interval = tracking_interval
+        self._update_norm = tracking_norm
+
+    @staticmethod
+    # @numba.jit(nopython=True)
+    def xi_matrix(
+        obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
+        alpha_norm: np.ndarray, beta_norm: np.ndarray, bayes: np.ndarray
+    ) -> np.ndarray:
+        """Routine to calculate the `xi` matrix, which represents the joint
+        probability term in the BW algorithm caluclation p(x_t, x_t-1 | Y^T)
+        For a more complete description of the term rationale, see supporting
+        documentation
+
+        Args:
+            obs_ts (np.ndarray): time series of observation values
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+            alpha_norm (np.ndarray): normalized (at point-in-time) alpha values
+                over time (dim: (n_obs, n_hidden_states))
+            beta_norm (np.ndarray): normalized (at point-in-time) beta values
+                over time (dim: (n_obs, n_hidden_states))
+            bayes (np.ndarray): Bayesian smoothed estimate of hidden state
+                probabilities (dim: (n_obs, n_hidden_states))
+
+        Returns:
+            np.ndarray: final xi-matrix, shape will be = shape(trans_matrix)
+        """
+        _shape = trans_matrix.shape
+        # Iniaitalize the xi array with all zeros
+        xi = np.zeros((*_shape, len(obs_ts) - 1))
+
+        for t in range(1, len(obs_ts)):
+            # Stack the column of observation matrix to repeat
+            stacked_obs = np.repeat(obs_matrix[:, obs_ts[t]], obs_matrix.shape[0]).reshape(*_shape)
+
+            # Outer products calculate the beta_i * alpha_j terms in the xi
+            # matrix term equation
+            numer_outer = np.outer(
+                beta_norm[t, :], (alpha_norm[t - 1, :] * bayes[t - 1, :])
+            )
+            outer_denom = np.outer(
+                beta_norm[t, :], alpha_norm[t - 1, :]
+            )
+
+            # Calculate the elements of numerator and denominator
+            numer = trans_matrix * stacked_obs * numer_outer
+            denom = np.repeat(
+                np.sum(trans_matrix * stacked_obs * outer_denom, axis=0),
+                obs_matrix.shape[0]
+            ).reshape(numer.shape).T
+
+            # Set the time-t element of the resulting xi matrix
+            xi[:, :, t - 1] = numer / denom
+
+        # Return the sum over all points in time
+        return xi.sum(axis=2)
+
+    @staticmethod
+    def _gamma_numer(obs: int, t: int, bayes: np.ndarray) -> np.ndarray:
+        """Helper routine to return a matrix with the bayesan estimate in the
+        row corresponding to the time-t observation, and zeros in the other
+
+        Args:
+            obs (int): observation value at time t
+            t (int): time index value
+            bayes (np.ndarray): bayesian state estimate at time t
+
+        Returns:
+            np.ndarray: n_state x n_state array with row `obs` replaced with
+            the bayesian estimate
+        """
+        obs_num = np.zeros((bayes.shape[1], bayes.shape[1]))
+        obs_num[obs, :] = bayes[t, :]
+        return obs_num
+
+    @staticmethod
+    # @numba.jit(nopython=True)
+    def _update_transition_matrix(
+        obs_ts: np.ndarray, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
+        alpha: np.ndarray, beta: np.ndarray, bayes: np.ndarray
+    ) -> np.ndarray:
+        """Baum-Welch update to transition matrix. This routine calls the
+        calculation of the xi-matrix (joint probability term) and divides the
+        result by the summation over all bayesian probability estimates, summed
+        over time (see supporting notebooks/documentation for a mathematical
+        rationale for each of these terms)
+
+        Args:
+            obs_ts (np.ndarray): time-series of HMM observations
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+            alpha (np.ndarray): (normed) alpha value over time
+                (dim: (n_observations, n_hidden_states))
+            beta (np.ndarray): (normed) beta value over time
+                (dim: (n_observations, n_hidden_states))
+            bayes (np.ndarray): bayesian state estimate over time
+                (dim: (n_observations, n_hidden_states))
+
+        Returns:
+            np.ndarray: Updated transition matrix
+                (dim: (n_hidden_states, n_hidden_states))
+        """
+        ratio = EMOptimizer.xi_matrix(
+            obs_ts, trans_matrix, obs_matrix, alpha, beta, bayes
+        )
+
+        bayes_matrix = np.repeat(
+            (1 / bayes[:-1, :].sum(axis=0)).reshape(1, trans_matrix.shape[0]),
+            trans_matrix.shape[1],
+            axis=0
+        )
+
+        trans_matrix_updated = ratio * bayes_matrix
+        return trans_matrix_updated
+
+    @staticmethod
+    def _update_observation_matrix(
+        obs_ts: np.ndarray, bayes: np.ndarray
+    ) -> np.ndarray:
+        """Routine to update the observation matrix, based on recorded
+        observations and the bayesian state estiamtes. See supporting
+        documentation and notebooks for a mathematical description of this term
+
+        Args:
+            obs_ts (np.ndarray): observation time-series
+            bayes (np.ndarray): bayesian state estiamtes
+
+        Returns:
+            np.ndarray: updated observation matrix
+                (dim: (n_possible_observation_values, n_hidden_states))
+        """
+        # This is almost certainly vectorizable, but I cant think of how to do it ATM...
+        gamma_mat = np.zeros((bayes.shape[1], bayes.shape[1], len(obs_ts)))
+
+        for i, obs in enumerate(obs_ts):
+            gamma_mat[:, :, i] = EMOptimizer._gamma_numer(obs, i, bayes)
+        gamma_denom = np.vstack(bayes.shape[1] * [bayes.T]).reshape(gamma_mat.shape)
+
+        return (gamma_mat.sum(axis=2) / gamma_denom.sum(axis=2))
+
+    def baum_welch_step(
+        self, trans_matrix: np.ndarray, obs_matrix: np.ndarray,
+        obs_ts: np.ndarray
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """Single-iteration of the Baum-Welch EM algorithm: Calculate expected
+        quantities first, and then update transition matrix and observation
+        matrix estimates.
+
+        Args:
+            trans_matrix (np.ndarray): current transition matrix estimate
+            obs_matrix (np.ndarray): current observation matrix estimate
+            obs_ts (np.ndarray): observation timeseries
+
+        Returns:
+            Tuple[np.ndarray, np.ndarray]: Updated transition and observation
+                matrices (respectively)
+        """
+        # Expectation step: calculate quantities
+        _alpha = bayesian.alpha_prob(obs_ts, trans_matrix, obs_matrix, norm=True)
+        _beta = bayesian.beta_prob(obs_ts, trans_matrix, obs_matrix, norm=True)
+        _bayes = bayesian.bayes_estimate(obs_ts, trans_matrix, obs_matrix)
+
+        # Maximization step: update matrices
+        trans_matrix_updated = EMOptimizer._update_transition_matrix(
+            obs_ts, trans_matrix, obs_matrix, _alpha, _beta, _bayes
+        )
+        obs_matrix_updated = EMOptimizer._update_observation_matrix(
+            obs_ts, _bayes
+        )
+
+        return trans_matrix_updated, obs_matrix_updated
+
+    def optimize(
+        self, obs_ts: np.ndarray, trans_matrix: np.ndarray,
+        obs_matrix: np.ndarray
+    ) -> EMOptimizationResult:
+        """Main entrypoint for executing on Baum-Welch optimization procedure
+        this routine will iterate updates to the input transition and
+        observation matrices until EITHER the iteration limit is hit OR the
+        maximum change to the A or B matrix during the previous step is below
+        a threshold (both the threshold level and maximum iteration number)
+        are specified in the constructor. Here, update size is quantified by a
+        matrix norm. THe defualt is the Frobenius norm, but can be changes to
+        any of the norms supported by `scipy.linalg.norm`
+        (https://docs.scipy.org/doc/scipy/reference/generated/scipy.linalg.norm.html)
+
+        Args:
+            obs_ts (np.ndarray): time series of observations
+            trans_matrix (np.ndarray): transition matrix
+            obs_matrix (np.ndarray): observation matrix
+
+        Returns:
+            EMOptimizationResult: Optimization result
+        """
+        iter_count = 0
+        update_size = self._opt_threshold + 1
+        update_tracker = []
+        if self._track:
+            trans_mat_tracker = []
+            obs_mat_tracker = []
+
+        while update_size > self._opt_threshold and iter_count < self._max_iter:
+            prev_trans, prev_obs = trans_matrix, obs_matrix
+
+            # Perform single-step update
+            trans_matrix, obs_matrix = self.baum_welch_step(
+                trans_matrix, obs_matrix, obs_ts
+            )
+
+            # Calculate update 'size'
+            update_size = np.max([
+                sl.norm(prev_trans - trans_matrix, ord=self._update_norm),
+                sl.norm(prev_obs - obs_matrix, ord=self._update_norm)
+            ])
+            update_tracker.append(update_size)
+
+            # Record the transition and observation matrices if tracking is
+            # specified
+            if self._track and (iter_count % self._interval == 0):
+                trans_mat_tracker.append(trans_matrix)
+                obs_mat_tracker.append(obs_matrix)
+            iter_count += 1
+
+        meta_dict = {}
+        if self._track:
+            meta_dict = {
+                "trans_tracker": trans_mat_tracker,
+                "obs_tracker": obs_mat_tracker
+            }
+
+        return EMOptimizationResult(
+            trans_matrix, obs_matrix, update_tracker, iter_count,
+            metadata=meta_dict
+        )
+
+
+if __name__ == "__main__":
+    import time
+    # import os
+    from hidden_py import dynamics, infer
+    from hidden_py.optimize.base import OptClass
+    # testing routines here, lets work with symmetric ''true' matrices
+    A = np.array([
+        [0.7, 0.3],
+        [0.3, 0.7]
+    ])
+
+    B = np.array([
+        [0.9, 0.1],
+        [0.1, 0.9]
+    ])
+
+    hmm = dynamics.HMM(2, 2)
+    hmm.initialize_dynamics(A, B)
+    hmm.run_dynamics(500)
+    obs_ts = hmm.get_obs_ts()
+
+    analyzer = infer.MarkovInfer(2, 2)
+
+    A_test = np.array([
+        [0.75, 0.25],
+        [0.25, 0.75]
+    ])
+
+    A_test_sym = np.array([
+        [0.8, 0.2],
+        [0.2, 0.8]
+    ])
+
+    B_test = np.array([
+        [0.95, 0.20],
+        [0.05, 0.80]
+    ])
+
+    B_test_sym = np.array([
+        [0.95, 0.05],
+        [0.05, 0.95]
+    ])
+
+    param_init_legacy = [0.2, 0.05]
+    start_leg = time.time()
+    # legacy_res = analyzer.max_likelihood(param_init_legacy, obs_ts)
+    end_leg = time.time()
+    opt = LocalLikelihoodOptimizer(algorithm="SLSQP")
+    opt_em = EMOptimizer()
+
+    start_new_nonsym = time.time()
+    # res_nosym = opt.optimize(obs_ts, A_test, B_test)
+    end_new_nonsym = time.time()
+
+    start_new_sym = time.time()
+    # res = opt.optimize(obs_ts, A_test_sym, B_test_sym, symmetric=True)
+    end_new_sym = time.time()
+
+    start_new_em = time.time()
+    res_em = opt_em.optimize(np.array(obs_ts), A_test, B_test)
+    res_em_2 = analyzer.optimize(obs_ts, A_test, B_test, opt_type=OptClass.ExpMax)
+    end_new_em = time.time()
+
+    print(f"Time Leg    : {end_leg - start_leg}")
+    print(f"Time NonSym : {end_new_nonsym - start_new_nonsym}")
+    print(f"Time Sym    : {end_new_sym - start_new_sym}")
+
+    print("--DONE--")
```

### Comparing `hidden-py-1.0.5/hidden_py/optimize/results.py` & `hidden-py-1.0.6/hidden_py/optimize/results.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-from abc import ABC, abstractmethod
-from typing import Optional, Dict, Iterable
-from scipy.optimize import OptimizeResult
-import numpy as np
-
-
-class OptimizationResult(ABC):
-    def __init__(
-        self, success: bool, algo_name: str,
-        results: Optional[OptimizeResult] = None
-    ):
-        self._success = success
-        self._algo_name = algo_name
-        self._results = results
-        self._report = None
-
-    @abstractmethod
-    def package_results(self):
-        pass
-
-    @property
-    def success(self) -> bool:
-        return self._success
-
-    @property
-    def summary(self) -> Dict:
-        if self._report is None:
-            return self.package_results()
-        else:
-            return self._report
-
-
-class LikelihoodOptimizationResult(OptimizationResult):
-    def __init__(
-        self, optimizer: OptimizeResult, A_opt: np.ndarray, B_opt: np.ndarray,
-        metadata: Optional[Dict] = {}
-    ):
-        super().__init__(optimizer.result.success, optimizer.algo, optimizer.result)
-        self.likelihood = optimizer.result.fun
-        self._optimal_params = optimizer.result.x
-        self.A = A_opt
-        self.B = B_opt
-        self.metadata = metadata
-
-    def package_results(self) -> Dict:
-        self._report = {
-            "trans_matrix_opt": self.A_opt,
-            "obs_matrix_opt": self.B_opt,
-            "final_likelihood": self.likelihood,
-            "success": self.success,
-            "metadata": list(self.metadata.keys())
-        }
-        return self._report
-
-
-class EMOptimizationResult(OptimizationResult):
-    def __init__(
-        self, A_opt: np.ndarray, B_opt: np.ndarray, change_tracker: Iterable,
-        iteration_count: int, metadata: Optional[Dict] = {}
-    ):
-        super().__init__(True, "baum-welch")
-        self.update_size_tracking = change_tracker
-        self._iterations = iteration_count
-        self.A = A_opt
-        self.B = B_opt
-        self.metadata = metadata
-
-    def package_results(self) -> Dict:
-        self._report = {
-            "trans_matrix_opt": self.A,
-            "obs_matrix_opt": self.B,
-            "iterations": self._iterations,
-            "final_iteration_norm": self.update_size_tracking[-1],
-            "success": True,
-            "metadata": list(self.metadata.keys())
-        }
-        return self._report
+from abc import ABC, abstractmethod
+from typing import Optional, Dict, Iterable
+from scipy.optimize import OptimizeResult
+import numpy as np
+
+
+class OptimizationResult(ABC):
+    def __init__(
+        self, success: bool, algo_name: str,
+        results: Optional[OptimizeResult] = None
+    ):
+        self._success = success
+        self._algo_name = algo_name
+        self._results = results
+        self._report = None
+
+    @abstractmethod
+    def package_results(self):
+        pass
+
+    @property
+    def success(self) -> bool:
+        return self._success
+
+    @property
+    def summary(self) -> Dict:
+        if self._report is None:
+            return self.package_results()
+        else:
+            return self._report
+
+
+class LikelihoodOptimizationResult(OptimizationResult):
+    def __init__(
+        self, optimizer: OptimizeResult, A_opt: np.ndarray, B_opt: np.ndarray,
+        metadata: Optional[Dict] = {}
+    ):
+        super().__init__(optimizer.result.success, optimizer.algo, optimizer.result)
+        self.likelihood = optimizer.result.fun
+        self._optimal_params = optimizer.result.x
+        self.A = A_opt
+        self.B = B_opt
+        self.metadata = metadata
+
+    def package_results(self) -> Dict:
+        self._report = {
+            "trans_matrix_opt": self.A_opt,
+            "obs_matrix_opt": self.B_opt,
+            "final_likelihood": self.likelihood,
+            "success": self.success,
+            "metadata": list(self.metadata.keys())
+        }
+        return self._report
+
+
+class EMOptimizationResult(OptimizationResult):
+    def __init__(
+        self, A_opt: np.ndarray, B_opt: np.ndarray, change_tracker: Iterable,
+        iteration_count: int, metadata: Optional[Dict] = {}
+    ):
+        super().__init__(True, "baum-welch")
+        self.update_size_tracking = change_tracker
+        self._iterations = iteration_count
+        self.A = A_opt
+        self.B = B_opt
+        self.metadata = metadata
+
+    def package_results(self) -> Dict:
+        self._report = {
+            "trans_matrix_opt": self.A,
+            "obs_matrix_opt": self.B,
+            "iterations": self._iterations,
+            "final_iteration_norm": self.update_size_tracking[-1],
+            "success": True,
+            "metadata": list(self.metadata.keys())
+        }
+        return self._report
```

### Comparing `hidden-py-1.0.5/hidden_py.egg-info/PKG-INFO` & `hidden-py-1.0.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,214 +1,196 @@
-Metadata-Version: 2.1
-Name: hidden-py
-Version: 1.0.5
-Summary: A python package for discrete-output hidden Markov models
-Author: Steven Large
-Author-email: stevelarge7@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/StevenJLarge/hmm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# **A Hidden Markov Model package for python**
-
-### Installation
-
-To install this package simply run the command:
-
-`pip install hidden-py`
-
-<br />
-
-## Table of Contents
-
-- [Overview](#overview)
-  - [Dynamics/Simulation](#dynamicssimulation)
-  - [System Identification](#system-identification)
-  - [Signal Processing](#signal-processing)
-- [Roadmap](#roadmap)
-- [References](#references)
-
----
-
-## Overview
-
-This package contains logic for inferring, simulating, and fitting Hidden Markov Models with discrete states and observations. This poackage serves as a complement to several common HMM packages that deal primarily with _mixture models_, where output symbols are continuous, and drawn from a distriubtion of values that is somehow conditional on the hidden state.
-
-Here, we have considered primarily scenarios where the observation value is an integer, and one of the possible hidden states, although this is not required, there could be more hidden states than possible observations, or vice-versa, all that really matters is that the observation values (and hidden state values) are discrete. There are three major use-cases for this codebase: dynamics/simulation, system identification/parameter fitting, and signal processing. In all cases, these functionalities are outlined in several tutorial notebooks in the `notebooks/tutorials` location of the [github repository](https://github.com/StevenJLarge/hmm)
-
-<br />
-
-## Hidden Markov Models
-
-Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
-
-Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
-
-<p align='center'>
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true" width="75%" vspace="30px"/>
-</p>
-
-Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step. For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
-
-$$ p_T = A^T \cdot p_0 $$
-
-A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
-
-<p align="center">
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true" width="75%" vspace="30px" />
-</p>
-
-Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
-
----
-
-As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
-
-### Dynamics/Simulation
-
-The `hidden.dynamics` submodule contains the code necessary to simulate the hidden state and observation dynamics as specified by a state transition matrix $A$ (with elements that quantify the rate of transitions between states) and an observation matrix $B$, with elements that quantify the probability of observing a given output symbol, given the current hidden state.
-
-For instance, the code necessary to initialize a hidden Markov model, run the dyanamics, and extract the observation and state time-series
-
-```python
-from hidden_py import dynamics
-
-# 2 hidden states, 2 possible observation values
-hmm = dynamics.HMM(2, 2)
-
-# Helper routine to initialize A and B matrices
-hmm.init_uniform_cycle()
-
-# Run dynamics for 100 time steps
-hmm.run_dynamics(100)
-
-# Pull out the observations, and true (simulated) hidden state values
-observations = hmm.get_obs_ts()
-hidden_states = hmm.get_state_ts()
-```
-
-As an example, the schematic below shows a possible trajectory for a HMM with 2 hidden states and 2 possible observation values.
-
-<p align="center">
-    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/sample_trajectory.png?raw=true" width="75%" vspace="30px" />
-</p>
-
-Here the red dots represent the state of the hidden system over time, while the black dots indicate the observed value at that point in time. So, at time point 3, for instance, the observed value differs from the hidden state. See the `notebooks/tutorials/02-hidden-markov-model.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) for a more in-depth review of this process.
-
-<br />
-
----
-
-### System Identification
-
-The `infer` submodule contains the code that wraps lower-level functionality (primarily in the `filters/bayesian.py` and `optimize/optimization.py` files) for both signal processing and system identification/parameter fitting.
-
-There are two separate means of performing system identification: Local/Global partial likelihood optimization, and complete-data likelihood optimization. While more comprehensive details are contained in the github notebooks, broadly speaking partial data likelihood optimization performs relatively standard optimizations on the likelihood function $\mathcal{L}(\theta | Y)$ which considers only the observations as the _data_. Effectively, these optimizers wrap the `scipy.opt.minimize` functions by encoding and decoding the $A$ and $B$ matrices into a parameter vector (ensuring that their column-normalization is preserved) and calculating the negative log-likelihood of a particular parameter vector. In practice, given a set of observations, we can initialize an `analyzer` and run either local (using, by default, the `scipy.opt.minimize` function with the `L-BFGS-B` algorithm) or global (using the `scipy` SHGO algorithm) as:
-
-```python
-from hidden_py import infer
-
-# Input the dimensions of the HMM and observations
-analyzer = infer.MarkovInfer(2, 2)
-
-# Initial estimates of the A and B matrices
-A_est = np.array([
-    [0.8, 0.1],
-    [0.2, 0.9]
-])
-
-B_est = np.array([
-    [0.9, 0.05],
-    [0.1, 0.95]
-])
-
-# Run local partial-data likelihood optimization (default behaviour), the symmetric keyword can be used to specify whether or not the A and B matrices are assumed to be symmetric
-opt_local = analyzer.optimize(observations, A_est, B_est, symmetric=False)
-
-# And the partial-data global likelihood optimization, the A and B initial matrices are not used in the optimizer, aside from providing a way of specifying the dimension of the parameter vectors
-opt_global = analyzer.optimize(observations, A_est, B_est, symmetric=False, opt_type=OptClass.Global)
-
-```
-
-Now, for the complete-data likeihood optimization, the interface is very similar, but behind the scenes the code will implement an implementation of the Baum-Welch reparameterization algorithm (an instance of an Expectation-Maximization algorithm) to find the optimal parameter values. In practice, this can be done as:
-
-```python
-from hidden_py import infer
-from hidden_py.optimize.base import OptClass
-
-analyzer = infer.MarkovInfer(2, 2)
-
-res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax)
-
-```
-
-In all cases, there is also an option to add algorithm options to customize the specifics of the optinization. Most relevant is for the expectation-maximization where you can specify a maximum number of iterations for the algorithm, as well as a threshold on the size of parameter changes (quantified by the matrix norm of pre- and post-update $A$ and $B$ matrices). This can be accessed through the `algo_opts` dictionary. For instance, if we wanted to change the maximum iterations in the BW algorithm to 1000 and set the termination threshold at `1e-10`, we would perform the previous call as
-
-```python
-options = {
-    'maxiter': 1000,
-    "threshold": 1e-10
-}
-
-res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax, algo_opts=options)
-```
-
-In essence, this set of tools allows you to infer the best model given a set of observed data. Under the hood, many of the tools from the signal processing module are used, but the `analyzer.optimize(...)` function calls largely hide that complexity.
-
-<br />
-
----
-
-### Signal Processing
-
-The `infer` submodule can also be used for the purposes of signal processing: given a valid estimate of the model parameters, how can we best estimate the hidden state value, given the observations. There are two distinct domains of application, first would be prediction in real time, where only observations in the past are available for inferring the current hidden state (this would use the so-called forward-filtered estiamte). There is also an _ex post_ approach, which uses the entirety of observations from a given period of time to estimate the hidden state at a particular point within that time period. This is the so-called Bayesian smoothed estiamte of the hidden state.
-
-Mathematically, if we denote $Y^t \equiv \{ y_0, y_1, \cdots, y_t \}$ as the sequence of observations from tie $t=0$ up to time $t$, then for a total trajectory length of $T$, the forward filter and Bayesian smoothed estimate are calculating
-
-$$
-p(x_t | Y^t) \quad \to \qquad \text{\sf Forward-filter} \\
-
-\, \\
-
-p(x_t | Y^T) \quad \to \quad \text{\sf Bayesian smoother}
-$$
-
-where, $x_t$ is the hidden state at time $t$.
-
-Quantitatively the forward filter and Bayesian smoothed estimates of a given HMM sequence of observations can be calculated in the following way:
-
-```python
-from hidden_py import infer
-
-analyzer = infer.MarkovInfer(2, 2)
-
-# Gets the forward algorithm results
-analyzer.forward_algo(observations, A, B)
-
-# Gets the Bayesian-smoothed estimate of the hidden state
-analyzer.bayesian_smooth(observations, A, B)
-
-```
-
-The tutorial notebook `notebooks/tutorials.03-slarge-hmm-filters.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) gives a more comprehensive overview and visualization of this procedure.
-
-<br />
-
----
-
-## References
-
-There is a breadth of research and literatur on HMMs out in the world, but below are a few sources that I found particularly helpful in working on this project
-
-<ol>
-    <li> <a href="https://www.cambridge.org/core/books/control-theory-for-physicists/21AFE5D6C475D1B44BCF9B8536338D98">"Control Theory for Physicists"</a>, J. Bechhoeffer, C
-    Cambridge University Press, 2021</li>
-    <li><a href="http://numerical.recipes/aboutNR3book.html">"Numerical Recipes: The Art of Scientific Computing"</a>, W.H. Press, S.A. Teukolsky, W.T. Vetterling, & B.P. Flannery, Cambridge University Press, 3rd ed., 2007</li>
-</ol>
+# **A Hidden Markov Model package for python**
+
+### Installation
+
+To install this package simply run the command:
+
+`pip install hidden-py`
+
+<br />
+
+## Table of Contents
+
+- [Overview](#overview)
+  - [Dynamics/Simulation](#dynamicssimulation)
+  - [System Identification](#system-identification)
+  - [Signal Processing](#signal-processing)
+- [Roadmap](#roadmap)
+- [References](#references)
+
+---
+
+## Overview
+
+This package contains logic for inferring, simulating, and fitting Hidden Markov Models with discrete states and observations. This poackage serves as a complement to several common HMM packages that deal primarily with _mixture models_, where output symbols are continuous, and drawn from a distriubtion of values that is somehow conditional on the hidden state.
+
+Here, we have considered primarily scenarios where the observation value is an integer, and one of the possible hidden states, although this is not required, there could be more hidden states than possible observations, or vice-versa, all that really matters is that the observation values (and hidden state values) are discrete. There are three major use-cases for this codebase: dynamics/simulation, system identification/parameter fitting, and signal processing. In all cases, these functionalities are outlined in several tutorial notebooks in the `notebooks/tutorials` location of the [github repository](https://github.com/StevenJLarge/hmm)
+
+<br />
+
+## Hidden Markov Models
+
+Markov Models are a class of stochastic models for characterizing the behaviour of systems that transition between states randomly, with a probability that depends only on the current state of the system (_i.e._ they are memoryless). Because if this simplification, the dynamics on a set of discrete states can be captured entirely by a single matrix, known as the _transition matrix_, $A$, with elements $A_{ij} = p(x_t=i | x_{t-1} = j)$ quantifying the probability that during timestep $t-1 \to t$, the system will transition from state $j\to i$. Because of the normalization of probability, the columns of $A$ are constrained to be equal to unity.
+
+Without any ambiguity in the observed value (_i.e._ the underlying Markov model is directly observed) the system is just a Markov model. The causal diagram of a Markov model is shown in the figure below.
+
+<p align='center'>
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/markov_schematic.png?raw=true" width="75%" vspace="30px"/>
+</p>
+
+Here, the state $x_t$ at time $t$ only depends on the state at the previous time $t-1$. As a result the ecolution of a probability distribution over states can be modelled by simply multiplying an initial distribution by the transition matrix, and repeating the process for each time step. For example, given an initial distribution over states at time 0 and a transition matrix $A$, the probability distribution at time $T$ is
+
+$$ p_T = A^T \cdot p_0 $$
+
+A hidden Markov model (HMM), on the other hand, is a probabilistic function of a Markov model. This means that the output of an HMM (th0e observation $y$) is correlated with the underlying (hidden/unobserved) state of the Markov model, but only probabilitsically so. For a set of discrete possible observations (as we capture in this package), the observation process can also be modelled by a matrix (the _observation matrix_) $B$ with elemetnts $B_{ij} = p(y_t = i | x_{t} = j)$ quantifying the probability that our measurement/observation $y_t$ at time $t$ is equal to $i$ given the hidden system is in state $j$. Here, the diagonal elements represent our probability of observing the _correct_ state, while off-diagonals represent the probability of error. In comparison to the figure used in the Markov system, the below diagram shows how causality works in a hidden Markov model.
+
+<p align="center">
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/hidden_markov_schematic.png?raw=true" width="75%" vspace="30px" />
+</p>
+
+Here, the observations ($y_t$) are stochastic (random) functions of the underlying state, but not necessarily equal to it. However (importantly) the observation at time $t$ only depends explicitly on the hiddenstate at time $t$.
+
+---
+
+As for the components of the package, the goal of the simulation functionality is simply to generate trajectories of both the hidden state and observation time-series that are conistent with these probabilities. The goal for system identification/parameter fitting is to fit the most likely parameters (elements of the $A$ and $B$) matrices, given only a time series of observations. Finally, the goal if signal processing is to make use of the observation sequence to infer what the hidden state is at a particular point in time.
+
+### Dynamics/Simulation
+
+The `hidden.dynamics` submodule contains the code necessary to simulate the hidden state and observation dynamics as specified by a state transition matrix $A$ (with elements that quantify the rate of transitions between states) and an observation matrix $B$, with elements that quantify the probability of observing a given output symbol, given the current hidden state.
+
+For instance, the code necessary to initialize a hidden Markov model, run the dyanamics, and extract the observation and state time-series
+
+```python
+from hidden_py import dynamics
+
+# 2 hidden states, 2 possible observation values
+hmm = dynamics.HMM(2, 2)
+
+# Helper routine to initialize A and B matrices
+hmm.init_uniform_cycle()
+
+# Run dynamics for 100 time steps
+hmm.run_dynamics(100)
+
+# Pull out the observations, and true (simulated) hidden state values
+observations = hmm.get_obs_ts()
+hidden_states = hmm.get_state_ts()
+```
+
+As an example, the schematic below shows a possible trajectory for a HMM with 2 hidden states and 2 possible observation values.
+
+<p align="center">
+    <img src="https://github.com/StevenJLarge/hmm/blob/master/public/resources/sample_trajectory.png?raw=true" width="75%" vspace="30px" />
+</p>
+
+Here the red dots represent the state of the hidden system over time, while the black dots indicate the observed value at that point in time. So, at time point 3, for instance, the observed value differs from the hidden state. See the `notebooks/tutorials/02-hidden-markov-model.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) for a more in-depth review of this process.
+
+<br />
+
+---
+
+### System Identification
+
+The `infer` submodule contains the code that wraps lower-level functionality (primarily in the `filters/bayesian.py` and `optimize/optimization.py` files) for both signal processing and system identification/parameter fitting.
+
+There are two separate means of performing system identification: Local/Global partial likelihood optimization, and complete-data likelihood optimization. While more comprehensive details are contained in the github notebooks, broadly speaking partial data likelihood optimization performs relatively standard optimizations on the likelihood function $\mathcal{L}(\theta | Y)$ which considers only the observations as the _data_. Effectively, these optimizers wrap the `scipy.opt.minimize` functions by encoding and decoding the $A$ and $B$ matrices into a parameter vector (ensuring that their column-normalization is preserved) and calculating the negative log-likelihood of a particular parameter vector. In practice, given a set of observations, we can initialize an `analyzer` and run either local (using, by default, the `scipy.opt.minimize` function with the `L-BFGS-B` algorithm) or global (using the `scipy` SHGO algorithm) as:
+
+```python
+from hidden_py import infer
+
+# Input the dimensions of the HMM and observations
+analyzer = infer.MarkovInfer(2, 2)
+
+# Initial estimates of the A and B matrices
+A_est = np.array([
+    [0.8, 0.1],
+    [0.2, 0.9]
+])
+
+B_est = np.array([
+    [0.9, 0.05],
+    [0.1, 0.95]
+])
+
+# Run local partial-data likelihood optimization (default behaviour), the symmetric keyword can be used to specify whether or not the A and B matrices are assumed to be symmetric
+opt_local = analyzer.optimize(observations, A_est, B_est, symmetric=False)
+
+# And the partial-data global likelihood optimization, the A and B initial matrices are not used in the optimizer, aside from providing a way of specifying the dimension of the parameter vectors
+opt_global = analyzer.optimize(observations, A_est, B_est, symmetric=False, opt_type=OptClass.Global)
+
+```
+
+Now, for the complete-data likeihood optimization, the interface is very similar, but behind the scenes the code will implement an implementation of the Baum-Welch reparameterization algorithm (an instance of an Expectation-Maximization algorithm) to find the optimal parameter values. In practice, this can be done as:
+
+```python
+from hidden_py import infer
+from hidden_py.optimize.base import OptClass
+
+analyzer = infer.MarkovInfer(2, 2)
+
+res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax)
+
+```
+
+In all cases, there is also an option to add algorithm options to customize the specifics of the optinization. Most relevant is for the expectation-maximization where you can specify a maximum number of iterations for the algorithm, as well as a threshold on the size of parameter changes (quantified by the matrix norm of pre- and post-update $A$ and $B$ matrices). This can be accessed through the `algo_opts` dictionary. For instance, if we wanted to change the maximum iterations in the BW algorithm to 1000 and set the termination threshold at `1e-10`, we would perform the previous call as
+
+```python
+options = {
+    'maxiter': 1000,
+    "threshold": 1e-10
+}
+
+res_bw = analyzer.optimize(observations, A_est, B_est, opt_type=OptClass.ExpMax, algo_opts=options)
+```
+
+In essence, this set of tools allows you to infer the best model given a set of observed data. Under the hood, many of the tools from the signal processing module are used, but the `analyzer.optimize(...)` function calls largely hide that complexity.
+
+<br />
+
+---
+
+### Signal Processing
+
+The `infer` submodule can also be used for the purposes of signal processing: given a valid estimate of the model parameters, how can we best estimate the hidden state value, given the observations. There are two distinct domains of application, first would be prediction in real time, where only observations in the past are available for inferring the current hidden state (this would use the so-called forward-filtered estiamte). There is also an _ex post_ approach, which uses the entirety of observations from a given period of time to estimate the hidden state at a particular point within that time period. This is the so-called Bayesian smoothed estiamte of the hidden state.
+
+Mathematically, if we denote $Y^t \equiv \{ y_0, y_1, \cdots, y_t \}$ as the sequence of observations from tie $t=0$ up to time $t$, then for a total trajectory length of $T$, the forward filter and Bayesian smoothed estimate are calculating
+
+$$
+p(x_t | Y^t) \quad \to \qquad \text{\sf Forward-filter} \\
+
+\, \\
+
+p(x_t | Y^T) \quad \to \quad \text{\sf Bayesian smoother}
+$$
+
+where, $x_t$ is the hidden state at time $t$.
+
+Quantitatively the forward filter and Bayesian smoothed estimates of a given HMM sequence of observations can be calculated in the following way:
+
+```python
+from hidden_py import infer
+
+analyzer = infer.MarkovInfer(2, 2)
+
+# Gets the forward algorithm results
+analyzer.forward_algo(observations, A, B)
+
+# Gets the Bayesian-smoothed estimate of the hidden state
+analyzer.bayesian_smooth(observations, A, B)
+
+```
+
+The tutorial notebook `notebooks/tutorials.03-slarge-hmm-filters.ipynb` in the [github source](https://github.com/StevenJLarge/hmm) gives a more comprehensive overview and visualization of this procedure.
+
+<br />
+
+---
+
+## References
+
+There is a breadth of research and literatur on HMMs out in the world, but below are a few sources that I found particularly helpful in working on this project
+
+<ol>
+    <li> <a href="https://www.cambridge.org/core/books/control-theory-for-physicists/21AFE5D6C475D1B44BCF9B8536338D98">"Control Theory for Physicists"</a>, J. Bechhoeffer, C
+    Cambridge University Press, 2021</li>
+    <li><a href="http://numerical.recipes/aboutNR3book.html">"Numerical Recipes: The Art of Scientific Computing"</a>, W.H. Press, S.A. Teukolsky, W.T. Vetterling, & B.P. Flannery, Cambridge University Press, 3rd ed., 2007</li>
+</ol>
```

### Comparing `hidden-py-1.0.5/hidden_py.egg-info/SOURCES.txt` & `hidden-py-1.0.6/hidden_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hidden-py-1.0.5/setup.py` & `hidden-py-1.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from setuptools import find_packages, setup
-
-# README contents
-with open('README.md', 'r', encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    name='hidden-py',
-    packages=find_packages(),
-    version="1.0.5",
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    description='''
-        A python package for discrete-output hidden Markov models
-    ''',
-    author='Steven Large',
-    author_email='stevelarge7@gmail.com',
-    license='MIT',
-    install_requires=[
-        'pytest',
-        'numpy',
-        'scipy',
-        'matplotlib',
-        'seaborn >= 0.11.1',
-        'numba'
-    ],
-    project_urls={
-        'Source': 'https://github.com/StevenJLarge/hmm'
-    },
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        "Programming Language :: Python",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence",
-        "Topic :: Scientific/Engineering :: Physics",
-        "Topic :: Scientific/Engineering :: Mathematics"
-    ]
-)
+from setuptools import find_packages, setup
+
+# README contents
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    name='hidden-py',
+    packages=find_packages(),
+    version="1.0.6",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    description='''
+        A python package for discrete-output hidden Markov models
+    ''',
+    author='Steven Large',
+    author_email='stevelarge7@gmail.com',
+    license='MIT',
+    install_requires=[
+        'pytest',
+        'numpy',
+        'scipy',
+        'matplotlib',
+        'seaborn >= 0.11.1',
+        'numba'
+    ],
+    project_urls={
+        'Source': 'https://github.com/StevenJLarge/hmm'
+    },
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: MIT License',
+        "Programming Language :: Python",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Scientific/Engineering :: Physics",
+        "Topic :: Scientific/Engineering :: Mathematics"
+    ]
+)
```

### Comparing `hidden-py-1.0.5/tests/test_filters.py` & `hidden-py-1.0.6/tests/test_filters.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,381 +1,381 @@
-import numpy as np
-import pytest
-import itertools
-
-from hidden_py import dynamics
-from hidden_py.filters import bayesian
-
-
-# Test suite for filters routines
-TEST_ITERATIONS = 3
-
-# Global configureations
-A_test_2 = np.array([
-    [0.8, 0.3],
-    [0.2, 0.7]
-])
-
-A_test_3 = np.array([
-    [0.8, 0.2, 0.0],
-    [0.1, 0.7, 0.1],
-    [0.1, 0.1, 0.9]
-])
-
-B_test_2 = np.array([
-    [0.9, 0.05],
-    [0.1, 0.95]
-])
-
-B_test_3 = np.array([
-    [0.85, 0.05, 0.10],
-    [0.10, 0.90, 0.10],
-    [0.05, 0.05, 0.80]
-])
-
-
-@pytest.fixture
-def test_hmm_2():
-    hmm = dynamics.HMM(2, 2)
-    hmm.A = A_test_2
-    hmm.B = B_test_2
-    return hmm
-
-
-@pytest.fixture
-def test_hmm_3():
-    hmm = dynamics.HMM(3, 3)
-    hmm.A = A_test_3
-    hmm.B = B_test_3
-    return hmm
-
-
-def sample_hmm(n_dim):
-    hmm = dynamics.HMM(n_dim, n_dim)
-    hmm.init_uniform_cycle(0.15, 0.1)
-    return hmm
-
-
-filter_functions = [
-    bayesian.bayes_estimate,
-    bayesian.forward_algo,
-    bayesian.backward_algo,
-    bayesian.alpha_prob,
-    bayesian.beta_prob
-]
-
-
-filter_test_data = [
-    (np.array([0.80, 0.20]), 2),
-    (np.array([0.50, 0.50]), 2),
-    (np.array([0.01, 0.99]), 2),
-    (np.array([0.15, 0.85]), 2),
-    (np.array([0.70, 0.20, 0.10]), 3),
-    (np.array([0.33, 0.33, 0.34]), 3),
-    (np.array([0.01, 0.98, 0.01]), 3),
-    (np.array([0.15, 0.75, 0.10]), 3),
-]
-
-sample_A_2 = np.array([
-    [0.7, 0.3],
-    [0.3, 0.7]
-])
-sample_B_2 = np.array([
-    [0.9, 0.1],
-    [0.1, 0.9]
-])
-
-sample_A_3 = np.array([
-    [0.6, 0.2, 0.2],
-    [0.2, 0.6, 0.2],
-    [0.2, 0.2, 0.6]
-])
-sample_B_3 = np.array([
-    [0.8, 0.1, 0.1],
-    [0.1, 0.8, 0.1],
-    [0.1, 0.1, 0.8]
-])
-
-
-sample_obs_seq_2 = np.array([1, 1, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 1, 0, 1])
-sample_obs_seq_3 = np.array([1, 0, 0, 0, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2])
-
-bayes_2_ini = np.array([0.05934857, 0.94065143])
-bayes_2_fin = np.array([0.16365312, 0.83634688])
-alpha_2_ini = np.array([0.1, 0.9])
-alpha_2_fin = np.array([1.16607475e-05, 5.95920813e-05])
-beta_2_ini = np.array([4.22875327e-05, 7.44711950e-05])
-beta_2_fin = np.array([1.0, 1.0])
-
-bayes_3_ini = np.array([0.22251862, 0.69124149, 0.08623989])
-bayes_3_fin = np.array([0.04392142, 0.04392197, 0.91215661])
-alpha_3_ini = np.array([0.1, 0.8, 0.1])
-alpha_3_fin = np.array([2.12415158e-07, 2.12417828e-07, 4.41142152e-06])
-beta_3_ini = np.array([1.07615669e-05, 4.17877471e-06, 4.17078047e-06])
-beta_3_fin = np.array([1.0, 1.0, 1.0])
-
-bayes_test_data = (
-    [sample_A_2, sample_B_2, sample_obs_seq_2, bayes_2_ini, bayes_2_fin],
-    [sample_A_3, sample_B_3, sample_obs_seq_3, bayes_3_ini, bayes_3_fin]
-)
-
-alpha_test_data = (
-    [sample_A_2, sample_B_2, sample_obs_seq_2, alpha_2_ini, alpha_2_fin],
-    [sample_A_3, sample_B_3, sample_obs_seq_3, alpha_3_ini, alpha_3_fin]
-)
-
-beta_test_data = (
-    [sample_A_2, sample_B_2, sample_obs_seq_2, beta_2_ini, beta_2_fin],
-    [sample_A_3, sample_B_3, sample_obs_seq_3, beta_3_ini, beta_3_fin]
-)
-
-norm_test_samples = [
-    [A_test_2, B_test_2],
-    [A_test_3, B_test_3]
-]
-
-
-@pytest.mark.parametrize(['filter_func', 'N'], itertools.product(filter_functions, [2, 3]))
-def test_return_from_estimate_is_correct_shape_2d(filter_func, N):
-    # Arrange
-    n_steps = 10
-    pred = None
-
-    test_hmm = sample_hmm(N)
- 
-    # Act
-    test_hmm.run_dynamics(n_steps)
-    obs_ts = np.array(test_hmm.get_obs_ts())
-    res = filter_func(obs_ts, test_hmm.A, test_hmm.B)
-
-    if isinstance(res, tuple):
-        pred = res[1]
-        res = res[0]
-
-    # Assert
-    assert res.shape == (n_steps, test_hmm.n_sys)
-    if pred is not None:
-        assert pred.shape == (n_steps, test_hmm.n_sys)
-
-
-# @pytest.mark.repeat(5)
-@pytest.mark.parametrize(['N'], [[2], [3]])
-def test_forward_algo_stays_normalized(N):
-    # Arange
-    test_model = sample_hmm(N)
-    test_model.init_uniform_cycle()
-    n_steps = 15
-
-    # Act
-    test_model.run_dynamics(n_steps)
-    obs = test_model.get_obs_ts()
-    fwd_tracker, _ = bayesian.forward_algo(obs, test_model.A, test_model.B)
-
-    # Assert
-    assert all(np.isclose(np.ones(n_steps), np.sum(fwd_tracker, axis=1)))
-
-
-# @pytest.mark.repeat(5)
-@pytest.mark.parametrize(['N'], [[2], [3]])
-def test_backward_algo_stays_normalized(N):
-    # Arange
-    test_model = sample_hmm(N)
-    test_model.init_uniform_cycle()
-    n_steps = 15
-
-    # Act
-    test_model.run_dynamics(n_steps)
-    obs = test_model.get_obs_ts()
-    back_tracker, _ = bayesian.backward_algo(np.array(obs), test_model.A, test_model.B)
-
-    # Assert
-    assert all(np.isclose(np.ones(n_steps), np.sum(back_tracker, axis=1)))
-
-
-# @pytest.mark.repeat(10)
-@pytest.mark.parametrize(['N', 'exec_num'], list(itertools.product([2, 3], range(10))))
-def test_bayesian_algo_stays_normalized(N, exec_num):
-    # Arange
-    test_model = sample_hmm(N)
-    test_model.init_uniform_cycle()
-    n_steps = 15
-
-    # Act
-    test_model.run_dynamics(n_steps)
-    obs = test_model.get_obs_ts()
-    bayes_tracker = bayesian.bayes_estimate(np.array(obs), test_model.A, test_model.B)
-
-    # Assert
-    assert all(np.isclose(np.ones(n_steps), np.sum(bayes_tracker, axis=1)))
-
-
-@pytest.mark.parametrize(['fwd_init', 'N'], filter_test_data)
-def test_forward_filter_equations(fwd_init, N):
-    # Arrange
-    test_model = sample_hmm(N)
-    obs = 1
-
-    # Act
-    # Prediction step
-    fwd_pred = test_model.A @ fwd_init
-    # Observation step
-    fwd_filter = test_model.B[:, obs] * fwd_pred
-    fwd_filter = fwd_filter / np.sum(fwd_filter)
-
-    # Perform forward filter inside the bayesian module
-    res = bayesian._forward_filter(np.array(obs), test_model.A, test_model.B, fwd_init)
-    fwd_filter_prod = res[0]
-    fwd_pred_prod = res[1]
-
-    # Assert
-    assert all(np.isclose(fwd_filter, fwd_filter_prod))
-    assert all(np.isclose(fwd_pred, fwd_pred_prod))
-
-
-@pytest.mark.parametrize(['back_init', 'N'], filter_test_data)
-def test_backward_filter_equations(back_init, N):
-    # Arrange
-    test_model = sample_hmm(N)
-    obs = 1
-
-    # Act
-    # Backwards prediction
-    back_pred = test_model.A.T @ back_init
-    # Observation step
-    back_filter = test_model.B[obs, :] * back_pred
-    back_filter = back_filter / np.sum(back_filter)
-
-    # Perform backward filter using the module
-    res = bayesian._forward_filter(np.array(obs), test_model.A.T, test_model.B.T, back_init)
-    back_filter_prod = res[0]
-    back_pred_prod = res[1]
-
-    # Assert
-    assert all(np.isclose(back_filter, back_filter_prod))
-    assert all(np.isclose(back_pred, back_pred_prod))
-
-
-@pytest.mark.parametrize(['A', 'B', 'obs', 'bayes_i', 'bayes_f'], bayes_test_data)
-def test_bayesian_smoothing_equation(A, B, obs, bayes_i, bayes_f):
-    # Act
-    bayes_tracker = bayesian.bayes_estimate(obs, A, B)
-
-    # Assert
-    assert all(np.isclose(bayes_tracker[0, :], bayes_i))
-    assert all(np.isclose(bayes_tracker[-1, :], bayes_f))
-
-
-@pytest.mark.parametrize(['A', 'B', 'obs', 'alpha_i', 'alpha_f'], alpha_test_data)
-def test_alpha_calculation(A, B, obs, alpha_i, alpha_f):
-    # Act
-    alpha_tracker = bayesian.alpha_prob(obs, A, B)
-
-    # Assert
-    assert all(np.isclose(alpha_tracker[0, :], alpha_i))
-    assert all(np.isclose(alpha_tracker[-1, :], alpha_f))
-
-
-@pytest.mark.parametrize(['A', 'B', 'obs', 'beta_i', 'beta_f'], beta_test_data)
-def test_beta_calculation(A, B, obs, beta_i, beta_f):
-    # Act
-    beta_tracker = bayesian.beta_prob(obs, A, B)
-
-    # Assert
-    assert all(np.isclose(beta_tracker[0, :], beta_i))
-    assert all(np.isclose(beta_tracker[-1, :], beta_f))
-
-
-@ pytest.mark.parametrize(['A', 'B', 'obs', 'alpha_i', "alpha_f"], alpha_test_data)
-def test_alpha_is_state_normalized_when_keyword_is_passed(A, B, obs, alpha_i, alpha_f):
-    # Act
-    alpha_norm = bayesian.alpha_prob(obs, A, B, norm=True)
-
-    # Assert
-    assert all(np.isclose(alpha_norm.sum(axis=1), 1.0))
-
-
-@ pytest.mark.parametrize(['A', 'B', 'obs', 'beta_i', "beta_f"], beta_test_data)
-def test_beta_is_state_normalized_when_keyword_is_passed(A, B, obs, beta_i, beta_f):
-    # Act
-    beta_norm = bayesian.beta_prob(obs, A, B, norm=True)
-
-    # Assert
-    assert all(np.isclose(beta_norm.sum(axis=1), 1.0))
-
-
-@ pytest.mark.parametrize(['A', 'B', 'obs', 'alpha_i', "alpha_f"], alpha_test_data)
-def test_alpha_normalized_result(A, B, obs, alpha_i, alpha_f):
-    # Act
-    alpha_norm = bayesian.alpha_prob(obs, A, B, norm=True)
-
-    # Assert
-    assert all(np.isclose(alpha_norm[0, :], alpha_i / sum(alpha_i)))
-    assert all(np.isclose(alpha_norm[-1, :], alpha_f / sum(alpha_f)))
-
-
-@ pytest.mark.parametrize(['A', 'B', 'obs', 'beta_i', "beta_f"], beta_test_data)
-def test_beta_normalized_result(A, B, obs, beta_i, beta_f):
-    # Act
-    beta_norm = bayesian.beta_prob(obs, A, B, norm=True)
-
-    # Assert
-    assert all(np.isclose(beta_norm[0, :], beta_i / sum(beta_i)))
-    assert all(np.isclose(beta_norm[-1, :], beta_f / sum(beta_f)))
-
-
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], norm_test_samples)
-def test_forward_filter_normalization(A_matrix, B_matrix, iteration):
-    # Arrange
-    n_steps = 100
-    _ = iteration
-    hmm = dynamics.HMM(A_matrix.shape[0], B_matrix.shape[0])
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-
-    # Act, second arg is prediction tracker
-    fwd_tracker, _ = bayesian.forward_algo(obs_ts, A_matrix, B_matrix)
-
-    print(fwd_tracker)
-    # Assert
-    assert np.all(np.isclose(fwd_tracker.sum(axis=1), np.ones(fwd_tracker.shape[0])))
-
-
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', "B_matrix"], norm_test_samples)
-def test_backward_filter_normalization(A_matrix, B_matrix, iteration):
-    # Arrange
-    _ = iteration
-    n_steps = 100
-    hmm = dynamics.HMM(A_matrix.shape[0], B_matrix.shape[0])
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-
-    # Act
-    back_tracker, _ = bayesian.backward_algo(obs_ts, A_matrix, B_matrix)
-
-    # Assert
-    assert np.all(np.isclose(back_tracker.sum(axis=1), np.ones(back_tracker.shape[0])))
-
-
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', "B_matrix"], norm_test_samples)
-def test_bayes_filter_normalization(A_matrix, B_matrix, iteration):
-    # Arrange
-    _ = iteration
-    n_steps = 100
-    hmm = dynamics.HMM(*A_matrix.shape)
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-
-    # Act
-    bayes_tracker = bayesian.bayes_estimate(obs_ts, A_matrix, B_matrix)
-
-    # Assert
-    assert np.all(np.isclose(bayes_tracker.sum(axis=1), np.ones(bayes_tracker.shape[0])))
-
-
-if __name__ == "__main__":
-    pytest.main([__file__])
+import numpy as np
+import pytest
+import itertools
+
+from hidden_py import dynamics
+from hidden_py.filters import bayesian
+
+
+# Test suite for filters routines
+TEST_ITERATIONS = 3
+
+# Global configureations
+A_test_2 = np.array([
+    [0.8, 0.3],
+    [0.2, 0.7]
+])
+
+A_test_3 = np.array([
+    [0.8, 0.2, 0.0],
+    [0.1, 0.7, 0.1],
+    [0.1, 0.1, 0.9]
+])
+
+B_test_2 = np.array([
+    [0.9, 0.05],
+    [0.1, 0.95]
+])
+
+B_test_3 = np.array([
+    [0.85, 0.05, 0.10],
+    [0.10, 0.90, 0.10],
+    [0.05, 0.05, 0.80]
+])
+
+
+@pytest.fixture
+def test_hmm_2():
+    hmm = dynamics.HMM(2, 2)
+    hmm.A = A_test_2
+    hmm.B = B_test_2
+    return hmm
+
+
+@pytest.fixture
+def test_hmm_3():
+    hmm = dynamics.HMM(3, 3)
+    hmm.A = A_test_3
+    hmm.B = B_test_3
+    return hmm
+
+
+def sample_hmm(n_dim):
+    hmm = dynamics.HMM(n_dim, n_dim)
+    hmm.init_uniform_cycle(0.15, 0.1)
+    return hmm
+
+
+filter_functions = [
+    bayesian.bayes_estimate,
+    bayesian.forward_algo,
+    bayesian.backward_algo,
+    bayesian.alpha_prob,
+    bayesian.beta_prob
+]
+
+
+filter_test_data = [
+    (np.array([0.80, 0.20]), 2),
+    (np.array([0.50, 0.50]), 2),
+    (np.array([0.01, 0.99]), 2),
+    (np.array([0.15, 0.85]), 2),
+    (np.array([0.70, 0.20, 0.10]), 3),
+    (np.array([0.33, 0.33, 0.34]), 3),
+    (np.array([0.01, 0.98, 0.01]), 3),
+    (np.array([0.15, 0.75, 0.10]), 3),
+]
+
+sample_A_2 = np.array([
+    [0.7, 0.3],
+    [0.3, 0.7]
+])
+sample_B_2 = np.array([
+    [0.9, 0.1],
+    [0.1, 0.9]
+])
+
+sample_A_3 = np.array([
+    [0.6, 0.2, 0.2],
+    [0.2, 0.6, 0.2],
+    [0.2, 0.2, 0.6]
+])
+sample_B_3 = np.array([
+    [0.8, 0.1, 0.1],
+    [0.1, 0.8, 0.1],
+    [0.1, 0.1, 0.8]
+])
+
+
+sample_obs_seq_2 = np.array([1, 1, 0, 1, 1, 1, 1, 0, 0, 0, 0, 0, 1, 0, 1])
+sample_obs_seq_3 = np.array([1, 0, 0, 0, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 2])
+
+bayes_2_ini = np.array([0.05934857, 0.94065143])
+bayes_2_fin = np.array([0.16365312, 0.83634688])
+alpha_2_ini = np.array([0.1, 0.9])
+alpha_2_fin = np.array([1.16607475e-05, 5.95920813e-05])
+beta_2_ini = np.array([4.22875327e-05, 7.44711950e-05])
+beta_2_fin = np.array([1.0, 1.0])
+
+bayes_3_ini = np.array([0.22251862, 0.69124149, 0.08623989])
+bayes_3_fin = np.array([0.04392142, 0.04392197, 0.91215661])
+alpha_3_ini = np.array([0.1, 0.8, 0.1])
+alpha_3_fin = np.array([2.12415158e-07, 2.12417828e-07, 4.41142152e-06])
+beta_3_ini = np.array([1.07615669e-05, 4.17877471e-06, 4.17078047e-06])
+beta_3_fin = np.array([1.0, 1.0, 1.0])
+
+bayes_test_data = (
+    [sample_A_2, sample_B_2, sample_obs_seq_2, bayes_2_ini, bayes_2_fin],
+    [sample_A_3, sample_B_3, sample_obs_seq_3, bayes_3_ini, bayes_3_fin]
+)
+
+alpha_test_data = (
+    [sample_A_2, sample_B_2, sample_obs_seq_2, alpha_2_ini, alpha_2_fin],
+    [sample_A_3, sample_B_3, sample_obs_seq_3, alpha_3_ini, alpha_3_fin]
+)
+
+beta_test_data = (
+    [sample_A_2, sample_B_2, sample_obs_seq_2, beta_2_ini, beta_2_fin],
+    [sample_A_3, sample_B_3, sample_obs_seq_3, beta_3_ini, beta_3_fin]
+)
+
+norm_test_samples = [
+    [A_test_2, B_test_2],
+    [A_test_3, B_test_3]
+]
+
+
+@pytest.mark.parametrize(['filter_func', 'N'], itertools.product(filter_functions, [2, 3]))
+def test_return_from_estimate_is_correct_shape_2d(filter_func, N):
+    # Arrange
+    n_steps = 10
+    pred = None
+
+    test_hmm = sample_hmm(N)
+ 
+    # Act
+    test_hmm.run_dynamics(n_steps)
+    obs_ts = np.array(test_hmm.get_obs_ts())
+    res = filter_func(obs_ts, test_hmm.A, test_hmm.B)
+
+    if isinstance(res, tuple):
+        pred = res[1]
+        res = res[0]
+
+    # Assert
+    assert res.shape == (n_steps, test_hmm.n_sys)
+    if pred is not None:
+        assert pred.shape == (n_steps, test_hmm.n_sys)
+
+
+# @pytest.mark.repeat(5)
+@pytest.mark.parametrize(['N'], [[2], [3]])
+def test_forward_algo_stays_normalized(N):
+    # Arange
+    test_model = sample_hmm(N)
+    test_model.init_uniform_cycle()
+    n_steps = 15
+
+    # Act
+    test_model.run_dynamics(n_steps)
+    obs = test_model.get_obs_ts()
+    fwd_tracker, _ = bayesian.forward_algo(obs, test_model.A, test_model.B)
+
+    # Assert
+    assert all(np.isclose(np.ones(n_steps), np.sum(fwd_tracker, axis=1)))
+
+
+# @pytest.mark.repeat(5)
+@pytest.mark.parametrize(['N'], [[2], [3]])
+def test_backward_algo_stays_normalized(N):
+    # Arange
+    test_model = sample_hmm(N)
+    test_model.init_uniform_cycle()
+    n_steps = 15
+
+    # Act
+    test_model.run_dynamics(n_steps)
+    obs = test_model.get_obs_ts()
+    back_tracker, _ = bayesian.backward_algo(np.array(obs), test_model.A, test_model.B)
+
+    # Assert
+    assert all(np.isclose(np.ones(n_steps), np.sum(back_tracker, axis=1)))
+
+
+# @pytest.mark.repeat(10)
+@pytest.mark.parametrize(['N', 'exec_num'], list(itertools.product([2, 3], range(10))))
+def test_bayesian_algo_stays_normalized(N, exec_num):
+    # Arange
+    test_model = sample_hmm(N)
+    test_model.init_uniform_cycle()
+    n_steps = 15
+
+    # Act
+    test_model.run_dynamics(n_steps)
+    obs = test_model.get_obs_ts()
+    bayes_tracker = bayesian.bayes_estimate(np.array(obs), test_model.A, test_model.B)
+
+    # Assert
+    assert all(np.isclose(np.ones(n_steps), np.sum(bayes_tracker, axis=1)))
+
+
+@pytest.mark.parametrize(['fwd_init', 'N'], filter_test_data)
+def test_forward_filter_equations(fwd_init, N):
+    # Arrange
+    test_model = sample_hmm(N)
+    obs = 1
+
+    # Act
+    # Prediction step
+    fwd_pred = test_model.A @ fwd_init
+    # Observation step
+    fwd_filter = test_model.B[:, obs] * fwd_pred
+    fwd_filter = fwd_filter / np.sum(fwd_filter)
+
+    # Perform forward filter inside the bayesian module
+    res = bayesian._forward_filter(np.array(obs), test_model.A, test_model.B, fwd_init)
+    fwd_filter_prod = res[0]
+    fwd_pred_prod = res[1]
+
+    # Assert
+    assert all(np.isclose(fwd_filter, fwd_filter_prod))
+    assert all(np.isclose(fwd_pred, fwd_pred_prod))
+
+
+@pytest.mark.parametrize(['back_init', 'N'], filter_test_data)
+def test_backward_filter_equations(back_init, N):
+    # Arrange
+    test_model = sample_hmm(N)
+    obs = 1
+
+    # Act
+    # Backwards prediction
+    back_pred = test_model.A.T @ back_init
+    # Observation step
+    back_filter = test_model.B[obs, :] * back_pred
+    back_filter = back_filter / np.sum(back_filter)
+
+    # Perform backward filter using the module
+    res = bayesian._forward_filter(np.array(obs), test_model.A.T, test_model.B.T, back_init)
+    back_filter_prod = res[0]
+    back_pred_prod = res[1]
+
+    # Assert
+    assert all(np.isclose(back_filter, back_filter_prod))
+    assert all(np.isclose(back_pred, back_pred_prod))
+
+
+@pytest.mark.parametrize(['A', 'B', 'obs', 'bayes_i', 'bayes_f'], bayes_test_data)
+def test_bayesian_smoothing_equation(A, B, obs, bayes_i, bayes_f):
+    # Act
+    bayes_tracker = bayesian.bayes_estimate(obs, A, B)
+
+    # Assert
+    assert all(np.isclose(bayes_tracker[0, :], bayes_i))
+    assert all(np.isclose(bayes_tracker[-1, :], bayes_f))
+
+
+@pytest.mark.parametrize(['A', 'B', 'obs', 'alpha_i', 'alpha_f'], alpha_test_data)
+def test_alpha_calculation(A, B, obs, alpha_i, alpha_f):
+    # Act
+    alpha_tracker = bayesian.alpha_prob(obs, A, B)
+
+    # Assert
+    assert all(np.isclose(alpha_tracker[0, :], alpha_i))
+    assert all(np.isclose(alpha_tracker[-1, :], alpha_f))
+
+
+@pytest.mark.parametrize(['A', 'B', 'obs', 'beta_i', 'beta_f'], beta_test_data)
+def test_beta_calculation(A, B, obs, beta_i, beta_f):
+    # Act
+    beta_tracker = bayesian.beta_prob(obs, A, B)
+
+    # Assert
+    assert all(np.isclose(beta_tracker[0, :], beta_i))
+    assert all(np.isclose(beta_tracker[-1, :], beta_f))
+
+
+@ pytest.mark.parametrize(['A', 'B', 'obs', 'alpha_i', "alpha_f"], alpha_test_data)
+def test_alpha_is_state_normalized_when_keyword_is_passed(A, B, obs, alpha_i, alpha_f):
+    # Act
+    alpha_norm = bayesian.alpha_prob(obs, A, B, norm=True)
+
+    # Assert
+    assert all(np.isclose(alpha_norm.sum(axis=1), 1.0))
+
+
+@ pytest.mark.parametrize(['A', 'B', 'obs', 'beta_i', "beta_f"], beta_test_data)
+def test_beta_is_state_normalized_when_keyword_is_passed(A, B, obs, beta_i, beta_f):
+    # Act
+    beta_norm = bayesian.beta_prob(obs, A, B, norm=True)
+
+    # Assert
+    assert all(np.isclose(beta_norm.sum(axis=1), 1.0))
+
+
+@ pytest.mark.parametrize(['A', 'B', 'obs', 'alpha_i', "alpha_f"], alpha_test_data)
+def test_alpha_normalized_result(A, B, obs, alpha_i, alpha_f):
+    # Act
+    alpha_norm = bayesian.alpha_prob(obs, A, B, norm=True)
+
+    # Assert
+    assert all(np.isclose(alpha_norm[0, :], alpha_i / sum(alpha_i)))
+    assert all(np.isclose(alpha_norm[-1, :], alpha_f / sum(alpha_f)))
+
+
+@ pytest.mark.parametrize(['A', 'B', 'obs', 'beta_i', "beta_f"], beta_test_data)
+def test_beta_normalized_result(A, B, obs, beta_i, beta_f):
+    # Act
+    beta_norm = bayesian.beta_prob(obs, A, B, norm=True)
+
+    # Assert
+    assert all(np.isclose(beta_norm[0, :], beta_i / sum(beta_i)))
+    assert all(np.isclose(beta_norm[-1, :], beta_f / sum(beta_f)))
+
+
+@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], norm_test_samples)
+def test_forward_filter_normalization(A_matrix, B_matrix, iteration):
+    # Arrange
+    n_steps = 100
+    _ = iteration
+    hmm = dynamics.HMM(A_matrix.shape[0], B_matrix.shape[0])
+    hmm.init_uniform_cycle()
+    hmm.run_dynamics(n_steps)
+    obs_ts = np.array(hmm.get_obs_ts())
+
+    # Act, second arg is prediction tracker
+    fwd_tracker, _ = bayesian.forward_algo(obs_ts, A_matrix, B_matrix)
+
+    print(fwd_tracker)
+    # Assert
+    assert np.all(np.isclose(fwd_tracker.sum(axis=1), np.ones(fwd_tracker.shape[0])))
+
+
+@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+@pytest.mark.parametrize(['A_matrix', "B_matrix"], norm_test_samples)
+def test_backward_filter_normalization(A_matrix, B_matrix, iteration):
+    # Arrange
+    _ = iteration
+    n_steps = 100
+    hmm = dynamics.HMM(A_matrix.shape[0], B_matrix.shape[0])
+    hmm.init_uniform_cycle()
+    hmm.run_dynamics(n_steps)
+    obs_ts = np.array(hmm.get_obs_ts())
+
+    # Act
+    back_tracker, _ = bayesian.backward_algo(obs_ts, A_matrix, B_matrix)
+
+    # Assert
+    assert np.all(np.isclose(back_tracker.sum(axis=1), np.ones(back_tracker.shape[0])))
+
+
+@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+@pytest.mark.parametrize(['A_matrix', "B_matrix"], norm_test_samples)
+def test_bayes_filter_normalization(A_matrix, B_matrix, iteration):
+    # Arrange
+    _ = iteration
+    n_steps = 100
+    hmm = dynamics.HMM(*A_matrix.shape)
+    hmm.init_uniform_cycle()
+    hmm.run_dynamics(n_steps)
+    obs_ts = np.array(hmm.get_obs_ts())
+
+    # Act
+    bayes_tracker = bayesian.bayes_estimate(obs_ts, A_matrix, B_matrix)
+
+    # Assert
+    assert np.all(np.isclose(bayes_tracker.sum(axis=1), np.ones(bayes_tracker.shape[0])))
+
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

### Comparing `hidden-py-1.0.5/tests/test_optimizers.py` & `hidden-py-1.0.6/tests/test_optimizers.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,260 +1,260 @@
-# Testing suite for inferrence routines
-import operator
-import pytest
-import numpy as np
-from hidden_py.dynamics import HMM
-from hidden_py.optimize import base, optimization
-from hidden_py.filters import bayesian
-
-TEST_ITERATIONS = 3
-
-A_test_2 = np.array([[0.7, 0.2], [0.3, 0.8]])
-A_test_2_sym = np.array([[0.7, 0.3], [0.3, 0.7]])
-
-B_test_2 = np.array([[0.9, 0.01], [0.1, 0.99]])
-B_test_2_sym = np.array([[0.9, 0.1], [0.1, 0.9]])
-
-A_test_3 = np.array([
-    [0.8, 0.1, 0.2],
-    [0.1, 0.7, 0.2],
-    [0.1, 0.2, 0.6]
-])
-
-A_test_3_sym = np.array([
-    [0.7, 0.1, 0.2],
-    [0.1, 0.7, 0.2],
-    [0.2, 0.2, 0.6]
-])
-
-B_test_3 = np.array([
-    [0.98, 0.1, 0.4],
-    [0.01, 0.7, 0.3],
-    [0.01, 0.2, 0.3]
-])
-
-B_test_3_sym = np.array([
-    [0.7, 0.1, 0.2],
-    [0.1, 0.6, 0.3],
-    [0.2, 0.3, 0.5]
-])
-
-test_2_enc = np.array([0.2, 0.3, 0.01, 0.1])
-test_2_enc_sym = np.array([0.3, 0.1])
-
-test_3_enc = np.array(
-    [0.1, 0.2, 0.1, 0.2, 0.1, 0.2, 0.1, 0.4, 0.01, 0.3, 0.01, 0.2]
-)
-test_3_enc_sym = np.array([0.1, 0.2, 0.2, 0.1, 0.2, 0.3])
-
-test_data = [[A_test_2, B_test_2], [A_test_3, B_test_3]]
-test_data_sym = [[A_test_2_sym, B_test_2_sym], [A_test_3_sym, B_test_3_sym]]
-
-test_data_comp = [
-    [A_test_2, B_test_2, test_2_enc],
-    [A_test_3, B_test_3, test_3_enc]
-]
-
-test_data_comp_sym = [
-    [A_test_2_sym, B_test_2_sym, test_2_enc_sym],
-    [A_test_3_sym, B_test_3_sym, test_3_enc_sym]
-]
-
-
-# IO tests
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_encoding_dimensions(A_matrix, B_matrix):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act
-    _, dim = opt._encode_parameters(A_matrix, B_matrix)
-
-    # Assert
-    assert dim[0] == A_matrix.shape
-    assert dim[1] == B_matrix.shape
-
-
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_encoded_length(A_matrix, B_matrix):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act
-    encoded, _ = opt._encode_parameters(A_matrix, B_matrix)
-
-    # Assert
-    assert (
-        len(encoded) == (
-            operator.mul(*A_matrix.shape)
-            + operator.mul(*B_matrix.shape)
-            - A_matrix.shape[1]
-            - B_matrix.shape[1]
-        )
-    )
-
-
-@pytest.mark.parametrize(['A_matrix', "B_matrix"], test_data_sym)
-def test_encoded_length_symmetric(A_matrix, B_matrix):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act
-    encoded, _ = opt._encode_parameters_symmetric(A_matrix, B_matrix)
-
-    # Assert
-    assert (
-        len(encoded) == (
-            (operator.mul(*A_matrix.shape) - A_matrix.shape[0]) // 2
-            + (operator.mul(*B_matrix.shape) - B_matrix.shape[0]) // 2
-        )
-    )
-
-
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data_sym)
-def test_non_square_matrix_in_symmetric_encoding_raises(A_matrix, B_matrix):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act/Assert
-    with pytest.raises(ValueError):
-        _ = opt._encode_parameters_symmetric(A_matrix[:-1, :], B_matrix)
-        _ = opt._encode_parameters_symmetric(A_matrix, B_matrix[1:, :])
-
-
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_non_symmetric_matrix_in_symmtric_encoding_raises(A_matrix, B_matrix):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act/Assert
-    with pytest.raises(ValueError):
-        _ = opt._encode_parameters_symmetric(A_matrix, B_matrix)
-
-
-# test matrix encoding and parameter extraction
-@pytest.mark.parametrize(['A_matrix', 'B_matrix', 'compressed'], test_data_comp)
-def test_matrix_encoding(A_matrix, B_matrix, compressed):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act
-    encoded, dim = opt._encode_parameters(A_matrix, B_matrix)
-
-    # Assert
-    assert all(encoded == compressed)
-    assert dim[0] == A_matrix.shape
-    assert dim[1] == B_matrix.shape
-
-
-@pytest.mark.parametrize(["A_matrix", "B_matrix", "compressed"], test_data_comp_sym)
-def test_matrix_encoding_symmetric(A_matrix, B_matrix, compressed):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act
-    encoded, dim = opt._encode_parameters_symmetric(A_matrix, B_matrix)
-
-    # Assert
-    assert all(encoded == compressed)
-    assert dim[0] == A_matrix.shape
-    assert dim[1] == B_matrix.shape
-
-
-# Test matrix decoding as well
-@pytest.mark.parametrize(['A_matrix', 'B_matrix', 'compressed'], test_data_comp)
-def test_matrix_decoding(A_matrix, B_matrix, compressed):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act
-    A_decode, B_decode = opt._extract_parameters(compressed, A_matrix.shape, B_matrix.shape)
-
-    # Assert
-    assert np.all(np.isclose(A_decode, A_matrix))
-    assert np.all(np.isclose(B_decode, B_matrix))
-
-
-@pytest.mark.parametrize(['A_matrix', 'B_matrix', 'compressed'], test_data_comp_sym)
-def test_matrix_decoding_symmetric(A_matrix, B_matrix, compressed):
-    # Arrange
-    opt = base.TestLikelihoodOptimizer()
-
-    # Act
-    A_decode, B_decode = opt._extract_parameters_symmetric(compressed, A_matrix.shape, B_matrix.shape)
-
-    # Assert
-    assert np.all(np.isclose(A_decode, A_matrix))
-    assert np.all(np.isclose(B_decode, B_matrix))
-
-
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_xi_matrix_shape(A_matrix, B_matrix, iteration):
-    # Arrange
-    _ = iteration
-    n_steps = 100
-    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-    opt = optimization.EMOptimizer()
-
-    # Act
-    alpha_mat = bayesian.alpha_prob(obs_ts, A_matrix, B_matrix, norm=True)
-    beta_mat = bayesian.beta_prob(obs_ts, A_matrix, B_matrix, norm=True)
-    bayes_mat = bayesian.bayes_estimate(obs_ts, A_matrix, B_matrix)
-
-    sample_xi = opt.xi_matrix(
-        obs_ts, A_matrix, B_matrix, alpha_mat, beta_mat, bayes_mat
-    )
-
-    # Assert
-    assert sample_xi.shape == (hmm.A.shape)
-
-
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_bw_update_preserves_A_matrix_normalization(A_matrix, B_matrix, iteration):
-    # Arrange
-    _ = iteration
-    n_steps = 10
-    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-    opt = optimization.EMOptimizer()
-
-    # Act
-    A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
-    A_new_2, _ = opt.baum_welch_step(A_new, B_new, obs_ts)
-
-    # Assert
-    assert all(np.isclose(A_new.sum(axis=0), np.ones(A_new.shape[1])))
-    assert all(np.isclose(A_new_2.sum(axis=0), np.ones(A_new_2.shape[1])))
-
-
-@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
-@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
-def test_bw_update_preserves_B_matrix_normalization(A_matrix, B_matrix, iteration):
-    # Arrange
-    _ = iteration
-    n_steps = 10
-    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
-    hmm.init_uniform_cycle()
-    hmm.run_dynamics(n_steps)
-    obs_ts = np.array(hmm.get_obs_ts())
-    opt = optimization.EMOptimizer()
-
-    # Act
-    A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
-    _, B_new_2 = opt.baum_welch_step(A_new, B_new, obs_ts)
-
-    # Assert
-    assert all(np.isclose(B_new.sum(axis=0), np.ones(B_new.shape[1])))
-    assert all(np.isclose(B_new_2.sum(axis=0), np.ones(B_new_2.shape[1])))
-
-
-if __name__ == "__main__":
-    # pytest.main([__file__])
-    for i, (A, B) in enumerate(test_data):
-        test_bw_update_preserves_A_matrix_normalization(A, B, i)
+# Testing suite for inferrence routines
+import operator
+import pytest
+import numpy as np
+from hidden_py.dynamics import HMM
+from hidden_py.optimize import base, optimization
+from hidden_py.filters import bayesian
+
+TEST_ITERATIONS = 3
+
+A_test_2 = np.array([[0.7, 0.2], [0.3, 0.8]])
+A_test_2_sym = np.array([[0.7, 0.3], [0.3, 0.7]])
+
+B_test_2 = np.array([[0.9, 0.01], [0.1, 0.99]])
+B_test_2_sym = np.array([[0.9, 0.1], [0.1, 0.9]])
+
+A_test_3 = np.array([
+    [0.8, 0.1, 0.2],
+    [0.1, 0.7, 0.2],
+    [0.1, 0.2, 0.6]
+])
+
+A_test_3_sym = np.array([
+    [0.7, 0.1, 0.2],
+    [0.1, 0.7, 0.2],
+    [0.2, 0.2, 0.6]
+])
+
+B_test_3 = np.array([
+    [0.98, 0.1, 0.4],
+    [0.01, 0.7, 0.3],
+    [0.01, 0.2, 0.3]
+])
+
+B_test_3_sym = np.array([
+    [0.7, 0.1, 0.2],
+    [0.1, 0.6, 0.3],
+    [0.2, 0.3, 0.5]
+])
+
+test_2_enc = np.array([0.2, 0.3, 0.01, 0.1])
+test_2_enc_sym = np.array([0.3, 0.1])
+
+test_3_enc = np.array(
+    [0.1, 0.2, 0.1, 0.2, 0.1, 0.2, 0.1, 0.4, 0.01, 0.3, 0.01, 0.2]
+)
+test_3_enc_sym = np.array([0.1, 0.2, 0.2, 0.1, 0.2, 0.3])
+
+test_data = [[A_test_2, B_test_2], [A_test_3, B_test_3]]
+test_data_sym = [[A_test_2_sym, B_test_2_sym], [A_test_3_sym, B_test_3_sym]]
+
+test_data_comp = [
+    [A_test_2, B_test_2, test_2_enc],
+    [A_test_3, B_test_3, test_3_enc]
+]
+
+test_data_comp_sym = [
+    [A_test_2_sym, B_test_2_sym, test_2_enc_sym],
+    [A_test_3_sym, B_test_3_sym, test_3_enc_sym]
+]
+
+
+# IO tests
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+def test_encoding_dimensions(A_matrix, B_matrix):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act
+    _, dim = opt._encode_parameters(A_matrix, B_matrix)
+
+    # Assert
+    assert dim[0] == A_matrix.shape
+    assert dim[1] == B_matrix.shape
+
+
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+def test_encoded_length(A_matrix, B_matrix):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act
+    encoded, _ = opt._encode_parameters(A_matrix, B_matrix)
+
+    # Assert
+    assert (
+        len(encoded) == (
+            operator.mul(*A_matrix.shape)
+            + operator.mul(*B_matrix.shape)
+            - A_matrix.shape[1]
+            - B_matrix.shape[1]
+        )
+    )
+
+
+@pytest.mark.parametrize(['A_matrix', "B_matrix"], test_data_sym)
+def test_encoded_length_symmetric(A_matrix, B_matrix):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act
+    encoded, _ = opt._encode_parameters_symmetric(A_matrix, B_matrix)
+
+    # Assert
+    assert (
+        len(encoded) == (
+            (operator.mul(*A_matrix.shape) - A_matrix.shape[0]) // 2
+            + (operator.mul(*B_matrix.shape) - B_matrix.shape[0]) // 2
+        )
+    )
+
+
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data_sym)
+def test_non_square_matrix_in_symmetric_encoding_raises(A_matrix, B_matrix):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act/Assert
+    with pytest.raises(ValueError):
+        _ = opt._encode_parameters_symmetric(A_matrix[:-1, :], B_matrix)
+        _ = opt._encode_parameters_symmetric(A_matrix, B_matrix[1:, :])
+
+
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+def test_non_symmetric_matrix_in_symmtric_encoding_raises(A_matrix, B_matrix):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act/Assert
+    with pytest.raises(ValueError):
+        _ = opt._encode_parameters_symmetric(A_matrix, B_matrix)
+
+
+# test matrix encoding and parameter extraction
+@pytest.mark.parametrize(['A_matrix', 'B_matrix', 'compressed'], test_data_comp)
+def test_matrix_encoding(A_matrix, B_matrix, compressed):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act
+    encoded, dim = opt._encode_parameters(A_matrix, B_matrix)
+
+    # Assert
+    assert all(encoded == compressed)
+    assert dim[0] == A_matrix.shape
+    assert dim[1] == B_matrix.shape
+
+
+@pytest.mark.parametrize(["A_matrix", "B_matrix", "compressed"], test_data_comp_sym)
+def test_matrix_encoding_symmetric(A_matrix, B_matrix, compressed):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act
+    encoded, dim = opt._encode_parameters_symmetric(A_matrix, B_matrix)
+
+    # Assert
+    assert all(encoded == compressed)
+    assert dim[0] == A_matrix.shape
+    assert dim[1] == B_matrix.shape
+
+
+# Test matrix decoding as well
+@pytest.mark.parametrize(['A_matrix', 'B_matrix', 'compressed'], test_data_comp)
+def test_matrix_decoding(A_matrix, B_matrix, compressed):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act
+    A_decode, B_decode = opt._extract_parameters(compressed, A_matrix.shape, B_matrix.shape)
+
+    # Assert
+    assert np.all(np.isclose(A_decode, A_matrix))
+    assert np.all(np.isclose(B_decode, B_matrix))
+
+
+@pytest.mark.parametrize(['A_matrix', 'B_matrix', 'compressed'], test_data_comp_sym)
+def test_matrix_decoding_symmetric(A_matrix, B_matrix, compressed):
+    # Arrange
+    opt = base.TestLikelihoodOptimizer()
+
+    # Act
+    A_decode, B_decode = opt._extract_parameters_symmetric(compressed, A_matrix.shape, B_matrix.shape)
+
+    # Assert
+    assert np.all(np.isclose(A_decode, A_matrix))
+    assert np.all(np.isclose(B_decode, B_matrix))
+
+
+@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+def test_xi_matrix_shape(A_matrix, B_matrix, iteration):
+    # Arrange
+    _ = iteration
+    n_steps = 100
+    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
+    hmm.init_uniform_cycle()
+    hmm.run_dynamics(n_steps)
+    obs_ts = np.array(hmm.get_obs_ts())
+    opt = optimization.EMOptimizer()
+
+    # Act
+    alpha_mat = bayesian.alpha_prob(obs_ts, A_matrix, B_matrix, norm=True)
+    beta_mat = bayesian.beta_prob(obs_ts, A_matrix, B_matrix, norm=True)
+    bayes_mat = bayesian.bayes_estimate(obs_ts, A_matrix, B_matrix)
+
+    sample_xi = opt.xi_matrix(
+        obs_ts, A_matrix, B_matrix, alpha_mat, beta_mat, bayes_mat
+    )
+
+    # Assert
+    assert sample_xi.shape == (hmm.A.shape)
+
+
+@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+def test_bw_update_preserves_A_matrix_normalization(A_matrix, B_matrix, iteration):
+    # Arrange
+    _ = iteration
+    n_steps = 10
+    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
+    hmm.init_uniform_cycle()
+    hmm.run_dynamics(n_steps)
+    obs_ts = np.array(hmm.get_obs_ts())
+    opt = optimization.EMOptimizer()
+
+    # Act
+    A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
+    A_new_2, _ = opt.baum_welch_step(A_new, B_new, obs_ts)
+
+    # Assert
+    assert all(np.isclose(A_new.sum(axis=0), np.ones(A_new.shape[1])))
+    assert all(np.isclose(A_new_2.sum(axis=0), np.ones(A_new_2.shape[1])))
+
+
+@pytest.mark.parametrize('iteration', range(TEST_ITERATIONS))
+@pytest.mark.parametrize(['A_matrix', 'B_matrix'], test_data)
+def test_bw_update_preserves_B_matrix_normalization(A_matrix, B_matrix, iteration):
+    # Arrange
+    _ = iteration
+    n_steps = 10
+    hmm = HMM(A_matrix.shape[0], B_matrix.shape[0])
+    hmm.init_uniform_cycle()
+    hmm.run_dynamics(n_steps)
+    obs_ts = np.array(hmm.get_obs_ts())
+    opt = optimization.EMOptimizer()
+
+    # Act
+    A_new, B_new = opt.baum_welch_step(A_matrix, B_matrix, obs_ts)
+    _, B_new_2 = opt.baum_welch_step(A_new, B_new, obs_ts)
+
+    # Assert
+    assert all(np.isclose(B_new.sum(axis=0), np.ones(B_new.shape[1])))
+    assert all(np.isclose(B_new_2.sum(axis=0), np.ones(B_new_2.shape[1])))
+
+
+if __name__ == "__main__":
+    # pytest.main([__file__])
+    for i, (A, B) in enumerate(test_data):
+        test_bw_update_preserves_A_matrix_normalization(A, B, i)
```

