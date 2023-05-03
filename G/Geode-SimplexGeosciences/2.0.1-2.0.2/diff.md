# Comparing `tmp/Geode_SimplexGeosciences-2.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_SimplexGeosciences-2.0.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 2125209 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      212 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/__init__.py
--rw-rw-rw-  2.0 fat      261 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/cross_section.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/structural_model.py
--rw-rw-rw-  2.0 fat  2039296 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll
--rw-rw-rw-  2.0 fat  2039296 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll
--rw-rw-rw-  2.0 fat   137216 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   137216 b- defN 23-Apr-27 11:31 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     3330 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1220 b- defN 23-Apr-27 11:31 Geode_SimplexGeosciences-2.0.1.dist-info/RECORD
-11 files, 4358439 bytes uncompressed, 2123065 bytes compressed:  51.3%
+Zip file size: 2125208 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      212 b- defN 23-May-03 10:01 geode_simplexgeosciences/__init__.py
+-rw-rw-rw-  2.0 fat      261 b- defN 23-May-03 10:01 geode_simplexgeosciences/cross_section.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-May-03 10:01 geode_simplexgeosciences/structural_model.py
+-rw-rw-rw-  2.0 fat  2039296 b- defN 23-May-03 10:01 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll
+-rw-rw-rw-  2.0 fat  2039296 b- defN 23-May-03 10:01 geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-May-03 10:01 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   137216 b- defN 23-May-03 10:01 geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     3330 b- defN 23-May-03 10:01 Geode_SimplexGeosciences-2.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-03 10:01 Geode_SimplexGeosciences-2.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-May-03 10:01 Geode_SimplexGeosciences-2.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1220 b- defN 23-May-03 10:01 Geode_SimplexGeosciences-2.0.2.dist-info/RECORD
+11 files, 4358439 bytes uncompressed, 2123064 bytes compressed:  51.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.1.dist-info/METADATA
+Filename: Geode_SimplexGeosciences-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.1.dist-info/WHEEL
+Filename: Geode_SimplexGeosciences-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.1.dist-info/top_level.txt
+Filename: Geode_SimplexGeosciences-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_SimplexGeosciences-2.0.1.dist-info/RECORD
+Filename: Geode_SimplexGeosciences-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001801615ec
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 27 11:31:19 2023
+Time/Date		Wed May  3 10:01:29 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000162e00
 SizeOfInitializedData	000000000008ec00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000001615ec
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		001f8000
 SizeOfHeaders		00000400
