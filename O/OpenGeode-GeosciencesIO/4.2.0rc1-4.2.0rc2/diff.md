# Comparing `tmp/OpenGeode_GeosciencesIO-4.2.0rc1-cp39-cp39-win_amd64.whl.zip` & `tmp/OpenGeode_GeosciencesIO-4.2.0rc2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 343320 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      192 b- defN 23-Jul-12 12:11 opengeode_geosciencesio/__init__.py
--rw-rw-rw-  2.0 fat     1233 b- defN 23-Jul-12 12:11 opengeode_geosciencesio/mesh.py
--rw-rw-rw-  2.0 fat     1265 b- defN 23-Jul-12 12:11 opengeode_geosciencesio/model.py
--rw-rw-rw-  2.0 fat   170496 b- defN 23-Jul-12 12:12 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll
--rw-rw-rw-  2.0 fat   361472 b- defN 23-Jul-12 12:12 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll
--rw-rw-rw-  2.0 fat   125952 b- defN 23-Jul-12 12:12 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   125440 b- defN 23-Jul-12 12:12 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3337 b- defN 23-Jul-12 12:12 OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-12 12:12 OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 23-Jul-12 12:12 OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1157 b- defN 23-Jul-12 12:12 OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/RECORD
-11 files, 790668 bytes uncompressed, 341302 bytes compressed:  56.8%
+-rw-rw-rw-  2.0 fat      192 b- defN 23-Jul-13 05:25 opengeode_geosciencesio/__init__.py
+-rw-rw-rw-  2.0 fat     1233 b- defN 23-Jul-13 05:25 opengeode_geosciencesio/mesh.py
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-Jul-13 05:25 opengeode_geosciencesio/model.py
+-rw-rw-rw-  2.0 fat   170496 b- defN 23-Jul-13 05:26 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll
+-rw-rw-rw-  2.0 fat   361472 b- defN 23-Jul-13 05:26 opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll
+-rw-rw-rw-  2.0 fat   125952 b- defN 23-Jul-13 05:26 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   125440 b- defN 23-Jul-13 05:26 opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3340 b- defN 23-Jul-13 05:26 OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-13 05:26 OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Jul-13 05:26 OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1157 b- defN 23-Jul-13 05:26 OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/RECORD
+11 files, 790671 bytes uncompressed, 341302 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd
 Comment: 
 
 Filename: opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/METADATA
+Filename: OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/WHEEL
+Filename: OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/top_level.txt
+Filename: OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/RECORD
+Filename: OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018001b54c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Jul 12 12:11:43 2023
+Time/Date		Thu Jul 13 05:25:46 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000001c800
 SizeOfInitializedData	000000000000ce00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001b54c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0002e000
 SizeOfHeaders		00000400
-CheckSum		000356e7
+CheckSum		00033b9f
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -41186,17 +41186,15 @@
    18001f6b3:	imul   $0x91f00000,0x6e(%rdi),%ebp
    18001f6ba:	add    0x1(%rax),%al
    18001f6c0:	nop
    18001f6c1:	xchg   %eax,%edx
    18001f6c2:	add    0x1(%rax),%al
    18001f6c8:	add    %al,(%rax)
    18001f6ca:	add    %al,(%rax)
-   18001f6cc:	jg     0x18001f666
-   18001f6ce:	scas   %es:(%rdi),%al
-   18001f6cf:	add    %al,%fs:(%rax)
+   18001f6cc:	fimull 0x64af(%rdx)
    18001f6d2:	add    %al,(%rax)
    18001f6d4:	or     $0x28000000,%eax
    18001f6d9:	add    (%rax),%eax
    18001f6db:	add    %bh,%ah
    18001f6dd:	adc    (%rdx),%al
    18001f6df:	add    %bh,%ah
    18001f6e1:	incb   (%rcx)
