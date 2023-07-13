# Comparing `tmp/svj_ntuple_processing-0.8.tar.gz` & `tmp/svj_ntuple_processing-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/svj_ntuple_processing-0.8.tar", last modified: Thu Feb  9 18:07:22 2023, max compression
+gzip compressed data, was "dist/svj_ntuple_processing-0.9.tar", last modified: Thu Mar 30 21:16:30 2023, max compression
```

## Comparing `svj_ntuple_processing-0.8.tar` & `svj_ntuple_processing-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-02-09 18:07:22.000000 svj_ntuple_processing-0.8/
-drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-02-09 18:07:22.000000 svj_ntuple_processing-0.8/svj_ntuple_processing/
-drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-02-09 18:07:22.000000 svj_ntuple_processing-0.8/svj_ntuple_processing/include/
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)        3 2023-02-09 17:27:20.000000 svj_ntuple_processing-0.8/svj_ntuple_processing/include/VERSION
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)    26702 2023-02-09 17:20:01.000000 svj_ntuple_processing-0.8/svj_ntuple_processing/__init__.py
-drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-02-09 18:07:22.000000 svj_ntuple_processing-0.8/svj_ntuple_processing.egg-info/
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)      281 2023-02-09 18:07:19.000000 svj_ntuple_processing-0.8/svj_ntuple_processing.egg-info/PKG-INFO
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)      391 2023-02-09 18:07:19.000000 svj_ntuple_processing-0.8/svj_ntuple_processing.egg-info/SOURCES.txt
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)        1 2023-02-09 18:07:19.000000 svj_ntuple_processing-0.8/svj_ntuple_processing.egg-info/dependency_links.txt
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)        1 2022-10-26 18:55:19.000000 svj_ntuple_processing-0.8/svj_ntuple_processing.egg-info/not-zip-safe
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)       23 2023-02-09 18:07:19.000000 svj_ntuple_processing-0.8/svj_ntuple_processing.egg-info/requires.txt
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)       22 2023-02-09 18:07:19.000000 svj_ntuple_processing-0.8/svj_ntuple_processing.egg-info/top_level.txt
-drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-02-09 18:07:22.000000 svj_ntuple_processing-0.8/test/
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)     6019 2022-12-13 20:50:17.000000 svj_ntuple_processing-0.8/test/test_filters.py
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)       39 2022-10-26 18:30:37.000000 svj_ntuple_processing-0.8/MANIFEST.in
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)     6106 2022-12-07 20:21:11.000000 svj_ntuple_processing-0.8/README.md
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)      785 2022-10-27 20:19:13.000000 svj_ntuple_processing-0.8/setup.py
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)      281 2023-02-09 18:07:22.000000 svj_ntuple_processing-0.8/PKG-INFO
--rw-r--r--   0 klijnsma (55957) us_cms    (5063)       38 2023-02-09 18:07:22.000000 svj_ntuple_processing-0.8/setup.cfg
+drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-03-30 21:16:30.000000 svj_ntuple_processing-0.9/
+drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-03-30 21:16:29.000000 svj_ntuple_processing-0.9/svj_ntuple_processing/
+drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-03-30 21:16:30.000000 svj_ntuple_processing-0.9/svj_ntuple_processing/include/
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)        3 2023-03-30 21:15:59.000000 svj_ntuple_processing-0.9/svj_ntuple_processing/include/VERSION
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)    32959 2023-03-30 21:12:48.000000 svj_ntuple_processing-0.9/svj_ntuple_processing/__init__.py
+drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-03-30 21:16:30.000000 svj_ntuple_processing-0.9/svj_ntuple_processing.egg-info/
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)      281 2023-03-30 21:16:27.000000 svj_ntuple_processing-0.9/svj_ntuple_processing.egg-info/PKG-INFO
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)      391 2023-03-30 21:16:27.000000 svj_ntuple_processing-0.9/svj_ntuple_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)        1 2023-03-30 21:16:27.000000 svj_ntuple_processing-0.9/svj_ntuple_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)        1 2022-10-26 18:55:19.000000 svj_ntuple_processing-0.9/svj_ntuple_processing.egg-info/not-zip-safe
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)       23 2023-03-30 21:16:27.000000 svj_ntuple_processing-0.9/svj_ntuple_processing.egg-info/requires.txt
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)       22 2023-03-30 21:16:27.000000 svj_ntuple_processing-0.9/svj_ntuple_processing.egg-info/top_level.txt
+drwxr-xr-x   0 klijnsma (55957) us_cms    (5063)        0 2023-03-30 21:16:30.000000 svj_ntuple_processing-0.9/test/
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)     6019 2022-12-13 20:50:17.000000 svj_ntuple_processing-0.9/test/test_filters.py
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)       39 2022-10-26 18:30:37.000000 svj_ntuple_processing-0.9/MANIFEST.in
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)     6106 2022-12-07 20:21:11.000000 svj_ntuple_processing-0.9/README.md
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)      785 2022-10-27 20:19:13.000000 svj_ntuple_processing-0.9/setup.py
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)      281 2023-03-30 21:16:30.000000 svj_ntuple_processing-0.9/PKG-INFO
+-rw-r--r--   0 klijnsma (55957) us_cms    (5063)       38 2023-03-30 21:16:30.000000 svj_ntuple_processing-0.9/setup.cfg
```

### Comparing `svj_ntuple_processing-0.8/svj_ntuple_processing/__init__.py` & `svj_ntuple_processing-0.9/svj_ntuple_processing/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,14 +74,34 @@
     'HLT_PFJet500_v',
     ]
 
 # Checked: 2017 identical to 2018
 triggers_per_year = {2016: triggers_2016, 2017: triggers_2018, 2018: triggers_2018}
 
 
