# Comparing `tmp/hdlib-0.1.8.tar.gz` & `tmp/hdlib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hdlib-0.1.8.tar", last modified: Fri Jun 30 17:05:33 2023, max compression
+gzip compressed data, was "hdlib-0.1.9.tar", last modified: Fri Jul  7 15:14:21 2023, max compression
```

## Comparing `hdlib-0.1.8.tar` & `hdlib-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.8/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     3317 2023-06-30 17:05:33.000000 hdlib-0.1.8/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)     2225 2023-06-13 01:38:11.000000 hdlib-0.1.8/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/hdlib/
--rw-r--r--   0 fabio      (501) staff       (20)      102 2023-06-30 15:21:23.000000 hdlib-0.1.8/hdlib/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     5724 2023-06-30 15:21:08.000000 hdlib-0.1.8/hdlib/arithmetic.py
--rw-r--r--   0 fabio      (501) staff       (20)    33770 2023-06-30 16:36:29.000000 hdlib-0.1.8/hdlib/model.py
--rw-r--r--   0 fabio      (501) staff       (20)     3862 2023-06-30 14:42:35.000000 hdlib-0.1.8/hdlib/parser.py
--rw-r--r--   0 fabio      (501) staff       (20)    41140 2023-06-30 15:26:03.000000 hdlib-0.1.8/hdlib/space.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/hdlib.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     3317 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      295 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       50 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        6 2023-06-30 17:05:32.000000 hdlib-0.1.8/hdlib.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-06-30 17:05:33.000000 hdlib-0.1.8/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1462 2023-06-15 14:40:58.000000 hdlib-0.1.8/setup.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-06-30 17:05:33.000000 hdlib-0.1.8/test/
--rw-r--r--   0 fabio      (501) staff       (20)     8036 2023-06-30 16:29:04.000000 hdlib-0.1.8/test/test.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-07-07 15:14:21.014284 hdlib-0.1.9/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2022-04-25 18:30:15.000000 hdlib-0.1.9/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     3870 2023-07-07 15:14:21.012981 hdlib-0.1.9/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)     3047 2023-07-04 21:42:59.000000 hdlib-0.1.9/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-07-07 15:14:20.915703 hdlib-0.1.9/hdlib/
+-rw-r--r--   0 fabio      (501) staff       (20)      101 2023-07-07 14:52:50.000000 hdlib-0.1.9/hdlib/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     5724 2023-06-30 15:21:08.000000 hdlib-0.1.9/hdlib/arithmetic.py
+-rw-r--r--   0 fabio      (501) staff       (20)    34691 2023-07-07 14:59:28.000000 hdlib-0.1.9/hdlib/model.py
+-rw-r--r--   0 fabio      (501) staff       (20)     3862 2023-06-30 14:42:35.000000 hdlib-0.1.9/hdlib/parser.py
+-rw-r--r--   0 fabio      (501) staff       (20)    41140 2023-06-30 15:26:03.000000 hdlib-0.1.9/hdlib/space.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-07-07 15:14:20.988094 hdlib-0.1.9/hdlib.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     3870 2023-07-07 15:14:19.000000 hdlib-0.1.9/hdlib.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      295 2023-07-07 15:14:20.000000 hdlib-0.1.9/hdlib.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-07-07 15:14:19.000000 hdlib-0.1.9/hdlib.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-07-07 15:14:19.000000 hdlib-0.1.9/hdlib.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       50 2023-07-07 15:14:20.000000 hdlib-0.1.9/hdlib.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        6 2023-07-07 15:14:20.000000 hdlib-0.1.9/hdlib.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-07-07 15:14:21.014641 hdlib-0.1.9/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1462 2023-06-15 14:40:58.000000 hdlib-0.1.9/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-07-07 15:14:20.990615 hdlib-0.1.9/test/
+-rw-r--r--   0 fabio      (501) staff       (20)     8036 2023-06-30 16:29:04.000000 hdlib-0.1.9/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `hdlib-0.1.8/LICENSE` & `hdlib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.8/hdlib/arithmetic.py` & `hdlib-0.1.9/hdlib/arithmetic.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.8/hdlib/model.py` & `hdlib-0.1.9/hdlib/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -440,59 +440,77 @@
             class_vector.tags.add(class_label)
 
             class_vectors.append(class_vector)
 
         # Retrieve the test vectors from the space        
         test_vectors = self.space.get(names=test_points)
 
+        # Also retrieve the training vectors from the space
+        training_vectors = self.space.get(names=training_points)
+
+        # Make a copy of the vector representation of classes for retraining the model
         retraining_class_vectors = copy.deepcopy(class_vectors)
 
-        # Retrain model
+        # Count retraining iterations
         retraining_iterations = 0
 
-        # Take track of the predictions in the last retraining iteration 
-        last_predictions = dict()
-
-        # Take track of the number of wrongly predicted points for the best retraining iteration
-        best_wrong_predictions = len(test_vectors)
-
-        best_prediction = list()
+        # Take track of the error rate while retraining the model
+        last_error_rate = 1.0
 
         while retrain + 1 > 0:
             if retraining_iterations > 0:
-                wrong_predictions = 0
+                wrongly_redicted_training_vectors = 0
 
-                for test_point in last_predictions:
+                for training_point in training_points:
                     true_class = None
 
-                    # Retrieve the test vector tags
-                    for test_vector in test_vectors:
-                        if test_vector.name == test_point:
+                    # Retrieve the training vector tags
+                    for training_vector in training_vectors:
+                        if training_vector.name == training_point:
                             # Vectors contain only their class info in tags
-                            true_class = list(test_vector.tags)[0]
+                            true_class = list(training_vector.tags)[0]
 
                             break
 
                     if true_class != None:
-                        # In case the test point has been wrongly predicted
-                        if last_predictions[test_point] != true_class:
-                            wrong_predictions += 1
+                        closest_class = None
+                        closest_dist = np.NINF
 
-                            for class_vector in retraining_class_vectors:
-                                if last_predictions[test_point] in class_vector.tags:
-                                    class_vector.vector = class_vector.vector - test_vector.vector
+                        for class_vector in retraining_class_vectors:
+                            # Compute the distance between the training points and the hyperdimensional representations of classes
+                            with np.errstate(invalid="ignore", divide="ignore"):
+                                distance = training_vector.dist(class_vector, method=distance_method)
+
+                            if closest_class is None:
+                                closest_class = list(class_vector.tags)[0]
+                                closest_dist = distance
+
+                            else:
+                                if distance > closest_dist:
+                                    closest_class = list(class_vector.tags)[0]
+                                    closest_dist = distance
 
+                        if closest_class != true_class:
+                            # Try to mitigate the error
+                            for class_vector in retraining_class_vectors:
                                 if true_class in class_vector.tags:
-                                    class_vector.vector = class_vector.vector + test_vector.vector
+                                    class_vector.vector = class_vector.vector + training_vector.vector
 
-                if wrong_predictions < best_wrong_predictions:
-                    best_wrong_predictions = wrong_predictions
+                                elif closest_class in class_vector.tags:
+                                    class_vector.vector = class_vector.vector - training_vector.vector
 
-                    # Get the last prediction
-                    best_prediction = prediction
+                            wrongly_redicted_training_vectors += 1
+
+                error_rate = wrongly_redicted_training_vectors / len(training_points)
+
+                if last_error_rate < error_rate:
+                    # Does not make sense to keep retraining if the error rate increases compared to the previous iteration
+                    break
+
+                last_error_rate = error_rate
 
             prediction = list()
 
             for test_vector in sorted(test_vectors, key=lambda vector: test_indices.index(int(vector.name.split("_")[-1]))):
                 closest_class = None
                 closest_dist = np.NINF
 
@@ -506,25 +524,20 @@
                         closest_dist = distance
 
                     else:
                         if distance > closest_dist:
                             closest_class = list(class_vector.tags)[0]
                             closest_dist = distance
 
-                last_predictions[test_vector.name] = closest_class
-
                 prediction.append(closest_class)
 
             retraining_iterations += 1
 
             retrain -= 1
 
-        if best_prediction:
-            prediction = best_prediction
-
         return test_indices, prediction, retraining_iterations
 
     def cross_val_predict(
         self,
         points: List[List[float]],
         labels: List[str],
         cv: int=5,
```

### Comparing `hdlib-0.1.8/hdlib/parser.py` & `hdlib-0.1.9/hdlib/parser.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.8/hdlib/space.py` & `hdlib-0.1.9/hdlib/space.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.8/setup.py` & `hdlib-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `hdlib-0.1.8/test/test.py` & `hdlib-0.1.9/test/test.py`

 * *Files identical despite different names*