```

## opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018003d10c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Jul 12 12:12:03 2023
+Time/Date		Thu Jul 13 05:26:10 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000003fc00
 SizeOfInitializedData	0000000000018400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000003d10c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0005c000
 SizeOfHeaders		00000400
-CheckSum		0005dc94
+CheckSum		0005d0f9
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -87246,20 +87246,16 @@
    180043eb3:	addb   $0x0,(%rcx)
    180043eb6:	add    %al,(%rax)
    180043eb8:	shlb   0x5(%rdi)
    180043ebb:	addb   $0x0,(%rcx)
    180043ebe:	add    %al,(%rax)
    180043ec0:	add    %al,(%rax)
    180043ec2:	add    %al,(%rax)
-   180043ec4:	xchg   %eax,%ebx
-   180043ec5:	cwtl
-   180043ec6:	scas   %es:(%rdi),%al
-   180043ec7:	add    %al,%fs:(%rax)
-   180043eca:	add    %al,(%rax)
-   180043ecc:	or     $0x50000000,%eax
+   180043ec4:	repnz mov 0x64(%rdi),%ch
+   180043ecb:	add    %cl,0x50000000(%rip)        # 0x1d0043ed1
    180043ed1:	add    (%rax),%eax
    180043ed3:	add    %cl,0x61(%rax)
    180043ed6:	add    $0x0,%al
    180043ed8:	rex.W push %rcx
    180043eda:	add    $0x0,%al
    180043edc:	add    %al,(%rax)
    180043ede:	add    %al,(%rax)
@@ -117957,17 +117953,18 @@
    180056511:	jo     0x180056588
    180056513:	je     0x18005655e
    180056515:	insl   (%dx),%es:(%rdi)
    180056516:	jo     0x180056584
    180056518:	rex.X push %rdx
    18005651a:	gs jo  0x18005655d
    18005651d:	(bad)
-   18005651e:	xor    %dil,0x63(%r8)
-   180056522:	xor    %ah,0x33(%rdx)
-   180056525:	xor    0x62(%rsi,%riz,2),%esp
+   18005651e:	xor    %dil,0x66(%r8)
+   180056522:	xor    %dh,(%rdi)
+   180056524:	xor    %esp,0x33(%rsi)
+   180056527:	(bad)
    180056529:	rex
    18005652a:	rex add %al,(%rax)
    18005652d:	add    %al,(%rax)
    18005652f:	add    %ah,0x180043e(%rax)
 	...
    18005653d:	add    %al,(%rax)
    18005653f:	add    %ch,(%rsi)
@@ -118003,23 +118000,23 @@
    180056589:	jo     0x180056600
    18005658b:	je     0x1800565d6
    18005658d:	insl   (%dx),%es:(%rdi)
    18005658e:	jo     0x1800565fc
    180056590:	push   %rbx
    180056591:	rex.WRB
    180056592:	rex (bad)
-   180056594:	xor    %dil,0x30(%r8)
-   180056598:	movsxd 0x65(%rdx),%esp
-   18005659b:	movsxd (%rax),%edi
-   18005659d:	xor    $0x404030,%eax
-	...
-   1800565ae:	add    %al,(%rax)
-   1800565b0:	movabs 0x180043e,%al
-   1800565b9:	add    %al,(%rax)
-   1800565bb:	add    %al,(%rax)
+   180056594:	xor    %dil,0x65(%r8)
+   180056598:	cmp    %esp,0x31(%rbp)
+   18005659b:	cmp    %ah,0x31(%rsi)
+   18005659e:	(bad)
+   18005659f:	rex
+   1800565a0:	rex add %al,(%rax)
+	...
+   1800565af:	add    %ah,0x180043e(%rax)
+	...
    1800565bd:	add    %al,(%rax)
    1800565bf:	add    %ch,(%rsi)
    1800565c1:	(bad)
    1800565c2:	push   %r14
    1800565c4:	(bad)
    1800565c5:	and    $0x4d,%al
    1800565c7:	rex.WR
```

