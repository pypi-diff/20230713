# Comparing `tmp/helperfns-0.0.4.tar.gz` & `tmp/helperfns-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\helperfns-0.0.4.tar", last modified: Mon Jul  3 10:22:18 2023, max compression
+gzip compressed data, was "dist\helperfns-0.0.5.tar", last modified: Thu Jul 13 11:20:16 2023, max compression
```

## Comparing `helperfns-0.0.4.tar` & `helperfns-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.464961 helperfns-0.0.4/
--rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     8223 2023-07-03 10:22:18.454963 helperfns-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6526 2022-09-01 10:27:40.000000 helperfns-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.345964 helperfns-0.0.4/helperfns/
--rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.4/helperfns/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.417960 helperfns-0.0.4/helperfns/tables/
--rw-rw-rw-   0        0        0     1917 2023-07-03 10:15:06.000000 helperfns-0.0.4/helperfns/tables/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.423964 helperfns-0.0.4/helperfns/text/
--rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.4/helperfns/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.427959 helperfns-0.0.4/helperfns/torch/
--rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.4/helperfns/torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.430962 helperfns-0.0.4/helperfns/torch/accuracy/
--rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.4/helperfns/torch/accuracy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.434971 helperfns-0.0.4/helperfns/torch/models/
--rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.4/helperfns/torch/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.440964 helperfns-0.0.4/helperfns/torch/text/
--rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.4/helperfns/torch/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.444962 helperfns-0.0.4/helperfns/utils/
--rw-rw-rw-   0        0        0      775 2022-08-25 07:27:13.000000 helperfns-0.0.4/helperfns/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.448963 helperfns-0.0.4/helperfns/visualization/
--rw-rw-rw-   0        0        0     8989 2022-07-19 07:52:44.000000 helperfns-0.0.4/helperfns/visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 10:22:18.413959 helperfns-0.0.4/helperfns.egg-info/
--rw-rw-rw-   0        0        0     8223 2023-07-03 10:22:16.000000 helperfns-0.0.4/helperfns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-07-03 10:22:18.000000 helperfns-0.0.4/helperfns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 10:22:17.000000 helperfns-0.0.4/helperfns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-07-03 10:22:17.000000 helperfns-0.0.4/helperfns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-03 10:22:17.000000 helperfns-0.0.4/helperfns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 10:22:18.465962 helperfns-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1989 2023-07-03 10:10:38.000000 helperfns-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.117739 helperfns-0.0.5/
+-rw-rw-rw-   0        0        0     1089 2022-07-19 04:53:06.000000 helperfns-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     8507 2023-07-13 11:20:16.107741 helperfns-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6791 2023-07-13 11:18:11.000000 helperfns-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:15.987743 helperfns-0.0.5/helperfns/
+-rw-rw-rw-   0        0        0        0 2022-07-19 06:30:21.000000 helperfns-0.0.5/helperfns/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.077741 helperfns-0.0.5/helperfns/tables/
+-rw-rw-rw-   0        0        0     1917 2023-07-03 10:15:06.000000 helperfns-0.0.5/helperfns/tables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.083742 helperfns-0.0.5/helperfns/text/
+-rw-rw-rw-   0        0        0     4766 2022-09-01 09:10:36.000000 helperfns-0.0.5/helperfns/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.088742 helperfns-0.0.5/helperfns/torch/
+-rw-rw-rw-   0        0        0        0 2022-09-01 09:23:02.000000 helperfns-0.0.5/helperfns/torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.090741 helperfns-0.0.5/helperfns/torch/accuracy/
+-rw-rw-rw-   0        0        0     1981 2022-08-25 07:48:07.000000 helperfns-0.0.5/helperfns/torch/accuracy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.094743 helperfns-0.0.5/helperfns/torch/models/
+-rw-rw-rw-   0        0        0      971 2022-09-06 05:59:54.000000 helperfns-0.0.5/helperfns/torch/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.098742 helperfns-0.0.5/helperfns/torch/text/
+-rw-rw-rw-   0        0        0     4848 2022-09-01 10:27:12.000000 helperfns-0.0.5/helperfns/torch/text/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.101741 helperfns-0.0.5/helperfns/utils/
+-rw-rw-rw-   0        0        0      775 2022-08-25 07:27:13.000000 helperfns-0.0.5/helperfns/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.104740 helperfns-0.0.5/helperfns/visualization/
+-rw-rw-rw-   0        0        0    12054 2023-07-13 11:18:19.000000 helperfns-0.0.5/helperfns/visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-13 11:20:16.069740 helperfns-0.0.5/helperfns.egg-info/
+-rw-rw-rw-   0        0        0     8507 2023-07-13 11:20:11.000000 helperfns-0.0.5/helperfns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-07-13 11:20:15.000000 helperfns-0.0.5/helperfns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-13 11:20:11.000000 helperfns-0.0.5/helperfns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-07-13 11:20:13.000000 helperfns-0.0.5/helperfns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-13 11:20:14.000000 helperfns-0.0.5/helperfns.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-13 11:20:16.119740 helperfns-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2157 2023-07-13 11:18:07.000000 helperfns-0.0.5/setup.py
```

### Comparing `helperfns-0.0.4/LICENSE` & `helperfns-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.4/PKG-INFO` & `helperfns-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
-Keywords: python,python3,helper-functions,text cleaning,visualization,machine-learning
+Keywords: helperfns,python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: MacOS X :: Carbon
 Classifier: Environment :: MacOS X :: Carbon
 Classifier: Environment :: MacOS X :: Cocoa
