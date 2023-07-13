# Comparing `tmp/ntdsdotsqlite-1.1.3.tar.gz` & `tmp/ntdsdotsqlite-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-1.1.3.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-1.1.4.tar", max compression
```

## Comparing `ntdsdotsqlite-1.1.3.tar` & `ntdsdotsqlite-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.3/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      821 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.3/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0      376 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.3/ntdsdotsqlite/basehandler.py
--rw-r--r--   0        0        0     7755 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.3/ntdsdotsqlite/computerhandler.py
--rw-r--r--   0        0        0     2066 2023-07-12 12:03:37.826505 ntdsdotsqlite-1.1.3/ntdsdotsqlite/containerhandler.py
--rw-r--r--   0        0        0    10591 2023-07-12 13:03:48.088424 ntdsdotsqlite-1.1.3/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     6842 2023-07-12 13:02:53.633713 ntdsdotsqlite-1.1.3/ntdsdotsqlite/domainhandler.py
--rw-r--r--   0        0        0     1743 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.3/ntdsdotsqlite/grouphandler.py
--rw-r--r--   0        0        0     3279 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.3/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     5733 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.3/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     2054 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/organizationalunithandler.py
--rw-r--r--   0        0        0     8022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/personhandler.py
--rw-r--r--   0        0        0     2022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/trusteddomainhandler.py
--rw-r--r--   0        0        0     3561 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.3/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      717 2023-07-12 13:05:31.989042 ntdsdotsqlite-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1494 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.3/README.md
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.3/setup.py
--rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.4/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.4/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0      376 2023-07-12 12:03:37.825507 ntdsdotsqlite-1.1.4/ntdsdotsqlite/basehandler.py
+-rw-r--r--   0        0        0     8127 2023-07-13 12:51:01.195762 ntdsdotsqlite-1.1.4/ntdsdotsqlite/computerhandler.py
+-rw-r--r--   0        0        0     2555 2023-07-13 12:59:07.536779 ntdsdotsqlite-1.1.4/ntdsdotsqlite/containerhandler.py
+-rw-r--r--   0        0        0    10591 2023-07-12 13:03:48.088424 ntdsdotsqlite-1.1.4/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     7226 2023-07-13 12:14:35.117775 ntdsdotsqlite-1.1.4/ntdsdotsqlite/domainhandler.py
+-rw-r--r--   0        0        0     1743 2023-07-12 12:03:37.827900 ntdsdotsqlite-1.1.4/ntdsdotsqlite/grouphandler.py
+-rw-r--r--   0        0        0     3425 2023-07-13 09:23:44.174030 ntdsdotsqlite-1.1.4/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     5751 2023-07-13 13:00:04.929780 ntdsdotsqlite-1.1.4/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     2100 2023-07-13 13:09:06.991011 ntdsdotsqlite-1.1.4/ntdsdotsqlite/organizationalunithandler.py
+-rw-r--r--   0        0        0     8374 2023-07-13 12:05:22.519068 ntdsdotsqlite-1.1.4/ntdsdotsqlite/personhandler.py
+-rw-r--r--   0        0        0     2022 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.4/ntdsdotsqlite/trusteddomainhandler.py
+-rw-r--r--   0        0        0     3561 2023-07-12 12:03:37.828930 ntdsdotsqlite-1.1.4/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      717 2023-07-13 13:10:05.609611 ntdsdotsqlite-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1494 2023-07-12 12:03:37.824508 ntdsdotsqlite-1.1.4/README.md
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.4/setup.py
+-rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.4/PKG-INFO
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/__main__.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/computerhandler.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/computerhandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -107,53 +107,61 @@
             :encrypted_ntPwdHistory, :ntPwdHistory, :accountExpires, :uac_flags, :parent, Null,
             :isDeleted, :primaryGroup, :isDisabled
             )
         """
         self.sqlite_db.execute(stmt, account)
 
     def callback(self):
-        # set the domain id
-        domain_id = self.sqlite_db.execute("SELECT id FROM domains").fetchone()[0]
         ous = {
-            oid: dn for oid, dn in self.sqlite_db.execute("SELECT id, dn FROM organizational_units")
+            oid: {"dn": dn, "domain": odid}
+            for oid, dn, odid in self.sqlite_db.execute(
+                "SELECT id, dn, domain FROM organizational_units"
+            )
         }
         machines = self.sqlite_db.execute(
-            "SELECT id, commonname, parent_OU, primaryGroup FROM user_accounts"
+            "SELECT id, commonname, parent_OU, primaryGroup FROM machine_accounts"
         )
         containers = {
-            cid: cdn for (cid, cdn) in self.sqlite_db.execute("SELECT id, dn FROM containers")
+            cid: {"dn": cdn, "domain": cdid}
+            for (cid, cdn, cdid) in self.sqlite_db.execute("SELECT id, dn, domain FROM containers")
         }
         domains = {
             did: ddn for (did, ddn) in self.sqlite_db.execute("SELECT id, dn FROM domain_dns")
         }
         for uid, cn, parent_OU, primaryGroup in machines:
             # Compute DN
             if parent_OU in ous.keys():
-                dn = f"CN={escape_dn_chars(cn)},{ous[parent_OU]}"
+                dn = f"CN={escape_dn_chars(cn)},{ous[parent_OU]['dn']}"
+                domain_id = ous[parent_OU]["domain"]
             elif parent_OU in containers.keys():
-                dn = f"CN={escape_dn_chars(cn)},{containers[parent_OU]}"
+                curdn = containers[parent_OU]['dn']
+                dn = f"CN={escape_dn_chars(cn)},{curdn}"
+                domain_id = containers[parent_OU]["domain"]
             elif parent_OU in domains.keys():
                 dn = f"CN={escape_dn_chars(cn)},{domains[parent_OU]}"
+                # Sets the domain ID to this "OU" ID since its the ID of the root domainDNS object
+                # in which this computer is.
+                domain_id = parent_OU
             else:
                 print(f"Warning: could not compute DN of machine {cn}")
             self.sqlite_db.execute(
-                "UPDATE machine_accounts set domain=?, primaryGroup=("
+                "UPDATE machine_accounts SET domain=?, primaryGroup=("
                 f"SELECT id from groups WHERE SID LIKE '%-{primaryGroup}'"
                 "), dn=? WHERE id=?",
                 (domain_id, dn, uid)
             )
-        # Decrypt users we could not decrypt previously
+        # Decrypt machine secrets we could not decrypt previously
         for account in self.could_not_decrypt_yet:
             account["nthash"] = decrypt_hash(self.peklist, account, "nt")
             account["lmhash"] = decrypt_hash(self.peklist, account, "lm")
             account["lmPwdHistory"] = decrypt_history(self.peklist, account, "lm")
             account["ntPwdHistory"] = decrypt_history(self.peklist, account, "nt")
             account["supplementalCredentials"] = decryptSupplementalInfo(self.peklist, account)
             self.sqlite_db.execute(
-                "UPDATE user_accounts set nthash=?, lmhash=?, ntPwdHistory=?, lmPwdHistory=?, "
+                "UPDATE machine_accounts set nthash=?, lmhash=?, ntPwdHistory=?, lmPwdHistory=?, "
                 "supplementalCredentials=? WHERE id=?",
                 (
                     account["nthash"], account["lmhash"], json.dumps(account["ntPwdHistory"]),
                     json.dumps(account["lmPwdHistory"]),
                     json.dumps(account["supplementalCredentials"]), account["id"]
                 )
             )
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/containerhandler.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/containerhandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 from ntdsdotsqlite.basehandler import BaseHandler
 from ntdsdotsqlite.utils import escape_dn_chars
 
 
 class ContainerHandler(BaseHandler):
+    def __init__(self, domainhandler, sqlite_db, attributes, ese_db):
+        super().__init__(sqlite_db, attributes, ese_db)
+        self.__domainhandler = domainhandler
+
     def handle(self, row):
         container = {
             "id": row.get("DNT_col"),
             "name": row.get(self.attributes["name"]),
             "cn": row.get(self.attributes["cn"]),
             "description": row.get(self.attributes["description"]),
             "parent": row.get("PDNT_col"),
             "is_deleted": row.get(self.attributes["isDeleted"]) == 1
         }
         stmt = """
             INSERT INTO containers VALUES (
-            :id, :name, :description, :cn, :parent, Null, :is_deleted
+            :id, :name, :description, :cn, :parent, Null, :is_deleted, Null
             )
         """
         self.sqlite_db.execute(stmt, container)
 
     def callback(self):
         # compute DNs
         roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
             "SELECT id, dn FROM domain_dns"
         ).fetchall()}
         containers = {
-            c_id: {"id": c_id, "name": name, "parent": parent, "cn": cn}
+            c_id: {"id": c_id, "name": name, "parent": parent, "cn": cn, "domain": None}
             for c_id, name, parent, cn in self.sqlite_db.execute(
                 "SELECT id, name, parent, commonname FROM containers"
             ).fetchall()
         }
         for container in containers.values():
             cur_object = container
             parts = [f"CN={escape_dn_chars(cur_object['cn'])}"]
+            domain_id = None
             while True:
                 if cur_object["parent"] in containers.keys():
                     cur_object = containers[cur_object["parent"]]
                     parts.append(f"CN={escape_dn_chars(cur_object['cn'])}")
                 elif cur_object["parent"] in roots.keys():
                     parts.append(roots[cur_object["parent"]])
+                    domain_id = cur_object["parent"]
+                    break
+                elif cur_object["parent"] in self.__domainhandler.builtin_ids:
+                    domain_id = self.__domainhandler.main_domain["id"]
                     break
                 else:
                     break
             container["dn"] = ",".join(parts)
             if ",DC=" not in container["dn"]:
                 container["dn"] = ""
             self.sqlite_db.execute(
-                "UPDATE containers SET dn=? WHERE id=?", (container["dn"], container["id"])
+                "UPDATE containers SET dn=?, domain=? WHERE id=?",
+                (container["dn"], domain_id, container["id"])
             )
         self.sqlite_db.commit()
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/decrypt.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/domainhandler.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/domainhandler.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class DomainHandler(BaseHandler):
     def __init__(self, sqlite_db, attributes, ese_db, bootkey):
         super().__init__(sqlite_db, attributes, ese_db)
         self.objects = []
         self.bootkey = bootkey
         self.pek = list()
+        self.builtin_ids = set()
 
     def handle(self, row):
         func_levels = {
             0: "2000", 2: "2003", 3: "2008", 4: "2008R2",
             5: "2012", 6: "2012R2", 7: "2016"
         }
         sid = row.get(self.attributes["objectSid"])
@@ -61,14 +62,15 @@
                 }
                 stmt = (
                     "INSERT INTO domains VALUES(:id, :name, :netbios_name, :functional_level, "
                     ":GUID, :gplink, :SID, :machineAccountQuota, :maxPwdAge, :lockoutDuration, "
                     ":minPwdLength, :pwdHistoryLength, :minPwdAge, :dn)"
                 )
                 self.sqlite_db.execute(stmt, domain)
+                self.main_domain = domain
                 # extract pek if bootkey available
                 if self.bootkey is not None:
                     peklist = row.get(self.attributes["pekList"])
                     encryptedPekList = PEKLIST_ENC(peklist)
                     if encryptedPekList['Header'][:4] == b'\x02\x00\x00\x00':
                         # Up to Windows 2012 R2 looks like header starts this way
                         md5h = md5()
@@ -111,14 +113,19 @@
             stmt = (
                 "INSERT INTO domain_dns "
                 "VALUES(:id, :name, :netbios_name, :GUID, :gplink, :SID, :dn)"
             )
             self.sqlite_db.execute(stmt, domain)
             self.sqlite_db.commit()
             self.objects.append(domain)
+        else:
+            # Here, SID is None, meaning we are looking at a built-in root domain object like
+            #   "ForestDnsZones" or "DomainDnsZones". We store their id to catch them in other
+            #   classes (containers) which need them
+            self.builtin_ids.add(row.get("DNT_col"))
 
     def callback(self):
         for object in self.objects:
             # Get the parents from id object to $ROOT_OBJECT$ and compute DN
             # and full name
             parents = []
             cur_object = object
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/grouphandler.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/grouphandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/model.sql`

 * *Files 3% similar despite different names*

```diff
@@ -118,25 +118,29 @@
 CREATE TABLE organizational_units (
     id INTEGER PRIMARY KEY,
     name TEXT,
     description TEXT,
     parent INTEGER,
     dn TEXT,
     isDeleted BOOLEAN,
-    FOREIGN KEY (id) REFERENCES organizational_units (parent)
+    domain INTEGER,
+    FOREIGN KEY (id) REFERENCES organizational_units (parent),
+    FOREIGN KEY (id) REFERENCES domain_dns (domain)
 );
 
 CREATE TABLE containers (
     id INTEGER PRIMARY KEY,
     name TEXT,
     description TEXT,
     commonname TEXT,
     parent INTEGER,
     dn TEXT,
-    isDeleted BOOLEAN
+    isDeleted BOOLEAN,
+    domain INTEGER,
+    FOREIGN KEY (id) REFERENCES domain_dns (domain)
 );
 
 CREATE TABLE trusted_domains (
     id INTEGER PRIMARY KEY,
     commonname TEXT,
     name TEXT,
     trustAttributes INTEGER,
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     # the ntds has been read entirely.
     # This dict can be ordered to choose in which order the callbacks will be called !
     dh = DomainHandler(sqlite_db, attributes, ese_db, bootkey)
     caught_classes = OrderedDict({
         "domainDNS": dh,
         "trustedDomain": TrustedDomainHandler(sqlite_db, attributes, ese_db),
         "group": GroupHandler(link_relations, sqlite_db, attributes, ese_db),
-        "container": ContainerHandler(sqlite_db, attributes, ese_db),
+        "container": ContainerHandler(dh, sqlite_db, attributes, ese_db),
         "organizationalUnit": OrganizationalUnitHandler(sqlite_db, attributes, ese_db),
         "person": PersonHandler(link_relations, sqlite_db, attributes, ese_db, dh),
         "computer": ComputerHandler(sqlite_db, attributes, ese_db, dh)
     })
     # "direct access" classes : {1511: SpecificHandler(...)}
     da_classes = {}
     attributeID_attr = "ATTc131102"
@@ -105,15 +105,17 @@
         # trigger the handle method of the associated handler if it exists
         try:
             da_classes[obj_category].handle(row)
         except KeyError:
             if store_tmp:
                 tmp_rows.append(row)
     # manage the first "few" rows we saw when classes and attributes were not set up yet
-    for row in filter(lambda r: r.get(attributes["objectCategory"]) in da_classes.keys(), tmp_rows):
+    for row in filter(
+        lambda r: r.get(attributes["objectCategory"]) in da_classes.keys(), tmp_rows
+    ):
         obj_category = row.get(objectCategory_attr)
         da_classes[obj_category].handle(row)
     sqlite_db.commit()
     # Trigger callbacks for all caught classes
     for _, obj in caught_classes.items():
         obj.callback()
         sqlite_db.commit()
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/organizationalunithandler.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/organizationalunithandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,45 +9,46 @@
             "description": row.get(self.attributes["description"]),
             "name": row.get(self.attributes["name"]),
             "parent": row.get("PDNT_col"),
             "isDeleted": row.get(self.attributes["isDeleted"]) == 1
         }
         stmt = """
             INSERT INTO organizational_units VALUES (
-            :id, :name, :description, :parent, Null, :isDeleted
+            :id, :name, :description, :parent, Null, :isDeleted, Null
             )
         """
         self.sqlite_db.execute(stmt, ou_object)
 
     def callback(self):
         # Compute DNs
         roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
             "SELECT id, dn FROM domain_dns"
         ).fetchall()}
-        ous = self.sqlite_db.execute("SELECT id, parent, name FROM organizational_units").fetchall()
+        ous = self.sqlite_db.execute(
+            "SELECT id, parent, name FROM organizational_units"
+        ).fetchall()
         ous = {
             ou_id: {"id": ou_id, "name": name, "parent": parent}
             for ou_id, parent, name in ous
         }
         for ou_id, ou in ous.items():
             dn_prefix = "OU=" + escape_dn_chars(ou["name"])
             cur_object = ou
             while True:
                 parent_dnt = cur_object["parent"]
                 if parent_dnt in ous.keys():
                     parent = ous[parent_dnt]
                 elif parent_dnt in roots.keys():
                     dn_prefix += ("," + roots[parent_dnt])
+                    domain_id = parent_dnt
                     break
                 else:
-                    print(
-                        f"Warning: could not compute DN of OU {cur_object['name']}."
-                    )
+                    print(f"Warning: could not compute DN of OU {cur_object['name']}.")
                     break
                 cur_object = parent
                 name = parent["name"]
                 dn_prefix += "," + "OU=" + escape_dn_chars(name)
             self.sqlite_db.execute(
-                "UPDATE organizational_units SET dn=? WHERE id=?",
-                (dn_prefix, ou_id)
+                "UPDATE organizational_units SET dn=?, domain=? WHERE id=?",
+                (dn_prefix, domain_id, ou_id)
             )
         self.sqlite_db.commit()
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/personhandler.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/personhandler.py`

 * *Files 20% similar despite different names*

```diff
@@ -108,37 +108,45 @@
             :encrypted_ntPwdHistory, :ntPwdHistory, :accountExpires, :uac_flags, :parent, Null,
             :isDeleted, :primaryGroup, Null, :isDisabled
             )
         """
         self.sqlite_db.execute(stmt, account)
 
     def callback(self):