+#  ECAL DEAD CELL LOCATIONS
+# ecaldeadcells 2018 remove 5sigma
+dataqcd_eta_ecaldead={}
+dataqcd_phi_ecaldead={}
+dataqcd_eta_ecaldead[2018] = np.array([
+    -1.632, -0.768, -2.112, -1.632, -0.384,  0.864, -1.536,  1.056,
+    1.44 , -2.016,  1.824, -2.4  , -1.44 , -0.192, -0.864, -1.536,
+    0.   , -1.248,  1.152, -0.288, -2.304,  1.632,  1.728, -2.4  ,
+    -0.768,  1.248,  0.96 , -1.728, -0.192, -2.304, -0.096,  1.536,
+    -2.208,  0.096,  0.864, -0.96 , -0.576,  1.728, -1.248
+    ])
+dataqcd_phi_ecaldead[2018] = np.array([
+    0.503, -0.754, -2.513,  0.628,  0.126,  2.765, -3.142, -3.142,
+    -0.251, -2.513, -2.136, -1.508, -3.142, -2.639, -1.759, -1.257,
+    1.759, -1.257, -0.503,  0.126, -1.508, -0.628, -0.628, -1.634,
+    -2.262, -0.503,  0.628, -0.503,  0.628, -1.634,  0.88 , -1.634,
+    -1.508,  1.759,  1.634,  2.011,  2.639, -2.136,  2.765
+    ])
+
+
 class Arrays:
     """
     Container class for an awkward.Array object + metadata about it.
 
     The functions filter_preselection, filter_zprime_in_cone, and filter_stitch
     can be used on this object to apply event selections.
 
@@ -223,14 +243,23 @@
     # Map to 0..2pi range
     dphi = (phi1 - phi2) % twopi
     # Map pi..2pi --> -pi..0
     dphi[dphi > np.pi] -= twopi
     return dphi
 
 
+def calculate_mass(pt, eta, e):
+    """
+    compute mass
+    """
+    pz = pt * np.sinh(eta)
+    mass = np.sqrt(e**2 - pt**2 - pz**2)
+    return mass
+
+
 def calc_dr(eta1, phi1, eta2, phi2):
     return np.sqrt((eta1-eta2)**2 + calc_dphi(phi1, phi2)**2)
 
 
 def calculate_mt(pt, eta, phi, e, met, metphi):
     """
     Calculates the transverse mass MT and RT (closely related calcs)