@@ -137,15 +137,24 @@
 ### visualization
 
 This sub package provides different helper functions for visualizing data using plots.
 
 Examples:
 
 ```python
-from helperfns.visualization import plot_complicated_confusion_matrix, plot_images, plot_images_predictions, plot_simple_confusion_matrix
+from helperfns.visualization import plot_complicated_confusion_matrix, plot_images, plot_images_predictions, plot_simple_confusion_matrix,
+plot_classification_report
+
+
+# plotting classification report
+
+fig, ax = plot_classification_report(labels, preds,
+                    title='Classification Report',
+                    figsize=(10, 5), dpi=70,
+                    target_names = classes)
 
 # plot predicted image labels with the images
 plot_images_predictions(images, true_labels, preds, classes=["dog", "cat"] ,cols=8)
 
 # plot the images with their labels
 plot_images(images[:24], true_labels[:24], cols=8)
```

### Comparing `helperfns-0.0.4/README.md` & `helperfns-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,24 @@
 ### visualization
 
 This sub package provides different helper functions for visualizing data using plots.
 
 Examples:
 
 ```python
-from helperfns.visualization import plot_complicated_confusion_matrix, plot_images, plot_images_predictions, plot_simple_confusion_matrix
+from helperfns.visualization import plot_complicated_confusion_matrix, plot_images, plot_images_predictions, plot_simple_confusion_matrix,
+plot_classification_report
+
+
+# plotting classification report
+
+fig, ax = plot_classification_report(labels, preds,
+                    title='Classification Report',
+                    figsize=(10, 5), dpi=70,
+                    target_names = classes)
 
 # plot predicted image labels with the images
 plot_images_predictions(images, true_labels, preds, classes=["dog", "cat"] ,cols=8)
 
 # plot the images with their labels
 plot_images(images[:24], true_labels[:24], cols=8)
```

### Comparing `helperfns-0.0.4/helperfns/tables/__init__.py` & `helperfns-0.0.5/helperfns/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.4/helperfns/text/__init__.py` & `helperfns-0.0.5/helperfns/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.4/helperfns/torch/accuracy/__init__.py` & `helperfns-0.0.5/helperfns/torch/accuracy/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.4/helperfns/torch/models/__init__.py` & `helperfns-0.0.5/helperfns/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.4/helperfns/torch/text/__init__.py` & `helperfns-0.0.5/helperfns/torch/text/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.4/helperfns/utils/__init__.py` & `helperfns-0.0.5/helperfns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `helperfns-0.0.4/helperfns/visualization/__init__.py` & `helperfns-0.0.5/helperfns/visualization/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,246 +1,274 @@
-from turtle import turtles
 import matplotlib.pyplot as plt
 import itertools
-from sklearn.metrics import confusion_matrix, ConfusionMatrixDisplay
+from sklearn.metrics import (
+    confusion_matrix,
+    ConfusionMatrixDisplay,
+    classification_report,
+)
 import numpy as np
