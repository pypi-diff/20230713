# Comparing `tmp/alanapy-0.12.tar.gz` & `tmp/alanapy-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alanapy-0.12.tar", last modified: Thu Jul 13 02:54:48 2023, max compression
+gzip compressed data, was "alanapy-0.9.tar", last modified: Thu Jun 22 00:10:02 2023, max compression
```

## Comparing `alanapy-0.12.tar` & `alanapy-0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 02:54:48.547022 alanapy-0.12/
--rw-rw-rw-   0        0        0     1085 2023-06-15 19:50:23.000000 alanapy-0.12/LICENSE
--rw-rw-rw-   0        0        0     2685 2023-07-13 02:54:48.545027 alanapy-0.12/PKG-INFO
--rw-rw-rw-   0        0        0     2097 2023-07-13 02:52:37.000000 alanapy-0.12/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 02:54:48.544030 alanapy-0.12/alanapy.egg-info/
--rw-rw-rw-   0        0        0     2685 2023-07-13 02:54:47.000000 alanapy-0.12/alanapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-13 02:54:48.000000 alanapy-0.12/alanapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 02:54:47.000000 alanapy-0.12/alanapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-07-13 02:54:47.000000 alanapy-0.12/alanapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 02:54:47.000000 alanapy-0.12/alanapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    76830 2023-07-13 02:35:45.000000 alanapy-0.12/alanapy.py
--rw-rw-rw-   0        0        0       42 2023-07-13 02:54:48.547022 alanapy-0.12/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-07-13 02:54:03.000000 alanapy-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:10:02.134517 alanapy-0.9/
+-rw-rw-rw-   0        0        0     1085 2023-06-15 19:50:23.000000 alanapy-0.9/LICENSE
+-rw-rw-rw-   0        0        0      634 2023-06-22 00:10:02.133519 alanapy-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-06-15 19:50:23.000000 alanapy-0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 00:10:02.130537 alanapy-0.9/alanapy.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-22 00:10:01.000000 alanapy-0.9/alanapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    71641 2023-06-21 23:47:13.000000 alanapy-0.9/alanapy.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 00:10:02.134517 alanapy-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      884 2023-06-22 00:09:51.000000 alanapy-0.9/setup.py
```

### Comparing `alanapy-0.12/LICENSE` & `alanapy-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alanapy-0.12/alanapy.py` & `alanapy-0.9/alanapy.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             self._fieldmasterdict_all = self._getGenericDict("fieldmaster", fulldict=True)
             self.fieldmasterdict = self._fieldmasterdict_all[1]
             self.fieldmasterdict_inv = self._fieldmasterdict_all[2]
             ## Formation dicts
             self._formationmasterdict_all = self._getGenericDict("formationmaster", fulldict=True)
             self.formationmasterdict = self._formationmasterdict_all[1]
             ## VA
+                                                                                            
+                                                                 
+                                                                      
+
             self._fdpmasterdict_all = self._getGenericDict("fdpmaster", fulldict=True)
             self.fdpmasterdict = self._getGenericDict("fdpmaster")
             self.fdpmaster_full = self._fdpmasterdict_all[0]
 
             self.dcamasterdict = self._getGenericDict("dcamaster")
             self.welltypemasterdict = self._getGenericDict('welltypemaster',fulldict=False)
             # self.fdpmasterdict = self._getGenericDict("fdpmaster")
@@ -245,14 +249,17 @@
             self.opexmasterdict = self._getGenericDict(master_table)
         elif master_table == "pricedeck":
             self.pricedeckdict = self._getGenericDict(master_table)
         elif master_table == "abandonmentmaster":
             self.abandonmentmaster = self._getGenericDict(master_table)
         elif master_table == "genericprodinjmaster":
             self.genericprodinjmaster = self._getGenericDict(master_table)
+
+        
+        
         if(mydata.status_code == 204):
             print("Success")
         else:
             print(mydata.status_code)
             print("Error")
         return mydata
     