-CheckSum		001f2467
+CheckSum		001fcbba
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -65,20 +65,20 @@
 The Import Tables (interpreted .rdata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
  001dae90	001db528 00000000 00000000 001dbb48 00164478
 
 	DLL Name: OpenGeode-Geosciences_explicit.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	1dbb26	  199  ??1CrossSection@geode@@QEAA@XZ
-	1dbaf4	   87  ??0CrossSection@geode@@QEAA@$$QEAVSection@1@@Z
-	1dbaca	   86  ??0CrossSection@geode@@QEAA@$$QEAV01@@Z
-	1db9f6	   89  ??0CrossSectionBuilder@geode@@QEAA@AEAVCrossSection@1@@Z
-	1dba32	  361  ?copy_geological_components@CrossSectionBuilder@geode@@QEAAXAEAV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVCrossSection@2@@Z
-	1db9c0	  462  ?initialize@GeosciencesExplicitLibrary@geode@@SAXXZ
+	1dbb26	  183  ??1CrossSection@geode@@QEAA@XZ
+	1dbaf4	   79  ??0CrossSection@geode@@QEAA@$$QEAVSection@1@@Z
+	1dbaca	   78  ??0CrossSection@geode@@QEAA@$$QEAV01@@Z
+	1db9f6	   81  ??0CrossSectionBuilder@geode@@QEAA@AEAVCrossSection@1@@Z
+	1dba32	  345  ?copy_geological_components@CrossSectionBuilder@geode@@QEAAXAEAV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVCrossSection@2@@Z
+	1db9c0	  446  ?initialize@GeosciencesExplicitLibrary@geode@@SAXXZ
 
  001daea4	001db178 00000000 00000000 001dbc3e 001640c8
 
 	DLL Name: Geode-Simplex_section.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	1dbb6c	    4  ?initialize@SimplexSectionLibrary@geode@@SAXXZ
 	1dbb9e	    6  ?simplex_remesh@geode@@YA?AV?$tuple@VSection@geode@@V?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@@std@@AEAVSection@1@AEBV?$Metric@$01@1@@Z
@@ -112,16 +112,16 @@
 	vma:  Hint/Ord Member-Name Bound-To
 	1dbd32	   68  GetAdaptersInfo
 
  001daef4	001db5b0 00000000 00000000 001dbe00 00164500
 
 	DLL Name: OpenGeode_model.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	1dbde4	  451  ??1Section@geode@@QEAA@XZ
-	1dbd52	  723  ?copy_relationships@RelationshipsBuilder@geode@@QEAAXAEBV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVRelationships@2@@Z
+	1dbde4	  407  ??1Section@geode@@QEAA@XZ
+	1dbd52	  679  ?copy_relationships@RelationshipsBuilder@geode@@QEAAXAEBV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVRelationships@2@@Z
 
  001daf08	001db560 00000000 00000000 001dbff0 001644b0
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	1dbe8a	   49  ??1Library@geode@@UEAA@XZ
 	1dbef0	   57  ??1Singleton@geode@@UEAA@XZ
@@ -34217,37 +34217,37 @@
 	  1050: 00 00 00 00 44 d7 1d 00 00 00 00 00 b8 d6 1d 00
 	  1060: 00 00 00 00 c2 d6 1d 00 00 00 00 00 82 d7 1d 00
 	  1070: 00 00 00 00 b0 d7 1d 00 00 00 00 00 a6 d7 1d 00
 	  1080: 00 00 00 00 00 00 00 00 00 00 00 00 30 d8 1d 00
 	  1090: 00 00 00 00 a4 d6 1d 00 00 00 00 00 6c d6 1d 00
 	  10a0: 00 00 00 00 5e d6 1d 00 00 00 00 00 00 00 00 00
 	  10b0: 00 00 00 00 7a d7 1d 00 00 00 00 00 00 00 00 00
-	  10c0: 00 00 00 00 ce 01 3f 69 6e 69 74 69 61 6c 69 7a
+	  10c0: 00 00 00 00 be 01 3f 69 6e 69 74 69 61 6c 69 7a
 	  10d0: 65 40 47 65 6f 73 63 69 65 6e 63 65 73 45 78 70
 	  10e0: 6c 69 63 69 74 4c 69 62 72 61 72 79 40 67 65 6f
-	  10f0: 64 65 40 40 53 41 58 58 5a 00 59 00 3f 3f 30 43
+	  10f0: 64 65 40 40 53 41 58 58 5a 00 51 00 3f 3f 30 43
 	  1100: 72 6f 73 73 53 65 63 74 69 6f 6e 42 75 69 6c 64
 	  1110: 65 72 40 67 65 6f 64 65 40 40 51 45 41 41 40 41
 	  1120: 45 41 56 43 72 6f 73 73 53 65 63 74 69 6f 6e 40
-	  1130: 31 40 40 5a 00 00 69 01 3f 63 6f 70 79 5f 67 65
+	  1130: 31 40 40 5a 00 00 59 01 3f 63 6f 70 79 5f 67 65
 	  1140: 6f 6c 6f 67 69 63 61 6c 5f 63 6f 6d 70 6f 6e 65
 	  1150: 6e 74 73 40 43 72 6f 73 73 53 65 63 74 69 6f 6e
 	  1160: 42 75 69 6c 64 65 72 40 67 65 6f 64 65 40 40 51
 	  1170: 45 41 41 58 41 45 41 56 3f 24 4d 6f 64 65 6c 4d
 	  1180: 61 70 70 69 6e 67 40 56 3f 24 42 69 6a 65 63 74
 	  1190: 69 76 65 4d 61 70 70 69 6e 67 40 55 75 75 69 64
 	  11a0: 40 67 65 6f 64 65 40 40 55 31 32 40 40 67 65 6f
 	  11b0: 64 65 40 40 40 32 40 41 45 42 56 43 72 6f 73 73
-	  11c0: 53 65 63 74 69 6f 6e 40 32 40 40 5a 00 00 56 00
+	  11c0: 53 65 63 74 69 6f 6e 40 32 40 40 5a 00 00 4e 00
 	  11d0: 3f 3f 30 43 72 6f 73 73 53 65 63 74 69 6f 6e 40
 	  11e0: 67 65 6f 64 65 40 40 51 45 41 41 40 24 24 51 45
-	  11f0: 41 56 30 31 40 40 5a 00 57 00 3f 3f 30 43 72 6f
+	  11f0: 41 56 30 31 40 40 5a 00 4f 00 3f 3f 30 43 72 6f
 	  1200: 73 73 53 65 63 74 69 6f 6e 40 67 65 6f 64 65 40
 	  1210: 40 51 45 41 41 40 24 24 51 45 41 56 53 65 63 74
-	  1220: 69 6f 6e 40 31 40 40 5a 00 00 c7 00 3f 3f 31 43
+	  1220: 69 6f 6e 40 31 40 40 5a 00 00 b7 00 3f 3f 31 43
 	  1230: 72 6f 73 73 53 65 63 74 69 6f 6e 40 67 65 6f 64
 	  1240: 65 40 40 51 45 41 41 40 58 5a 00 00 4f 70 65 6e
 	  1250: 47 65 6f 64 65 2d 47 65 6f 73 63 69 65 6e 63 65
 	  1260: 73 5f 65 78 70 6c 69 63 69 74 2e 64 6c 6c 00 00
 	  1270: 04 00 3f 69 6e 69 74 69 61 6c 69 7a 65 40 53 69
 	  1280: 6d 70 6c 65 78 53 65 63 74 69 6f 6e 4c 69 62 72
 	  1290: 61 72 79 40 67 65 6f 64 65 40 40 53 41 58 58 5a
@@ -34274,24 +34274,24 @@
 	  13e0: 72 74 46 72 65 65 43 65 72 74 69 66 69 63 61 74
 	  13f0: 65 43 6f 6e 74 65 78 74 00 00 46 00 43 65 72 74
 	  1400: 47 65 74 43 65 72 74 69 66 69 63 61 74 65 43 6f
 	  1410: 6e 74 65 78 74 50 72 6f 70 65 72 74 79 00 43 52
 	  1420: 59 50 54 33 32 2e 64 6c 6c 00 57 53 32 5f 33 32
 	  1430: 2e 64 6c 6c 00 00 44 00 47 65 74 41 64 61 70 74
 	  1440: 65 72 73 49 6e 66 6f 00 49 50 48 4c 50 41 50 49
-	  1450: 2e 44 4c 4c 00 00 d3 02 3f 63 6f 70 79 5f 72 65
+	  1450: 2e 44 4c 4c 00 00 a7 02 3f 63 6f 70 79 5f 72 65
 	  1460: 6c 61 74 69 6f 6e 73 68 69 70 73 40 52 65 6c 61
 	  1470: 74 69 6f 6e 73 68 69 70 73 42 75 69 6c 64 65 72
 	  1480: 40 67 65 6f 64 65 40 40 51 45 41 41 58 41 45 42
 	  1490: 56 3f 24 4d 6f 64 65 6c 4d 61 70 70 69 6e 67 40
 	  14a0: 56 3f 24 42 69 6a 65 63 74 69 76 65 4d 61 70 70
 	  14b0: 69 6e 67 40 55 75 75 69 64 40 67 65 6f 64 65 40
 	  14c0: 40 55 31 32 40 40 67 65 6f 64 65 40 40 40 32 40
 	  14d0: 41 45 42 56 52 65 6c 61 74 69 6f 6e 73 68 69 70
-	  14e0: 73 40 32 40 40 5a 00 00 c3 01 3f 3f 31 53 65 63
+	  14e0: 73 40 32 40 40 5a 00 00 97 01 3f 3f 31 53 65 63
 	  14f0: 74 69 6f 6e 40 67 65 6f 64 65 40 40 51 45 41 41
 	  1500: 40 58 5a 00 4f 70 65 6e 47 65 6f 64 65 5f 6d 6f
 	  1510: 64 65 6c 2e 64 6c 6c 00 c0 00 3f 73 65 74 5f 69
 	  1520: 6e 73 74 61 6e 63 65 40 53 69 6e 67 6c 65 74 6f
 	  1530: 6e 40 67 65 6f 64 65 40 40 43 41 58 41 45 42 56
 	  1540: 74 79 70 65 5f 69 6e 66 6f 40 40 50 45 41 56 31
 	  1550: 32 40 40 5a 00 00 8c 00 3f 69 6e 73 74 61 6e 63
@@ -616814,18 +616814,17 @@
    1801cac38:	(bad)
    1801cac3d:	insb   (%dx),%es:(%rdi)
    1801cac3e:	insb   (%dx),%es:(%rdi)
    1801cac3f:	outsl  %ds:(%rsi),(%dx)
    1801cac40:	movsxd 0x74(%rcx),%esp
    1801cac43:	imul   $0x0,0x6e(%rdi),%ebp
    1801cac4a:	add    %al,(%rax)
-   1801cac4c:	(bad)
-   1801cac4d:	pop    %rbp
-   1801cac4e:	rex.WX
-   1801cac4f:	add    %al,%fs:(%rax)
+   1801cac4c:	stc
+   1801cac4d:	xor    %dl,0x64(%rdx)
+   1801cac50:	add    %al,(%rax)
    1801cac52:	add    %al,(%rax)
    1801cac54:	or     $0x60000000,%eax
    1801cac59:	add    (%rax),%eax
    1801cac5b:	add    %ah,%ah
    1801cac5d:	ret    $0x1c
    1801cac60:	in     $0xb4,%al
    1801cac62:	sbb    $0x0,%al
@@ -642313,33 +642312,34 @@
    1801db99a:	sbb    $0x0,%eax
    1801db99f:	add    %bl,-0x2a(%rsi)
    1801db9a2:	sbb    $0x0,%eax
 	...
    1801db9af:	add    %bh,-0x29(%rdx)
    1801db9b2:	sbb    $0x0,%eax
 	...
-   1801db9bf:	add    %cl,%dh
-   1801db9c1:	add    %edi,(%rdi)
-   1801db9c3:	imul   $0x6c616974,0x69(%rsi),%ebp
-   1801db9ca:	imul   $0x6f654740,0x65(%rdx),%edi
+   1801db9bf:	add    %bh,0x6e693f01(%rsi)
+   1801db9c5:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   1801db9cd:	rex
+   1801db9ce:	rex.RXB
+   1801db9cf:	outsl  %gs:(%rsi),(%dx)
    1801db9d1:	jae    0x1801dba36
    1801db9d3:	imul   $0x45736563,0x6e(%rbp),%esp
    1801db9da:	js     0x1801dba4c
    1801db9dc:	insb   (%dx),%es:(%rdi)
    1801db9dd:	imul   $0x62694c74,0x69(%rbx),%esp
    1801db9e4:	jb     0x1801dba47
    1801db9e6:	jb     0x1801dba61
    1801db9e8:	rex
    1801db9e9:	outsl  %gs:(%esi),(%dx)
    1801db9ec:	fs gs rex
    1801db9ef:	rex push %rbx
    1801db9f1:	pop    %r8
    1801db9f3:	pop    %rax
    1801db9f4:	pop    %rdx
-   1801db9f5:	add    %bl,0x0(%rcx)
+   1801db9f5:	add    %dl,0x0(%rcx)
    1801db9f8:	(bad)
    1801db9f9:	(bad)
    1801db9fa:	xor    %al,0x72(%rbx)
    1801db9fd:	outsl  %ds:(%rsi),(%dx)
    1801db9fe:	jae    0x1801dba73
    1801dba00:	push   %rbx
    1801dba01:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
@@ -642361,15 +642361,17 @@
    1801dba22:	jae    0x1801dba97
    1801dba24:	push   %rbx
    1801dba25:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    1801dba2a:	outsb  %ds:(%rsi),(%dx)
    1801dba2b:	rex xor %eax,0x40(%rax)
    1801dba2f:	pop    %rdx
    1801dba30:	add    %al,(%rax)
-   1801dba32:	imul   $0x706f633f,(%rcx),%eax
+   1801dba32:	pop    %rcx
+   1801dba33:	add    %edi,(%rdi)
+   1801dba35:	movsxd 0x70(%rdi),%ebp
    1801dba38:	jns    0x1801dba99
    1801dba3a:	outsl  %gs:(%esi),(%dx)
    1801dba3d:	insb   (%dx),%es:(%rdi)
    1801dba3e:	outsl  %ds:(%rsi),(%dx)
    1801dba3f:	imul   $0x6f635f6c,0x61(%ebx),%esp
    1801dba47:	insl   (%dx),%es:(%rdi)
    1801dba48:	jo     0x1801dbab9
@@ -642421,16 +642423,15 @@
    1801dbaba:	jae    0x1801dbb2f
    1801dbabc:	push   %rbx
    1801dbabd:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    1801dbac2:	outsb  %ds:(%rsi),(%dx)
    1801dbac3:	rex xor 0x40(%rax),%al
    1801dbac7:	pop    %rdx
    1801dbac8:	add    %al,(%rax)
-   1801dbaca:	push   %rsi
-   1801dbacb:	add    %bh,(%rdi)
+   1801dbaca:	rex.WRX add %r15b,(%rdi)
    1801dbacd:	(bad)
    1801dbace:	xor    %al,0x72(%rbx)
    1801dbad1:	outsl  %ds:(%rsi),(%dx)
    1801dbad2:	jae    0x1801dbb47
    1801dbad4:	push   %rbx
    1801dbad5:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    1801dbada:	outsb  %ds:(%rsi),(%dx)
@@ -642444,15 +642445,15 @@
    1801dbae7:	rex and $0x24,%al
    1801dbaea:	push   %rcx
    1801dbaeb:	rex.RB
    1801dbaec:	push   %r14
    1801dbaee:	xor    %dh,(%rcx)
    1801dbaf0:	rex
    1801dbaf1:	rex pop %rdx
-   1801dbaf3:	add    %dl,0x0(%rdi)
+   1801dbaf3:	add    %cl,0x0(%rdi)
    1801dbaf6:	(bad)
    1801dbaf7:	(bad)
    1801dbaf8:	xor    %al,0x72(%rbx)
    1801dbafb:	outsl  %ds:(%rsi),(%dx)
    1801dbafc:	jae    0x1801dbb71
    1801dbafe:	push   %rbx
    1801dbaff:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
@@ -642470,16 +642471,19 @@
    1801dbb16:	push   %r14
    1801dbb18:	push   %rbx
    1801dbb19:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    1801dbb1e:	outsb  %ds:(%rsi),(%dx)
    1801dbb1f:	rex xor %eax,0x40(%rax)
    1801dbb23:	pop    %rdx
    1801dbb24:	add    %al,(%rax)
-   1801dbb26:	movl   $0x43313f3f,(%rax)
-   1801dbb2c:	jb     0x1801dbb9d
+   1801dbb26:	mov    $0x0,%bh
+   1801dbb28:	(bad)
+   1801dbb29:	(bad)
+   1801dbb2a:	xor    %eax,0x72(%rbx)
+   1801dbb2d:	outsl  %ds:(%rsi),(%dx)
    1801dbb2e:	jae    0x1801dbba3
    1801dbb30:	push   %rbx
    1801dbb31:	movsxd %gs:0x6f(%rcx,%rbp,2),%esi
    1801dbb36:	outsb  %ds:(%rsi),(%dx)
    1801dbb37:	rex
    1801dbb38:	outsl  %gs:(%esi),(%dx)
    1801dbb3b:	fs gs rex
@@ -642698,16 +642702,16 @@
    1801dbd46:	rex.W
    1801dbd47:	rex.WR push %rax
    1801dbd49:	push   %r8
    1801dbd4b:	rex.WB
    1801dbd4c:	cs rex.R
    1801dbd4e:	rex.WR
    1801dbd4f:	rex.WR add %r8b,(%rax)
-   1801dbd52:	roll   %cl,(%rdx)
-   1801dbd54:	(bad)
+   1801dbd52:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   1801dbd53:	add    (%rdi),%bh
    1801dbd55:	movsxd 0x70(%rdi),%ebp
    1801dbd58:	jns    0x1801dbdb9
    1801dbd5a:	jb     0x1801dbdc1
    1801dbd5c:	insb   (%dx),%es:(%rdi)
    1801dbd5d:	(bad)
    1801dbd5e:	je     0x1801dbdc9
    1801dbd60:	outsl  %ds:(%rsi),(%dx)
@@ -642759,15 +642763,15 @@
    1801dbdd4:	je     0x1801dbe3f
    1801dbdd6:	outsl  %ds:(%rsi),(%dx)
    1801dbdd7:	outsb  %ds:(%rsi),(%dx)
    1801dbdd8:	jae    0x1801dbe42
    1801dbdda:	imul   $0x40403240,0x73(%rax),%esi
    1801dbde1:	pop    %rdx
    1801dbde2:	add    %al,(%rax)
-   1801dbde4:	ret
+   1801dbde4:	xchg   %eax,%edi
    1801dbde5:	add    %edi,(%rdi)
    1801dbde7:	(bad)
    1801dbde8:	xor    %edx,0x65(%rbx)
    1801dbdeb:	movsxd 0x6f(%rcx,%rbp,2),%esi
    1801dbdef:	outsb  %ds:(%rsi),(%dx)
    1801dbdf0:	rex
    1801dbdf1:	outsl  %gs:(%esi),(%dx)
```

## geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001801615ec
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr 27 11:31:20 2023
+Time/Date		Wed May  3 10:01:30 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000162e00
 SizeOfInitializedData	000000000008ec00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000001615ec
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		001f8000
 SizeOfHeaders		00000400
-CheckSum		002005c7
+CheckSum		001fad03
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -65,20 +65,20 @@
 The Import Tables (interpreted .rdata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
  001daea8	001db540 00000000 00000000 001dbb72 00164478
 
 	DLL Name: OpenGeode-Geosciences_explicit.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	1dbb4e	  229  ??1StructuralModel@geode@@QEAA@XZ
-	1dbb1c	  176  ??0StructuralModel@geode@@QEAA@$$QEAVBRep@1@@Z
-	1dbaee	  175  ??0StructuralModel@geode@@QEAA@$$QEAV01@@Z
-	1dba0e	  178  ??0StructuralModelBuilder@geode@@QEAA@AEAVStructuralModel@1@@Z
-	1dba50	  362  ?copy_geological_components@StructuralModelBuilder@geode@@QEAAXAEAV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVStructuralModel@2@@Z
-	1db9d8	  462  ?initialize@GeosciencesExplicitLibrary@geode@@SAXXZ
+	1dbb4e	  213  ??1StructuralModel@geode@@QEAA@XZ
+	1dbb1c	  160  ??0StructuralModel@geode@@QEAA@$$QEAVBRep@1@@Z
+	1dbaee	  159  ??0StructuralModel@geode@@QEAA@$$QEAV01@@Z
+	1dba0e	  162  ??0StructuralModelBuilder@geode@@QEAA@AEAVStructuralModel@1@@Z
+	1dba50	  346  ?copy_geological_components@StructuralModelBuilder@geode@@QEAAXAEAV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVStructuralModel@2@@Z
+	1db9d8	  446  ?initialize@GeosciencesExplicitLibrary@geode@@SAXXZ
 
  001daebc	001db190 00000000 00000000 001dbc5e 001640c8
 
 	DLL Name: Geode-Simplex_brep.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	1dbb96	    4  ?initialize@SimplexBRepLibrary@geode@@SAXXZ
 	1dbbc4	    8  ?simplex_remesh@geode@@YA?AV?$tuple@VBRep@geode@@V?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@@std@@AEAVBRep@1@AEBV?$Metric@$02@1@@Z
@@ -112,16 +112,16 @@
 	vma:  Hint/Ord Member-Name Bound-To
 	1dbd50	   68  GetAdaptersInfo
 
  001daf0c	001db5c8 00000000 00000000 001dbe1c 00164500
 
 	DLL Name: OpenGeode_model.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	1dbe02	  393  ??1BRep@geode@@QEAA@XZ
-	1dbd70	  723  ?copy_relationships@RelationshipsBuilder@geode@@QEAAXAEBV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVRelationships@2@@Z
+	1dbe02	  349  ??1BRep@geode@@QEAA@XZ
+	1dbd70	  679  ?copy_relationships@RelationshipsBuilder@geode@@QEAAXAEBV?$ModelMapping@V?$BijectiveMapping@Uuuid@geode@@U12@@geode@@@2@AEBVRelationships@2@@Z
 
  001daf20	001db578 00000000 00000000 001dc00c 001644b0
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	1dbea6	   49  ??1Library@geode@@UEAA@XZ
 	1dbf0c	   57  ??1Singleton@geode@@UEAA@XZ
@@ -34218,39 +34218,39 @@
 	  1060: 00 00 00 00 9c d6 1d 00 00 00 00 00 60 d7 1d 00
 	  1070: 00 00 00 00 d4 d6 1d 00 00 00 00 00 de d6 1d 00
 	  1080: 00 00 00 00 9e d7 1d 00 00 00 00 00 cc d7 1d 00
 	  1090: 00 00 00 00 c2 d7 1d 00 00 00 00 00 00 00 00 00
 	  10a0: 00 00 00 00 4c d8 1d 00 00 00 00 00 c0 d6 1d 00
 	  10b0: 00 00 00 00 88 d6 1d 00 00 00 00 00 7a d6 1d 00
 	  10c0: 00 00 00 00 00 00 00 00 00 00 00 00 96 d7 1d 00
-	  10d0: 00 00 00 00 00 00 00 00 00 00 00 00 ce 01 3f 69
+	  10d0: 00 00 00 00 00 00 00 00 00 00 00 00 be 01 3f 69
 	  10e0: 6e 69 74 69 61 6c 69 7a 65 40 47 65 6f 73 63 69
 	  10f0: 65 6e 63 65 73 45 78 70 6c 69 63 69 74 4c 69 62
 	  1100: 72 61 72 79 40 67 65 6f 64 65 40 40 53 41 58 58
-	  1110: 5a 00 b2 00 3f 3f 30 53 74 72 75 63 74 75 72 61
+	  1110: 5a 00 a2 00 3f 3f 30 53 74 72 75 63 74 75 72 61
 	  1120: 6c 4d 6f 64 65 6c 42 75 69 6c 64 65 72 40 67 65
 	  1130: 6f 64 65 40 40 51 45 41 41 40 41 45 41 56 53 74
 	  1140: 72 75 63 74 75 72 61 6c 4d 6f 64 65 6c 40 31 40
-	  1150: 40 5a 00 00 6a 01 3f 63 6f 70 79 5f 67 65 6f 6c
+	  1150: 40 5a 00 00 5a 01 3f 63 6f 70 79 5f 67 65 6f 6c
 	  1160: 6f 67 69 63 61 6c 5f 63 6f 6d 70 6f 6e 65 6e 74
 	  1170: 73 40 53 74 72 75 63 74 75 72 61 6c 4d 6f 64 65
 	  1180: 6c 42 75 69 6c 64 65 72 40 67 65 6f 64 65 40 40
 	  1190: 51 45 41 41 58 41 45 41 56 3f 24 4d 6f 64 65 6c
 	  11a0: 4d 61 70 70 69 6e 67 40 56 3f 24 42 69 6a 65 63
 	  11b0: 74 69 76 65 4d 61 70 70 69 6e 67 40 55 75 75 69
 	  11c0: 64 40 67 65 6f 64 65 40 40 55 31 32 40 40 67 65
 	  11d0: 6f 64 65 40 40 40 32 40 41 45 42 56 53 74 72 75
 	  11e0: 63 74 75 72 61 6c 4d 6f 64 65 6c 40 32 40 40 5a
-	  11f0: 00 00 af 00 3f 3f 30 53 74 72 75 63 74 75 72 61
+	  11f0: 00 00 9f 00 3f 3f 30 53 74 72 75 63 74 75 72 61
 	  1200: 6c 4d 6f 64 65 6c 40 67 65 6f 64 65 40 40 51 45
 	  1210: 41 41 40 24 24 51 45 41 56 30 31 40 40 5a 00 00
-	  1220: b0 00 3f 3f 30 53 74 72 75 63 74 75 72 61 6c 4d
+	  1220: a0 00 3f 3f 30 53 74 72 75 63 74 75 72 61 6c 4d
 	  1230: 6f 64 65 6c 40 67 65 6f 64 65 40 40 51 45 41 41
 	  1240: 40 24 24 51 45 41 56 42 52 65 70 40 31 40 40 5a
-	  1250: 00 00 e5 00 3f 3f 31 53 74 72 75 63 74 75 72 61
+	  1250: 00 00 d5 00 3f 3f 31 53 74 72 75 63 74 75 72 61
 	  1260: 6c 4d 6f 64 65 6c 40 67 65 6f 64 65 40 40 51 45
 	  1270: 41 41 40 58 5a 00 4f 70 65 6e 47 65 6f 64 65 2d
 	  1280: 47 65 6f 73 63 69 65 6e 63 65 73 5f 65 78 70 6c
 	  1290: 69 63 69 74 2e 64 6c 6c 00 00 04 00 3f 69 6e 69
 	  12a0: 74 69 61 6c 69 7a 65 40 53 69 6d 70 6c 65 78 42
 	  12b0: 52 65 70 4c 69 62 72 61 72 79 40 67 65 6f 64 65
 	  12c0: 40 40 53 41 58 58 5a 00 08 00 3f 73 69 6d 70 6c
@@ -34276,24 +34276,24 @@
 	  1400: 46 72 65 65 43 65 72 74 69 66 69 63 61 74 65 43
 	  1410: 6f 6e 74 65 78 74 00 00 46 00 43 65 72 74 47 65
 	  1420: 74 43 65 72 74 69 66 69 63 61 74 65 43 6f 6e 74
 	  1430: 65 78 74 50 72 6f 70 65 72 74 79 00 43 52 59 50
 	  1440: 54 33 32 2e 64 6c 6c 00 57 53 32 5f 33 32 2e 64
 	  1450: 6c 6c 00 00 44 00 47 65 74 41 64 61 70 74 65 72
 	  1460: 73 49 6e 66 6f 00 49 50 48 4c 50 41 50 49 2e 44
-	  1470: 4c 4c 00 00 d3 02 3f 63 6f 70 79 5f 72 65 6c 61
+	  1470: 4c 4c 00 00 a7 02 3f 63 6f 70 79 5f 72 65 6c 61
 	  1480: 74 69 6f 6e 73 68 69 70 73 40 52 65 6c 61 74 69
 	  1490: 6f 6e 73 68 69 70 73 42 75 69 6c 64 65 72 40 67
 	  14a0: 65 6f 64 65 40 40 51 45 41 41 58 41 45 42 56 3f
 	  14b0: 24 4d 6f 64 65 6c 4d 61 70 70 69 6e 67 40 56 3f
 	  14c0: 24 42 69 6a 65 63 74 69 76 65 4d 61 70 70 69 6e
 	  14d0: 67 40 55 75 75 69 64 40 67 65 6f 64 65 40 40 55
 	  14e0: 31 32 40 40 67 65 6f 64 65 40 40 40 32 40 41 45
 	  14f0: 42 56 52 65 6c 61 74 69 6f 6e 73 68 69 70 73 40
-	  1500: 32 40 40 5a 00 00 89 01 3f 3f 31 42 52 65 70 40
+	  1500: 32 40 40 5a 00 00 5d 01 3f 3f 31 42 52 65 70 40
 	  1510: 67 65 6f 64 65 40 40 51 45 41 41 40 58 5a 00 00
 	  1520: 4f 70 65 6e 47 65 6f 64 65 5f 6d 6f 64 65 6c 2e
 	  1530: 64 6c 6c 00 c0 00 3f 73 65 74 5f 69 6e 73 74 61
 	  1540: 6e 63 65 40 53 69 6e 67 6c 65 74 6f 6e 40 67 65
 	  1550: 6f 64 65 40 40 43 41 58 41 45 42 56 74 79 70 65
 	  1560: 5f 69 6e 66 6f 40 40 50 45 41 56 31 32 40 40 5a
 	  1570: 00 00 8c 00 3f 69 6e 73 74 61 6e 63 65 40 53 69
@@ -616819,16 +616819,17 @@
    1801cac38:	(bad)
    1801cac3d:	insb   (%dx),%es:(%rdi)
    1801cac3e:	insb   (%dx),%es:(%rdi)
    1801cac3f:	outsl  %ds:(%rsi),(%dx)
    1801cac40:	movsxd 0x74(%rcx),%esp
    1801cac43:	imul   $0x0,0x6e(%rdi),%ebp
    1801cac4a:	add    %al,(%rax)
-   1801cac4c:	or     %bl,0x4a(%rbp)
-   1801cac4f:	add    %al,%fs:(%rax)
+   1801cac4c:	cli
+   1801cac4d:	xor    %dl,0x64(%rdx)
+   1801cac50:	add    %al,(%rax)
    1801cac52:	add    %al,(%rax)
    1801cac54:	or     $0x60000000,%eax
    1801cac59:	add    (%rax),%eax
    1801cac5b:	add    %ah,%ah
    1801cac5d:	ret    $0x1c
    1801cac60:	in     $0xb4,%al
    1801cac62:	sbb    $0x0,%al
@@ -642335,33 +642336,34 @@
    1801db9b5:	add    %al,(%rax)
    1801db9b7:	add    %bh,-0x2a(%rdx)
    1801db9ba:	sbb    $0x0,%eax
 	...
    1801db9c7:	add    %dl,0x1dd7(%rsi)
 	...
    1801db9d5:	add    %al,(%rax)
-   1801db9d7:	add    %cl,%dh
-   1801db9d9:	add    %edi,(%rdi)
-   1801db9db:	imul   $0x6c616974,0x69(%rsi),%ebp
-   1801db9e2:	imul   $0x6f654740,0x65(%rdx),%edi
+   1801db9d7:	add    %bh,0x6e693f01(%rsi)
+   1801db9dd:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   1801db9e5:	rex
+   1801db9e6:	rex.RXB
+   1801db9e7:	outsl  %gs:(%rsi),(%dx)
    1801db9e9:	jae    0x1801dba4e
    1801db9eb:	imul   $0x45736563,0x6e(%rbp),%esp
    1801db9f2:	js     0x1801dba64
    1801db9f4:	insb   (%dx),%es:(%rdi)
    1801db9f5:	imul   $0x62694c74,0x69(%rbx),%esp
    1801db9fc:	jb     0x1801dba5f
    1801db9fe:	jb     0x1801dba79
    1801dba00:	rex
    1801dba01:	outsl  %gs:(%esi),(%dx)
    1801dba04:	fs gs rex
    1801dba07:	rex push %rbx
    1801dba09:	pop    %r8
    1801dba0b:	pop    %rax
    1801dba0c:	pop    %rdx
-   1801dba0d:	add    %dh,0x303f3f00(%rdx)
+   1801dba0d:	add    %ah,0x303f3f00(%rdx)
    1801dba13:	push   %rbx
    1801dba14:	je     0x1801dba88
    1801dba16:	jne    0x1801dba7b
    1801dba18:	je     0x1801dba8f
    1801dba1a:	jb     0x1801dba7d
    1801dba1c:	insb   (%dx),%es:(%rdi)
    1801dba1d:	rex.WRB outsl %ds:(%rsi),(%dx)
@@ -642386,16 +642388,16 @@
    1801dba41:	jb     0x1801dbaa4
    1801dba43:	insb   (%dx),%es:(%rdi)
    1801dba44:	rex.WRB outsl %ds:(%rsi),(%dx)
    1801dba46:	fs gs insb (%dx),%es:(%rdi)
    1801dba49:	rex xor %eax,0x40(%rax)
    1801dba4d:	pop    %rdx
    1801dba4e:	add    %al,(%rax)
-   1801dba50:	push   $0x1
-   1801dba52:	(bad)
+   1801dba50:	pop    %rdx
+   1801dba51:	add    %edi,(%rdi)
    1801dba53:	movsxd 0x70(%rdi),%ebp
    1801dba56:	jns    0x1801dbab7
    1801dba58:	outsl  %gs:(%esi),(%dx)
    1801dba5b:	insb   (%dx),%es:(%rdi)
    1801dba5c:	outsl  %ds:(%rsi),(%dx)
    1801dba5d:	imul   $0x6f635f6c,0x61(%ebx),%esp
    1801dba65:	insl   (%dx),%es:(%rdi)
@@ -642453,15 +642455,15 @@
    1801dbadf:	jb     0x1801dbb42
    1801dbae1:	insb   (%dx),%es:(%rdi)
    1801dbae2:	rex.WRB outsl %ds:(%rsi),(%dx)
    1801dbae4:	fs gs insb (%dx),%es:(%rdi)
    1801dbae7:	rex xor 0x40(%rax),%al
    1801dbaeb:	pop    %rdx
    1801dbaec:	add    %al,(%rax)
-   1801dbaee:	scas   %es:(%rdi),%eax
+   1801dbaee:	lahf
    1801dbaef:	add    %bh,(%rdi)
    1801dbaf1:	(bad)
    1801dbaf2:	xor    %dl,0x74(%rbx)
    1801dbaf5:	jb     0x1801dbb6c
    1801dbaf7:	movsxd 0x72(%rbp,%rsi,2),%esi
    1801dbafb:	(bad)
    1801dbafc:	insb   (%dx),%es:(%rdi)
@@ -642478,19 +642480,15 @@
    1801dbb11:	push   %rcx
    1801dbb12:	rex.RB
    1801dbb13:	push   %r14
    1801dbb15:	xor    %dh,(%rcx)
    1801dbb17:	rex
    1801dbb18:	rex pop %rdx
    1801dbb1a:	add    %al,(%rax)
-   1801dbb1c:	mov    $0x0,%al
-   1801dbb1e:	(bad)
-   1801dbb1f:	(bad)
-   1801dbb20:	xor    %dl,0x74(%rbx)
-   1801dbb23:	jb     0x1801dbb9a
+   1801dbb1c:	movabs 0x75727453303f3f00,%al
    1801dbb25:	movsxd 0x72(%rbp,%rsi,2),%esi
    1801dbb29:	(bad)
    1801dbb2a:	insb   (%dx),%es:(%rdi)
    1801dbb2b:	rex.WRB outsl %ds:(%rsi),(%dx)
    1801dbb2d:	fs gs insb (%dx),%es:(%rdi)
    1801dbb30:	rex
    1801dbb31:	outsl  %gs:(%esi),(%dx)
@@ -642504,16 +642502,16 @@
    1801dbb40:	rex.RB
    1801dbb41:	push   %r14
    1801dbb43:	rex.X push %rdx
    1801dbb45:	gs jo  0x1801dbb88
    1801dbb48:	xor    %eax,0x40(%rax)
    1801dbb4b:	pop    %rdx
    1801dbb4c:	add    %al,(%rax)
-   1801dbb4e:	in     $0x0,%eax
-   1801dbb50:	(bad)
+   1801dbb4e:	(bad)
+   1801dbb4f:	add    %bh,(%rdi)
    1801dbb51:	(bad)
    1801dbb52:	xor    %edx,0x74(%rbx)
    1801dbb55:	jb     0x1801dbbcc
    1801dbb57:	movsxd 0x72(%rbp,%rsi,2),%esi
    1801dbb5b:	(bad)
    1801dbb5c:	insb   (%dx),%es:(%rdi)
    1801dbb5d:	rex.WRB outsl %ds:(%rsi),(%dx)
@@ -642730,16 +642728,16 @@
    1801dbd64:	rex.W
    1801dbd65:	rex.WR push %rax
    1801dbd67:	push   %r8
    1801dbd69:	rex.WB
    1801dbd6a:	cs rex.R
    1801dbd6c:	rex.WR
    1801dbd6d:	rex.WR add %r8b,(%rax)
-   1801dbd70:	roll   %cl,(%rdx)
-   1801dbd72:	(bad)
+   1801dbd70:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   1801dbd71:	add    (%rdi),%bh
    1801dbd73:	movsxd 0x70(%rdi),%ebp
    1801dbd76:	jns    0x1801dbdd7
    1801dbd78:	jb     0x1801dbddf
    1801dbd7a:	insb   (%dx),%es:(%rdi)
    1801dbd7b:	(bad)
    1801dbd7c:	je     0x1801dbde7
    1801dbd7e:	outsl  %ds:(%rsi),(%dx)
@@ -642791,16 +642789,16 @@
    1801dbdf2:	je     0x1801dbe5d
    1801dbdf4:	outsl  %ds:(%rsi),(%dx)
    1801dbdf5:	outsb  %ds:(%rsi),(%dx)
    1801dbdf6:	jae    0x1801dbe60
    1801dbdf8:	imul   $0x40403240,0x73(%rax),%esi
    1801dbdff:	pop    %rdx
    1801dbe00:	add    %al,(%rax)
-   1801dbe02:	mov    %eax,(%rcx)
-   1801dbe04:	(bad)
+   1801dbe02:	pop    %rbp
+   1801dbe03:	add    %edi,(%rdi)
    1801dbe05:	(bad)
    1801dbe06:	xor    %eax,0x52(%rdx)
    1801dbe09:	gs jo  0x1801dbe4c
    1801dbe0c:	outsl  %gs:(%esi),(%dx)
    1801dbe0f:	fs gs rex
    1801dbe12:	rex push %rcx
    1801dbe14:	rex.RB
```

## Comparing `Geode_SimplexGeosciences-2.0.1.dist-info/METADATA` & `Geode_SimplexGeosciences-2.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Geode-SimplexGeosciences
-Version: 2.0.1
+Version: 2.0.2
 Summary: Geosciences simplex remeshing Geode-solutions OpenGeode module
 Home-page: https://github.com/Geode-solutions/Geode-SimplexGeosciences
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Geode-SimplexGeosciences Version: 2.0.1 Summary:
+Metadata-Version: 2.1 Name: Geode-SimplexGeosciences Version: 2.0.2 Summary:
 Geosciences simplex remeshing Geode-solutions OpenGeode module Home-page:
 https://github.com/Geode-solutions/Geode-SimplexGeosciences Author: Geode-
 solutions Author-email: contact@geode-solutions.com License: Proprietary
 Platform: UNKNOWN Description-Content-Type: text/markdown Requires-Dist: geode-
 common (==25.*,>=25.0.0) Requires-Dist: geode-numerics (==3.*,>=3.0.0)
 Requires-Dist: geode-simplex (==6.*,>=6.0.1) Requires-Dist: opengeode-core
 (==14.*,>=14.0.0) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.0)