+import pandas as pd
+import seaborn as sns
+import pathlib
+import matplotlib as mpl
+
 
 def plot_simple_confusion_matrix(
-    y_true:list, 
-    y_pred:list, 
-    classes:list=[], 
-    figsize:tuple=(10, 10), 
-    fontsize: int = 15
+    y_true: list,
+    y_pred: list,
+    classes: list = [],
+    figsize: tuple = (10, 10),
+    fontsize: int = 15,
 ):
     """
-    Plot Complicated Confusion Matrix 
+    Plot Complicated Confusion Matrix
 
     This function simply plots a confusion matrix.
 
     Parameters
     ----------
     y_true : list
         Takes in a collection of true labels.
     y_pred : list
         Takes in a collection of predicted labels.
-    
+
     Keyword Args
     ------------
     classes : list
         A list of class name e.g ['dog', 'cat'] default is y_true.
     figsize : tuple
         The figsize of the confusion matrix plot default is (10, 10);
     fontsize : int
         Font size for the contents of the confusion matrix, default is 15.
-        
+
     Returns
     -------
     None
 
     See Also
     --------
     plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
     plot_images: Plots the images and display them.
     plot_images_predictions: Plots the images with their predictions and display them.
-    
+
     Examples
     --------
     >>> y_true = [random.randint(0, 1) for _ in range (100)]
     >>> y_pred = [random.randint(0, 1) for _ in range (100)]
     >>> classes =["dog", "cat"]
     >>> plot_complicated_confusion_matrix(y_true, y_pred, classes)
     """
-    assert len(y_true) == len(y_pred), f"The length of predicted and real labels must be equal, received {len(y_pred)} and {len(y_true)}."
+    assert len(y_true) == len(
+        y_pred
+    ), f"The length of predicted and real labels must be equal, received {len(y_pred)} and {len(y_true)}."
 
-    fig = plt.figure(figsize = figsize)
+    fig = plt.figure(figsize=figsize)
     ax = fig.add_subplot(1, 1, 1)
     cm = confusion_matrix(y_true, y_pred)
 
     if len(classes) == 0:
         classes = list(set(y_true))
 
-    cm = ConfusionMatrixDisplay(cm, display_labels= classes)
-    cm.plot(values_format = 'd', cmap = 'Blues', ax = ax)
-    plt.xticks(rotation = 20, color="black", fontsize=fontsize)
-    plt.yticks(rotation = 20, color="black", fontsize=fontsize)
+    cm = ConfusionMatrixDisplay(cm, display_labels=classes)
+    cm.plot(values_format="d", cmap="Blues", ax=ax)
+    plt.xticks(rotation=20, color="black", fontsize=fontsize)
+    plt.yticks(rotation=20, color="black", fontsize=fontsize)
     plt.show()
 
-def plot_complicated_confusion_matrix(y_true:list, y_pred:list, 
-                                    classes:list=[], 
-                                    figsize:turtles=(5, 5), 
-                                    fontsize:int=20,
-                                    title:str="Confusion Matrix",
-                                    xlabel:str="Predicted label",
-                                    ylabel:str="True label",
-                                      ):
-    
+
+def plot_complicated_confusion_matrix(
+    y_true: list,
+    y_pred: list,
+    classes: list = [],
+    figsize: tuple = (5, 5),
+    fontsize: int = 20,
+    title: str = "Confusion Matrix",
+    xlabel: str = "Predicted label",
+    ylabel: str = "True label",
+):
     """
-    Plot Complicated Confusion Matrix 
+    Plot Complicated Confusion Matrix
 
     This function simply plots a confusion matrix with some percentage(%) of confusion between class labels.
 
     Parameters
     ----------
     y_true : list
         Takes in a collection of true labels.
     y_pred : list
         Takes in a collection of predicted labels.
-    
+
     Keyword Args
     ------------
     classes : list
         A list of class name e.g ['dog', 'cat'].
     figsize : turple
         The figsize of the confusion matrix plot
     title : str
         The title to display for the confusion matrix, default is 'Confusion Matrix' .
     xlabel : str
         The x-axis label, default is 'True label'.
     ylabel : str
         The y-axis label, default is 'Predicted label'.
     fontsize : int
         Font size for the contents of the confusion matrix, default is 20.
-        
+
     Returns
     -------
     None
 
     See Also
     --------
     plot_simple_confusion_matrix : Plots a simple confusion matrix.
     plot_images: Plots the images and display them.
     plot_images_predictions: Plots the images with their predictions and display them.
-    
+
     Examples
     --------
     >>> y_true = [random.randint(0, 1) for _ in range (100)]
     >>> y_pred = [random.randint(0, 1) for _ in range (100)]
     >>> classes =["dog", "cat"]
     >>> plot_simple_confusion_matrix(y_true, y_pred, classes)
     """