@@ -456,43 +463,40 @@
 
 class Economics:
     def __init__(self):
         self.master = Singleton().master
 
     def runEconomics(self, params={}):
         """
-        {
-        "description":,
-        "returns":,
-        "example":,
-        }
+            args(self, master_fk)
         """
         if len(params) == 0:
             return "Please provide the params dictionary, refer to the documentation of this function"
 
         url = self.master.root_url + "/api/economics/runeconomics/"
         header = self.master.header
         mydata = requests.get(url, headers=header, params=params)  # .json()
         results = mydata.json()
         return results
 
     def createEconomicForecastMaster(self, _dict: dict):
         """
         {
-        "description":"Function that creates a Master for Economic Forecast",
-        "arguments":{
+        "description": "Function that creates a Master for Economic Forecast",
+        "arguments":
+            {
                 "name": "",
                 "description": ""
             },
-        "return":{
+        "return": {
                 "id": "",
                 "name": "",
                 "description": ""
             },
-        "example":,
+        "example": ""
         }
         """
         dict_response_api = self.master._createMaster("economics", "economicforecastmaster", _dict)
         return dict_response_api
 
     def editEconomicForecastMaster(self, master_fk: int, dict_edit_master: dict):
         """
@@ -1003,43 +1007,35 @@
                 "updated_at": "YYYY-MM-DD",
                 "description": "Empty",
                 "start_date": "YYYY-MM-DD",
                 "end_date": "YYYY-MM-DD",
                 "scope": "PUBLIC"
                 }
             },
-        "return":{
-            dict_response : {
-            }
-        },
         "example": ""
         }
         """
         dict_fdpmaster = self.master._createMaster("fdp", "fdpmaster", fdp_master_dict)
         return dict_fdpmaster
     
     def createFDPCase(self, case_app, case_table, list_of_dicts, str_fdp_name):
         """
         {
-            "description": "Create a Field Development Plan ",
-            "arguments" : {
-                dict_main : {
-                    "name": "str_fdp_name",
-                    "created_at": "YYYY-MM-DD",
-                    "updated_at": "YYYY-MM-DD",
-                    "description": "Empty",
-                    "start_date": "YYYY-MM-DD",
-                    "end_date": "YYYY-MM-DD",
-                    "scope": "PUBLIC"
-                    }
-                },
-            "return":{
-                "dict_response": {
+        "description": "Create a Field Development Plan ",
+        "arguments" : {
+            dict_main : {
+                "name": "str_fdp_name",
+                "created_at": "YYYY-MM-DD",
+                "updated_at": "YYYY-MM-DD",
+                "description": "Empty",
+                "start_date": "YYYY-MM-DD",
+                "end_date": "YYYY-MM-DD",
+                "scope": "PUBLIC"
                 }
-        },
+            },
         "example": ""
         }
         """
         df_temp = pd.DataFrame(list_of_dicts)
         df_temp["welltype_fk"] = ""
         df_temp["dcamaster_fk"] = ""       
         # fdpMaster