@@ -243,14 +272,31 @@
     # m^2 + pT^2 = E^2 - pT^2 - pz^2 + pT^2 = E^2 - pz^2
     pz = pt * np.sinh(eta)
     transverse_e = np.sqrt(e**2 - pz**2)
     mt = np.sqrt( (transverse_e + met)**2 - (jet_x + met_x)**2 - (jet_y + met_y)**2 )
     return mt
 
 
+def veto_phi_spike(eta_veto, phi_veto, eta_jets, phi_jets, rad=0.01):
+    """
+    Returns an array with length of the number of jets, indicating for
+    each jet if it is vetoed (False) or is okay (True).
+    """
+    # deta is a matrix with delta_eta to every dead cell location, per jet
+    # e.g. deta[0] gives you a np.array of all delta_etas to all dead cells
+    deta = np.expand_dims(eta_jets, -1) - eta_veto
+    assert deta.shape == ( len(eta_jets), len(eta_veto) )
+    dphi = calc_dphi(np.expand_dims(phi_jets, -1), phi_veto)
+    assert dphi.shape == ( len(phi_jets), len(phi_veto) )
+    # Only True for jets that are not close to _any_ dead cell location
+    veto_mask = np.all((deta**2 + dphi**2) > rad, axis=-1)
+    assert veto_mask.shape == (len(eta_jets),)
+    return veto_mask
+
+
 def cr_filter_preselection(array):
     """
     Preselection for the control region.
     
     w.r.t. `filter_preselection`, does not include:
     - leading ak8 jet pt > 500
     - rtx > 1.1
@@ -279,20 +325,20 @@
     cutflow['n_ak15jets>=2'] = len(a)
 
     # At least 2 AK4 jets --> deadcells study
     a = a[ak.count(a['Jets.fCoordinates.fPt'], axis=-1) >= 2]
     cutflow['n_ak4jets>=2'] = len(a)
 
     # subleading eta < 2.4 eta
-    a = a[a['JetsAK15.fCoordinates.fEta'][:,1]<2.4]
+    a = a[np.abs(a['JetsAK15.fCoordinates.fEta'][:,1])<2.4]
     cutflow['ak15j2_eta<2.4'] = len(a)
 
     # leading and subleading ak4 eta < 2.4 --> deadcells study
-    a = a[a['Jets.fCoordinates.fEta'][:,0]<2.4]
-    a = a[a['Jets.fCoordinates.fEta'][:,1]<2.4]
+    a = a[np.abs(a['Jets.fCoordinates.fEta'][:,0])<2.4]
+    a = a[np.abs(a['Jets.fCoordinates.fEta'][:,1])<2.4]
     cutflow['ak4j1j2_eta<2.4'] = len(a)
 
     # lepton vetoes
     a = a[(a['NMuons']==0) & (a['NElectrons']==0)]
     cutflow['nleptons=0'] = len(a)
 
     # MET filters
@@ -331,16 +377,20 @@
         a = a[(trigger_decisions == 1).any(axis=-1)]
     cutflow['triggers'] = len(a)
 
     # At least 2 AK15 jets
     a = a[ak.count(a['JetsAK15.fCoordinates.fPt'], axis=-1) >= 2]
     cutflow['n_ak15jets>=2'] = len(a)
 
+    # At least 2 AK4 jets --> deadcells study
+    a = a[ak.count(a['Jets.fCoordinates.fPt'], axis=-1) >= 2]
+    cutflow['n_ak4jets>=2'] = len(a)
+
     # subleading eta < 2.4 eta
-    a = a[a['JetsAK15.fCoordinates.fEta'][:,1]<2.4]
+    a = a[np.abs(a['JetsAK15.fCoordinates.fEta'][:,1])<2.4]
     cutflow['subl_eta<2.4'] = len(a)
 
     # positive ECF values
     for ecf in [
         'JetsAK15_ecfC2b1', 'JetsAK15_ecfD2b1',
         'JetsAK15_ecfM2b1', 'JetsAK15_ecfN2b2',
         ]:
@@ -364,22 +414,37 @@
         'ecalBadCalibFilter' if UL else 'ecalBadCalibReducedFilter',
         'BadPFMuonFilter',
         'BadChargedCandidateFilter',
         'globalSuperTightHalo2016Filter',
         ]:
         a = a[a[b]!=0] # Pass events if not 0, is that correct?
     cutflow['metfilter'] = len(a)
+
+    # Filter out jets that are too close to dead cells
+    ak4jet_eta = a['Jets.fCoordinates.fEta'][:,1].to_numpy()
+    ak4jet_phi = a['Jets.fCoordinates.fPhi'][:,1].to_numpy()
+    dead_cell_mask = veto_phi_spike(
+        dataqcd_eta_ecaldead[array.year], dataqcd_phi_ecaldead[array.year],
+        ak4jet_eta, ak4jet_phi,
+        rad = 0.01
+        )
+    a = a[dead_cell_mask]
+    cutflow['ecaldeadcells'] = len(a)
+
     cutflow['preselection'] = len(a)
 
     copy.array = a
     logger.debug('cutflow:\n%s', pprint.pformat(copy.cutflow))
     return copy
 
 
 def filter_zprime_in_cone(array):
+    """
+    Require both dark quarks and the zprime to be INSIDE 1.5 cone of the subleading jet
+    """
     copy = array.copy()
     a, cutflow = copy.array, copy.cutflow
 
     # at least 1 zprime particle
     a = a[ak.sum(a['GenParticles_PdgId']==4900023, axis=-1)>=1]
     # at least 2 dark quarks
     a = a[ak.sum((np.abs(a['GenParticles_PdgId'])==4900101) & (a['GenParticles_Status']==71), axis=-1)>=2]
@@ -401,14 +466,87 @@
         & (calc_dr(eta_subl, phi_subl, eta_darkquark2, phi_darkquark2)<=1.5)
         ]
     cutflow['zdq<1.5'] = len(a)
     copy.array = a
     return copy
 
 
+def filter_zprime_not_in_cone(array):
+    """
+    Require both dark quarks and the zprime to be OUTSIDE 1.5 cone of the subleading jet
+    """
+    copy = array.copy()
+    a, cutflow = copy.array, copy.cutflow
+
+    # at least 1 zprime particle
+    a = a[ak.sum(a['GenParticles_PdgId']==4900023, axis=-1)>=1]
+    # at least 2 dark quarks
+    a = a[ak.sum((np.abs(a['GenParticles_PdgId'])==4900101) & (a['GenParticles_Status']==71), axis=-1)>=2]
+    cutflow['1zprime2darkquarks'] = len(a)
+
+    # Require both dark quarks and the zprime to be OUTSIDE 1.5 cone of the subleading jet
+    eta_subl = a['JetsAK15.fCoordinates.fEta'][:,1].to_numpy()
+    phi_subl = a['JetsAK15.fCoordinates.fPhi'][:,1].to_numpy()
+    eta_zprime = a['GenParticles.fCoordinates.fEta'][a['GenParticles_PdgId']==4900023][:,0].to_numpy()
+    phi_zprime = a['GenParticles.fCoordinates.fPhi'][a['GenParticles_PdgId']==4900023][:,0].to_numpy()
+    select_darkquarks = (np.abs(a['GenParticles_PdgId'])==4900101) & (a['GenParticles_Status']==71)
+    eta_darkquark1 = a['GenParticles.fCoordinates.fEta'][select_darkquarks][:,0].to_numpy()
+    phi_darkquark1 = a['GenParticles.fCoordinates.fPhi'][select_darkquarks][:,0].to_numpy()
+    eta_darkquark2 = a['GenParticles.fCoordinates.fEta'][select_darkquarks][:,1].to_numpy()
+    phi_darkquark2 = a['GenParticles.fCoordinates.fPhi'][select_darkquarks][:,1].to_numpy()
+    a = a[
+        (calc_dr(eta_subl, phi_subl, eta_zprime, phi_zprime)>1.5)
+        & (calc_dr(eta_subl, phi_subl, eta_darkquark1, phi_darkquark1)>1.5)
+        & (calc_dr(eta_subl, phi_subl, eta_darkquark2, phi_darkquark2)>1.5)
+        ]
+
+    cutflow['zdq>1.5'] = len(a)
+    copy.array = a
+    return copy
+
+
+def filter_zprime_half_in_cone(array):
+    """
+    Require at least 1 dark quark / zprime to be OUTSIDE 1.5 cone around subjet,
+    AND     at least 1 dark quark / zprime to be INSIDE 1.5 cone around subjet
+    """
+    copy = array.copy()
+    a, cutflow = copy.array, copy.cutflow
+
+    # at least 1 zprime particle
+    a = a[ak.sum(a['GenParticles_PdgId']==4900023, axis=-1)>=1]
+    # at least 2 dark quarks
+    a = a[ak.sum((np.abs(a['GenParticles_PdgId'])==4900101) & (a['GenParticles_Status']==71), axis=-1)>=2]
+    cutflow['1zprime2darkquarks'] = len(a)
+
+    # Require at least 1 dark quark / zprime to be OUTSIDE 1.5 cone around subjet,
+    # AND     at least 1 dark quark / zprime to be INSIDE 1.5 cone around subjet
+    eta_subl = a['JetsAK15.fCoordinates.fEta'][:,1].to_numpy()
+    phi_subl = a['JetsAK15.fCoordinates.fPhi'][:,1].to_numpy()
+    eta_zprime = a['GenParticles.fCoordinates.fEta'][a['GenParticles_PdgId']==4900023][:,0].to_numpy()
+    phi_zprime = a['GenParticles.fCoordinates.fPhi'][a['GenParticles_PdgId']==4900023][:,0].to_numpy()
+    select_darkquarks = (np.abs(a['GenParticles_PdgId'])==4900101) & (a['GenParticles_Status']==71)
+    eta_darkquark1 = a['GenParticles.fCoordinates.fEta'][select_darkquarks][:,0].to_numpy()
+    phi_darkquark1 = a['GenParticles.fCoordinates.fPhi'][select_darkquarks][:,0].to_numpy()
+    eta_darkquark2 = a['GenParticles.fCoordinates.fEta'][select_darkquarks][:,1].to_numpy()
+    phi_darkquark2 = a['GenParticles.fCoordinates.fPhi'][select_darkquarks][:,1].to_numpy()
+    a = a[
+        ((calc_dr(eta_subl, phi_subl, eta_zprime, phi_zprime)<=1.5)
+        | (calc_dr(eta_subl, phi_subl, eta_darkquark1, phi_darkquark1)<=1.5)
+        | (calc_dr(eta_subl, phi_subl, eta_darkquark2, phi_darkquark2)<=1.5))
+        & ((calc_dr(eta_subl, phi_subl, eta_zprime, phi_zprime)>1.5)
+        | (calc_dr(eta_subl, phi_subl, eta_darkquark1, phi_darkquark1)>1.5)
+        | (calc_dr(eta_subl, phi_subl, eta_darkquark2, phi_darkquark2)>1.5))
+        ]
+
+    cutflow['half_truth'] = len(a)
+    copy.array = a
+    return copy
+
+
 def filter_stitch(array):
     """
     Filter to cut away kinematic regions from ttjets/wjets that are covered in
     dedicated samples
     """
     copy = array.copy()
     a = copy.array
```

### Comparing `svj_ntuple_processing-0.8/test/test_filters.py` & `svj_ntuple_processing-0.9/test/test_filters.py`

 * *Files identical despite different names*

### Comparing `svj_ntuple_processing-0.8/README.md` & `svj_ntuple_processing-0.9/README.md`

 * *Files identical despite different names*

### Comparing `svj_ntuple_processing-0.8/setup.py` & `svj_ntuple_processing-0.9/setup.py`

 * *Files identical despite different names*