-    
-    assert len(y_true) == len(y_pred), f"The length of predicted and real labels must be equal, received {len(y_pred)} and {len(y_true)}."
+
+    assert len(y_true) == len(
+        y_pred
+    ), f"The length of predicted and real labels must be equal, received {len(y_pred)} and {len(y_true)}."
     cm = confusion_matrix(y_true, y_pred)
     cm_norm = cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
     n_classes = cm.shape[0]
 
     fig, ax = plt.subplots(figsize=figsize)
     cax = ax.matshow(cm, cmap=plt.cm.Blues)
     fig.colorbar(cax)
 
     if len(classes):
         labels = classes
     else:
         labels = np.arange(cm.shape[0])
 
     ax.set(
-         title=title,
-         xlabel=xlabel,
-         ylabel=ylabel,
-         xticks=np.arange(n_classes),
-         yticks=np.arange(n_classes),
-         xticklabels=labels,
-         yticklabels=labels,
-          )
-    ax.yaxis.label.set_color('green')
-    ax.xaxis.label.set_color('green')
-
+        title=title,
+        xlabel=xlabel,
+        ylabel=ylabel,
+        xticks=np.arange(n_classes),
+        yticks=np.arange(n_classes),
+        xticklabels=labels,
+        yticklabels=labels,
+    )
+    ax.yaxis.label.set_color("green")
+    ax.xaxis.label.set_color("green")
 
     ax.xaxis.set_label_position("bottom")
     ax.xaxis.tick_bottom()
 
-    threshold = (cm.max() + cm.min()) / 2.
+    threshold = (cm.max() + cm.min()) / 2.0
     # Plot the text on each cell
     for i, j in itertools.product(range(cm.shape[0]), range(cm.shape[1])):
-        plt.text(j, i, f"{cm[i, j]} ({cm_norm[i, j]*100:.1f}%)",
-                 horizontalalignment="center",
-                 color="white" if cm[i, j] > threshold else "black",
-                 size=fontsize)
+        plt.text(
+            j,
+            i,
+            f"{cm[i, j]} ({cm_norm[i, j]*100:.1f}%)",
+            horizontalalignment="center",
+            color="white" if cm[i, j] > threshold else "black",
+            size=fontsize,
+        )
     plt.show()
 
-def plot_images(images:list, labels:list, cols:int=5, rows: int=3, fontsize: int=16)->None:
+
+def plot_images(
+    images: list, labels: list, cols: int = 5, rows: int = 3, fontsize: int = 16
+) -> None:
     """
-    Plot images 
+    Plot images
 
     This function simply plots Images with their labels.
 
     Parameters
     ----------
     images : list
         Takes in a collection of images.
     labels : list
         Takes in a collection of image labels.
-    
+
     Keyword Args
     ------------
     cols : int
         Number of columns for images, default is 5.
     rows : int
         Number of rows for images, default is 3
     fontsize : int
         Font size for labels, default is 16.
-        
+
     Returns
     -------
     None
 
     See Also
     --------
     plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
     plot_simple_confusion_matrix : Plots a simple confusion matrix.
     plot_images_predictions: Plots the images with their predictions and display them.
-    
+
     Examples
     --------
     >>> plot_images(images[:24], true_labels[:24], cols=8)
     """
-    
-    assert len(images) == len(labels), f"The length for images and labels must match but got {len(images)} {len(labels)}"
-    
+
+    assert len(images) == len(
+        labels
+    ), f"The length for images and labels must match but got {len(images)} {len(labels)}"
+
     fig = plt.figure()
     fig.set_size_inches(cols * 2, rows * 2)
     for i, (image, label) in enumerate(zip(images, labels)):
         plt.subplot(rows, cols, i + 1)
-        plt.axis('off')
+        plt.axis("off")
         plt.imshow(image, cmap="gray")
-        plt.title(label, color ='g', fontsize=fontsize )
-        
+        plt.title(label, color="g", fontsize=fontsize)
+
     plt.show()
 
 
