# Comparing `tmp/fotosort-1.2.0-py3-none-any.whl.zip` & `tmp/fotosort-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 28041 bytes, number of entries: 12
+Zip file size: 28622 bytes, number of entries: 13
 -rw-r--r--  2.0 unx     1038 b- defN 19-Jun-23 08:15 fotosort/__init__.py
--rw-r--r--  2.0 unx     3702 b- defN 23-Jul-09 10:28 fotosort/controller.py
--rw-r--r--  2.0 unx     1064 b- defN 19-Jun-22 13:16 fotosort/imgutils.py
--rw-r--r--  2.0 unx     6195 b- defN 23-Jul-09 10:28 fotosort/ui.py
+-rw-r--r--  2.0 unx     3702 b- defN 23-Jul-13 12:40 fotosort/controller.py
+-rw-r--r--  2.0 unx     1143 b- defN 23-Jul-13 11:54 fotosort/imgutils.py
+-rw-r--r--  2.0 unx     6097 b- defN 23-Jul-13 12:41 fotosort/ui.py
 -rw-r--r--  2.0 unx     6121 b- defN 19-Mar-17 16:29 fotosort/images/noimage.png
--rw-r--r--  2.0 unx     8737 b- defN 23-Jul-09 10:28 fotosort/qml/main.qml
--rwxr-xr-x  2.0 unx       40 b- defN 23-Jul-09 10:45 fotosort-1.2.0.data/scripts/fotosort
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8866 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      948 b- defN 23-Jul-09 10:45 fotosort-1.2.0.dist-info/RECORD
-12 files, 71961 bytes uncompressed, 26459 bytes compressed:  63.2%
+-rw-r--r--  2.0 unx      996 b- defN 23-Jul-13 11:32 fotosort/qml/ShortcutMenuItem.qml
+-rw-r--r--  2.0 unx     8673 b- defN 23-Jul-13 12:40 fotosort/qml/main.qml
+-rwxr-xr-x  2.0 unx       40 b- defN 23-Jul-13 12:42 fotosort-1.3.0.data/scripts/fotosort
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-13 12:42 fotosort-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8866 b- defN 23-Jul-13 12:42 fotosort-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-13 12:42 fotosort-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-13 12:42 fotosort-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1037 b- defN 23-Jul-13 12:42 fotosort-1.3.0.dist-info/RECORD
+13 files, 72963 bytes uncompressed, 26898 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -9,29 +9,32 @@
 
 Filename: fotosort/ui.py
 Comment: 
 
 Filename: fotosort/images/noimage.png
 Comment: 
 
+Filename: fotosort/qml/ShortcutMenuItem.qml
+Comment: 
+
 Filename: fotosort/qml/main.qml
 Comment: 
 
-Filename: fotosort-1.2.0.data/scripts/fotosort
+Filename: fotosort-1.3.0.data/scripts/fotosort
 Comment: 
 
-Filename: fotosort-1.2.0.dist-info/LICENSE
+Filename: fotosort-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fotosort-1.2.0.dist-info/METADATA
+Filename: fotosort-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fotosort-1.2.0.dist-info/WHEEL
+Filename: fotosort-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fotosort-1.2.0.dist-info/top_level.txt
+Filename: fotosort-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fotosort-1.2.0.dist-info/RECORD
+Filename: fotosort-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fotosort/imgutils.py

```diff
@@ -25,11 +25,14 @@
     except (AttributeError, KeyError, IndexError):
         # cases: image don't have getexif
         return 0
 
 
 def get_timestamp(filepath):
     try:
-        s = Image.open(filepath)._getexif()[36867]
+        exifdata = Image.open(filepath)._getexif()
+        if exifdata is None:
+            return ''
+        s = exifdata[36867]
         return s.replace(':', '_').replace(' ', '-')
     except (AttributeError, KeyError, IndexError):
         return ''
```

## fotosort/ui.py

