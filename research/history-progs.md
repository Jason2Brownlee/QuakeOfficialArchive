# QuakeC Source History

History of the `progs.dat` source code and QCC compiler release (i.e. release of the QuakeC code).

Excludes QuakeC for QuakeWorld.

Releases:

* 1996 Jul 25, QuakeC v1.01, qcc.tar.gz, qcc.zip, qcc.txt
* 1996 Sep 13, QuakeC v1.05, q105beta.zip, qutils.zip, qutils.txt
* 1996 Sep 30, QuakeC v1.06, progs106.zip, progs106.txt

Later related releases include:

* 1997 Mar 14, QuakeC Scourge of Armagon, all.zip, qcc.zip, qc.zip, etc.
* 1997 Apr 30, QuakeC, Dissolution of Eternity, doe_qc.zip, doe_qc.txt
* 2000 May 09, QuakeC v1.01 GPL, q1tools_gpl.tgz
* 2022 Apr 07, QuakeC Rerelease Update 3, GitHub
* 2022 Aug 19, QuakeC Rerelease Update 4, GitHub

## QuakeC v1.01

QuakeC source v1.01 for `progs.dat` was released on July 25th, 1996.

It was released as the archive files `qcc.tar.gz` and `qcc.zip` and with the readme file `qcc.txt`.

Announced on USENET:

```text
id releases QCC and updated QBSP
Frans P. de Vries
25 July 1996

John Carmack today released the Quake C compiler QCC, as well as an
updated version (v29) of QBSP:
ftp://ftp.idsoftware.com/idstuff/source/qcc.tar.gz
ftp://ftp.idsoftware.com/idstuff/source/qbsp_29.tar.gz

They have already been mirrored to the primary Quake archive:

ftp://ftp.cdrom.com/pub/idgames2/idstuff/source/qcc.tar.gz
ftp://ftp.cdrom.com/pub/idgames2/idstuff/source/qbsp_29.tar.gz

and should appear on all idgames[2] mirrors within a day or two.

QCC includes a DOS executable, the source code of the compiler, lots of
Quake C examples by way of the QC files for the monsters and various other
items, and hardly any documentation ;) Hackers, eat your heart out! :-)
--
Frans P. de Vries | f...@ftp.cdrom.com | Doom/Quake archive backup maintainer
```

