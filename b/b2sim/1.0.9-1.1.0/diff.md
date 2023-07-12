# Comparing `tmp/b2sim-1.0.9.tar.gz` & `tmp/b2sim-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2sim-1.0.9.tar", last modified: Mon Jul 10 23:51:55 2023, max compression
+gzip compressed data, was "b2sim-1.1.0.tar", last modified: Tue Jul 11 04:30:16 2023, max compression
```

## Comparing `b2sim-1.0.9.tar` & `b2sim-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:21.287904 b2sim-1.0.9/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.0.9/LICENSE
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.0.9/MANIFEST.in
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-11 23:59:21.273824 b2sim-1.0.9/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    14173 2023-07-10 20:01:59.000000 b2sim-1.0.9/README.md
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:20.368952 b2sim-1.0.9/b2sim/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.0.9/b2sim/__init__.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10590 2023-07-11 16:22:42.000000 b2sim-1.0.9/b2sim/actions.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8687 2023-07-04 00:16:01.000000 b2sim-1.0.9/b2sim/info.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   105812 2023-07-11 23:53:37.000000 b2sim-1.0.9/b2sim/main.py
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     3818 2023-07-04 23:08:48.000000 b2sim-1.0.9/b2sim/rounds.py
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:21.158188 b2sim-1.0.9/b2sim/templates/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-06-26 11:10:38.000000 b2sim-1.0.9/b2sim/templates/eco_send_info.csv
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      418 2023-07-11 02:24:19.000000 b2sim-1.0.9/b2sim/templates/nat_send_lengths.csv
-drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-11 23:59:20.853323 b2sim-1.0.9/b2sim.egg-info/
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/PKG-INFO
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/SOURCES.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/dependency_links.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/requires.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-11 23:59:19.000000 b2sim-1.0.9/b2sim.egg-info/top_level.txt
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-11 23:59:21.292768 b2sim-1.0.9/setup.cfg
--rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-10 22:20:35.000000 b2sim-1.0.9/setup.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:19.069376 b2sim-1.1.0/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    35823 2023-05-09 05:51:58.000000 b2sim-1.1.0/LICENSE
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       87 2023-06-20 11:17:51.000000 b2sim-1.1.0/MANIFEST.in
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-12 23:51:19.054637 b2sim-1.1.0/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    13601 2023-07-12 23:50:40.000000 b2sim-1.1.0/README.md
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:18.482022 b2sim-1.1.0/b2sim/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       81 2023-06-20 01:13:34.000000 b2sim-1.1.0/b2sim/__init__.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)    10817 2023-07-12 23:37:31.000000 b2sim-1.1.0/b2sim/actions.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     8804 2023-07-12 20:35:37.000000 b2sim-1.1.0/b2sim/info.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)   103530 2023-07-12 23:42:28.000000 b2sim-1.1.0/b2sim/main.py
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     3818 2023-07-04 23:08:48.000000 b2sim-1.1.0/b2sim/rounds.py
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:18.923626 b2sim-1.1.0/b2sim/templates/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)     2027 2023-07-12 20:07:14.000000 b2sim-1.1.0/b2sim/templates/eco_send_info.csv
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      418 2023-07-11 02:24:19.000000 b2sim-1.1.0/b2sim/templates/nat_send_lengths.csv
+drwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        0 2023-07-12 23:51:18.772886 b2sim-1.1.0/b2sim.egg-info/
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      274 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/PKG-INFO
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      332 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/SOURCES.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        1 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/dependency_links.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       24 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/requires.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)        6 2023-07-12 23:51:17.000000 b2sim-1.1.0/b2sim.egg-info/top_level.txt
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)       38 2023-07-12 23:51:19.073328 b2sim-1.1.0/setup.cfg
+-rwxrwxrwx   0 redlaserbm  (1000) redlaserbm  (1000)      401 2023-07-12 19:38:52.000000 b2sim-1.1.0/setup.py
```

### Comparing `b2sim-1.0.9/LICENSE` & `b2sim-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.9/README.md` & `b2sim-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,58 @@
 # Overview
 
 The `b2sim` Python library is an extensive feature-rich library for simulating flowcharts within battles 2. Simulating essential aspects of battles 2's income sources with virtually 100% accuracy, the library is a must-use tool for optimizing eco'ing and farming with any flowchart. Results from the simulator can be used to better inform practical decisions made during games, improving player game sense and leading to more optimal play. The code is relatively easy to use and does not require prior coding experience to effectively operate.
 
