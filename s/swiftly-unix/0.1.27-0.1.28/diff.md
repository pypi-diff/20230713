# Comparing `tmp/swiftly-unix-0.1.27.tar.gz` & `tmp/swiftly-unix-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-unix-0.1.27.tar", last modified: Wed Jul 12 12:20:33 2023, max compression
+gzip compressed data, was "swiftly-unix-0.1.28.tar", last modified: Thu Jul 13 21:10:52 2023, max compression
```

## Comparing `swiftly-unix-0.1.27.tar` & `swiftly-unix-0.1.28.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.576922 swiftly-unix-0.1.27/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.27/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:20:33.576786 swiftly-unix-0.1.27/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.575252 swiftly-unix-0.1.27/scripts/
--rwxr-xr-x   0 brainspoof   (501) staff       (20)     6904 2023-07-12 12:17:41.000000 swiftly-unix-0.1.27/scripts/swiftly
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-12 12:20:33.576960 swiftly-unix-0.1.27/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-12 12:20:31.000000 swiftly-unix-0.1.27/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.576164 swiftly-unix-0.1.27/swiftly_unix/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.27/swiftly_unix/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.27/swiftly_unix/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.27/swiftly_unix/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.27/swiftly_unix/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.27/swiftly_unix/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.27/swiftly_unix/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-12 12:20:33.576627 swiftly-unix-0.1.27/swiftly_unix.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-12 12:20:33.000000 swiftly-unix-0.1.27/swiftly_unix.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-13 21:10:52.567836 swiftly-unix-0.1.28/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-10 14:57:15.000000 swiftly-unix-0.1.28/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-13 21:10:52.567687 swiftly-unix-0.1.28/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-13 21:10:52.565801 swiftly-unix-0.1.28/scripts/
+-rwxr-xr-x   0 brainspoof   (501) staff       (20)     7186 2023-07-13 21:07:17.000000 swiftly-unix-0.1.28/scripts/swiftly
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-13 21:10:52.567877 swiftly-unix-0.1.28/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      163 2023-07-13 21:10:29.000000 swiftly-unix-0.1.28/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-13 21:10:52.566937 swiftly-unix-0.1.28/swiftly_unix/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-10 17:23:27.000000 swiftly-unix-0.1.28/swiftly_unix/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-11 17:34:13.000000 swiftly-unix-0.1.28/swiftly_unix/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-11 18:43:09.000000 swiftly-unix-0.1.28/swiftly_unix/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3291 2023-07-12 08:49:15.000000 swiftly-unix-0.1.28/swiftly_unix/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2169 2023-07-11 17:57:38.000000 swiftly-unix-0.1.28/swiftly_unix/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-11 18:17:29.000000 swiftly-unix-0.1.28/swiftly_unix/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-13 21:10:52.567496 swiftly-unix-0.1.28/swiftly_unix.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       79 2023-07-13 21:10:52.000000 swiftly-unix-0.1.28/swiftly_unix.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      318 2023-07-13 21:10:52.000000 swiftly-unix-0.1.28/swiftly_unix.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-13 21:10:52.000000 swiftly-unix-0.1.28/swiftly_unix.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       13 2023-07-13 21:10:52.000000 swiftly-unix-0.1.28/swiftly_unix.egg-info/top_level.txt
```

### Comparing `swiftly-unix-0.1.27/LICENSE` & `swiftly-unix-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.27/scripts/swiftly` & `swiftly-unix-0.1.28/scripts/swiftly`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 #!/bin/bash
 
+# Check if 'python' command is available
+if command -v python &> /dev/null
+then
+    PYTHON_CMD=python
+    PIP_CMD=pip
+else
+    PYTHON_CMD=python3
+    PIP_CMD=pip3
+fi
+
 # Disable job control
 set +m
 
 # Define the spinner characters
 spinner_chars=('🌑' '🌒' '🌓' '🌔' '🌕' '🌖' '🌗' '🌘')
 
 # Define the spinner function
@@ -82,73 +92,73 @@
 trap handle_sigint SIGINT
 
 
 # Now, you can use spin_start and spin_stop in your functions
 
 function init(){
     spin_start "Checking swiftly"
-    pip install swiftly-unix --upgrade > /dev/null
+    $PIP_CMD install swiftly-unix --upgrade > /dev/null
     spin_stop "Checked swiftly"
 
     if [ -z "$1" ]
     then
         spin_start "Checking remote origin for changes"
         fetch_remote=$(git fetch | tr '\n' ' ' > /dev/null 2>&1)
 
         git_status=$(git status -uno | tr '\n' ' ' | sed 's/"/\\"/g')
 
-        pull_changes=$(python -c 'from swiftly_unix.init import pull_changes; print(pull_changes("'$git_status'"))')
+        pull_changes=$($PYTHON_CMD -c 'from swiftly_unix.init import pull_changes; print(pull_changes("'$git_status'"))')
         if [ "$pull_changes" = "True" ]
         then
             git pull > /dev/null
             spin_stop "Remote changes pulled"
 
         else
             spin_stop "Codebase up-to-date"
         fi
 
         spin_start "Checking your project"
-        project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
+        project_name=$($PYTHON_CMD -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
         export PROJECT_NAME=$project_name
         spin_stop "Project '$PROJECT_NAME' ready"
 
         spin_start "Activating virtual environment"
-        venv_location=$(python -c 'from swiftly_unix.init import get_venv_location; print(get_venv_location())')
+        venv_location=$($PYTHON_CMD -c 'from swiftly_unix.init import get_venv_location; print(get_venv_location())')
         source $venv_location/bin/activate
         export PROJECT_VENV_LOCATION=$venv_location
 
-        pip install swiftly-unix --upgrade > /dev/null 2>&1
+        $PIP_CMD install swiftly-unix --upgrade > /dev/null 2>&1
         spin_stop "Virtual environment activated"
 
         spin_start "Checking for new packages"
-        available_packages=$(pip freeze | tr '\n' ' ')
-        new_packages=$(python -c "from swiftly_unix.init import check_new_packages; print(check_new_packages('$available_packages'))")
+        available_packages=$($PIP_CMD freeze | tr '\n' ' ')
+        new_packages=$($PYTHON_CMD -c "from swiftly_unix.init import check_new_packages; print(check_new_packages('$available_packages'))")
 
         if [ "$new_packages" = "True" ]
         then
-            pip install -r requirements.txt > /dev/null
+            $PIP_CMD install -r requirements.txt > /dev/null
             spin_stop "New packages installed"
         else
             spin_stop "All packages already installed"
         fi
 
         spin_start "Checking swiftly"
-        pip install --upgrade pip > /dev/null 2>&1
+        $PIP_CMD install --upgrade pip > /dev/null 2>&1
 
         install swiftly-unix --upgrade > /dev/null 2>&1
         spin_stop "All checks completed swiftly"
 
     else
-        is_github_repo=$(python -c "from swiftly_unix.init import is_repo; print(is_repo('$1'))")
+        is_github_repo=$($PYTHON_CMD -c "from swiftly_unix.init import is_repo; print(is_repo('$1'))")
         if [ "$is_github_repo" = "True" ]
         then
             spin_start "Cloning git repository"
             git_clone=$(git clone $1 2>&1 | tr '\n' '=' | sed 's/"/\\"/g')
 
-            clone_successful=$(python -c 'from swiftly_unix.init import clone_successful; print(clone_successful("'$git_clone'"))')
+            clone_successful=$($PYTHON_CMD -c 'from swiftly_unix.init import clone_successful; print(clone_successful("'$git_clone'"))')
 
             if [ "$clone_successful" = "True" ]
             then
                 spin_stop "Git repository cloned"
             else
                 spin_stop "$clone_successful" "fail"
                 echo "Do you want to create a new project? (y/n)"
@@ -159,64 +169,64 @@
                     return 1
                 fi
             fi
         fi
 
 
         spin_start "Creating project $1"
-        venv_location=$(python -c "from swiftly_unix.init import initialise; print(initialise('$1'))")
+        venv_location=$($PYTHON_CMD -c "from swiftly_unix.init import initialise; print(initialise('$1'))")
         source $venv_location/bin/activate
         export PROJECT_VENV_LOCATION=$venv_location
 
         cd $venv_location
         cd ..
 
-        pip install swiftly-unix --upgrade > /dev/null 2>&1
+        $PIP_CMD install swiftly-unix --upgrade > /dev/null 2>&1
 
-        project_name=$(python -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
+        project_name=$($PYTHON_CMD -c 'from swiftly_unix.init import get_project_name; print(get_project_name())')
         export PROJECT_NAME=$project_name
 
         spin_stop "Project '$PROJECT_NAME' ready"
 
         spin_start "Installing requirements"
-        pip install --upgrade pip > /dev/null 2>&1
+        $PIP_CMD install --upgrade pip > /dev/null 2>&1
 
-        pip install -r requirements.txt > /dev/null
+        $PIP_CMD install -r requirements.txt > /dev/null
         spin_stop "Requirements installed"
 
         spin_start "Checking swiftly"
         install swiftly-unix --upgrade > /dev/null 2>&1
         spin_stop "All checks completed swiftly"
     fi
 
     echo "✨ Project '$PROJECT_NAME' initiated successfully :)"
 }
 
 
 function makeapp(){
-    python -c "from swiftly_unix.makeapp import makeapp; makeapp('$1', '$PROJECT_VENV_LOCATION')"
+    $PYTHON_CMD -c "from swiftly_unix.makeapp import makeapp; makeapp('$1', '$PROJECT_VENV_LOCATION')"
     sleep 1
     printf "\033[0;32m✓\033[0m %s\n" "App '${1}' created successfully"
 }
 
 function run(){
-    path=$(python -c "from swiftly_unix.runapp import run_app; print(run_app('$1', '$PROJECT_NAME'))")
-    python -m $path
+    path=$($PYTHON_CMD -c "from swiftly_unix.runapp import run_app; print(run_app('$1', '$PROJECT_NAME'))")
+    $PYTHON_CMD -m $path
 }
 
 function install(){
-    pip install "$@"
-    updated_packages=$(pip freeze)
+    $PIP_CMD install "$@"
+    updated_packages=$($PIP_CMD freeze)
     requirements_path=$PROJECT_VENV_LOCATION/../requirements.txt
     echo "$updated_packages" > $requirements_path
 }
 
 function uninstall(){
-    pip uninstall "$@"
-    updated_packages=$(pip freeze)
+    $PIP_CMD uninstall "$@"
+    updated_packages=$($PIP_CMD freeze)
     requirements_path=$PROJECT_VENV_LOCATION/../requirements.txt
     echo "$updated_packages" > $requirements_path
 }
 
 function push(){
     git add *
     git commit -m "$*"
```

### Comparing `swiftly-unix-0.1.27/swiftly_unix/gitignore.py` & `swiftly-unix-0.1.28/swiftly_unix/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.27/swiftly_unix/init.py` & `swiftly-unix-0.1.28/swiftly_unix/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-unix-0.1.27/swiftly_unix/makeapp.py` & `swiftly-unix-0.1.28/swiftly_unix/makeapp.py`

 * *Files identical despite different names*