```

## Comparing `Geode_SimplexGeosciences-2.0.1.dist-info/RECORD` & `Geode_SimplexGeosciences-2.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 geode_simplexgeosciences/__init__.py,sha256=9Xfy1rpJuIS2R_cfuk994vKEKycGjnMfO2gksAOUo00,212
 geode_simplexgeosciences/cross_section.py,sha256=iDB6FabUvuIeMb0Iz-MCZCIJ6kKumhhC88Man2GZ1SY,261
 geode_simplexgeosciences/structural_model.py,sha256=3BXiqsIwvfscpzxGP-Mi5oMzw15AcWoo_lwKC_hgwcE,267
-geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll,sha256=xEn_3LwZs3KGgk12E1qdw00V48Ycnl3HM2KqtPAcZsk,2039296
-geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll,sha256=Xf8GYVd4VvglxkkLoxHyF_Npq3CcTM5VbMt-EN11Zgg,2039296
-geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd,sha256=wWkc8Wxgj34RdWXvAzXw5atbkXa477Vg6DEdmFkmEYU,137216
-geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd,sha256=H0DsaHxXMNdhiIteeYViJbJMp4YrtzjA9xuqHJV2l9M,137216
-Geode_SimplexGeosciences-2.0.1.dist-info/METADATA,sha256=gS-aYS3CttsGpxPryyUGC-K795JljCvARwyA2KU6RVs,3330
-Geode_SimplexGeosciences-2.0.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_SimplexGeosciences-2.0.1.dist-info/top_level.txt,sha256=2n7r8_YGfMeW_LYPqU_ijrPfdfp4XwWFxWWYhLvzJDU,25
-Geode_SimplexGeosciences-2.0.1.dist-info/RECORD,,
+geode_simplexgeosciences/bin/Geode-SimplexGeosciences_cross_section.dll,sha256=jK-c61RlZYGa5tUQKdhBcAlSYsdQ-rQSlpD9F6iPXys,2039296
+geode_simplexgeosciences/bin/Geode-SimplexGeosciences_structural_model.dll,sha256=fU0O6-ajcV01pea8FY4EJ-nbale3f5ZpOK1GSKEtR9w,2039296
+geode_simplexgeosciences/bin/geode_simplexgeosciences_py_cross_section.cp39-win_amd64.pyd,sha256=IBpp-MzaNhCYOT0P7mZ1J1PEtABGOv87CGj1keGV1kE,137216
+geode_simplexgeosciences/bin/geode_simplexgeosciences_py_structural_model.cp39-win_amd64.pyd,sha256=ZsEfiszePEISntfKMe7_hRHfoFjStomxggdB0CjFcHM,137216
+Geode_SimplexGeosciences-2.0.2.dist-info/METADATA,sha256=6dosaq03plu7M19XhhnEyWLbpUgPcSqc90NSC9uNvzY,3330
+Geode_SimplexGeosciences-2.0.2.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_SimplexGeosciences-2.0.2.dist-info/top_level.txt,sha256=2n7r8_YGfMeW_LYPqU_ijrPfdfp4XwWFxWWYhLvzJDU,25
+Geode_SimplexGeosciences-2.0.2.dist-info/RECORD,,
```