-def plot_images_predictions(images:list, labels_true:list, 
-                            labels_pred:list, classes:list=[], cols:int=5,
-                            rows:int = 3, fontsize:int=16):
+def plot_images_predictions(
+    images: list,
+    labels_true: list,
+    labels_pred: list,
+    classes: list = [],
+    cols: int = 5,
+    rows: int = 3,
+    fontsize: int = 16,
+):
     """
     Plot images predictions
 
     This function simply plots predicted images. Images with wrongly predicted labels their
-    labels will be red and green otherwise. 
+    labels will be red and green otherwise.
 
     Parameters
     ----------
     images : list
         Takes in a collection of images.
     labels_true : list
         Takes in a collection of correct labels.
     labels_pred : list
         Takes in a collection of predicted labels.
-        
+
     Keyword Args
     ------------
     classes : list
-        Takes in a collection  of class labels example can be ['cat', 'dog'] if 
+        Takes in a collection  of class labels example can be ['cat', 'dog'] if
         not passed then labels_pred will be used.
     cols : int
         Number of columns for images, default is 5.
     rows : int
         Number of rows for images, default is 3
     fontsize : int
         Font size for labels, default is 16.
-        
+
     Returns
     -------
     None
 
     See Also
     --------
     plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
@@ -248,27 +276,135 @@
     plot_images: Plots the images and display them.
 
     Examples
     --------
     >>> plot_images_predictions(images, true_labels, preds, classes=["dog", "cat"] ,cols=8)
 
     """
-    assert len(images) == len(labels_true) == len(labels_pred), f"The image classes, true labels and predicted labels must be equal but received {len(images)}, {len(labels_true)} and {len(labels_pred)}."
-    
+    assert (
+        len(images) == len(labels_true) == len(labels_pred)
+    ), f"The image classes, true labels and predicted labels must be equal but received {len(images)}, {len(labels_true)} and {len(labels_pred)}."
+
     fig = plt.figure()
     fig.set_size_inches(cols * 2, rows * 2)
     if len(classes):
         classes = classes
     else:
         classes = list(set(label_pred))
-        
-    for i, (image, label_true, label_pred) in enumerate(zip(images, labels_true, labels_pred)):
+
+    for i, (image, label_true, label_pred) in enumerate(
+        zip(images, labels_true, labels_pred)
+    ):
         plt.subplot(rows, cols, i + 1)
-        plt.axis('off')
+        plt.axis("off")
         plt.imshow(image, cmap="gray")
-        plt.title(classes[label_true], color ='g' if label_true == label_pred else 'r', fontsize=fontsize )
-        
-    plt.show()   
-        
-        
-        
-        
+        plt.title(
+            classes[label_true],
+            color="g" if label_true == label_pred else "r",
+            fontsize=fontsize,
+        )
+
+    plt.show()
+
+
+def plot_classification_report(
+    y_true: list,
+    y_pred: list,
+    title: str = "Classification Report",
+    figsize: tuple = (10, 5),
+    dpi: int = 70,
+    save_fig_path=None,
+    **kwargs,
+):
+    """
+    Plot Classification Report
+
+    Parameters
+    ----------
+    y_true : pandas.Series or list of shape (n_samples,)
+        Targets.
+    y_pred : pandas.Series or list of shape (n_samples,)
+        Predictions.
+    title : str, default = 'Classification Report'
+        Plot title.
+    fig_size : tuple, default = (10, 5)
+        Size (inches) of the plot.
+    dpi : int, default = 70
+        Image DPI.
+    save_fig_path : str, defaut=None
+        Full path where to save the plot. Will generate the folders if they don't exist already.
+    **kwargs : attributes of classification_report class of sklearn
+
+    Returns
+    -------
+        fig : Matplotlib.pyplot.Figure
+            Figure from matplotlib
+        ax : Matplotlib.pyplot.Axe
+            Axe object from matplotlib
+
+    See Also
+    --------
+    plot_complicated_confusion_matrix : Plots a confusion matrix with some percentage(%) of confusion.
+    plot_simple_confusion_matrix : Plots a simple confusion matrix.
+    plot_images: Plots the images and display them.
+
+    Examples
+    --------
+    >>> fig, ax = plot_classification_report(labels, preds,
+                    title='Classification Report',
+                    figsize=(10, 5), dpi=70,
+                    target_names = classes)
+    """
+    fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
+
+    clf_report = classification_report(y_true, y_pred, output_dict=True, **kwargs)
+    keys_to_plot = [
+        key
+        for key in clf_report.keys()
+        if key not in ("accuracy", "macro avg", "weighted avg")
+    ]
+    df = pd.DataFrame(clf_report, columns=keys_to_plot).T
+    # the following line ensures that dataframe are sorted from the majority classes to the minority classes
+    df.sort_values(by=["support"], inplace=True)
+
+    # first, let's plot the heatmap by masking the 'support' column
+    rows, cols = df.shape
+    mask = np.zeros(df.shape)
+    mask[:, cols - 1] = True
+    ax = sns.heatmap(
+        df,
+        mask=mask,
+        annot=True,
+        cmap="Blues",
+        fmt=".3g",
+        vmin=0.0,
+        vmax=1.0,
+        linewidths=2,
+        linecolor="white",
+    )
+
+    # then, let's add the support column by normalizing the colors in this column
+    mask = np.zeros(df.shape)
+    mask[:, : cols - 1] = True
+
+    ax = sns.heatmap(
+        df,
+        mask=mask,
+        annot=True,
+        cbar=False,
+        linewidths=2,
+        linecolor="white",
+        fmt=".0f",
+        vmin=df["support"].min(),
+        vmax=df["support"].sum(),
+        norm=mpl.colors.Normalize(vmin=df["support"].min(), vmax=df["support"].sum()),
+    )
+
+    plt.title(title)
+    plt.xticks(rotation=45)
+    plt.yticks(rotation=360)
+
+    if save_fig_path != None:
+        path = pathlib.Path(save_fig_path)
+        path.parent.mkdir(parents=True, exist_ok=True)
+        fig.savefig(save_fig_path)
+    return fig, ax
```

### Comparing `helperfns-0.0.4/helperfns.egg-info/PKG-INFO` & `helperfns-0.0.5/helperfns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: helperfns
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package provide some python helper functions that are useful in machine learning.
 Author: Crispen Gari
 Author-email: <crispengari@gmail.com>