-- To install the code, first download Python on your machine, and then in the terminal type `pip install b2sim` and hit 'Enter'.
-- To learn how to operate the code, see the examples folder in this GitHub repo. It contains numerous examples with code explained in plain English.
-- Want to request features for the code? Want to help out with the code? Found a bug? Don't hesitate to contact me! The most immediate way to get my attention with regards to this code is to join the b2 Popology discord server and ping me there: https://discord.gg/axHnkcVe6E
-- Potential collaborators interested with helping out with the code should view the "Feature Requests" section below for more info on tasks that need to be completed.
-
-# Operating the Code
-
-To run the code, do the following: 
-1. Install python on your computer. 
-2. In the terminal, do `pip install b2sim`.
-3. Using an IDE like Visual Studio Code, open a new .ipynb file and type `import b2sim as b2` in the first line and hit enter.
-4. You now have a file which you can use to generate simulations! Check out the tutorial files for more info on how to operate the library. 
+# Running the Code
+
+## For noobs:
+1. Install python on your computer here: https://www.anaconda.com/download/
+2. Open the anaconda prompt and type `pip install b2sim`.
+3. Your installation of anaconda came with a program called "Jupyter Notebook", which allows you to create and edit .ipynb files which you will use to operate the code. Open Jupyter, and create a new .ipynb file wherever you wish on your computer.
+4. In the first cell of this new .ipynb file you've created, type `import b2sim as b2` and hit enter. 
+5. Congratulations, you now have a file which you can use to generate simulations! Check out the tutorial files in this repo (examples folder) for more info on how to operate the library.
+6. (Bonus step) Instead of Jupyter Notebook, I recommend using [Visual Studio Code](https://code.visualstudio.com/) to operate the code. VS Code comes with a number of bells and whistles and QOL features that can speed up the code-writing process.
+
+## For experienced coders:
+1. Type `pip install b2sim` in the terminal to download.
+2. Check out the tutorial files in this repo (tutorials folder) for more info on how to operate the library.
+
+## Alternative installation instructions:
+If for whatever reason pip installation does not work, try the following:
+1. Clone this GitHub repository onto your computer (using a program like GitHub Desktop)
+2. Navigate to where you cloned the repository in the terminal, and then run the command `python3 setup.py install --user`
 
 # Code Features
 
 1. **Simultaneous simulation of eco, farms, and alt-eco:** When given an eco send to use and some arrangement of farms and alt-eco, the simulator accurately tracks the progression of the player's cash and eco over time. The results of the simulator are nearly true to the game.
 2. **Easy operation:** Simply input your initial cash and eco, the round to start on, and the purchases you intend to make and the eco flowchart you intend to follow over the course of the match. The code runs in one click and delivers results in seconds.
 3. **Complete Farm support:** The simulator supports IMF Loans and Monkeyopolis. Also, the simulator supports compound purchases, such as selling into Monkey Wall Street.
-4. **Advanced Optimization Potential:** The code can be used in conjuction with optimization or nonlinear root-finding methods to determine the absolute best times to makes your moves during the game. 
+4. **Advanced Optimization Potential:** The code can be used in conjuction with optimization or nonlinear root-finding methods to determine the absolute best times to makes your moves during the game.
+
+# Contributing to the Code
+
+Potential contributors are urged to join the [b2 popology discord](https://discord.gg/YBkvcdBN4H) where I can be easily reached with a ping. Look in the "issues" section of this repo for tasks which need to be completed but have not yet been tended to.
+
+## First-Time Contributors
+
+If it's your first time ever contributing to the code, follow these steps to made the contribution process easy and hassle-free:
+1. Download [GitHub Desktop](https://desktop.github.com/).
+2. Clone the repository to your desktop.
+3. When you're ready to make changes after working on the code, [create a pull request](https://www.nexmo.com/legacy-blog/2020/10/01/how-to-create-a-pull-request-with-github-desktop).
 
 # Update Log
+- (July 11, 2023 - v1.0.9)
+   - Adjusted the lengths of some of the rounds in `nat_send_lengths.csv`
+   - Fixed an error in `eco_send_info.csv` which caused Grouped Reds and Grouped Blues to be unavailable in the simulator on Round 11
+   - Fixed a bug which made the code throw an error if a fail-safe was triggered as a consequence of the simulator attempting to use an eco send after it became unavailable.
+   - Renamed "examples" folder to "tutorials". Revised the tutorial files so that they are more instructive.
+   - Updated `GameState.viewCashEcoHistory` so that it is easier to see when key transactions or changes in eco occur during the simulation.
+- (July 10, 2023 - v1.0.8)
+   - Initializing boat farms is now also done with a list structure just like with regular farms.
+   - Changed round lengths in the spreadsheet. Natural round lengths were inferred by a test between spoonoil and ninjayas but the old numbers led to underestimates. The new numbers may still underestimate actual natural round lengths but are closer to the truth than before.
 - (July 4, 2023 - v1.0.7)
    - Fixed various bugs which caused the simulator to behave incorrectly when fail-safes were triggered. Such issues were related to when the eco sim tried to change eco sends as a consequence of a break condition (such as `max_eco_amount`) on the current send being satisfied.
    - Updated display for graphs. The legend shows (approximated to the nearest tenth) when each action is carried out in the simulation.
 - (July 2, 2023 - v1.0.6)
    - Fixed an issue which effectively caused the attack queue size to be 5 instead of 6.
    - New action `sellAllFarms` for rapidly selling all farms.
 - (July 2, 2023 - v1.0.5)
@@ -77,31 +103,7 @@
 - (May 12, 2023 - v0.9.2) 
    - Graphs from `GameState.viewCashEcoHistory()` are now more informative.
    - `GameState.viewCashEcoHistory(dim=(w,h))` lets you set the width and height of the graphs.
    - Fixed a bug which would cause the code to get stuck in an infinite loop if `GameState.fastForward()` if the argument interval was set to a small number.
    - `GameState.fastForward()` now by default uses `interval = 0.1`. This will lead to sharper graphs and surprisngly does not appear to slow down the code much.
 - (May 11, 2023 - v0.9.1) 
    - Added druid farm support. Currently untested!
-
-# Feature Requests
-
-- (High Priority) More actions in `actions.py` to expand functionality and improve ease of use, including:
-   - Selling all Supply Drops, Selling all Druid Farms, Selling all Boat Farms
-   - Selling into a farm upgrade
-   - Withdrawing from all banks at once
-   - Buying, selling, and using overclock (on farms)
-- (High Priority) Expanded revenue tracking:
-   - It would also be nice if the sim could track stats related to alt eco. Such stats could include revenue, expenses, long-run eco, and the aggregate revenue and expenses of each alt eco over the course of the simulation.
-   - In order for players to understand the `eco impact` statistic, display the farm's start and end of availability during the simulation.
-- (High Priority) Change the formatting for storing farms and boat farms:
-   - In a previous update, the behavior of farm selling was changed so that, from the perspective of the simulator, the farm is not sold, but rather "disabled". The `GameState` class continues to store the farms but does not compute their payments or award them.
-   - This new behavior circumvents an issue in early builds that used a list structure to store farms where a selling one farm could cause other farms' identifying index to shift, essentially making it impossible to implement support for compound transactions.
-   - Because of this, farms can now be stored in a simple list structure.
-   - Naturally, when revenue/expense tracking support is also implemented for boat farms, we will in the same way want to change the data structure for storing them to a list.
-- (Medium priority) Village support:
-   - Village support would help answer the question of how useful Monkey City/Monkey Town actually are.
-- (Medium priority) Restructure the code:
-   - There may be a way to rewrite 'processBuyQueue' so that it uses less lines of code and is easier to understand. (will explain idea here later)
-- (Low priority) Robust logging when comparing different strategies
-   - The idea here is this: If I have two or more game states that share the same round class and are simulated over the same time span, they are directly comparable. While a method already exists to compare multiple game states with this principle, because it does not share code with the `Game State` class method `viewCashAndEcoHistory`, it is currently inflexible with regards to updates and lacks some of the pizazz the class method has right now.
-- (Low Priority) Optimization of the buy queue to prevent redundant computations
-   - The code is already reasonably fast, but there are selected cases where the simulator is known to perform the same computation repeatedly when this sort of thing can be avoided.
```

### Comparing `b2sim-1.0.9/b2sim/actions.py` & `b2sim-1.1.0/b2sim/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,22 @@
         'Index': index,
         'Path': path,
         'Buffer': buffer,
         'Minimum Buy Time': min_buy_time,
         'Message': 'Upgrade farm %s at path %s'%(index, path) 
     }
 
-def sellFarm(index, min_buy_time = 0):
+def sellFarm(index, min_buy_time = 0, withdraw = False):
     #Look, I know this is confusing, but "min_buy_time" really is the minimum selling time in this case!
     return {
         'Type': 'Sell Farm',
         'Index': index,
         'Minimum Buy Time': min_buy_time,
-        'Message': 'Sell farm %s'%(index)
+        'Message': 'Sell farm %s'%(index),
+        'Withdraw': withdraw
     }
 
 def buyDefense(cost, buffer = 0, min_buy_time = 0, message = 'Buy Defense'):
     return {
         'Type': 'Buy Defense',
         'Cost': cost,
         'Buffer': buffer,
@@ -50,18 +51,19 @@
     return {
         'Type': 'Activate IMF',
         'Index': index,
         'Minimum Buy Time': min_buy_time,
         'Message': 'Take out loan from farm %s'%(index)
     }
 
-def sellAllFarms(min_buy_time = 0):
+def sellAllFarms(min_buy_time = 0, withdraw = False):
     return {
         'Type': 'Sell All Farms',
-        'Minimum Buy Time': min_buy_time #Okay, this might be confusing, but this is actually the minimum *sell* time for this action.
+        'Minimum Buy Time': min_buy_time,
+        'Withdraw': withdraw #Okay, this might be confusing, but this is actually the minimum *sell* time for this action.
     }
 
 # WARNING: This function is for declaring farms in the initial game state. 
 # Do NOT use it to add farms during simulation
 def initFarm(purchase_time = None, upgrades = [0,0,0]):
     return {
         'Purchase Time': purchase_time,
@@ -299,15 +301,15 @@
         'Message': 'Trigger Jericho Steal'
     }
 
 ###########
 # ECO QUEUE
 ###########
 
-def ecoSend(time = None, send_name = 'Zero', property = 'Normal', max_send_amount = None, max_eco_amount = None):
+def ecoSend(time = None, send_name = 'Zero', property = 'Normal', max_send_amount = None, max_eco_amount = None, max_send_time = None, queue_threshold = 6):
     
     fortified = False
     camo = False
     regrow = False
 
     if property == 'Fortified':
         fortified = True
@@ -335,9 +337,11 @@
     return {
         'Time': time,
         'Send Name': send_name,
         'Max Send Amount': max_send_amount,
         'Fortified': fortified,
         'Camoflauge': camo,
         'Regrow': regrow,
-        'Max Eco Amount': max_eco_amount
+        'Max Eco Amount': max_eco_amount,
+        'Max Send Time': max_send_time,
+        'Queue Threshold': queue_threshold
     }
```

### Comparing `b2sim-1.0.9/b2sim/info.py` & `b2sim-1.1.0/b2sim/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,16 @@
     'Eco Delay': 0.15, #The delay between eco sends, in seconds, assuming the attack queue is not full and the player has enough cash to send eco.
     'Fortified Multiplier': 2.0,
     'Camoflauge Multiplier': 2.0,
     'Regrow Multiplier': 1.6,
     'Regrow Round': 8,
     'Camoflauge Round': 12,
     'Fortified Round': 18,
-    'Sellback Value': 0.7
+    'Sellback Value': 0.7,
+    'Max Queue Length': 6 #The maximum number of bloon sends that can exist in the attack queue at any given time.
 }
 
 farm_globals = {
     'Farm Cost': 1000,
     'Farm Upgrade Costs': [[550,550,2600,16000,66000],[200,700,5100,7500,45000],[250,200,2800,13000,46000]],
     'Farm Bank Capacity': [0,0,0,14000,20000,30000],
     'IMF Loan Amount': 20000,
```

### Comparing `b2sim-1.0.9/b2sim/main.py` & `b2sim-1.1.0/b2sim/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -184,33 +184,34 @@
         # }
 
         # Max send amount is useful if we need to simulate sending a precise number of sets of bloons
         # Max eco amount is useful for eco strategies which may demand strategy decisions like "stop eco at 3000 eco"
 
         self.eco_queue = initial_state.get('Eco Queue')
         if self.eco_queue is None:
-            self.eco_queue = []
+            self.eco_queue = [ecoSend(time = 0, send_name = 'Zero')]
         self.number_of_sends = 0
 
         eco_send = initial_state.get('Eco Send')
-        if eco_send is None:
-            eco_send = ecoSend(send_name = 'Zero')
-        eco_send['Time'] = 0
-        self.eco_queue.insert(0,eco_send)
+        if eco_send is not None:
+            eco_send['Time'] = 0
+            self.eco_queue.insert(0,eco_send)
         
         #Upgrade queue
         self.buy_queue = initial_state.get('Buy Queue')
         self.buy_cost = None
         self.buffer = 0
         self.min_buy_time = None
 
         #Attack queue - This is the list of bloons in the center of the screen that pops up whenever you send eco
         self.attack_queue = []
         self.attack_queue_unlock_time = self.current_time
         self.eco_delay = game_globals['Eco Delay']
+        self.max_queue_length = game_globals['Max Queue Length']
+        self.attack_queue_threshold = game_globals['Max Queue Length']
 
         #For repeated supply drop buys
         self.supply_drop_max_buy_time = -1
         self.supply_drop_buffer = 0
 
         #For repeated druid farm buys
         self.druid_farm_max_buy_time = -1
@@ -221,15 +222,15 @@
         self.heli_farm_buffer = 0
 
         #~~~~~~~~~~
         #FAIL-SAFES
         #~~~~~~~~~~
         
         if self.farms is None:
-            self.farms = {}
+            self.farms = []
         if self.buy_queue is None:
             self.buy_queue = []
         if self.loan is None:
             self.loan = 0
         if self.boat_farms is None:
             self.boat_farms = {}
         if self.druid_farms is None:
@@ -312,15 +313,15 @@
             ax1.plot([message['Time'],message['Time']],[cash_min-1, cash_max+1], label = thing_to_say, linestyle = line_style, color = line_color)
 
         #~~~~~~~~~~~~~~~~
         #Label the graphs
         #~~~~~~~~~~~~~~~~
 
         ax1.set_title("Cash & Eco vs Time")
-        ax1.legend(bbox_to_anchor = (1.02, 1), fontsize = font_size)
+        ax1.legend(bbox_to_anchor = (1.1, 1), fontsize = font_size)
         fig.tight_layout()
 
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         #Create a table that displays the revenue/expenses of each farm
         #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         #Create a list of revenues and expenses for every farm
@@ -427,15 +428,15 @@
                             self.logs.append("Warning! Time %s is too late to call %s. Removing from eco queue"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name']))
                             self.eco_queue.pop(0)
                             
                         else:
                             #No, the send is not too late
                             
                             #Is the eco send too early?
-                            self.logs.append("The candidate round is %s"%(eco_send_info[self.eco_queue[0]['Send Name']]['Start Round']))
+                            #self.logs.append("The candidate round is %s"%(eco_send_info[self.eco_queue[0]['Send Name']]['Start Round']))
                             candidate_time = self.rounds.getTimeFromRound(eco_send_info[self.eco_queue[0]['Send Name']]['Start Round'])
                             if self.eco_queue[0]['Time'] < candidate_time:
                                 #Yes, the send is too early
                                 self.logs.append("Warning! Time %s is too early to call %s. Adjusting the queue time to %s"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name'], candidate_time))
                                 self.eco_queue[0]['Time'] = candidate_time
                                 #Is the adjusted time still valid?
                                 if len(self.eco_queue) < 2 or self.eco_queue[0]['Time'] < self.eco_queue[1]['Time']:
@@ -447,15 +448,15 @@
                                     self.logs.append("Warning! Time %s is too late to call %s because the next item in the eco queue is slated to come earlier. Removing from eco queue"%(self.eco_queue[0]['Time'],self.eco_queue[0]['Send Name']))
                                     self.eco_queue.pop(0)
                             else:
                                 #No, the send is not too early
                                 self.checkProperties()
                                 break_flag = True
             
-            if len(self.eco_queue) > 0 and self.eco_queue[0]['Time'] is not None and self.eco_queue[0]['Time'] <= self.current_time:
+            if len(self.eco_queue) > 0 and (self.eco_queue[0]['Time'] is not None and self.eco_queue[0]['Time'] <= self.current_time):
                 self.changeEcoSend()
             else:
                 future_flag = True
         
     def changeEcoSend(self):
         # Attempt to change to the first send available in the eco queue
         # This method is triggered either when reaching the specified time for the next send in the eco queue OR when a break condition (such as max_eco_amount) is satisfied for the current send
@@ -530,14 +531,20 @@
         #Setting the max_send_amount
         self.max_send_amount = send_info['Max Send Amount']
         self.number_of_sends = 0
 
         #Setting the max_eco_amount
         self.max_eco_amount = send_info['Max Eco Amount']
 
+        #Setting the max_send_time
+        self.max_send_time = send_info['Max Send Time']
+
+        #Setting the queue threshold
+        self.attack_queue_threshold = send_info['Queue Threshold']
+
         self.logs.append("Modified the eco send to %s"%(self.send_name))
         self.event_messages.append({
             'Time': self.current_time, 
             'Type': "Eco",
             'Message': "Change eco to %s"%(self.send_name)
         })
 
@@ -648,29 +655,21 @@
             
             #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
             #First, compute the impact of eco from the previous payout (or starting time) to the current one
             #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
             self.updateEco(payout['Time'])
 
-            if (self.max_send_amount is not None and self.number_of_sends == self.max_send_amount) or (self.max_eco_amount is not None and self.eco >= self.max_eco_amount):
+            if (self.max_send_amount is not None and self.number_of_sends >= self.max_send_amount) or (self.max_eco_amount is not None and self.eco >= self.max_eco_amount) or (self.max_send_time is not None and self.current_time > self.max_send_time):
                 self.logs.append("Reached the limit on eco'ing for this send! Moving to the next send in the queue.")
 
                 #Switch to the zero send
                 if len(self.eco_queue) == 0:
                     self.logs.append("No more sends in the eco queue! Switching to the zero send.")
-                    self.eco_queue.append({
-                        'Time': self.current_time,
-                        'Send Name': 'Zero',
-                        'Max Send Amount': None,
-                        'Max Eco Amount': None,
-                        'Fortified': False,
-                        'Camoflauge': False,
-                        'Regrow': False
-                    })
+                    self.eco_queue.append(ecoSend(send_name = 'Zero'))
                 else:
                     # Adjust the time of the next eco send so that the simulator attempts to change to it at simulation end
                     self.eco_queue[0]['Time'] = self.current_time
                 
                 # In rare cases, we may break from the eco queue on exactly same time that we are slated to receive a payment
                 # In that rare case, we need to award the payment for that time and check the buy queue to ensure that we do not "skip" over anything essential.
                 if self.current_time < payout['Time']:
@@ -1109,47 +1108,47 @@
         # There is a known fix for this issue, but I do not wish to implement out of fear that it may hamper code performance and make the code more difficult to read and understand.
 
         # self.logs.append("Attack Queue Unlock time: %s"%(self.attack_queue_unlock_time))
         # self.logs.append("Send Name: %s"%(self.send_name))
         # self.logs.append("Number of Sends: %s"%(self.number_of_sends))
         # self.logs.append("Max Send Amount: %s"%(self.max_send_amount))
 
-        while self.attack_queue_unlock_time <= target_time and self.send_name != 'Zero' and (self.max_send_amount is None or self.number_of_sends < self.max_send_amount) and (self.max_eco_amount is None or self.eco < self.max_eco_amount):
+        while self.attack_queue_unlock_time <= target_time and self.send_name != 'Zero' and (self.max_send_amount is None or self.number_of_sends < self.max_send_amount) and (self.max_eco_amount is None or self.eco < self.max_eco_amount) and (self.max_send_time is None or self.attack_queue_unlock_time <= self.max_send_time):
             self.current_time = max(self.attack_queue_unlock_time, self.current_time)
             # self.logs.append("Advanced current time to %s"%(self.current_time))
 
             # First, check if we can remove any items from the attack queue
             while len(self.attack_queue) > 0 and self.current_time >= self.attack_queue[0]:
                 self.attack_queue.pop(0)
             
             # Next, try to add an attack to the attack_queue.
             # Can we send an attack?
-            if self.cash >= self.eco_cost and len(self.attack_queue) < 6:
+            if self.cash >= self.eco_cost and len(self.attack_queue) < min(6, self.attack_queue_threshold):
                 # Yes, the queue is empty and we have enough cash
                 if len(self.attack_queue) == 0:
                     self.attack_queue.append(self.current_time + self.eco_time)
                 else:
                     self.attack_queue.append(max(self.attack_queue[-1] + self.eco_time, self.current_time + self.eco_time))
                 self.cash -= self.eco_cost
                 self.eco += self.eco_gain
                 self.logs.append("Sent a set of %s at time %s"%(self.send_name, self.current_time))
                 self.logs.append("Currently, the send queue looks like this: ")
                 self.logs.append(str(self.attack_queue))
 
                 # Did the attack fill up the eco queue?
-                if len(self.attack_queue) == 6:
+                if len(self.attack_queue) >= min(6, self.attack_queue_threshold):
                     # Yes, The next send will cause the attack queue to fill up. Wait until the queue empties (if necessary)
                     self.attack_queue_unlock_time = max(self.current_time + self.eco_delay, self.attack_queue[0])
                 else:
                     # No, there's still space afterwards. Check again after the eco delay is up.
                     self.attack_queue_unlock_time = self.current_time + self.eco_delay
                 
                 self.number_of_sends += 1
 
-            elif len(self.attack_queue) == 6:
+            elif len(self.attack_queue) >= min(6, self.attack_queue_threshold):
                 # No, the queue is full!
                 # NOTE: This block of code won't get reached unless the game state is initalized with a full attack queue.
                 self.attack_queue_unlock_time = self.attack_queue[0]
             
             elif self.cash < self.eco_cost:
                 # No, we don't have money!
                 self.attack_queue_unlock_time = target_time + self.eco_delay/2
@@ -1222,205 +1221,35 @@
             #For tracking the revenue of boat farms
             for key in self.boat_farms.keys():
                 boat_farm = self.boat_farms[key]
                 boat_farm['Hypothetical Revenue'] = boat_farm['Revenue']
             
             for dict_obj in purchase_info:
 
-                # DEFENSE RELATED MATTERS
-                if dict_obj['Type'] == 'Buy Defense':
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*dict_obj['Cost'])
-                    
-                # FARM RELATED MATTERS
-                elif dict_obj['Type'] == 'Buy Farm':
-                    h_new_cash, h_new_loan = impact(h_cash, h_loan, -1*farm_globals['Farm Cost'])
-                elif dict_obj['Type'] == 'Upgrade Farm':
-                    ind = dict_obj['Index']
-                    path = dict_obj['Path']
-                    farm = self.farms[ind]
-                    #Do not upgrade a farm that has already been sold!
-                    if farm.sell_time is not None:
-                        self.logs.append("WARNING! Tried to upgrade a farm that was already sold! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-
-                    #The following code prevents from the player from having multiple T5's in play
-                    if farm.upgrades[path]+1 == 5 and self.T5_exists[path] == True:
-                        self.logs.append("WARNING! Tried to purchase a T5 farm when one of the same kind already existed! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*farm_upgrades_costs[path][farm.upgrades[path]])
-                elif dict_obj['Type'] == 'Sell Farm':
-                    ind = dict_obj['Index']
-                    farm = self.farms[ind]
-
-                    #Check whether the farm is actually on screen before selling it:
-                    if farm.sell_time is None:
-                        #Selling a farm counts as that farm generating revenue
-                        h_new_cash, h_new_loan = impact(h_cash, h_loan, farm_sellback_values[tuple(farm.upgrades)])
-                        farm.h_revenue += h_new_cash - h_cash
-                        h_cash, h_loan = h_new_cash, h_new_loan
-                    else:
-                        self.logs.append("WARNING! Tried to sell a farm that is not on screen! Aborting buy queue")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                elif dict_obj['Type'] == 'Sell All Farms':
-                    for farm in self.farms:
-                        if farm.sell_time is None:
-                            h_new_cash, h_new_loan = impact(h_cash, h_loan, farm_sellback_values[tuple(farm.upgrades)])
-                            farm.h_revenue += h_new_cash - h_cash
-                            h_cash, h_loan = h_new_cash, h_new_loan
-
-
-                elif dict_obj['Type'] == 'Withdraw Bank':
-                    #WARNING: The farm in question must actually be a bank for us to perform a withdrawal!
-                    #If it isn't, break the loop prematurely
-                    ind = dict_obj['Index']
-                    farm = self.farms[ind]
-                    if farm.sell_time is not None:
-                        self.logs.append("WARNING! Tried to withdraw from a bank that was already sold! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-
-                    if farm.upgrades[1] < 3:
-                        self.logs.append("WARNING! Tried to Withdraw from a farm that is not a bank! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                    
-                    h_new_cash, h_new_loan = impact(h_cash, h_loan, farm.account_value)
-                    # self.logs.append("Detected bank withdrawal of %s"%(h_new_cash - h_cash))
-                    farm.h_revenue += h_new_cash - h_cash
-                    h_cash, h_loan = h_new_cash, h_new_loan
-
-                elif dict_obj['Type'] == 'Activate IMF':
-                    #WARNING: The farm in question must actually be an IMF Loan for us to use this ability!
-                    #If it isn't, set a flag to False and break the loop.
-                    #DEVELOPER'S NOTE: A farm that has a min_use_time is not necessarily an IMF loan, it could also be an Monkeyopolis
-                    #Do not upgrade a farm that has already been sold!
-                    if farm.sell_time is not None:
-                        self.logs.append("WARNING! Tried to take out a loan from a bank that was already sold! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-
-                    if farm.upgrades[1] != 4:
-                        self.logs.append("WARNING! Tried to take out a loan from a farm that is not an IMF! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                        
-                    ind = dict_obj['Index']
-                    farm = self.farms[ind]
-                    
-                    #When, a loan is activated, treat it like a payment, then add the debt
-                    h_new_cash, h_new_loan = impact(h_cash, h_loan, farm_globals['IMF Loan Amount'])
-                    farm.h_revenue += h_new_cash - h_cash
-                    h_new_loan += farm_globals['IMF Loan Amount']
-                    h_cash, h_loan = h_new_cash, h_new_loan
-                
-                # BOAT FARM RELATED MATTERS
-                elif dict_obj['Type'] == 'Buy Boat Farm':
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*boat_globals['Merchantmen Cost'])
-                elif dict_obj['Type'] == 'Upgrade Boat Farm':
-                    ind = dict_obj['Index']
-                    boat_farm = self.boat_farms[ind]
-                    #The following code prevents from the player from having multiple Trade Empires in play
-                    if boat_farm['Upgrade']+1 == 5 and self.Tempire_exists == True:
-                        self.logs.append("WARNING! Tried to purchase a Trade Empire when one already exists! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                    upgrade_cost = boat_upgrades_costs[boat_farm['Upgrade']-3]
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*upgrade_cost)
-                elif dict_obj['Type'] == 'Sell Boat Farm':
-                    ind = dict_obj['Index']
-                    boat_farm = self.boat_farms[ind]
+                h_cash, h_loan = self.processAction(dict_obj, payout, h_cash = h_cash, h_loan = h_loan, stage = 'check')
 
-                    #Check whether the boat farm is actually on screen before selling it:
-                    if boat_farm['Sell Time'] is None:
-                        #Selling a farm counts as that farm generating revenue
-                        h_new_cash, h_new_loan = impact(h_cash, h_loan, boat_sell_values[boat_farm['Upgrade']-3])
-                        boat_farm['Hypothetical Revenue'] += h_new_cash - h_cash
-                        h_cash, h_loan = h_new_cash, h_new_loan
-                    else:
-                        self.logs.append("WARNING! Tried to sell a boat farm that is not on screen! Aborting buy queue")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-
-                # DRUID FARM RELATED MATTERS
-                elif dict_obj['Type'] == 'Buy Druid Farm':
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*druid_globals['Druid Farm Cost'])
-                elif dict_obj['Type'] == 'Sell Druid Farm':
-                    if dict_obj['Index'] == self.sotf:
-                        h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(druid_globals['Druid Farm Cost'] + druid_globals['Spirit of the Forest Upgrade Cost']))
-                    else:
-                        h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*druid_globals['Druid Farm Cost'])
-                elif dict_obj['Type'] == 'Buy Spirit of the Forest':
-                    #WARNING: There can only be one sotf at a time!
-                    if self.sotf is not None:
-                        self.logs.append("WARNING! Tried to purchase a Spirit of the Forest when one already exists! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*druid_globals['Spirit of the Forest Upgrade Cost'])
-                
-                # SUPPLY DROP RELATED MATTERS
-                elif dict_obj['Type'] == 'Buy Supply Drop':
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*sniper_globals['Supply Drop Cost'])
-                elif dict_obj['Type'] == 'Sell Supply Drop':
-                    if dict_obj['Index'] == self.elite_sniper:
-                        h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(sniper_globals['Supply Drop Cost'] + sniper_globals['Elite Sniper Upgrade Cost']) )
-                    else:
-                        h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*sniper_globals['Supply Drop Cost'])
-                elif dict_obj['Type'] == 'Buy Elite Sniper':
-                    #WARNING: There can only be one e-sniper at a time!
-                    if self.elite_sniper is not None:
-                        self.logs.append("WARNING! Tried to purchase an Elite Sniper when one already exists! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*sniper_globals['Elite Sniper Upgrade Cost'])
-
-                # HELI FARM RELATED MATTERS
-                elif dict_obj['Type'] == 'Buy Heli Farm':
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*heli_globals['Heli Farm Cost'])
-                elif dict_obj['Type'] == 'Sell Heli Farm':
-                    if dict_obj['Index'] == self.special_poperations:
-                        h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(heli_globals['Heli Farm Cost'] + heli_globals['Special Poperations Upgrade Cost']) )
-                    else:
-                        h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*heli_globals['Heli Farm Cost'])
-                elif dict_obj['Type'] == 'Buy Special Poperations':
-                    #WARNING: There can only be one Special Poperations on screen at a time!
-                    if self.special_poperations is not None:
-                        self.logs.append("WARNING! Tried to purchase Special Poperations when one already exists! Aborting buy queue!")
-                        self.warnings.append(len(self.logs)-1)
-                        self.valid_action_flag = False
-                        break
-                    h_cash, h_loan = impact(h_cash, h_loan, -1*heli_globals['Special Poperations Upgrade Cost'])
+                #Immediately abort attempting the purchase if we try to process an action that is not possible:
+                if not self.valid_action_flag:
+                    break
                     
                 #If at any point while performing these operations our cash becomes negative, then prevent the transaction from occurring:
                 if h_cash < 0:
                     # self.logs.append("WARNING! Reached negative cash while attempting the transaction!")
                     break
 
                 #Read the buffer associated with the buy if any
                 #NOTE: Only one object in purchase_info should have buffer info
                 #If there are multiple buffers, the code rectifies the matter by
                 #adding them all together
+
                 if dict_obj.get('Buffer') is not None:
                     self.buffer += dict_obj.get('Buffer')
             
-            #If the purchase sequence triggered a warning in the logs, do NOT perform it and break the while loop
-            if self.valid_action_flag == False:
+            #Immediately break from processing the buy queue entirely if we try to process an action that is not possible.
+            if not self.valid_action_flag:
                 break
             
             # If the amount of cash we have exceeds our buffer, perform the transaction.
             # Note at this point we have already checked whether we have reached the minimum time for the buy and also
             # we have already checked whether the buy item is valid. We now just need to check whether we have enough money!
             
             #self.logs.append("We have %s cash, but the next buy costs %s and has a buffer of %s and needs to be made on or after time %s!"%(np.round(self.cash,2), np.round(self.cash - h_cash,2),np.round(self.buffer,2), self.min_buy_time))
@@ -1445,240 +1274,16 @@
                 # self.logs.append("The new lists of farm revenues and expenses are given by: ")
                 # self.logs.append(str(self.farm_revenues))
                 # self.logs.append(str(self.farm_expenses))
 
                 for dict_obj in purchase_info:
 
                     buy_message_list.append(dict_obj['Message'])
-                    
-                    #FARM RELATED MATTERS
-                    if dict_obj['Type'] == 'Buy Farm':
-                        self.logs.append("Purchasing farm!")
-                        farm_info = {
-                            'Purchase Time': self.current_time,
-                            'Upgrades': [0,0,0]
-                        }
-                        farm = MonkeyFarm(farm_info)
-                        self.farms.append(farm)
-
-                        #For revenue and expense tracking
-                        farm.revenue = 0
-                        farm.expenses = farm_globals['Farm Cost']
-                        
-                    elif dict_obj['Type'] == 'Upgrade Farm':
-                        ind = dict_obj['Index']
-                        path = dict_obj['Path']
-                        
-                        self.logs.append("Upgrading path %s of the farm at index %s"%(path, ind))
-                        farm = self.farms[ind]
-
-                        #For expense tracking
-                        farm.expenses += farm_upgrades_costs[path][farm.upgrades[path]]
-
-                        farm.upgrades[path] += 1
-
-                        #Update the payout information of the farm
-                        farm.payout_amount = farm_payout_values[tuple(farm.upgrades)][0]
-                        farm.payout_frequency = farm_payout_values[tuple(farm.upgrades)][1]
-                        
-                        #So that we can accurately track payments for the farm
-                        farm.purchase_time = payout['Time']
-                        
-                        #Update the sellback value of the farm
-                        farm.sell_value = farm_sellback_values[tuple(farm.upgrades)]
-                        
-                        self.logs.append("The new farm has upgrades (%s,%s,%s)"%(farm.upgrades[0],farm.upgrades[1],farm.upgrades[2]))
-                        
-                        #If the resulting farm is a Monkey Bank, indicate as such and set its max account value appropriately
-                        if farm.upgrades[1] >= 3 and path == 1:
-                            farm.bank = True
-                            farm.max_account_value = farm_bank_capacity[farm.upgrades[1]]
-                            self.logs.append("The new farm is a bank! The bank's max capacity is %s"%(farm.max_account_value))
-                            
-                        #If the resulting farm is an IMF Loan or Monkeyopolis, determine the earliest time the loan can be used
-                        if farm.upgrades[1] > 3 and path == 1:
-                            farm.min_use_time = payout['Time'] + farm_globals['Monkeynomics Initial Cooldown']
-                        
-                        #If the resulting farm is a Banana Central, activate the BRF buff, giving them 25% more payment amount
-                        if farm.upgrades[0] == 5 and path == 0:
-                            self.logs.append("The new farm is a Banana Central!")
-                            self.T5_exists[0] = True
-                            
-                        #If the resutling farm is a Monkeyopolis, mark the x5x_exists flag as true to prevent the user from trying to have multiple of them
-                        if farm.upgrades[1] == 5:
-                            self.T5_exists[1] = True
-                        
-                        #If the resulting farm is a MWS, mark the MWS_exists flag as true to prevent the user from trying to have multiple of them.
-                        if farm.upgrades[2] == 5:
-                            self.T5_exists[2] = True
-                        
-                    elif dict_obj['Type'] == 'Sell Farm':
-                        ind = dict_obj['Index']
-                        farm = self.farms[ind]
-                        self.logs.append("Selling the farm at index %s"%(ind))
-
-                        # If the farm being sold is a Banana Central, we must turn off the BRF buff
-                        # If the farm is a T5 of any sorts, ensure that the game state knows we no longer that particular T5
-
-                        if farm.upgrades[0] == 5:
-                            self.logs.append("The farm we're selling is a Banana Central! Removing the BRF buff.")
-                            self.T5_exists[0] = False
-                        elif farm.upgrades[1] == 5:
-                            self.T5_exists[1] = False
-                        elif farm.upgrades[2] == 5:
-                            self.T5_exists[2] = False
-
-                        #Mark the farm's sell time. The code checks whether this value is a number or not before trying to compute farm payments
-                        farm.sell_time = payout['Time']
-                        
-                    elif dict_obj['Type'] == 'Sell All Farms':
-                        self.logs.append("Selling all farms!")
-                        self.T5_exists = [False for i in range(3)] #Obviously, if we sell all farms we won't have any T5's anymore!
-                        for farm in self.farms:
-                            farm.sell_time = payout['Time']
-                    
-                    elif dict_obj['Type'] == 'Withdraw Bank':
-                        self.logs.append("Withdrawing money from the bank at index %s"%(ind))
-                        ind = dict_obj['Index']
-                        farm = self.farms[ind]
-                        farm.account_value = 0
-                    elif dict_obj['Type'] == 'Activate IMF':
-                        ind = dict_obj['Index']
-                        farm = self.farms[ind]
-                        self.logs.append("Taking out a loan from the IMF at index %s"%(ind))
-                        farm.min_use_time = payout['Time'] + farm_globals['IMF Usage Cooldown']
-                        
-                    # BOAT FARM RELATED MATTERS
-                    elif dict_obj['Type'] == 'Buy Boat Farm':
-                        self.logs.append("Purchasing boat farm!")
-                        boat_farm = {
-                            'Initial Purchase Time': self.current_time,
-                            'Purchase Time': self.current_time,
-                            'Upgrade': 3,
-                            'Revenue': 0,
-                            'Expenses': boat_globals['Merchantmen Cost'],
-                            'Hypothetical Revenue': 0,
-                            'Sell Time': None
-                        }
-                        self.boat_farms[self.boat_key] = boat_farm
-                        self.boat_key += 1
-                    elif dict_obj['Type'] == 'Upgrade Boat Farm':
-                        ind = dict_obj['Index']
-                        
-                        self.logs.append("Upgrading the boat farm at index %s"%(ind))
-                        boat_farm = self.boat_farms[ind]
-                        boat_farm['Upgrade'] += 1
-
-                        #Expense tracking
-                        boat_farm['Expenses'] += boat_upgrades_costs[boat_farm['Upgrade'] - 4]
-                        
-                        #Update the payout information of the boat farm
-                        boat_farm['Payout'] = boat_payout_values[boat_farm['Upgrade'] - 3]
-                        
-                        #So that we can accurately track payments for the boat farm
-                        boat['Purchase Time'] = payout['Time']
-                        
-                        #Update the sellback value of the boat farm
-                        boat['Sell Value'] = boat_sell_values[boat_farm['Upgrade'] - 3]
-
-                        #If the new boat farm is a Trade Empire, indicate as such
-                        if boat_farm['Upgrade'] == 5:
-                            self.logs.append("The new boat farm is a Trade Empire!")
-                            self.Tempire_exists = True
+                    self.processAction(dict_obj, payout, stage = 'process')
 
-                    elif dict_obj['Type'] == 'Sell Boat Farm':
-                        ind = dict_obj['Index']
-                        self.logs.append("Selling the boat farm at index %s"%(ind))
-                        #If the farm being sold is a Trade Empire, indicate as such
-                        if boat_farm['Upgrade'] == 5:
-                            self.logs.append("The boat farm we're selling is a Trade Empire! Removing the Tempire buff.")
-                            self.Tempire_exists = False
-
-                        #Mark the boat farm's sell time
-                        boat_farm['Sell Time'] = payout['Time']
-
-                    # DRUID FARMS
-                    elif dict_obj['Type'] == 'Buy Druid Farm':
-                        self.druid_farms[self.druid_key] = payout['Time']
-                        self.druid_key += 1
-                        self.logs.append("Purchased a druid farm!")
-                    elif dict_obj['Type'] == 'Sell Druid Farm':
-                        ind = dict_obj['Index']
-                        self.logs.append("Selling the druid farm at index %s"%(ind))
-                        #If the druid we're selling is actually SOTF...
-                        if self.sotf is not None and ind == self.sotf:
-                            self.logs.append("The druid farm being sold is a Spirit of the Forest!")
-                            self.sotf = None
-                            self.sotf_min_use_time = None
-                    elif dict_obj['Type'] == 'Buy Spirit of the Forest':
-                        ind = dict_obj['Index']
-                        self.sotf = ind
-                        self.logs.append("Upgrading the druid farm at index %s into a Spirit of the Forest!"%(ind))
-                        #Determine the minimum time that the SOTF active could be used
-                        i = np.floor((20 + payout['Time'] - self.druid_farms[ind])/40) + 1
-                        self.sotf_min_use_time = payout['Time'] + 20 + 40*(i-1)
-                    elif dict_obj['Type'] == 'Repeatedly Buy Druid Farms':
-                        self.druid_farm_max_buy_time = dict_obj['Maximum Buy Time']
-                        self.druid_farm_buffer = dict_obj['Buffer']
-                        self.logs.append("Triggered automated druid farm purchases until time %s"%(self.druid_farm_max_buy_time))
-
-                    # SUPPLY DROP RELATED MATTERS
-                    elif dict_obj['Type'] == 'Buy Supply Drop':
-                        self.supply_drops[self.sniper_key] = payout['Time']
-                        self.sniper_key += 1
-                        self.logs.append("Purchased a supply drop!")
-                    elif dict_obj['Type'] == 'Sell Supply Drop':
-                        ind = dict_obj['Index']
-                        self.logs.append("Selling the supply drop at index %s"%(ind))
-                        #If the supply drop we're selling is actually an E-sniper, then...
-                        if self.elite_sniper is not None:
-                            if ind == self.elite_sniper:
-                                self.logs.append("The supply drop being sold is an elite sniper!")
-                                self.elite_sniper = None
-                        
-                        self.supply_drops.pop(ind)
-                    elif dict_obj['Type'] == 'Buy Elite Sniper':
-                        ind = dict_obj['Index']
-                        self.elite_sniper = ind
-                        self.logs.append("Upgrading the supply drop at index %s into an elite sniper!"%(ind))
-                    elif dict_obj['Type'] == 'Repeatedly Buy Supply Drops':
-                        self.supply_drop_max_buy_time = dict_obj['Maximum Buy Time']
-                        self.supply_drop_buffer = dict_obj['Buffer']
-                        self.logs.append("Triggered automated supply drop purchases until time %s"%(self.supply_drop_max_buy_time))
-
-                    # HELI FARM RELATED MATTERS
-                    elif dict_obj['Type'] == 'Buy Heli Farm':
-                        self.heli_farms[self.heli_key] = payout['Time']
-                        self.heli_key += 1
-                        self.logs.append("Purchased a heli farm!")
-                    elif dict_obj['Type'] == 'Sell Supply Drop':
-                        ind = dict_obj['Index']
-                        self.logs.append("Selling the heli farm at index %s"%(ind))
-                        #If the supply drop we're selling is actually a special poperations, then...
-                        if self.special_poperations is not None:
-                            if ind == self.special_poperations:
-                                self.logs.append("The heli farm being sold is a special poperations!")
-                                self.elite_sniper = None
-                        
-                        self.supply_drops.pop(ind)
-                    elif dict_obj['Type'] == 'Buy Special Poperations':
-                        ind = dict_obj['Index']
-                        self.special_poperations = ind
-                        self.logs.append("Upgrading the heli farm at index %s into special poperations!"%(ind))
-                    elif dict_obj['Type'] == 'Repeatedly Buy Heli Farms':
-                        self.heli_farm_max_buy_time = dict_obj['Maximum Buy Time']
-                        self.heli_farm_buffer = dict_obj['Buffer']
-                        self.logs.append("Triggered automated heli farm purchases until time %s"%(self.heli_farm_max_buy_time))
-
-                    # JERICHO RELATED MATTERS
-                    elif dict_obj['Type'] == 'Jericho Steal':
-                        self.jericho_steal_time = dict_obj['Minimum Buy Time']
-                        self.jericho_steal_amount = dict_obj['Steal Amount']
-                        self.cash, self.loan = impact(self.cash,self.loan, dict_obj['Steal Amount']) #If this line is not here, the sim would fail to capture the jeri payment that occurs immediately upon activation.
-                        
                 #Now, we have finished the for loop through purchase_info and thus correctly performed the buys
                 #Remove the buy from the queue and set self.buy_cost to None so the code knows next time to re-compute
                 #the buy cost for the next item in the buy queue
                 self.min_buy_time = None
                 self.buffer = 0
                 self.buy_queue.pop(0)
                 self.logs.append("Completed the buy operation! The buy queue now has %s items remaining in it"%(len(self.buy_queue)))
@@ -1693,14 +1298,433 @@
             self.event_messages.append({
                 'Time': payout['Time'], 
                 'Type': "Buy", 
                 'Message': buy_message
             })
         
         return made_purchase
+    
+    def processAction(self, dict_obj, payout, h_cash = None, h_loan = None, stage = 'check'):
+        # Helper method for processBuyQueue
+        # This is essentially just one giant if-elif block
+
+        # processBuyQueue will use this method in two stages. 
+        # The first stage is for checking if the next transaction in the buy queue can be performed.
+        # The second stage is for actually carrying out the transaction
+
+        # DEFENSE RELATED MATTERS
+        if dict_obj['Type'] == 'Buy Defense':
+            if stage == 'check':
+                h_cash, h_loan = impact(h_cash, h_loan, -1*dict_obj['Cost'])
+            # We don't need to do anything here in the processing stage
+        # FARM RELATED MATTERS
+        elif dict_obj['Type'] == 'Buy Farm':
+            if stage == 'check':
+                h_new_cash, h_new_loan = impact(h_cash, h_loan, -1*farm_globals['Farm Cost'])
+            else:
+                self.logs.append("Purchasing farm!")
+                farm_info = {
+                    'Purchase Time': self.current_time,
+                    'Upgrades': [0,0,0]
+                }
+                farm = MonkeyFarm(farm_info)
+                self.farms.append(farm)
+
+                #For revenue and expense tracking
+                farm.revenue = 0
+                farm.expenses = farm_globals['Farm Cost']
+        elif dict_obj['Type'] == 'Upgrade Farm':
+            if stage == 'check':
+                ind = dict_obj['Index']
+                path = dict_obj['Path']
+                farm = self.farms[ind]
+                #Do not upgrade a farm that has already been sold!
+                if farm.sell_time is not None:
+                    self.logs.append("WARNING! Tried to upgrade a farm that was already sold! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+
+                #The following code prevents from the player from having multiple T5's in play
+                if farm.upgrades[path]+1 == 5 and self.T5_exists[path] == True:
+                    self.logs.append("WARNING! Tried to purchase a T5 farm when one of the same kind already existed! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                h_cash, h_loan = impact(h_cash, h_loan, -1*farm_upgrades_costs[path][farm.upgrades[path]])
+            else:
+                ind = dict_obj['Index']
+                path = dict_obj['Path']
+                
+                self.logs.append("Upgrading path %s of the farm at index %s"%(path, ind))
+                farm = self.farms[ind]
+
+                #For expense tracking
+                farm.expenses += farm_upgrades_costs[path][farm.upgrades[path]]
+
+                farm.upgrades[path] += 1
+
+                #Update the payout information of the farm
+                farm.payout_amount = farm_payout_values[tuple(farm.upgrades)][0]
+                farm.payout_frequency = farm_payout_values[tuple(farm.upgrades)][1]
+                
+                #So that we can accurately track payments for the farm
+                farm.purchase_time = payout['Time']
+                
+                #Update the sellback value of the farm
+                farm.sell_value = farm_sellback_values[tuple(farm.upgrades)]
+                
+                self.logs.append("The new farm has upgrades (%s,%s,%s)"%(farm.upgrades[0],farm.upgrades[1],farm.upgrades[2]))
+                
+                #If the resulting farm is a Monkey Bank, indicate as such and set its max account value appropriately
+                if farm.upgrades[1] >= 3 and path == 1:
+                    farm.bank = True
+                    farm.max_account_value = farm_bank_capacity[farm.upgrades[1]]
+                    self.logs.append("The new farm is a bank! The bank's max capacity is %s"%(farm.max_account_value))
+                    
+                #If the resulting farm is an IMF Loan or Monkeyopolis, determine the earliest time the loan can be used
+                if farm.upgrades[1] > 3 and path == 1:
+                    farm.min_use_time = payout['Time'] + farm_globals['Monkeynomics Initial Cooldown']
+                
+                #If the resulting farm is a Banana Central, activate the BRF buff, giving them 25% more payment amount
+                if farm.upgrades[0] == 5 and path == 0:
+                    self.logs.append("The new farm is a Banana Central!")
+                    self.T5_exists[0] = True
+                    
+                #If the resutling farm is a Monkeyopolis, mark the x5x_exists flag as true to prevent the user from trying to have multiple of them
+                if farm.upgrades[1] == 5:
+                    self.T5_exists[1] = True
+                
+                #If the resulting farm is a MWS, mark the MWS_exists flag as true to prevent the user from trying to have multiple of them.
+                if farm.upgrades[2] == 5:
+                    self.T5_exists[2] = True
+        elif dict_obj['Type'] == 'Sell Farm':
+            if stage == 'check':
+                ind = dict_obj['Index']
+                farm = self.farms[ind]
+                withdraw = dict_obj['Withdraw']
+
+                #Check whether the farm is actually on screen before selling it:
+                h_new_cash, h_new_loan = h_cash, h_loan
+                if farm.sell_time is None:
+                    #If indicated, withdraw from the bank before selling it
+                    if withdraw and farm.upgrades[1] >= 3:
+                        h_new_cash, h_new_loan = impact(h_new_cash, h_new_loan, farm.account_value)
+                    #Selling a farm counts as that farm generating revenue
+                    h_new_cash, h_new_loan = impact(h_new_cash, h_new_loan, farm_sellback_values[tuple(farm.upgrades)])
+                    farm.h_revenue += h_new_cash - h_cash
+                    h_cash, h_loan = h_new_cash, h_new_loan
+                else:
+                    self.logs.append("WARNING! Tried to sell a farm that is not on screen! Aborting buy queue")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+            else:
+                ind = dict_obj['Index']
+                farm = self.farms[ind]
+                self.logs.append("Selling the farm at index %s"%(ind))
+
+                # If the farm being sold is a Banana Central, we must turn off the BRF buff
+                # If the farm is a T5 of any sorts, ensure that the game state knows we no longer that particular T5
+
+                if farm.upgrades[0] == 5:
+                    self.logs.append("The farm we're selling is a Banana Central! Removing the BRF buff.")
+                    self.T5_exists[0] = False
+                elif farm.upgrades[1] == 5:
+                    self.T5_exists[1] = False
+                elif farm.upgrades[2] == 5:
+                    self.T5_exists[2] = False
+
+                #Mark the farm's sell time. The code checks whether this value is a number or not before trying to compute farm payments
+                farm.sell_time = payout['Time']
+        elif dict_obj['Type'] == 'Sell All Farms':
+            if stage == 'check':
+                for farm in self.farms:
+                    if farm.sell_time is None:
+                        h_new_cash, h_new_loan = h_cash, h_loan
+                        #Withdraw from the bank first, provided that the withdraw argument is True *and* the farm given is actually a bank
+                        if withdraw and farm.upgrades[1] >= 3:
+                            h_new_cash, h_new_loan = impact(h_new_cash, h_new_loan, farm.account_value)
+
+                        #Now, sell the farm
+                        h_new_cash, h_new_loan = impact(h_new_cash, h_new_loan, farm_sellback_values[tuple(farm.upgrades)])
+                        farm.h_revenue += h_new_cash - h_cash
+                        h_cash, h_loan = h_new_cash, h_new_loan
+            else:
+                self.logs.append("Selling all farms!")
+                self.T5_exists = [False for i in range(3)] #Obviously, if we sell all farms we won't have any T5's anymore!
+                for farm in self.farms:
+                    farm.sell_time = payout['Time']
+        elif dict_obj['Type'] == 'Withdraw Bank':
+            if stage == 'check':
+                #WARNING: The farm in question must actually be a bank for us to perform a withdrawal!
+                #If it isn't, break the loop prematurely
+                ind = dict_obj['Index']
+                farm = self.farms[ind]
+                if farm.sell_time is not None:
+                    self.logs.append("WARNING! Tried to withdraw from a bank that was already sold! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+
+                if farm.upgrades[1] < 3:
+                    self.logs.append("WARNING! Tried to Withdraw from a farm that is not a bank! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                
+                h_new_cash, h_new_loan = impact(h_cash, h_loan, farm.account_value)
+                # self.logs.append("Detected bank withdrawal of %s"%(h_new_cash - h_cash))
+                farm.h_revenue += h_new_cash - h_cash
+                h_cash, h_loan = h_new_cash, h_new_loan
+            else:
+                ind = dict_obj['Index']
+                self.logs.append("Withdrawing money from the bank at index %s"%(ind))
+                farm = self.farms[ind]
+                farm.account_value = 0
+        elif dict_obj['Type'] == 'Activate IMF':
+            if stage == 'check':
+                #WARNING: The farm in question must actually be an IMF Loan for us to use this ability!
+                #If it isn't, set a flag to False and break the loop.
+                #DEVELOPER'S NOTE: A farm that has a min_use_time is not necessarily an IMF loan, it could also be an Monkeyopolis
+                #Do not upgrade a farm that has already been sold!
+                ind = dict_obj['Index']
+                farm = self.farms[ind]
+
+                if farm.sell_time is not None:
+                    self.logs.append("WARNING! Tried to take out a loan from a bank that was already sold! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+
+                if farm.upgrades[1] != 4:
+                    self.logs.append("WARNING! Tried to take out a loan from a farm that is not an IMF! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                    
+                ind = dict_obj['Index']
+                farm = self.farms[ind]
+                
+                #When, a loan is activated, treat it like a payment, then add the debt
+                h_new_cash, h_new_loan = impact(h_cash, h_loan, farm_globals['IMF Loan Amount'])
+                farm.h_revenue += h_new_cash - h_cash
+                h_new_loan += farm_globals['IMF Loan Amount']
+                h_cash, h_loan = h_new_cash, h_new_loan
+            else:
+                ind = dict_obj['Index']
+                farm = self.farms[ind]
+                self.logs.append("Taking out a loan from the IMF at index %s"%(ind))
+                farm.min_use_time = payout['Time'] + farm_globals['IMF Usage Cooldown']
+        # BOAT FARM RELATED MATTERS
+        elif dict_obj['Type'] == 'Buy Boat Farm':
+            if stage == 'check':
+                h_cash, h_loan = impact(h_cash, h_loan, -1*boat_globals['Merchantmen Cost'])
+            else:
+                self.logs.append("Purchasing boat farm!")
+                boat_farm = {
+                    'Initial Purchase Time': self.current_time,
+                    'Purchase Time': self.current_time,
+                    'Upgrade': 3,
+                    'Revenue': 0,
+                    'Expenses': boat_globals['Merchantmen Cost'],
+                    'Hypothetical Revenue': 0,
+                    'Sell Time': None
+                }
+                self.boat_farms[self.boat_key] = boat_farm
+                self.boat_key += 1
+        elif dict_obj['Type'] == 'Upgrade Boat Farm':
+            if stage == 'check':
+                ind = dict_obj['Index']
+                boat_farm = self.boat_farms[ind]
+                #The following code prevents from the player from having multiple Trade Empires in play
+                if boat_farm['Upgrade']+1 == 5 and self.Tempire_exists == True:
+                    self.logs.append("WARNING! Tried to purchase a Trade Empire when one already exists! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                upgrade_cost = boat_upgrades_costs[boat_farm['Upgrade']-3]
+                h_cash, h_loan = impact(h_cash, h_loan, -1*upgrade_cost)
+            else:
+                ind = dict_obj['Index']
+                        
+                self.logs.append("Upgrading the boat farm at index %s"%(ind))
+                boat_farm = self.boat_farms[ind]
+                boat_farm['Upgrade'] += 1
+
+                #Expense tracking
+                boat_farm['Expenses'] += boat_upgrades_costs[boat_farm['Upgrade'] - 4]
+                
+                #Update the payout information of the boat farm
+                boat_farm['Payout'] = boat_payout_values[boat_farm['Upgrade'] - 3]
+                
+                #So that we can accurately track payments for the boat farm
+                boat['Purchase Time'] = payout['Time']
+                
+                #Update the sellback value of the boat farm
+                boat['Sell Value'] = boat_sell_values[boat_farm['Upgrade'] - 3]
+
+                #If the new boat farm is a Trade Empire, indicate as such
+                if boat_farm['Upgrade'] == 5:
+                    self.logs.append("The new boat farm is a Trade Empire!")
+                    self.Tempire_exists = True
+        elif dict_obj['Type'] == 'Sell Boat Farm':
+            if stage == 'check':
+                ind = dict_obj['Index']
+                boat_farm = self.boat_farms[ind]
+
+                #Check whether the boat farm is actually on screen before selling it:
+                if boat_farm['Sell Time'] is None:
+                    #Selling a farm counts as that farm generating revenue
+                    h_new_cash, h_new_loan = impact(h_cash, h_loan, boat_sell_values[boat_farm['Upgrade']-3])
+                    boat_farm['Hypothetical Revenue'] += h_new_cash - h_cash
+                    h_cash, h_loan = h_new_cash, h_new_loan
+                else:
+                    self.logs.append("WARNING! Tried to sell a boat farm that is not on screen! Aborting buy queue")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+            else:
+                ind = dict_obj['Index']
+                boat_farm = self.boat_farms[ind]
+                self.logs.append("Selling the boat farm at index %s"%(ind))
+                #If the farm being sold is a Trade Empire, indicate as such
+                if boat_farm['Upgrade'] == 5:
+                    self.logs.append("The boat farm we're selling is a Trade Empire! Removing the Tempire buff.")
+                    self.Tempire_exists = False
+
+                #Mark the boat farm's sell time
+                boat_farm['Sell Time'] = payout['Time']
+        # DRUID FARM RELATED MATTERS
+        elif dict_obj['Type'] == 'Buy Druid Farm':
+            if stage == 'check':
+                h_cash, h_loan = impact(h_cash, h_loan, -1*druid_globals['Druid Farm Cost'])
+            else:
+                self.druid_farms[self.druid_key] = payout['Time']
+                self.druid_key += 1
+                self.logs.append("Purchased a druid farm!")
+        elif dict_obj['Type'] == 'Sell Druid Farm':
+            if stage == 'check':
+                if dict_obj['Index'] == self.sotf:
+                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(druid_globals['Druid Farm Cost'] + druid_globals['Spirit of the Forest Upgrade Cost']))
+                else:
+                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*druid_globals['Druid Farm Cost'])
+            else:
+                ind = dict_obj['Index']
+                self.logs.append("Selling the druid farm at index %s"%(ind))
+                #If the druid we're selling is actually SOTF...
+                if self.sotf is not None and ind == self.sotf:
+                    self.logs.append("The druid farm being sold is a Spirit of the Forest!")
+                    self.sotf = None
+                    self.sotf_min_use_time = None
+        elif dict_obj['Type'] == 'Buy Spirit of the Forest':
+            if stage == 'check':
+                #WARNING: There can only be one sotf at a time!
+                if self.sotf is not None:
+                    self.logs.append("WARNING! Tried to purchase a Spirit of the Forest when one already exists! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                h_cash, h_loan = impact(h_cash, h_loan, -1*druid_globals['Spirit of the Forest Upgrade Cost'])
+            else:
+                ind = dict_obj['Index']
+                self.sotf = ind
+                self.logs.append("Upgrading the druid farm at index %s into a Spirit of the Forest!"%(ind))
+                #Determine the minimum time that the SOTF active could be used
+                i = np.floor((20 + payout['Time'] - self.druid_farms[ind])/40) + 1
+                self.sotf_min_use_time = payout['Time'] + 20 + 40*(i-1)
+        elif dict_obj['Type'] == 'Repeatedly Buy Druid Farms':
+            #Note, there is no "checking" stage for this action.
+            if stage != 'check':
+                self.druid_farm_max_buy_time = dict_obj['Maximum Buy Time']
+                self.druid_farm_buffer = dict_obj['Buffer']
+                self.logs.append("Triggered automated druid farm purchases until time %s"%(self.druid_farm_max_buy_time))
+        # SUPPLY DROP RELATED MATTERS
+        elif dict_obj['Type'] == 'Buy Supply Drop':
+            if stage == 'check':
+                h_cash, h_loan = impact(h_cash, h_loan, -1*sniper_globals['Supply Drop Cost'])
+            else:
+                self.supply_drops[self.sniper_key] = payout['Time']
+                self.sniper_key += 1
+                self.logs.append("Purchased a supply drop!")
+        elif dict_obj['Type'] == 'Sell Supply Drop':
+            if stage == 'check':
+                if dict_obj['Index'] == self.elite_sniper:
+                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(sniper_globals['Supply Drop Cost'] + sniper_globals['Elite Sniper Upgrade Cost']) )
+                else:
+                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*sniper_globals['Supply Drop Cost'])
+            else:
+                ind = dict_obj['Index']
+                self.logs.append("Selling the supply drop at index %s"%(ind))
+                #If the supply drop we're selling is actually an E-sniper, then...
+                if self.elite_sniper is not None:
+                    if ind == self.elite_sniper:
+                        self.logs.append("The supply drop being sold is an elite sniper!")
+                        self.elite_sniper = None
+        elif dict_obj['Type'] == 'Buy Elite Sniper':
+            if stage == 'check':
+                #WARNING: There can only be one e-sniper at a time!
+                if self.elite_sniper is not None:
+                    self.logs.append("WARNING! Tried to purchase an Elite Sniper when one already exists! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                h_cash, h_loan = impact(h_cash, h_loan, -1*sniper_globals['Elite Sniper Upgrade Cost'])
+            else:
+                ind = dict_obj['Index']
+                self.elite_sniper = ind
+                self.logs.append("Upgrading the supply drop at index %s into an elite sniper!"%(ind))
+        elif dict_obj['Type'] == 'Repeatedly Buy Supply Drops':
+            #There is no checking stage for this action
+            if stage != 'check':
+                self.supply_drop_max_buy_time = dict_obj['Maximum Buy Time']
+                self.supply_drop_buffer = dict_obj['Buffer']
+                self.logs.append("Triggered automated supply drop purchases until time %s"%(self.supply_drop_max_buy_time))
+        # HELI FARM RELATED MATTERS
+        elif dict_obj['Type'] == 'Buy Heli Farm':
+            if stage == 'check':
+                h_cash, h_loan = impact(h_cash, h_loan, -1*heli_globals['Heli Farm Cost'])
+            else:
+                self.heli_farms[self.heli_key] = payout['Time']
+                self.heli_key += 1
+                self.logs.append("Purchased a heli farm!")
+        elif dict_obj['Type'] == 'Sell Heli Farm':
+            if stage == 'check':
+                if dict_obj['Index'] == self.special_poperations:
+                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*(heli_globals['Heli Farm Cost'] + heli_globals['Special Poperations Upgrade Cost']) )
+                else:
+                    h_cash, h_loan = impact(h_cash, h_loan, game_globals['Sellback Value']*heli_globals['Heli Farm Cost'])
+            else:
+                ind = dict_obj['Index']
+                self.logs.append("Selling the heli farm at index %s"%(ind))
+                #If the supply drop we're selling is actually a special poperations, then...
+                if self.special_poperations is not None:
+                    if ind == self.special_poperations:
+                        self.logs.append("The heli farm being sold is a special poperations!")
+                        self.elite_sniper = None
+                
+                self.supply_drops.pop(ind)
+        elif dict_obj['Type'] == 'Buy Special Poperations':
+            if stage == 'check':
+                #WARNING: There can only be one Special Poperations on screen at a time!
+                if self.special_poperations is not None:
+                    self.logs.append("WARNING! Tried to purchase Special Poperations when one already exists! Aborting buy queue!")
+                    self.warnings.append(len(self.logs)-1)
+                    self.valid_action_flag = False
+                h_cash, h_loan = impact(h_cash, h_loan, -1*heli_globals['Special Poperations Upgrade Cost'])
+            else:
+                ind = dict_obj['Index']
+                self.special_poperations = ind
+                self.logs.append("Upgrading the heli farm at index %s into special poperations!"%(ind))
+        elif dict_obj['Type'] == 'Repeatedly Buy Heli Farms':
+            #This action does not have a checking stage.
+            if stage != 'check':
+                self.heli_farm_max_buy_time = dict_obj['Maximum Buy Time']
+                self.heli_farm_buffer = dict_obj['Buffer']
+                self.logs.append("Triggered automated heli farm purchases until time %s"%(self.heli_farm_max_buy_time))
+        # JERICHO RELATED MATTERS
+        elif dict_obj['Type'] == 'Jericho Steal':
+            if stage != 'check':
+                self.jericho_steal_time = dict_obj['Minimum Buy Time']
+                self.jericho_steal_amount = dict_obj['Steal Amount']
+                self.cash, self.loan = impact(self.cash,self.loan, dict_obj['Steal Amount']) #If this line is not here, the sim would fail to capture the jeri payment that occurs immediately upon activation.
+                
+        if stage == 'check':
+            return h_cash, h_loan
+        elif stage == 'process':
+            return None
             
 # %% [markdown]
 # Now it's time to define the MonkeyFarm class!
 
 # %%
 class MonkeyFarm():
     def __init__(self, initial_state):
@@ -1876,43 +1900,8 @@
     ax[1].legend(loc='upper left', fontsize = font_size)
     
     d = {'Game State': [i for i in range(N)], 'Farm Income': [farm_incomes[i] for i in range(N)]}
     df = pd.DataFrame(data=d)
     
     fig.tight_layout()
     display(df)
-    logs.append("Successfully generated graph! \n")
-
-# def equivalentEcoImpact(time_tuple, rounds, farms = None, boat_farms = None, druid_farms = None, supply_drops = None, time_type = 'Rounds'):
-#     #Given some collection of farms and a span of time, determine the amount of the eco that would make the same amount of money as those farms in that time span
-#     assert type(time_tuple) == tuple and len(time_tuple) == 2, "ERROR! time_tuple must be of the form (start, end)"
-
-#     #We expect in most cases that the player will indicate start and end rounds for this function. In that case, convert the starting round and ending rounds to times
-#     if time_type == 'Rounds':
-#         start_time = rounds.getTimeFromRound(time_tuple[0])
-#         end_time = rounds.getTimeFromRound(time_tuple[1])
-
-#     #If the farms contain any banks, we will add actions to the buy queue to withdraw from these banks upon reaching the target time
-#     buy_queue = []
-
-#     for farm_info_entry in farms:
-#         if farms[key]['Upgrades'][1] >= 3:
-#             buy_queue.append([withdrawBank(key, min_buy_time = end_time)])
-
-#     initial_state_game = {
-#         'Cash': 0,
-#         'Eco': 0,
-#         'Rounds': rounds,
-#         'Game Time': start_time,
-#         'Farms': farms,
-#         'Boat Farms': boat_farms,
-#         'Druid Farms': druid_farms,
-#         'Supply Drops': supply_drops
-#     }
-
-#     game_state = GameState(initial_state_game)
-#     game_state.fastForward(target_time = end_time)
-
-#     #Now compute the formula for equivlaent eco impact
-#     return 6*game_state.cash/(end_time - start_time)
-
-# %%
+    logs.append("Successfully generated graph! \n")
```

### Comparing `b2sim-1.0.9/b2sim/rounds.py` & `b2sim-1.1.0/b2sim/rounds.py`

 * *Files identical despite different names*

### Comparing `b2sim-1.0.9/b2sim/templates/eco_send_info.csv` & `b2sim-1.1.0/b2sim/templates/eco_send_info.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿send_name,price,eco,start_round,end_round,send_duration,fortified,camo,regrow,moab_class
 Zero,0,0,0,50,0,FALSE,FALSE,FALSE,FALSE
-Grouped Reds,20,1,1,10,0.8,FALSE,TRUE,TRUE,FALSE
+Grouped Reds,20,1,1,11,0.8,FALSE,TRUE,TRUE,FALSE
 Spaced Blues,15,0.8,1,2,1.5,FALSE,TRUE,TRUE,FALSE
-Grouped Blues,24,1,3,10,0.6,FALSE,TRUE,TRUE,FALSE
+Grouped Blues,24,1,3,11,0.6,FALSE,TRUE,TRUE,FALSE
 Spaced Greens,18,0.9,2,4,1.15,FALSE,TRUE,TRUE,FALSE
 Grouped Greens,35,1.4,5,16,0.4,FALSE,TRUE,TRUE,FALSE
 Spaced Yellows,24,1.2,3,6,1.15,FALSE,TRUE,TRUE,FALSE
 Grouped Yellows,40,1.6,7,19,0.24,FALSE,TRUE,TRUE,FALSE
 Spaced Pinks,28,1.4,4,8,0.9,FALSE,TRUE,TRUE,FALSE
 Grouped Pinks,65,2.4,9,50,0.2,FALSE,TRUE,TRUE,FALSE
 Spaced Whites,30,1.5,5,50,0.84,FALSE,TRUE,TRUE,FALSE
```