```diff
@@ -1,10 +1,10 @@
-from PySide2.QtWidgets import QApplication, QErrorMessage
-from PySide2.QtQml import QQmlApplicationEngine
-from PySide2.QtCore import QUrl, QObject, Signal, Slot, QStringListModel
+from PySide6.QtWidgets import QApplication, QErrorMessage
+from PySide6.QtQml import QQmlApplicationEngine
+from PySide6.QtCore import QUrl, QObject, Signal, Slot, QStringListModel
 import os
 
 from . import imgutils
 
 
 class UI(QObject):
     imageChangedSignal = Signal()
@@ -30,14 +30,20 @@
 
         self.setCurrentImage(self.controller.current())
         self.root.selectAll()
 
     def run(self):
         self.app.exec_()
 
+    @Slot(result=str)
+    def getVersion(self):
+        with open('VERSION') as f:
+            v = self.version = f.read()
+        return v
+
     def excepthook(self, cls, exception, traceback):
         self.root.showStatus("An error occured.", "red")
         self.root.showError("An error occured:\n\n{}".format(exception))
 
     @Slot(str, result=str)
     def autocomplete(self, searchtext):
         if len(searchtext) == 0:
@@ -60,17 +66,15 @@
 
     @Slot(result=str)
     def getCurrentImageTimestamp(self):
         return imgutils.get_timestamp(self.currentImage)
 
     def setCurrentImage(self, new_image):
         self.currentImage = new_image
-        w, h = self.root.width(), self.root.height()  # Save previous window geometry
-        self.imageChangedSignal.emit()  # This loads the picture and displays it, unfortunately resizing the window
-        self.root.resize(w,h)  # Programatically restore the window geometry prior to the load to avoid huge window
+        self.imageChangedSignal.emit() # This loads the picture and displays it
         # Adjust undo button
         if self.root.setUndoEnabled(len(self.controller.history) > 0):
             self.root.setUndoText("Undo {}".format(self.controller.history[-1][0]))
 
     @Slot()
     def first(self):
         self.setCurrentImage(self.controller.first())
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## fotosort/qml/main.qml

```diff
@@ -1,23 +1,22 @@
-import QtQuick 2.5
-import QtQuick.Controls 2.5
-import QtQuick.Controls 1.4
-import QtQuick.Controls.Styles 1.4
-import QtQuick.Layouts 1.12
-import QtQuick.Dialogs 1.1
+import QtCore 6.5
+import QtQuick 6.5
+import QtQuick.Controls 6.5
+import QtQuick.Layouts 6.5
+import QtQuick.Dialogs 6.5
 
 ApplicationWindow {
     id: window
     visible: true
     title: "FotoSort"
 
     function updateImage(){
         var filepath = ui.getCurrentImage()
         image.source = filepath
-        window.title = "FotoSort " + filepath + ' ' + ui.getCurrentImageTimestamp()
+        window.title = "FotoSort " + ui.getVersion() + ' ' + filepath + ' ' + ui.getCurrentImageTimestamp()
     }
 
     function selectAll(){
         combobox.selectAll();
     }
 
     function setUndoEnabled(enabled){
@@ -73,26 +72,26 @@
         errorDialog.text = message;
         errorDialog.open();
     }
 
     MessageDialog {
     id: errorDialog
         title: "An error occured"
-        text: "(No info available)"
-        standardButtons: StandardButton.Ok
-        icon: StandardIcon.Critical
+        Label {
+            text: "(No info available)"
+        }
+        buttons: MessageDialog.Ok
         onAccepted: focusCombobox();
     }
 
-    FileDialog {
+    FolderDialog {
         id: folderDialog
-        selectFolder: true
         title: "Select a directory with photos to move"
-        folder: shortcuts.home
-        onAccepted: ui.setLocation(folderDialog.folder)
+        currentFolder: StandardPaths.standardLocations(StandardPaths.PicturesLocation)[0]
+        onAccepted: ui.setLocation(folderDialog.selectedFolder)
         onRejected: focusCombobox();
     }
 
     Dialog {
         id: targetsDialog
         title: "Edit target locations"
         standardButtons: Dialog.Save | Dialog.Cancel
@@ -134,25 +133,23 @@
 
         Column {
             anchors.fill: parent
             
             TextField {
                 id: newTempLocation
                 width: parent.width
-                style: TextFieldStyle {
-                    textColor: "black"
-                    background: Rectangle {
-                        radius: 2
-                        implicitWidth: 100
-                        implicitHeight: 24
-                        border.color: "#333"
-                        border.width: 1
-                    }
+                color: "black"
+                background: Rectangle {
+                    radius: 2
+                    implicitWidth: 100
+                    implicitHeight: 24
+                    border.color: "#333"
+                    border.width: 1
                 }
-                Keys.onPressed: {
+                Keys.onPressed: function(event) {
                     if (event.key == Qt.Key_Return || event.key == Qt.Key_Enter) {
                         addTempTargetDialog.accept()
                         event.accepted = true;
                     }
                 }
             }
         }
@@ -173,54 +170,52 @@
             columns: 2
 
             Text { text: "Path to pictures folder:  "}
 
             TextField {
                 id: tempOutputPrefix
                 width: parent.width
-                style: TextFieldStyle {
-                    textColor: "black"
-                    background: Rectangle {
-                        radius: 2
-                        implicitWidth: 100
-                        implicitHeight: 24
-                        border.color: "#333"
-                        border.width: 1
-                    }
+                color: "black"
+                background: Rectangle {
+                    radius: 2
+                    implicitWidth: 100
+                    implicitHeight: 24
+                    border.color: "#333"
+                    border.width: 1
                 }
             }
 
             Text { text: "Copy pictures? (otherwise moved):  "}
 
             CheckBox { id: copyPictures }
 
             Button { text: "Edit traget locations"; onClicked: ui.openTargetsDialog() }
         }
     }
 
     menuBar: MenuBar {
         Menu {
             title: "Fotosort"
-            MenuItem { text: "Open folder"; shortcut: "Ctrl+O"; onTriggered: folderDialog.open() }
-            MenuItem { text: "Manage settings"; shortcut: "Ctrl+,"; onTriggered: ui.openSettingsDialog() }
-            MenuItem { text: "Manage target locations"; shortcut: "Ctrl+Shift+T"; onTriggered: ui.openTargetsDialog() }
-            MenuItem { text: "Add temporary target location"; shortcut: "Ctrl+T"; onTriggered: ui.openAddTempTargetDialog() }
-            MenuItem { text: "Quit"; shortcut: "Ctrl+Q"; onTriggered: Qt.quit() }
+            ShortcutMenuItem { text: "Open folder"; sequence: "Ctrl+O"; onTriggered: folderDialog.open() }
+            ShortcutMenuItem { text: "Manage settings"; sequence: "Ctrl+,"; onTriggered: ui.openSettingsDialog() }
+            ShortcutMenuItem { text: "Manage target locations"; sequence: "Ctrl+Shift+T"; onTriggered: ui.openTargetsDialog() }
+            ShortcutMenuItem { text: "Add temporary target location"; sequence: "Ctrl+T"; onTriggered: ui.openAddTempTargetDialog() }
+            ShortcutMenuItem { text: "Quit"; sequence: "Ctrl+Q"; onTriggered: Qt.quit() }
         }
         Menu {
             title: "Navigate"
-            MenuItem { text: "First"; shortcut: "Ctrl+Shift+Tab"; onTriggered: ui.first() }
-            MenuItem { text: "Prev"; shortcut: "Shift+Tab"; onTriggered: ui.prev() }
-            MenuItem { text: "Next"; shortcut: "Tab"; onTriggered: ui.next() }
-            MenuItem { text: "Last"; shortcut: "Ctrl+Tab"; onTriggered: ui.last() }
+            ShortcutMenuItem { text: "First"; sequence: "Ctrl+Shift+Tab"; onTriggered: ui.first() }
+            ShortcutMenuItem { text: "Prev"; sequence: "Shift+Tab"; onTriggered: ui.prev() }
+            ShortcutMenuItem { text: "Next"; sequence: "Tab"; onTriggered: ui.next() }
+            ShortcutMenuItem { text: "Last"; sequence: "Ctrl+Tab"; onTriggered: ui.last() }
         }
         Menu {
             title: "Actions"
-            MenuItem { text: "Undo"; shortcut: "Ctrl+Z"; onTriggered: { ui.undo(); ui.reload(); } id: undoMenuItem; enabled: false }
-            MenuItem { text: "Trash"; shortcut: "Ctrl+D"; onTriggered: { ui.trashCurrentFile(); ui.reload(); } }
+            ShortcutMenuItem { text: "Undo"; sequence: "Ctrl+Z"; onTriggered: { ui.undo(); ui.reload(); } id: undoMenuItem; enabled: false }
+            ShortcutMenuItem { text: "Trash"; sequence: "Ctrl+D"; onTriggered: { ui.trashCurrentFile(); ui.reload(); } }
         }
     }
 
     ColumnLayout {
         anchors.fill: parent
 
         Image {
@@ -241,19 +236,19 @@
             Layout.margins: 5
 
             ComboBox {
                 id: combobox
                 model: output_dirs
                 editable: true
                 focus: true;
-                Keys.onPressed: {
+                Keys.onPressed: function(event) {
                     if (event.key == Qt.Key_Return || event.key == Qt.Key_Enter) {
                         if (suggestionText.text !== ""){
                             ui.moveOrCopyCurrentFile(suggestionText.text);
-                            ui.reload(); 
+                            ui.reload();
                             selectAll();
                             event.accepted = true;
                         }
                     }
                     if(event.modifiers & Qt.ControlModifier && event.key == Qt.Key_Z){
                         ui.undo();
                         ui.reload();
```

## Comparing `fotosort-1.2.0.dist-info/LICENSE` & `fotosort-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fotosort-1.2.0.dist-info/METADATA` & `fotosort-1.3.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fotosort
-Version: 1.2.0
+Version: 1.3.0
 Summary: Fotosort is a program for quickly copying or moving pictures from different events into different folders.
 Home-page: https://github.com/kalsan/fotosort
 Author: Sandro Kalbermatter
 Author-email: 
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pillow
 Requires-Dist: pyyaml
-Requires-Dist: pyside2
+Requires-Dist: pyside6
 Requires-Dist: appdirs
 
 # Fotosort
 
 Fotosort is a program for quickly copying or moving pictures from different events into different folders. This sounds quite abstract, so let's look at a few scenarios to spice things up:
 
 ## Scenario 1: Random stuff
```

## Comparing `fotosort-1.2.0.dist-info/RECORD` & `fotosort-1.3.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 fotosort/__init__.py,sha256=CmL5cmcPC8bIkzNzXGTHMXSetHv5MNpOdkkl6mr-Q-g,1038
 fotosort/controller.py,sha256=OLfJ7JQWPn3Wj-wJY_n77oeco3qOi1VpnRnItghrPiQ,3702
-fotosort/imgutils.py,sha256=IlUT8EaFr_a59iaAVpq_29N2TnqAtpQTQBVaK2kosVw,1064
-fotosort/ui.py,sha256=3o0gvTHzuapZlKC-pHBXAsDaPE5UhTOBacSBl4G85GY,6195
+fotosort/imgutils.py,sha256=a8EDlu-aGlMVSI0n2GeyXe125PJvJYQiks1LEf4AbsA,1143
+fotosort/ui.py,sha256=PkzuyXgT_BqWDUrcMBHIjU3K6O2-Jsw5bPnXgokjLx8,6097
 fotosort/images/noimage.png,sha256=VS4SycBpmX6D9pj6zuVXubXecPZQ0xJAYe3xTT5Togg,6121
-fotosort/qml/main.qml,sha256=B-tNUHpqtqLLde1vxKPl4FMcgGPSZNnwE3YQVrHSdI0,8737
-fotosort-1.2.0.data/scripts/fotosort,sha256=h88OVbpM4qpnl_RUYS1pLUXmndGNSQf7bquxzEdaQYk,40
-fotosort-1.2.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-fotosort-1.2.0.dist-info/METADATA,sha256=0bf-ycz2MbsKmFkSdThjfIhb1q1twbJhi39j9uPRQAY,8866
-fotosort-1.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-fotosort-1.2.0.dist-info/top_level.txt,sha256=cq2wXg6U38bTuEr0ptmcqEp-0YWCsjrRptVeHb30RTg,9
-fotosort-1.2.0.dist-info/RECORD,,
+fotosort/qml/ShortcutMenuItem.qml,sha256=jqeEMIFdIR8BE7j1P_dGOF-9L53jjZFUZBMdyq5cXM8,996
+fotosort/qml/main.qml,sha256=-qvp-jf6mMr1DLJGW1-YlJxGn8FOigsEFBLo3dpbOLI,8673
+fotosort-1.3.0.data/scripts/fotosort,sha256=h88OVbpM4qpnl_RUYS1pLUXmndGNSQf7bquxzEdaQYk,40
+fotosort-1.3.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+fotosort-1.3.0.dist-info/METADATA,sha256=xQT9IkyoEsS5RIV-h-eNaMGdkDQ70W5ByZk35NgI_iQ,8866
+fotosort-1.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+fotosort-1.3.0.dist-info/top_level.txt,sha256=cq2wXg6U38bTuEr0ptmcqEp-0YWCsjrRptVeHb30RTg,9
+fotosort-1.3.0.dist-info/RECORD,,
```