@@ -1148,24 +1144,20 @@
             bool_status = mygeneric.statusCodeCheck(mydata)
             if bool_status:
                 fdp_case = mydata.json()
                 
     def runFDP(self, str_fdp_name, preffix="FDP_"):
         """
         }
-            "description": "Run FDP given by a FDP master and its cases",
-            "arguments" : {
-                "FDP_master_name" : "str_fdp_master"
-                "Preffix" : "FDP_"
-                },
-            "return" : {
-            "dict_response":{
-            }
+        "description": "",
+        "arguments" : {
+            "FDP_master_name" : "str_fdp_master"
+            "Preffix" : "FDP_"
             },
-            "example": "",
+        "example": "",
         }
         """
         int_id_master = self.master.fdpmasterdict[str_fdp_name]
         url = self.master.root_url + "/api/" + "fdp/runfdp/"
         header = self.master.header
         params = {
             "fdpmaster_fk" : int_id_master ,
@@ -1181,25 +1173,18 @@
         """
         tuple_response_api = self.master._createMasterCases("fdp", "fdpmaster", _dict, list_of_dicts, "fdp", "fdpcase")
         print(tuple_response_api)
         return tuple_response_api
 
     def getFDPCases(self, master_fk: str):
         """
-        {
-            "description":"Function that return the cases that match with the master_fk",
-            "arguments":{
-                "master_fk" : int
-            },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
-        }
+        Function that return the cases that match with the master_fk
+        args(master_fk)
+        master_fk = Integer
+        RETURN dict_get_cases
         """
         dict_get_cases = self.master._getMaster("fdp", "fdpcase", str(master_fk))
         print(dict_get_cases)
         return dict_get_cases
 
     def createFDPMasterAndCases(self, _dict: dict, list_of_dicts: list):
         """
@@ -1207,419 +1192,316 @@
         """
         tuple_response_api = self.master._createMasterCases("downtime", "downtimemaster", _dict, list_of_dicts, "downtime", "downtimecase")
         print(tuple_response_api)
         return tuple_response_api
 
     def getFDPDowtimeCases(self, master_fk: str):
         """
-        {
-            "description":"Function that return the cases that match with the master_fk",
-            "arguments":{
-                "master_fk" : int
-            },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
-        }
+        Function that return the cases that match with the master_fk
+        args(master_fk)
+        master_fk = Integer
+        RETURN dict_get_cases
         """
         dict_get_cases = self.master._getMaster("fdp", "downtimecase", str(master_fk))
         print(dict_get_cases)
         return dict_get_cases
 
 class Datasource:
     def __init__(self):
         self.master = Singleton().master
 
     def createWellMaster(self, well_master_dict: dict):
         """
         {
-            "description": "Function that create Wells",
-            "arguments" : {
-                "dict_main" : {
-                    "well_name": "",
-                    "spud_date": "YYYY-MM-DD",
-                    "production_date": "YYYY-MM-DD",
-                    "api_code": int,
-                    "latitude": float,
-                    "longitude": float,
-                    "utm_x": float,
-                    "utm_y": float,
-                    "comment": "",
-                    "type": ""
-                    "field": "str_field"
-                    }
-                },
-            "return": {
-                dict_response : {
-                }
+        "description": "Function that create Wells",
+        "arguments" : {
+            "well_name": "",
+            "spud_date": "YYYY-MM-DD",
+            "production_date": "YYYY-MM-DD",
+            "api_code": int,
+            "latitude": float,
+            "longitude": float,
+            "utm_x": float,
+            "utm_y": float,
+            "comment": "",
+            "type": ""
+            "field": "str_field"
             },
-            "example": ""
+        "example": ""
         }
         """
         well_master_dict["field_fk"] = self.master.fieldmasterdict[well_master_dict["field"]]
         well_master_dict["formation_fk"] = self.master.formationmasterdict[well_master_dict["formation"]]
         dict_wellmaster = self.master._createMaster("datasource", "wellmaster", well_master_dict)
         return dict_wellmaster
 
     def getWellMaster(self, str_well_name=None):
         """
         {
             "description":"Function that fetch wellmaster information of a given name or whole table and return a dict.",
             "arguments":
-                {
-                    "str_well_name" : "str = None"
-                },
-            "return":{
-                "dict_response":{
-                }
+            {
+                "str_well_name" : "str = None"
             },
             "example" : "myapi.getWellMaster() or myapi.getWellMaster("well_name")"
         }
         """
         if str_well_name is None:
             dict_get_cases = self.master._getMaster("datasource", "wellmaster")
         else:
             int_well_id = self.master.wellmasterdict[str_well_name]
             dict_get_cases = self.master._getMaster("datasource", "wellmaster", str(int_well_id))
         return dict_get_cases
 
     def editWellMaster(self, master_fk: int, dict_edit_master: dict):
         """
-        {
-            "description":"Function that update a well master record",
-            "arguments":{
-                "dict_main" : {
-                    "well_name": "",
-                    "spud_date": "YYYY-MM-DD",
-                    "production_date": "YYYY-MM-DD",
-                    "api_code": int,
-                    "latitude": float,
-                    "longitude": float,
-                    "utm_x": float,
-                    "utm_y": float,
-                    "comment": "",
-                    "type": ""
-                    "field": "str_field"
-                    }
-                },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
+        Function that update a Master
+
+        dict_edit_master = {
+            "well_name": "",
+            "spud_date": None,
+            "production_date": None,
+            "api_code": "",
+            "latitude": "",
+            "longitude": "",
+            "utm_x": None,
+            "utm_y": None,
+            "comment": "",
+            "type": None,
+            "field_fk": None,
+            "formation_fk": None
         }
+        RETURN dict_edit_master
         """
         dict_edit_master = self.master._editMaster("datasource", "wellmaster", dict_edit_master,  str(master_fk))
         return dict_edit_master
 
     def deleteWellMaster(self, master_fk):
+        
         """
-        {
-            "description":"Function that delete the master that match with the master_fk",
-            "arguments":{
-                "master_fk" : int
-            },
-            "return":{
-                "dict_response":{
-                }
-            },
-            "example":,
-        }
+        Function that delete the master that match with the master_fk
+        args(master_fk)
+        RETURN deleted_master
         """
         deleted_master = self.master._deleteMaster("datasource", "wellmaster", str(master_fk))
         return deleted_master
 
     def createFormationMaster(self, formation_master_dict: dict):
         """
         {
-            "description": "Function that create Formations"
-            "arguments" : {
-                "main_dict":{
-                    "formation_name": "",
-                    "comment": ""
-                    }
-                },
-            "return":{
-                "dict_response":{
-                }
+        "description": "Function that create Formations"
+        }
+        "arguments" : {
+            "formation_name": "",
+            "comment": ""
             },
         "example": ""
         }
+            
         """
 
         dict_wellmaster = self.master._createMaster("datasource", "formationmaster", formation_master_dict)
         return dict_wellmaster
 
     def getFormationMaster(self, str_formation_name=None):
         """
         {
             "description":"Function that fetch formation information of a given name or whole table and return a dict.",
             "arguments":
             {
                 "str_formation_name" : "str = None"
             },
-            "return": {
-                "dict_response":{
-                }
-            },
             "example" : "myapi.getFormationMaster() or myapi.getFormationMaster("formation_name")"
         }
         """
         if str_formation_name is None:
             dict_get_cases = self.master._getMaster("datasource", "formationmaster")
         else:
             int_formation_id = self.master.formationmasterdict[str_formation_name]
             dict_get_cases = self.master._getMaster("datasource", "formationmaster", str(int_formation_id))
         return dict_get_cases
 
     def editFormationMaster(self, master_fk: int, dict_formation_master: dict):
         """
-        {
-            "description":"Function that updates a formation master record",
-            "arguments":{
-                "dict_main":{
-                    "formation_name":"",
-                    "comment":""
-                }
-            },
-            "return":,
-            "example":,
+        Function that update a Master
+        well_master_dict = {
+            "formation_name":"",
+            "comment":"",
         }
+        RETURN dict_edit_master
         """
         dict_edit_master = self.master._editMaster("datasource", "formationmaster", dict_formation_master,  str(master_fk))
         return dict_edit_master
 
     def deleteFormationMaster(self, master_fk):
         """
-        {
-			"description":"Function that delete the master that match with the master_fk",
-			"arguments":{
-                "master_fk":int
-            },
-			"return":{
-                "dict_response":{
-                }
-            },
-			"example":,
-        }
+        Function that delete the master that match with the master_fk
+        args(master_fk)
+        RETURN deleted_master
         """
         deleted_master = self.master._deleteMaster("datasource", "formationmaster", str(master_fk))
         return deleted_master
 
     def createFieldMaster(self, field_master_dict: dict):
         """
         {
-            "description": "Function that create Fields"
-            "arguments" : {
-                "field_name": "",
-                "comment": "",
-                "Country": "",
-                "Basin":"",
-                "Block":""
-                },
-            "return":{
-                "dict_main":{
-                }
+        "description": "Function that create Fields"
+        }
+        "arguments" : {
+            "field_name": "",
+            "comment": "",
+            "Country": "",
+            "Basin":"",
+            "Block":""
             },
-            "example": ""
+        "example": ""
         }
         """
+
         response_api = self.master._createMaster("datasource", "fieldmaster", field_master_dict)
         return response_api
 
     def getFieldMaster(self, str_field_name=None):
         """
         {
             "description":"Function that fetch field information of a given name or whole table and return a dict.",
-            "arguments":{
-                    "str_field_name" : "str = None"
-                },
-            "return":{
-                "dict_response":{
-                }
+            "arguments":
+            {
+                "str_field_name" : "str = None"
             },
             "example" : "myapi.getFieldMaster() or myapi.getFieldMaster("field_name")"
         }
         """
         if str_field_name is None:
             dict_get_cases = self.master._getMaster("datasource", "fieldmaster")
         else:
             int_field_id = self.master.fieldmasterdict[str_field_name]
             dict_get_cases = self.master._getMaster("datasource", "fieldmaster", str(int_field_id))
         return dict_get_cases
 
-    def editFieldMaster(self, master_fk: int, dict_field_master: dict):
+    def editFieldMaster(self, master_fk: int, dict_formation_master: dict):
         """
-        {
-			"description":"Function that update a field master record",
-			"arguments":{
-                "dict_main": {
-                    "field_name": "Given_Name",
-                    "comment": "",
-                    "Country": "",
-                    "Basin":"",
-                    "Block":""
-                }
-            },
-			"return": {
-                "dict_response":{
-                }
-            },
-			"example":,
+        Function that update a Master
+        field_master_dict = {
+            "field_name": "Given_Name",
+            "comment": "",
+            "Country": "",
+            "Basin":"",
+            "Block":""
         }
+        RETURN dict_edit_master
         """
-        dict_edit_master = self.master._editMaster("datasource", "fieldmaster", dict_field_master,  str(master_fk))
+        dict_edit_master = self.master._editMaster("datasource", "fieldmaster", dict_formation_master,  str(master_fk))
         return dict_edit_master
 
     def deleteFieldMaster(self, master_fk):
         """
         {
-            "description": "Function that deletes a Field"
-            "arguments" : {
-                "master_fk": int,
-                },
-            "return":{
-                "dict_response":{
-                }
+        "description": "Function that deletes a Field"
+        }
+        "arguments" : {
+            "master_fk": int,
             },
-            "example": ""
+        "example": ""
         }
             
         """
+        """
+        Function that delete the master that match with the master_fk
+        args(master_fk)
+        RETURN deleted_master
+        """
         deleted_master = self.master._deleteMaster("datasource", "fieldmaster", str(master_fk))
         return deleted_master
 
     def getFieldWellsDict(self):
         """
         {
-            "description":"Preloaded dictionary of fields and its wells",
-            "arguments":{
-            },
-            "return":{
-                "dict_response":{
-                }
+            "description":"Preloaded dictionary of {field_name: [well_name]}",
+            "arguments":
+            {
             },
             "example" : ""
         }
         """
         field_wells_dict = {}
         for field in list(self.master.fieldmasterdict.keys()):
             field_wells_dict[field] = self.master._getKeysDictList(field, self.getWellFieldDict())
         return field_wells_dict
 
     def getWellFieldDict(self):
         """
         {
-            "description":"Preloaded dictionary of well names and its field",
-            "arguments":{
-            },
-            return:{
-                "dict_response":{
-                }
+            "description":"Preloaded dictionary of {well_name:field_name}",
+            "arguments":
+            {
             },
             "example" : ""
         }
         """
         results = {}
         for welldict in self.master.wellmasterdict_full:
             results[welldict['well_name']] = self.master.fieldmasterdict_inv[welldict['field_fk']]
         return results
-        
-    def getWellDeviation(self,str_well_name = None):
-        """
-        {
-            "description":"Function that fetch the well deviation data of a given well name",
-            "arguments":{
-                "str_well_name":"str = None"
-            },
-            "return":{
-                "list_response":[{"keys":"items"
-                }]
-            }
-        """
-        if str_well_name == None:
-            print("Missing well name")
-        else : 
-            dict_welldeviations = self.master._getMaster("datasource", "welldeviation")
-            df = pd.DataFrame(dict_welldeviations)
-            int_well_id = self.master.wellmasterdict[str_well_name]
-            df_final = df[df["well_fk"] == int_well_id]
-            return df_final.to_dict(orient="records")
 
     def getMonthlyProduction(self, str_well_name: str):
         """
         {
             "description":"Function that fetch monthly production profile of a given well name",
-            "arguments":{
-                    "str_well_name" : "str = None"
-                },
-            "return":{
-                "dict_response":{
-                }
+            "arguments":
+            {
+                "str_well_name" : "str = None"
             },
             "example" : "myapi.getMonthlyProduction("well_name")"
         }
         """
         int_well_id = self.master.wellmasterdict[str_well_name]
         monthly_volume = self.master._getCase("datasource", "wellmonthly", "well_fk", int_well_id)
         return monthly_volume
     
     def getDailyProduction(self,str_well_name: str):
         """
         {
             "description":"Function that fetch daily production profile of a given well name",
-            "arguments":{
+            "arguments":
+            {
                 "str_well_name" : "str = None"
             },
-            "return":{
-                "dict_response":{
-                }
-            },
             "example" : "myapi.getDailyProduction("well_name")"
         }
         """
         int_well_id = self.master.wellmasterdict[str_well_name]
         daily_volume = self.master._getCase("datasource", "welldaily", "well_fk", int_well_id)
         return daily_volume
     
     def getFieldMonthlyProduction(self,str_field_name: str):
         """
         {
             "description":"Function that fetch field monthly production profile of a given field name",
-            "arguments":{
+            "arguments":
+            {
                 "str_field_name" : "str = None"
             },
-            "return":{
-                "dict_response":{
-                }
-            },
             "example" : "myapi.getFieldMonthlyProduction("field_name")"
         }
         """
         monthly_volume = self.master._getCase("datasource","fieldmonthly","fields[]", str_field_name)
         return monthly_volume
         
     def importDataSource(self, tablename, df_table, is_new_data=False):
         """
         {
-            "description": "Function that uploads a csv with data",
-            "arguments" : {
-                dict_main : {
-                    "tablename": "",
-                    "df_table": df_table,
-                    "is_new_date": True
-                }
+        "description": "Function that uploads a csv with data"
+        }
+        "arguments" : {
+            "tablename": "",
+            "df_table": df_table,
+            "is_new_date": True,
             },
-            "return":{
-                "dict_response":{
-                }
-            }
-            "example": ""
+        "example": ""
         }
             
         """
         #test_file = open("/Users/alejandroprimeranavarro/Alana/jupyter_samples/DCA_Summary_sampledata.csv", "rb")
         df_table.to_csv("importDataSource_temp.csv", index=False)
         file = open("importDataSource_temp.csv", "rb")
         url = self.master.root_url +"/api/datasource/dataloader/import/"
@@ -1774,31 +1656,27 @@
 class DCA:
     def __init__(self):
         self.master = Singleton().master
         
     def createDCAMaster(self, dca_master_dict):
         """
         {
-            "description": "Function that creates master for DCA Data",
-            "arguments" : {
-                "dict_main":{
-                    "name": "",
-                    "dca_method": "ARPS",
-                    "forecast_type": "DET",
-                    "primary_fluid_phase": "OIL",
-                    "dca_defaults": "",
-                    "dca_scope": "PUBLIC"
-                }
-            },
-            "return":{
-                "dict_response":{
-                }
+        "description": "Function that creates master for DCA Data"
+        }
+        "arguments" : {
+            "name": "",
+            "dca_method": "ARPS",
+            "forecast_type": "DET",
+            "primary_fluid_phase": "OIL",
+            "dca_defaults": "",
+            "dca_scope": "PUBLIC"
             },
-            "example": ""
+        "example": ""
         }
+            
         """
         dca_master_dict["name"] = dca_master_dict["str_dca_name"]
         dict_dca_master = self.master._createMaster("dca", "dcamaster", dca_master_dict)
         return dict_dca_master
         
     def runDCA(self, dict_dca):
         """
@@ -1821,15 +1699,14 @@
             return "All lists provided need to have the same size"
         url = self.master.root_url + "/api/dca/fit_forecast/"
         header = self.master.header
         mydata = requests.get(url, headers=header)
         dca_template_fit_forecast_base = mydata.json()
         wells_nofit = []
         wells_noprod = []
-        print("DCA Master")
         dca_master = self.createDCAMaster(dict_dca)
         dcamaster_fk = dca_master['id']
         mydatasource = Datasource()
         list_well_ids = [item["id"] for item in mydatasource.getWellMaster() for well in dict_dca["list_well_names"] if item["well_name"] == well]
         count_time_to_fit = 60
         count_time_to_discard_well_if_zero_rates = 6
         if (dict_dca["str_date_prod"] == "daily") or (dict_dca["str_date_prod"] == "monthly"):
@@ -1870,32 +1747,30 @@
                 x_selected = [x.strftime('%Y-%m-%d') for x in dates]
                 dca_template_fit_forecast['x_selected'] = x_selected
                 dca_template_fit_forecast['y_selected'] = rates
                 dca_template_fit_forecast['primary_phase_forecast_rate'] = rates_or[-1]
                 dca_template_fit_forecast['forecast_months'] = 420.0
                 dca_template_fit_forecast['primary_forecast_date'] = dict_dca["date_primary_forecast"][n]
                 dca_template_fit_forecast['primary_forecast_last_date'] = x_selected[-1]
-                dca_template_fit_forecast['primary_phase_abandonment'] = 0.0
+                dca_template_fit_forecast['primary_phase_abandonment'] = 1.0
                 dca_template_fit_forecast['fit_dates'] = x_selected
                 dca_template_fit_forecast['reinitialize_choice'] = 'NO'
                 dca_template_fit_forecast['fc_date_choice'] = "DEFAULT"
                 dca_template_fit_forecast['fc_rate_choice'] = "LASTVALFIT"
                 #print("dca_template_fit_forecast: ",dca_template_fit_forecast)
                 dca_forecast = self.master._fitForecastDCA(dates, rates, dca_template_fit_forecast)
                 # print("dca_forecast: ",dca_forecast)
                 # dca_forecast['primary_phase_forecast_rate'] = rates_or[-1]
                 # dca_forecast['arps_type'] = dca_arps
-                #print(f"_saveDCA:\n {dcamaster_fk}\n{list_well_ids[n]}\n{dca_forecast}\n{x_selected}\n{rates}\n{dca_template_fit_forecast}")
                 self.master._saveDCA(dcamaster_fk, list_well_ids[n], dca_forecast, x_selected, rates, dca_template_fit_forecast)
         #print("Total analyzed wells: ", len(dict_dca["list_well_names"]))#, "\nWells with issues: ",
               #[self.master._getKeyFromDict(well, self.master.wellmasterdict) for well in wells_nofit], "\n Total with issues: ",
               #len(wells_nofit), [self.master._getKeyFromDict(well, self.master.wellmasterdict) for well in wells_noprod],
               #"\n Total with no Production in the last 6 months: ", len(wells_noprod))
-        #print(f"Total analyzed wells: {len(dict_dca['list_well_names'])} \nWells with issues: {wells_nofit}")
-        print(f"Total analyzed wells:\n{len(dict_dca['list_well_names'])} \nWells with DCA: \n{[x for x in dict_dca['list_well_names'] if x not in wells_nofit]}\nWells with issues: \n{wells_nofit}")
+        print(f"Total analyzed wells: {len(dict_dca['list_well_names'])} \nWells with issues: {[self.master._getKeyFromDict(well, self.master.wellmasterdict) for well in wells_nofit]}")
 
     def editDCAMaster(self, master_fk: int, dict_edit_master: dict):
         dict_edit_master = self.master._editMaster("dca", "dcamaster", dict_edit_master, str(master_fk))
         return dict_edit_master
 
     def getDCAMaster(self, master_fk: str):
         dict_get_master = self.master._getMaster("dca", "dcamaster", str(master_fk))
@@ -1909,63 +1784,17 @@
         dict_response_api = self.master._createCases(list_of_dicts, "dca", "dcacase")
         return dict_response_api
 
     def createDCAMasterCases(self, _dict: dict, list_of_dicts: list):
         tuple_response_api = self.master._createMasterCases("dca", "dcamaster", _dict, list_of_dicts, "dca", "dcacase")
         return tuple_response_api
         
-class DatasourceEDA:
-    def __init__(self):
-        self.master = Singleton().master
-
-    def runNearByWells(self, dict_input):
-        """
-        {
-        "description": "Get Nearby wells given a well name and radius around it in metres"
-        }
-        "arguments" : {
-            well_name: "",
-            radius: float
-            },
-        "example": ""
-        }
-        """
-
-        url = self.master.root_url + "/api/datasource/eda/nearbywells/"
-        header = self.master.header
-        mydata = requests.get(url, headers=header, params=dict_input)  # .json()
-        results = mydata.json()
-        return results
-        
-
-
 class WellType:
-    def __init__(self):
+    def _init_(self):
         self.master = Singleton().master
-
-    def createWellType(self, welltype_master_dict):
-        """
-        {
-        "description": "Function that creates master for DCA Data"
-        }
-        "arguments" : {
-            "name": "",
-            "dca_method": "ARPS",
-            "forecast_type": "DET",
-            "primary_fluid_phase": "OIL",
-            "dca_defaults": "",
-            "dca_scope": "PUBLIC"
-            },
-        "example": ""
-        }
-
-        """
-        welltype_master_dict["name"] = welltype_master_dict["str_dca_name"]
-        dict_welltype_master = self.master._createMaster("welltype", "welltypemaster", welltype_master_dict)
-        return dict_welltype_master
         
     def runWellType(self, dict_welltype):
         """
         {
         "description": "Function that runs a welltype for a list of wells",
         "arguments":
             {
@@ -1989,15 +1818,15 @@
         }
         """
         mygeneric = Generic()
         url = self.master.root_url + "/api/welltype/welltype_calc/"
         dict_welltype = json.dumps(dict_welltype)
         header = {'Authorization': 'Token ' + self.master.credentials["alana_token"],
                   "content-type": "application/json"}
-        mydata = requests.get(url, headers=header, data=dict_welltype)  # .json()
+        mydata = requests.post(url, headers=header, data=dict_welltype)  # .json()
         bool_status = mygeneric.statusCodeCheck(mydata)
         if bool_status:
             dict_welltype_results = mydata.json()
             self.master._print(f"dict_welltype_results:{dict_welltype_results}")
             return dict_welltype_results
     
     def editWellTypeMaster(self, master_fk: int, dict_edit_master: dict):
```

### Comparing `alanapy-0.12/setup.py` & `alanapy-0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from pathlib import Path
 from setuptools import setup
 
 setup(
     name="alanapy",
-    version="0.12",
+    #packages=["alanapy"],
+    version="0.9",
     license="MIT",
     author = "Orkahub Energy",
 	author_email = "orkahub@gmail.com",
 	url = "https://github.com/orkahub/alanapy",
-    long_description=Path("README.md").read_text(encoding="utf-8"),
-    long_description_content_type = "text/markdown",
+    long_description="Script for Alana API connection and functions https://alana.tech/open/accounts/login",
+    long_description_content_type = "text/x-rst",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Topic :: Scientific/Engineering :: Visualization",
     ],
```