-Keywords: python,python3,helper-functions,text cleaning,visualization,machine-learning
+Keywords: helperfns,python,python3,helper-functions,text cleaning,visualization,machine-learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Environment :: MacOS X :: Carbon
 Classifier: Environment :: MacOS X :: Carbon
 Classifier: Environment :: MacOS X :: Cocoa
@@ -137,15 +137,24 @@
 ### visualization
 
 This sub package provides different helper functions for visualizing data using plots.
 
 Examples:
 
 ```python
-from helperfns.visualization import plot_complicated_confusion_matrix, plot_images, plot_images_predictions, plot_simple_confusion_matrix
+from helperfns.visualization import plot_complicated_confusion_matrix, plot_images, plot_images_predictions, plot_simple_confusion_matrix,
+plot_classification_report
+
+
+# plotting classification report
+
+fig, ax = plot_classification_report(labels, preds,
+                    title='Classification Report',
+                    figsize=(10, 5), dpi=70,
+                    target_names = classes)
 
 # plot predicted image labels with the images
 plot_images_predictions(images, true_labels, preds, classes=["dog", "cat"] ,cols=8)
 
 # plot the images with their labels
 plot_images(images[:24], true_labels[:24], cols=8)
```

### Comparing `helperfns-0.0.4/setup.py` & `helperfns-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,37 +3,52 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = "0.0.5"
 DESCRIPTION = "This package provide some python helper functions that are useful in machine learning."
 # setting up
 setup(
     name="helperfns",
     version=VERSION,
     author="Crispen Gari",
     author_email="<crispengari@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[
-        "prettytable", "nltk", "sklearn", "matplotlib", "numpy", "torch"
+        "prettytable",
+        "nltk",
+        "sklearn",
+        "matplotlib",
+        "numpy",
+        "torch",
+        "pandas",
+        "seaborn",
+    ],
+    keywords=[
+        "helperfns",
+        "python",
+        "python3",
+        "helper-functions",
+        "text cleaning",
+        "visualization",
+        "machine-learning",
     ],
-    keywords=['python', 'python3', 'helper-functions', "text cleaning", "visualization", "machine-learning"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Development Status :: 3 - Alpha",
         "Environment :: Console",
         "Environment :: MacOS X",
         "Environment :: MacOS X :: Carbon",
-         "Environment :: MacOS X :: Carbon",
+        "Environment :: MacOS X :: Carbon",
         "Environment :: MacOS X :: Cocoa",
         "Environment :: Web Environment",
         "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Education",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Other Audience",
         "Intended Audience :: Science/Research",
```