-        # set the domain id
-        domain_id = self.sqlite_db.execute("SELECT id FROM domains").fetchone()[0]
         ous = {
-            oid: dn for oid, dn in self.sqlite_db.execute("SELECT id, dn FROM organizational_units")
+            oid: {"dn": dn, "domain": odid}
+            for oid, dn, odid in self.sqlite_db.execute(
+                "SELECT id, dn, domain FROM organizational_units"
+            )
         }
         users = self.sqlite_db.execute(
             "SELECT id, commonname, parent_OU, primaryGroup FROM user_accounts"
         )
         containers = {
-            cid: cdn for (cid, cdn) in self.sqlite_db.execute("SELECT id, dn FROM containers")
+            cid: {"dn": cdn, "domain": cdid}
+            for (cid, cdn, cdid) in self.sqlite_db.execute("SELECT id, dn, domain FROM containers")
         }
         domains = {
             did: ddn for (did, ddn) in self.sqlite_db.execute("SELECT id, dn FROM domain_dns")
         }
         group_ids = [x[0] for x in self.sqlite_db.execute("SELECT id FROM groups").fetchall()]
         for uid, cn, parent_OU, primaryGroup in users:
             # Compute DN
             if parent_OU in ous.keys():
-                dn = f"CN={escape_dn_chars(cn)},{ous[parent_OU]}"
+                dn = f"CN={escape_dn_chars(cn)},{ous[parent_OU]['dn']}"
+                domain_id = ous[parent_OU]["domain"]
             elif parent_OU in containers.keys():