## Comparing `OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/METADATA` & `OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: OpenGeode-GeosciencesIO
-Version: 4.2.0rc1
+Version: 4.2.0rc2
 Summary: Input/Output formats for OpenGeode-Geosciences
 Home-page: https://github.com/Geode-solutions/OpenGeode-GeosciencesIO
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: opengeode-core (==14.*,>=14.4.2)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.1.2)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.1.3rc1)
 
 <h1 align="center">OpenGeode-GeosciencesIO<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Input/Output formats for OpenGeode-Geosciences</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeode-GeosciencesIO/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 4.2.0rc1 Summary:
+Metadata-Version: 2.1 Name: OpenGeode-GeosciencesIO Version: 4.2.0rc2 Summary:
 Input/Output formats for OpenGeode-Geosciences Home-page: https://github.com/
 Geode-solutions/OpenGeode-GeosciencesIO Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: MIT Platform: UNKNOWN Description-Content-
 Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.4.2) Requires-
-Dist: opengeode-geosciences (==7.*,>=7.1.2)
+Dist: opengeode-geosciences (==7.*,>=7.1.3rc1)
             ****** OpenGeode-GeosciencesIOby Geode-solutions ******
            **** Input/Output formats for OpenGeode-Geosciences ****
        [Build Status] [Deploy Status] [Coverage Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
          [Language] [License] [Semantic-release] [Slack_invite] [DOI]
 --- ## Introduction OpenGeode-GeosciencesIO provides input and output formats
 for [OpenGeode-Geosciences] objects. [OpenGeode-Geosciences]: https://
```

## Comparing `OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/RECORD` & `OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 opengeode_geosciencesio/__init__.py,sha256=xE-gZywWE--rkStQEDSE8BazKirqHemxkeGijYOjdD0,192
 opengeode_geosciencesio/mesh.py,sha256=T_E8VlR2vePN2T3JDWjfslwiOY3PtuamayN6FNzV_e0,1233
 opengeode_geosciencesio/model.py,sha256=j6juGjbp0coO5RVc24Fy40-6RMbOCPvkjKpBXbponh4,1265
-opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll,sha256=Bbd9Vsueyuo-Jl3rjVmaVmmqWSq14Li4RLLD6K22Dag,170496
-opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll,sha256=vYnRq7XieSNqIcJgsNKas5qdDV-vk9yK3zmj2teLGYE,361472
-opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd,sha256=CbAxcSAjzgSHqBpZUZ-0MfuJtMMAG5_tytAxd1G727M,125952
-opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd,sha256=ExoaFSiYvjQZbPE-OQD8yn2G7-5Ne_3zs4Gjh3rG_kQ,125440
-OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/METADATA,sha256=7wJd5bXvLEjeWong3HPbRV5IX6sn_bkgI6R-IxEA-JY,3337
-OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/top_level.txt,sha256=PitPPl6JTchA3_fMFrNtchDNB9Ip8YkRyhMiQmuJWe4,24
-OpenGeode_GeosciencesIO-4.2.0rc1.dist-info/RECORD,,
+opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_mesh.dll,sha256=npgXsIc8FKcPrkEqSKrKonMVPASGiF0gp3YXaMlUtgA,170496
+opengeode_geosciencesio/bin/OpenGeode-GeosciencesIO_model.dll,sha256=9SBXTWhLbLXEYejI2_Gr5F3eOTfxRNpS_aJdvCTU88I,361472
+opengeode_geosciencesio/bin/opengeode_geosciencesio_py_mesh.cp39-win_amd64.pyd,sha256=xZddSDp_JuO3gw9BlM8AzZ6dFweSHD9uc-v6QdwVRPQ,125952
+opengeode_geosciencesio/bin/opengeode_geosciencesio_py_model.cp39-win_amd64.pyd,sha256=dypmVxwWVfaste6Yzpyda_K3Pe8vscQxUWU8ZdG4P1A,125440
+OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/METADATA,sha256=UpyO0-oWFNK1dDSCgP6dynPGh5Sl2bmS9f_AoJl5O7Y,3340
+OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/top_level.txt,sha256=PitPPl6JTchA3_fMFrNtchDNB9Ip8YkRyhMiQmuJWe4,24
+OpenGeode_GeosciencesIO-4.2.0rc2.dist-info/RECORD,,
```