-- [rec.games.computer.quake.editing](https://groups.google.com/g/rec.games.computer.quake.editing/c/m_SOUEe39Mo/m/_dbg7CDn_HAJ)


Announced on BluesNews:

```text
July 25th
Quake C Released

True to their word, hot on the heels of releasing the registered Quake, id has also released the Quake C source and compiler. They can be downloaded from id's FTP Site. For you literate types, here's the text file (qcc.txt).
```

-- https://www.bluesnews.com/archives/july96.html

Links:

* ftp://206.86.8.31/idstuff/source/
* https://www.bluesnews.com/archives/qcc.txt




This release included the source code for the QCC compiler and the source code for version 1.01 of the QuakeC game code.


> This is the last major component of the quake utilities to be released.  To be honest, I have been a little reticent to release this because most of the actual qc code is basically rather embarassing crap.  The time never became available to even give it a good top to bottom going over.  I never spent any quality engineering time on my parts, American wrote a lot of qc code, and even Romero has a bit of work in there.  It is a mess.  If you look through the code and occasionally think "This is stupid!", you are probably right...

-- qcc.txt


The content of the two archives are identical (via diff), only some timestamps differ.


The `qcc.tar.gz` archive contents:


```text
  29602 25 Jul  1996 builtin.c
   8278 25 Jul  1996 cmdlib.c
   1716 25 Jul  1996 cmdlib.h
  25870 25 Jul  1996 cwsdpmi.exe
    377 25 Jul  1996 makefile
  21751 25 Jul  1996 pr_comp.c
   2338 25 Jul  1996 pr_comp.h
  11912 25 Jul  1996 pr_lex.c
   2455 25 Jul  1996 progdefs.h
  23588 25 Jul  1996 qcc.c
  13077 25 Jul  1996 qcc.h
 155416 25 Jul  1996 qccdos.exe
   3081 25 Jul  1996 readme.txt
   1216 25 Jul  1996 v101qc
```

The `qcc.tar.gz/v101qc` directory contents:

```text
 14521 25 Jul  1996 ai.qc
  1697 25 Jul  1996 amtest.qc
 12423 25 Jul  1996 boss.qc
  2910 25 Jul  1996 buttons.qc
 32135 25 Jul  1996 client.qc
  6130 25 Jul  1996 combat.qc
 17423 25 Jul  1996 defs.qc
  9916 25 Jul  1996 demon.qc
  9554 25 Jul  1996 dog.qc
 16997 25 Jul  1996 doors.qc
 10739 25 Jul  1996 enforcer.qc
  7208 25 Jul  1996 fight.qc
  7759 25 Jul  1996 fish.qc
 18310 25 Jul  1996 hknight.qc
 27432 25 Jul  1996 items.qc
   222 25 Jul  1996 jctest.qc
  9696 25 Jul  1996 knight.qc
 15088 25 Jul  1996 misc.qc
  9788 25 Jul  1996 models.qc
  4798 25 Jul  1996 monsters.qc
 14669 25 Jul  1996 ogre.qc
  9400 25 Jul  1996 oldone.qc
  7693 25 Jul  1996 plats.qc
 17566 25 Jul  1996 player.qc
   407 25 Jul  1996 progs.src
  7892 25 Jul  1996 shalrath.qc
 12737 25 Jul  1996 shambler.qc
  9837 25 Jul  1996 soldier.qc
   486 25 Jul  1996 sprites.qc
  6062 25 Jul  1996 subs.qc
  7128 25 Jul  1996 tarbaby.qc
 14259 25 Jul  1996 triggers.qc
 24023 25 Jul  1996 weapons.qc
 10675 25 Jul  1996 wizard.qc
 11058 25 Jul  1996 world.qc
 20120 25 Jul  1996 zombie.qc
```


The `qcc.zip` archive contents:

```text
  29602 25 Jul  1996 builtin.c
   8278 24 Jul  1996 cmdlib.c
   1716 24 Jul  1996 cmdlib.h
  25870 24 Jul  1996 cwsdpmi.exe
    377 24 Jul  1996 makefile
  21751 24 Jul  1996 pr_comp.c
   2338 24 Jul  1996 pr_comp.h
  11912 24 Jul  1996 pr_lex.c
   2455 24 Jul  1996 progdefs.h
  23588 24 Jul  1996 qcc.c
  13077 24 Jul  1996 qcc.h
 155416 24 Jul  1996 qccdos.exe
   3081 25 Jul  1996 readme.txt
   1216 21 Aug  1996 v101qc
```

The `qcc.zip/v101qc` directory contents:

```text
 14521 24 Jul  1996 ai.qc
  1697 24 Jul  1996 amtest.qc
 12423 24 Jul  1996 boss.qc
  2910 24 Jul  1996 buttons.qc
 32135 24 Jul  1996 client.qc
  6130 24 Jul  1996 combat.qc
 17423 24 Jul  1996 defs.qc
  9916 24 Jul  1996 demon.qc
  9554 24 Jul  1996 dog.qc
 16997 24 Jul  1996 doors.qc
 10739 24 Jul  1996 enforcer.qc
  7208 24 Jul  1996 fight.qc
  7759 24 Jul  1996 fish.qc
 18310 24 Jul  1996 hknight.qc
 27432 24 Jul  1996 items.qc
   222 24 Jul  1996 jctest.qc
  9696 24 Jul  1996 knight.qc
 15088 24 Jul  1996 misc.qc
  9788 24 Jul  1996 models.qc
  4798 24 Jul  1996 monsters.qc
 14669 24 Jul  1996 ogre.qc
  9400 24 Jul  1996 oldone.qc
  7693 24 Jul  1996 plats.qc
 17566 24 Jul  1996 player.qc
   407 24 Jul  1996 progs.src
  7892 24 Jul  1996 shalrath.qc
 12737 24 Jul  1996 shambler.qc
  9837 24 Jul  1996 soldier.qc
   486 24 Jul  1996 sprites.qc
  6062 24 Jul  1996 subs.qc
  7128 24 Jul  1996 tarbaby.qc
 14259 24 Jul  1996 triggers.qc
 24023 24 Jul  1996 weapons.qc
 10675 24 Jul  1996 wizard.qc
 11058 24 Jul  1996 world.qc
 20120 24 Jul  1996 zombie.qc
```

## QuakeC v1.05

The next release was on September 13 1996.

This included the `q105beta.zip` that contained an updated executable, `progs.dat`, and QuakeC source code for the `progs.dat`. A fix was released the next day as `beta5a.exe`.

The release also included `qutils.zip` and `qutils.txt` with updated source code and binaries for the map tools and QCC compiler.

The release was announced in John Carmack's .plan file:

```text
-----------------------------------------
John Carmack's .plan for Sep 13, 1996
-----------------------------------------

There is a BETA distribution of 1.05 up on our ftp site.

ftp://ftp.idsoftware.com/idstuff/unsup/q105beta.exe

It includes quake.exe winded.exe progs.dat, and a zip of the latest .qc files. Back up your current version before messing with this, in case something is broken.

There is new source code available. ftp://ftp.idsoftware.com//idstuff/source/qutils.zip has win-32 compiled versions and VC++ projects for all of the quake command line utilities. The qbsp/light/vis programs have not been tested all that well here, because we still use a dec alpha running unix for most of our work, but it has been converted from doubles to floats, which should reduce the memory requirements quite a bit (and possibly cause more numeric instabilities...).

I also uploaded the DOOM ipxsetup / sersetup source code, which we haven't had on our ftp site before.

We are going to begin internal testing of a 1.05 Quake release tomorrow. When we upload for general release, we will also upload the current .qc source. The old qcc.tar.gz file is still present on the ftp site for the original .qc files for now.
```

-- [johnc .plan file archive 1996](https://github.com/ESWAT/john-carmack-plan-archive/blob/cab9497f3b22194314a29513d3d03301fbfe7521/by_year/johnc_plan_1996.txt#L560)

The game update was announced on BluesNews:

```text
September 13th

Quake 1.05 Beta Released

John Carmack abruptly released a beta version of Quake 1.05 on their FTP site. The list of what's new is in the readme. WARNING! From his plan:

	There is a BETA distribution of 1.05 up on our ftp site.
	ftp.idsoftware.com:/idstuff/unsup/q105beta.exe
	It includes quake.exe winded.exe progs.dat, and a zip of the latest .qc files.
	Back up your current version before messing with this, in case something
	is broken.
```

-- https://www.bluesnews.com/archives/sept96-2.html

Links:

* https://www.bluesnews.com/archives/qb105rm.txt
* ftp://ftp.idsoftware.com/
* ftp://ftp.idsoftware.com/idstuff/unsup/q105beta.exe


The updated utilities were announced on Redwood's Quake Page:

```text
==September 13== 12:40a.m. CDT

John Carmack's .plan update:

	There is new source code available. ftp.idsoftware.com : /idstuff/source/qutils.zip has win-32 compiled versions and VC++ projects for all of the quake commandline utilities.

	The qbsp/light/vis programs have not been tested all that well here, because we still use a dec alpha running unix for most of our work, but it has been convertedfrom doubles to floats, which should reduce the memory requirements quite a bit (and possibly cause more numeric instabilities...).
	...
```

Two day's later, Redwood announced the game update and subsequent fix:

```text
==September 15== 2:30p.m. CDT

...
Quake v1.05beta as well as a later beta5a.exe patch that fixxes the disappearing weapon bug.
...
```

Links:

* ftp://ftp.idsoftware.com/idstuff/unsup/q105beta.exe
* ftp://ftp.idsoftware.com/idstuff/unsup/beta5a.exe


The q105beta.zip archive contained `Q105BETA.EXE`, a self-expanding executable.

```text
 657403 13 Sep  1996 Q105BETA.EXE
```

The `Q105BETA.EXE` archive contained:

```text
 411704 13 Sep  1996 PROGS.DAT
 105161 13 Sep  1996 PROGSSRC.ZIP
 400384 13 Sep  1996 QUAKE.EXE
   4316 13 Sep  1996 README.TXT
 609792 13 Sep  1996 WINDED.EXE
```

Readme snippet:

```text
This is a beta release of Quake v1.05.  The full, supported release will be mid next week if there are no problems.

In addition to the new exe files, the progs.dat has also been changed.
```

-- Q105BETA.EXE/README.TXT


The archive of QuakeC source in `PROGSSRC.ZIP` contained:

```
 14521 13 Sep  1996 AI.QC
  1697 13 Sep  1996 AMTEST.QC
 12411 13 Sep  1996 BOSS.QC
  2910 13 Sep  1996 BUTTONS.QC
  6130 13 Sep  1996 COMBAT.QC
 17423 13 Sep  1996 DEFS.QC
  9904 13 Sep  1996 DEMON.QC
  9542 13 Sep  1996 DOG.QC
 17028 13 Sep  1996 DOORS.QC
 10727 13 Sep  1996 ENFORCER.QC
  7208 13 Sep  1996 FIGHT.QC
  7747 13 Sep  1996 FISH.QC
 18298 13 Sep  1996 HKNIGHT.QC
 27461 13 Sep  1996 ITEMS.QC
   222 13 Sep  1996 JCTEST.QC
  9684 13 Sep  1996 KNIGHT.QC
 15088 13 Sep  1996 MISC.QC
  8996 13 Sep  1996 MODELS.QC
  4798 13 Sep  1996 MONSTERS.QC
 14657 13 Sep  1996 OGRE.QC
  9537 13 Sep  1996 OLDONE.QC
  7693 13 Sep  1996 PLATS.QC
 17554 13 Sep  1996 PLAYER.QC
  2455 13 Sep  1996 PROGDEFS.H
   407 13 Sep  1996 PROGS.SRC
  7880 13 Sep  1996 SHALRATH.QC
 12725 13 Sep  1996 SHAMBLER.QC
  9825 13 Sep  1996 SOLDIER.QC
   450 13 Sep  1996 SPRITES.QC
  6062 13 Sep  1996 SUBS.QC
  7116 13 Sep  1996 TARBABY.QC
 14259 13 Sep  1996 TRIGGERS.QC
 25413 13 Sep  1996 WEAPONS.QC
 10663 13 Sep  1996 WIZARD.QC
 11058 13 Sep  1996 WORLD.QC
 20108 13 Sep  1996 ZOMBIE.QC
 31892 13 Sep  1996 client.qc
```


The `qutils.txt` contained:


```text
This is the latest version of all released quake utilities as of
september 13, 1996.
Each utility has a seperate directory and VC++ project file.
Be sure to pkunzip -d to get all the directories.
Precompiled versions for win32 are also included.
The .qc source files are not icluded here, you will have to get them
elsewhere.

--- John Carmack
```

The `progs.dat` contained a bug and an updated `progs.dat` was released the next day on Septeber 14 as `beta5a.exe` and `beta5a.txt`.

This was a self-extracting executable that only contained the `progs.dat` file, no QuakeC source.


The `qutils.zip` does not include the QuakeC source code.

The contents of `qutils.zip` were:


```text
.
├── BIN
│   ├── BSPINFO.EXE
│   ├── LIGHT.EXE
│   ├── MODELGEN.EXE
│   ├── QBSP.EXE
│   ├── QCC.EXE
│   ├── QFILES.EXE
│   ├── QLUMPY.EXE
│   ├── SPRGEN.EXE
│   ├── TEXMAKE.EXE
│   └── VIS.EXE
├── BSPINFO
│   ├── BSPINFO.C
│   ├── BSPINFO.MAK
│   ├── BSPINFO.MDP
│   └── BSPINFO.NCB
├── COMMON
│   ├── BSPFILE.C
│   ├── BSPFILE.H
│   ├── CMDLIB.C
│   ├── CMDLIB.H
│   ├── LBMLIB.C
│   ├── LBMLIB.H
│   ├── MATHLIB.C
│   ├── MATHLIB.H
│   ├── POLYLIB.C
│   ├── POLYLIB.H
│   ├── SCRIPLIB.C
│   ├── SCRIPLIB.H
│   ├── THREADS.C
│   ├── THREADS.H
│   ├── TRILIB.C
│   ├── TRILIB.H
│   ├── WADLIB.C
│   └── WADLIB.H
├── INSTALL.BAT
├── LIGHT
│   ├── ENTITIES.C
│   ├── ENTITIES.H
│   ├── LIGHT.C
│   ├── LIGHT.H
│   ├── LIGHT.MAK
│   ├── LIGHT.MDP
│   ├── LIGHT.NCB
│   ├── LTFACE.C
│   ├── THREADS.C
│   ├── THREADS.H
│   └── TRACE.C
├── MODELGEN
│   ├── ANORMS.H
│   ├── MODELGEN.C
│   ├── MODELGEN.H
│   ├── MODELGEN.MAK
│   ├── MODELGEN.MDP
│   └── MODELGEN.NCB
├── QBSP
│   ├── BRUSH.C
│   ├── BSP5.H
│   ├── CSG4.C
│   ├── MAKEFILE
│   ├── MAP.C
│   ├── MAP.H
│   ├── MERGE.C
│   ├── NODRAW.C
│   ├── OUTSIDE.C
│   ├── PORTALS.C
│   ├── QBSP.C
│   ├── QBSP.MAK
│   ├── QBSP.MDP
│   ├── QBSP.NCB
│   ├── REGION.C
│   ├── SOLIDBSP.C
│   ├── SURFACES.C
│   ├── TJUNC.C
│   └── WRITEBSP.C
├── QCC
│   ├── MAKEFILE
│   ├── PR_COMP.C
│   ├── PR_COMP.H
│   ├── PR_LEX.C
│   ├── QCC
│   ├── QCC.C
│   ├── QCC.H
│   ├── QCC.MAK
│   ├── QCC.MDP
│   ├── QCC.NCB
│   ├── QCC.PDB
│   └── VC40.PDB
├── QFILES
│   ├── QFILES.C
│   ├── QFILES.MAK
│   ├── QFILES.MDP
│   └── QFILES.NCB
├── QLUMPY
│   ├── QLUMPY.C
│   ├── QLUMPY.H
│   ├── QLUMPY.MAK
│   ├── QLUMPY.MDP
│   ├── QLUMPY.NCB
│   └── QUAKEGRB.C
├── README.TXT
├── SPRGEN
│   ├── SPRGEN.C
│   ├── SPRGEN.MAK
│   ├── SPRGEN.MDP
│   ├── SPRGEN.NCB
│   ├── SPRITEGN.H
│   ├── S_BUBBLE.SPR
│   ├── S_EXPLOD.SPR
│   └── S_LIGHT.SPR
├── TEXMAKE
│   ├── TEXMAKE.C
│   ├── TEXMAKE.MAK
│   ├── TEXMAKE.MDP
│   └── TEXMAKE.NCB
└── VIS
    ├── FLOW.C
    ├── SOUNDPVS.C
    ├── VIS.C
    ├── VIS.H
    ├── VIS.MAK
    ├── VIS.MDP
    └── VIS.NCB
```

The timestamps were:

```text
  384 12 Sep  1996 BIN
  192 12 Sep  1996 BSPINFO
  640 12 Sep  1996 COMMON
 1058 12 Sep  1996 INSTALL.BAT
  416 12 Sep  1996 LIGHT
  256 12 Sep  1996 MODELGEN
  672 12 Sep  1996 QBSP
  448 12 Sep  1996 QCC
  192 12 Sep  1996 QFILES
  256 12 Sep  1996 QLUMPY
 8564 12 Sep  1996 README.TXT
  320 12 Sep  1996 SPRGEN
  192 12 Sep  1996 TEXMAKE
  288 12 Sep  1996 VIS
```




## QuakeC v1.06

The next release was on October 02 as `progs106.zip` and `progs106.txt`.

The announce coincided with an updated shareware release `quake106.zip` and update patch `q101-106.zip` and an updated Windows dedicated server `qwded106.exe`.

This release was announced on USENET:

```text
() Quake v1.06 released ()
Frans P. de Vries
2 Oct 1996,

id Software just released the long-awaited version 1.06 of Quake.
The complete array of files is available:
quake106.zip full 9MB shareware release
qsw106_?.zip shareware release in 7 parts of 1.44MB
q101-106.zip upgrade patch v1.01 to v1.06 (363kB)
qwded106.exe dedicated Win32 server (217kB)
progs106.zip latest Quake-C sources and progs.dat (231kB)

from id's server and the idgames2 archive:

ftp://ftp.idsoftware.com/idstuff/quake/
ftp://ftp.cdrom.com/pub/idgames2/idstuff/quake/

and within a day or so from more than a dozen idgames2 mirrors around
the world.
--
Frans P. de Vries | f...@ftp.cdrom.com | Doom/Quake archive backup maintainer
```

-- [rec.games.computer.quake.announce](https://groups.google.com/g/rec.games.computer.quake.announce/c/tDP8TEJpxDI/m/cFP95gXVrlIJ)

The release was announced on Redwood's Quake page:

```text
==October 2== 10:30p.m. CDT
...
Uhh, since nobody I noticed seems to have noticed, QUAKE 1.06 is OUT!! Read what's changed. Get the shareware quake106.zip (9meg), or the patch q101-106.zip (355k). Don't forget about the Win32 v1.06 Server. And you thought I was getting slow in my old age. BTW, I give credit to Notify (part of Symantec's Internet Fast Find package) for keeping me young and swift. Everybody must be having a nice siesta right now. ;) What was that? You say Stomped was supposed to be first? I hate when I do that. ;)
```

-- [http://redwood.gatsbyhouse.com/quake/1096.html](https://web.archive.org/web/19970327200948/http://redwood.gatsbyhouse.com/quake/1096.html)

Links:

* http://redwood.gatsbyhouse.com/quake/quake/q101-106.txt
* ftp://ftp.idsoftware.com/idstuff/quake/quake106.zip
* ftp://ftp.idsoftware.com/idstuff/quake/q101-106.zip
* ftp://ftp.idsoftware.com/idstuff/unsup/qwded106.exe



The release was also announced on BluesNews:

```text
October 2nd
Quake 1.06 Released

Available at id's FTP site. Thanks to everyone who mailed me, the first being Ronald J Davis aka PostalWorker.
```

-- https://www.bluesnews.com/archives/sept96-5.html


The contents of the readme:

```text
Quake C progs for version 1.06
```

-- progs106.txt


The `progs106.zip` archive only contained the QuakeC source and a compiled `progs.dat` file.

```text
  14521 26 Sep  1996 ai.qc
   1697 26 Sep  1996 amtest.qc
  12411 26 Sep  1996 boss.qc
   2910 26 Sep  1996 buttons.qc
  32354 29 Sep  1996 client.qc
   6130 26 Sep  1996 combat.qc
  17423 26 Sep  1996 defs.qc
   9904 26 Sep  1996 demon.qc
   9542 26 Sep  1996 dog.qc
  17028 26 Sep  1996 doors.qc
  10727 26 Sep  1996 enforcer.qc
   7208 26 Sep  1996 fight.qc
   7747 26 Sep  1996 fish.qc
    141 26 Sep  1996 flag.qc
  18298 26 Sep  1996 hknight.qc
  29811 26 Sep  1996 items.qc
    222 26 Sep  1996 jctest.qc
   9684 26 Sep  1996 knight.qc
  15088 26 Sep  1996 misc.qc
   8996 26 Sep  1996 models.qc
   4798 26 Sep  1996 monsters.qc
  14657 26 Sep  1996 ogre.qc
   9537 26 Sep  1996 oldone.qc
   7693 26 Sep  1996 plats.qc
  17554 26 Sep  1996 player.qc
 413116 30 Sep  1996 progs.dat
    407 26 Sep  1996 progs.src
   7880 26 Sep  1996 shalrath.qc
  12725 26 Sep  1996 shambler.qc
   9825 26 Sep  1996 soldier.qc
    450 26 Sep  1996 sprites.qc
   6062 26 Sep  1996 subs.qc
   7116 26 Sep  1996 tarbaby.qc
  14259 26 Sep  1996 triggers.qc
  25227 30 Sep  1996 weapons.qc
  10663 26 Sep  1996 wizard.qc
  11058 26 Sep  1996 world.qc
  20108 26 Sep  1996 zombie.qc
```