-                dn = f"CN={escape_dn_chars(cn)},{containers[parent_OU]}"
+                curdn = containers[parent_OU]['dn']
+                dn = f"CN={escape_dn_chars(cn)},{curdn}"
+                domain_id = containers[parent_OU]["domain"]
             elif parent_OU in domains.keys():
                 dn = f"CN={escape_dn_chars(cn)},{domains[parent_OU]}"
+                # Sets the domain ID to this "OU" ID since its the ID of the root domainDNS object
+                # in which this user is.
+                domain_id = parent_OU
             else:
                 print(f"Warning: could not compute DN of user {cn}")
             links_list = self.links[uid]
             memberof = json.dumps([link for link in links_list if link in group_ids])
             self.sqlite_db.execute(
                 "UPDATE user_accounts set domain=?, memberOf=?, primaryGroup=("
                 f"SELECT id from groups WHERE SID LIKE '%-{primaryGroup}'"
```

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/trusteddomainhandler.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/trusteddomainhandler.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.3/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-1.1.4/ntdsdotsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.3/pyproject.toml` & `ntdsdotsqlite-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "1.1.3"
+version = "1.1.4"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
```

### Comparing `ntdsdotsqlite-1.1.3/README.md` & `ntdsdotsqlite-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-1.1.3/setup.py` & `ntdsdotsqlite-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['ntdsdotsqlite = ntdsdotsqlite.__main__:main']}
 
 setup_kwargs = {
     'name': 'ntdsdotsqlite',
-    'version': '1.1.3',
+    'version': '1.1.4',
     'description': 'A small utility to get an SQLite  database from an NTDS.DIT file.',
     'long_description': '# NTDS.Sqlite\n\nThis software can be used either directly as a CLI utility or as a library to get an SQLite database from an NTDS.DIT one. Encrypted bits can be decrypted if the associated system hive is provided altogether.\n\n# Installation\n\n`python -m pip install ntdsdotsqlite`\n\n# Usage\n\n`ntdsdotsqlite NTDS.DIT --system SYSTEM -o NTDS.sqlite`\n\n```\nusage: NTDS.sqlite [-h] [--system SYSTEM] -o OUTFILE NTDS\n\nThis tool helps dumping NTDS.DIT file to an SQLite database\n\npositional arguments:\n  NTDS                  The NTDS.DIT file\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --system SYSTEM       The SYSTEM hive to decrypt hashes. If not provided, hashes will be encrypted inside the sqlite database.\n  -o OUTFILE, --outfile OUTFILE\n                        The sqlite database. Example : NTDS.sqlite\n```\n\n# SQL model\n\nThe SQL model is described in the `sql_model.md` file in this repository. Basicaly, not all objects are extracted (at all), but the following are retrieved as of today : domain object, user accounts, machine accounts, groups, organizational units and containers. I thought these would be the most useful. If you need more object classes to be extracted or additional attributes, feel free to open an issue or a pull request !\n\n# Performances\n\nPerformances can be a bit low for huge NTDS files. The whole NTDS is not stored in memory to prevent memory exhaustion when working on huge files (NTDS databases can grow to several gigabytes).\n',
     'author': 'Virgile Jarry',
     'author_email': 'virgile@mailbox.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/almandin/ntdsdotsqlite',
```

### Comparing `ntdsdotsqlite-1.1.3/PKG-INFO` & `ntdsdotsqlite-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 1.1.3
+Version: 1.1.4
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

