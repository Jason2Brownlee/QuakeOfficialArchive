# Quake Tools History

History of the Quake modding tools (e.g. map tools, etc.)


Releases:

* 1996 May 19, QuakeEd.tar.gz and QuakeEd.txt
* 1996 Jun 27, qbsp.tar.gz and qbsp.txt
* 1996 Jul 02, qutils.tar.gz and qutils.txt
* 1996 Jul 25, qcc.tar.gz, qcc.zip, qcc.txt, qbsp_29.tar.gz, qbsp_29.txt
* 1996 Sep 13, qutils.zip, qutils.txt
* 1997 Mar 14, Scourge of Armagon
* 2000 May 09, q1tools_gpl.tgz


## QuakeEd.tar.gz

Released as `QuakeEd.tar.gz`.

Announcements:

```text
QuakeEd source released

Frans P. de Vries
19 May 1996

John Carmack released the current source of QuakeEd, id's map editor:
ftp://ftp.idsoftware.com/idstuff/source/QuakeEd.tar.gz
ftp://ftp.cdrom.com/pub/idgames/source/QuakeEd.tar.gz (& mirrors)
Here is the .txt file (lines wrapped for readibility):


5/18/96

This is a dump of the current source code for QuakeEd, our map editing
application.

This does not include everything necessary to build maps. There are
graphics files, prog files, and other utilities needed. I plan on
releasing a full development set of tools after the game ships. This is
just intended to help out anyone working on their own map editor.

This is a NEXTSTEP application, so hardly anyone is going to be able to
use the code as is. This is not an OPENSTEP application. It doesn't even
use the foundation kit, so porting to gnustep or openstep-solaris/mach/nt
would not be trivial.

There are lots of mixed case and >8 character filenames, so I'm using unix
gnutar (compressed) format.

Because most people won't have access to a NEXTSTEP machine, I took
pictures of some of the more important stuff from interface builder:

mainwindow.tiff : a screenshot of the primary window
inspectors.tiff : a screenshot of the important inspector views
help.txt : a dump of the (minimal) help inspector's contents.

I included some sample data to help you follow the code:

quake.qpr : our current project file
jrbase1.map : a sample map
triggers.qc : a sample qc source file that includes some /*QUAKED comments

There will not be any major changes to this code base. I am eagerly
looking forward to writing a brand new editor for windows NT + open GL as
soon as Quake ships.

This application was really not a very good fit for NEXTSTEP. The display
postscript model fundamentally doesn't fit very well with what we need
here -- if you run in an 8 bit color mode, the line drawing runs at an ok
speed, but the texture view goes half the speed it should as it dithers
from 24 bit color down to 8 bit. If you run in 24 bit color mode, you get
less screen real estate and significantly slower line drawing as a 3
megabyte XY view is flushed. Sigh. If anyone does actually run this on
NEXTSTEP be advised that you want a fast machine. I never had the time to
properly optimize QuakeEd.

The texture view rendering code in here is crap. Anyone coding a new
editor is strongly advised to just use an available optimized library,
like open GL or direct 3D.


John Carmack
Id Software
jo...@idsoftware.com


--
Frans P. de Vries | f...@ftp.cdrom.com | Doom/Quake archive backup maintainer
```

-- [rec.games.computer.quake.editing](https://groups.google.com/g/rec.games.computer.quake.editing/c/VlriJfH2cOM/m/P0YYJtBQJ-sJ)

```text
James E Rowland
19 May 1996

Anyone interested in writing a Quake editor will want to download the
current source code for QuakeEd which appeared on id's ftp server today.
It's URL is:
ftp://ftp.idsoftware.com/idstuff/source/QuakeEd.tar.gz

The file's 385K in size. There's also a short (2K) text file by John
Carmack about the problems with porting QuakeEd from the NeXT API, etc.
and what's missing from the source. An example of QuakeC is included and
is well worth reading if you're interested in designing levels for Quake.
A map file (level geometry before bsp build) is also in there. It seems
to be all integer numbers... clever.

--
James Rowland - d1m
http://www.fen.bris.ac.uk/students/jr4854/
```

-- [rec.games.computer.quake.editing](https://groups.google.com/g/rec.games.computer.quake.editing/c/ybQY8mPuLks/m/EJpniKGqtc0J)


```text
==May 19==10:55a.m. CST
The source code for most of QuakeEd has been released in Nextstep format by John Carmack. Read about it here. He mentions creating an NT OpenGL editor after Quake ships. I hope they release that one. NT Rules! You can get it from ftp.idsoftware.com in the /idstuff/source directory.
```

-- [http://redwood.stomped.com/596.html](https://web.archive.org/web/19980511171437/http://redwood.stomped.com/596.html) (archived)

Links:

* http://redwood.stomped.com/quake/quakeed.html
* ftp://ftp.idsoftware.com/idstuff/source


Archive content:

```text
     949 19 May  1996 Brush.h
    1088 19 May  1996 CameraView.h
   16334 19 May  1996 CameraView.m
     301 19 May  1996 Clipper.h
    3234 19 May  1996 Clipper.m
    1037 19 May  1996 Dict.h
    8403 19 May  1996 Dict.m
     165 19 May  1996 DictList.h
     914 19 May  1996 DictList.m
     256 19 May  1996 DownArrow.tiff
     128 19 May  1996 English.lproj
     653 19 May  1996 Entity.h
    8192 19 May  1996 Entity.m
     717 19 May  1996 EntityClass.h
    3975 19 May  1996 EntityClass.m
    1627 19 May  1996 InspectorControl.h
    2971 19 May  1996 InspectorControl.m
     164 19 May  1996 KeypairView.h
    1444 19 May  1996 KeypairView.m
    1704 19 May  1996 Makefile
    4954 19 May  1996 Makefile.postamble
    4426 19 May  1996 Makefile.preamble
    1269 19 May  1996 Map.h
   18963 19 May  1996 Map.m
     118 19 May  1996 PB.gdbinit
    1338 19 May  1996 PB.project
     168 19 May  1996 PopScrollView.h
    1521 19 May  1996 PopScrollView.m
    1881 19 May  1996 Preferences.h
    5725 19 May  1996 Preferences.m
    3142 19 May  1996 Project.h
    8882 19 May  1996 Project.m
    1706 19 May  1996 QuakeEd.h
      48 19 May  1996 QuakeEd.iconheader
   17880 19 May  1996 QuakeEd.m
     327 19 May  1996 QuakeEd_main.m
    2692 19 May  1996 SetBrush.h
   36164 19 May  1996 SetBrush.m
    1807 19 May  1996 TexturePalette.h
   14896 19 May  1996 TexturePalette.m
     109 19 May  1996 TextureView.h
    2664 19 May  1996 TextureView.m
     615 19 May  1996 Things.h
    5748 19 May  1996 Things.m
     258 19 May  1996 UpArrow.tiff
    2981 19 May  1996 UserPath.h
    5334 19 May  1996 UserPath.m
    1132 19 May  1996 XYView.h
   25320 19 May  1996 XYView.m
     145 19 May  1996 ZScrollView.h
     950 19 May  1996 ZScrollView.m
     677 19 May  1996 ZView.h
   15382 19 May  1996 ZView.m
    8202 19 May  1996 cmdlib.c
    1460 19 May  1996 cmdlib.h
    6799 19 May  1996 help.txt
    1346 19 May  1996 i_90d.tiff
    1346 19 May  1996 i_add.tiff
    1346 19 May  1996 i_brushes.tiff
    1346 19 May  1996 i_fliph.tiff
    1346 19 May  1996 i_flipv.tiff
   29799 19 May  1996 i_quakeed.tiff
    1346 19 May  1996 i_sub.tiff
  231654 19 May  1996 inspectors.tiff
  671282 19 May  1996 jrbase1.map
   45188 19 May  1996 mainwindow.tiff
    1523 19 May  1996 mathlib.c
     902 19 May  1996 mathlib.h
    4163 19 May  1996 misc.m
    1213 19 May  1996 qedefs.h
    1102 19 May  1996 quake.qpr
    2232 19 May  1996 readme.txt
     316 19 May  1996 render.h
   12553 19 May  1996 render.m
    1346 19 May  1996 short.tiff
    1346 19 May  1996 tall.tiff
   15727 19 May  1996 triggers.qc
```

Tree:

```text
.
├── Brush.h
├── CameraView.h
├── CameraView.m
├── Clipper.h
├── Clipper.m
├── Dict.h
├── Dict.m
├── DictList.h
├── DictList.m
├── DownArrow.tiff
├── English.lproj
│   ├── Info.nib
│   │   ├── data.classes
│   │   └── data.nib
│   └── QuakeEd.nib
│       ├── data.classes
│       └── data.nib
├── Entity.h
├── Entity.m
├── EntityClass.h
├── EntityClass.m
├── InspectorControl.h
├── InspectorControl.m
├── KeypairView.h
├── KeypairView.m
├── Makefile
├── Makefile.postamble
├── Makefile.preamble
├── Map.h
├── Map.m
├── PB.gdbinit
├── PB.project
├── PopScrollView.h
├── PopScrollView.m
├── Preferences.h
├── Preferences.m
├── Project.h
├── Project.m
├── QuakeEd.h
├── QuakeEd.iconheader
├── QuakeEd.m
├── QuakeEd_main.m
├── SetBrush.h
├── SetBrush.m
├── TexturePalette.h
├── TexturePalette.m
├── TextureView.h
├── TextureView.m
├── Things.h
├── Things.m
├── UpArrow.tiff
├── UserPath.h
├── UserPath.m
├── XYView.h
├── XYView.m
├── ZScrollView.h
├── ZScrollView.m
├── ZView.h
├── ZView.m
├── cmdlib.c
├── cmdlib.h
├── help.txt
├── i_90d.tiff
├── i_add.tiff
├── i_brushes.tiff
├── i_fliph.tiff
├── i_flipv.tiff
├── i_quakeed.tiff
├── i_sub.tiff
├── inspectors.tiff
├── jrbase1.map
├── mainwindow.tiff
├── mathlib.c
├── mathlib.h
├── misc.m
├── qedefs.h
├── quake.qpr
├── readme.txt
├── render.h
├── render.m
├── short.tiff
├── tall.tiff
└── triggers.qc
```

Readme snippet:

```text
5/18/96

This is a dump of the current source code for QuakeEd, our map editing application.

This does not include everything necessary to build maps.  There are graphics files, prog files, and other utilities needed.  I plan on releasing a full development set of tools after the game ships.  This is just intended to help out anyone working on their own map editor.

This is a NEXTSTEP application, so hardly anyone is going to be able to use the code as is.  This is not an OPENSTEP application.  It doesn't even use the foundation kit, so porting to gnustep or openstep-solaris/mach/nt would not be trivial.
...
```

-- readme.txt

Locations:

* http://ftp.mancubus.net/pub/idgames2/idstuff/source/QuakeEd.tar.gz
* http://gamers.org/pub/3dgamers/00archives/doom2/addons/idstuff/source/QuakeEd.tar.gz
* http://gamers.org/pub/games/idgames/idstuff/source/QuakeEd.tar.gz
* http://reality.sgi.com/rae_aw/quake/dev/QuakeEd.tar.gz
* http://reality.sgi.com/rae_aw/quake/dev/QuakeEd.tar.gz
* http://www.gamers.org/pub/games/idgames/idstuff/source/QuakeEd.tar.gz
* http://www.gamers.org/pub/games/idgames2/idstuff/source/QuakeEd.tar.gz
* http://www.gamers.org/pub/idgames/idstuff/source/QuakeEd.tar.gz
* http://www.gamers.org/pub/idgames2/idstuff/source/QuakeEd.tar.gz
* http://www.gamesmania.com/english/../common/quake/quakeed_tar.gz
* http://www.gamesmania.com/german/../common/quake/quakeed_tar.gz
* http://www.gamesmania.com/italian/../common/quake/quakeed_tar.gz
* http://www.gamesmania.com/japanese/common/quake/quakeed_tar.gz
* http://www.idsoftware.com/ftp/source/QuakeEd.tar.gz
* https://www.quaddicted.com/files/idgames/idstuff/source/QuakeEd.tar.gz
* https://www.quaddicted.com/files/idgames2/idstuff/source/QuakeEd.tar.gz


## qbsp.tar.gz

Released as `qbsp.tar.gz`.

Announcements:

```text
==June 26== 4:30p.m. CDT

The qbsp/vis and light source for Quake (three utilities that a .map file passes through) is out on ftp://ftp.idsoftware.com/idstuff/source/qbsp.tar.gz or on the mirror sites soon. John Carmack says it has been compiled on digital unix, irix, and NT and should be easily portable to any environment. He adds that the NT version has not been well tested yet. This will allow the creation of add-on Quake levels. :)
```

-- [http://redwood.stomped.com/696.html](https://web.archive.org/web/20011122032321/http://redwood.stomped.com/696.html)

Links:

* ftp://ftp.idsoftware.com/idstuff/source/qbsp.tar.gz


```text
###############################################################################
#
# -- DIR, 27-Jun-1996
# dir /mirrors/idsoft/idstuff/source

#
# -- 385k, 27-Jun-1996
get /mirrors/idsoft/idstuff/source/qbsp.tar.gz

#
# -- 5.0k, 27-Jun-1996
read /mirrors/idsoft/idstuff/source/qbsp.txt
```

-- [relcom.games](https://groups.google.com/g/relcom.games/c/vz_KbGRbtQ4/m/vtAEvnIcWogJ)


Archive content:

```text
   16779 27 Jun  1996 brush.c
    7410 27 Jun  1996 bsp5.h
    9489 27 Jun  1996 bspfile.c
    5230 27 Jun  1996 bspfile.h
     453 27 Jun  1996 bspinfo.c
    8436 27 Jun  1996 cmdlib.c
    1651 27 Jun  1996 cmdlib.h
    8757 27 Jun  1996 csg4.c
  547656 27 Jun  1996 dm1.bsp
   86732 27 Jun  1996 dm1.h1
   57419 27 Jun  1996 dm1.h2
  266217 27 Jun  1996 dm1.map
   84567 27 Jun  1996 dm1.prt
    6728 27 Jun  1996 draw.m
    5552 27 Jun  1996 entities.c
     694 27 Jun  1996 entities.h
    5851 27 Jun  1996 entmap.c
    9689 27 Jun  1996 flow.c
    1916 27 Jun  1996 light.c
     749 27 Jun  1996 light.h
   11617 27 Jun  1996 ltface.c
     944 27 Jun  1996 makefile_alpha
    1785 27 Jun  1996 makefile_irix
    1049 27 Jun  1996 makefile_next
     958 27 Jun  1996 makefile_nt
   10097 27 Jun  1996 map.c
     949 27 Jun  1996 map.h
    1711 27 Jun  1996 mathlib.c
    1113 27 Jun  1996 mathlib.h
    5267 27 Jun  1996 merge.c
     486 27 Jun  1996 nodraw.c
    4798 27 Jun  1996 outside.c
   11442 27 Jun  1996 portals.c
   19864 27 Jun  1996 qbsp.c
    5156 27 Jun  1996 readme.txt
    9061 27 Jun  1996 region.c
   13609 27 Jun  1996 solidbsp.c
    2767 27 Jun  1996 soundpvs.c
   10801 27 Jun  1996 surfaces.c
    1343 27 Jun  1996 threads.c
     333 27 Jun  1996 threads.h
    9149 27 Jun  1996 tjunc.c
    3567 27 Jun  1996 trace.c
   18456 27 Jun  1996 vis.c
    2341 27 Jun  1996 vis.h
    9507 27 Jun  1996 writebsp.c
```

Readme snippet:

```text
This is the source for the three utilties that a .map file passes through before it becomes a finished .bsp file.  I went through 28 iterations of the output format, and eight major rewrites of the code during the development, so there are probably a few code skeletons lying around.

I have compiled this code on nextstep, digital unix, irix, and nt, so it should be easily portable to any environment you choose.  The digital unix version is multi-threaded to run on SMP systems.  The NT version has not been tested very well.
...
```

-- readme.txt

Locations:

* ftp://ftp.idsoftware.com/idstuff/source/qbsp.tar.gz
* http://reality.sgi.com/rae/quake/idfiles/qbsp.tar.gz
* http://reality.sgi.com/rae_aw/quake/idfiles/qbsp.tar.gz
* http://www.gamesmania.com/english/../common/quake/qbsp_tar.gz
* http://www.gamesmania.com/german/../common/quake/qbsp_tar.gz
* http://www.gamesmania.com/italian/../common/quake/qbsp_tar.gz
* http://www.gamesmania.com/japanese/common/quake/qbsp_tar.gz

## qutils.tar.gz

Released as `qutils.tar.gz`.

Announcements:


```text
==July 2== 11:00p.m. CDT

8:30a.m.
id has released more Quake utils on their ftp site in /idstuff/source/qutils.tar.gz. Read the text file here. Those trying to reach Stomped, try ns.stomped.com.
```

-- [http://redwood.stomped.com/796.html](https://web.archive.org/web/20011125205804/http://redwood.stomped.com/796.html) (archived)

Links:

* ftp://ftp.idsoftware.com/idstuff/source/qutils.tar.gz
* http://redwood.stomped.com/quake/qutils.txt
* http://ns.stomped.com/

```text
...
7/2 id released more source code for their editing utilities. You can get the
source here as qutils.tar.gz or qutils.zip, but I personally am waiting on the
full editors to come out.
...

-- [fido7.game.doom](https://groups.google.com/g/fido7.game.doom/c/-RwtQ-1o3lk/m/KSikAEq9Bl8J)


```text
###############################################################################
#
# -- DIR, 04-Jul-1996
# dir /mirrors/idsoft/tonsmore/idstuff/source

#
# -- 29k, 02-Jul-1996
get /mirrors/idsoft/tonsmore/idstuff/source/qutils.tar.gz

#
# -- 1.2k, 02-Jul-1996
read /mirrors/idsoft/tonsmore/idstuff/source/qutils.txt
```

-- [relcom.games](https://groups.google.com/g/relcom.games/c/WqbJHOyIAYw/m/cMhxZGhRi6oJ)

Archive content:


```text
    5565  2 Jul  1996 anorms.h
    8288  2 Jul  1996 cmdlib.c
    1548  2 Jul  1996 cmdlib.h
    2074  2 Jul  1996 dirpack.c
    1623  2 Jul  1996 fatso.c
   10031  2 Jul  1996 lbmlib.c
     651  2 Jul  1996 lbmlib.h
    1196  2 Jul  1996 makefile
    2516  2 Jul  1996 mathlib.c
    1011  2 Jul  1996 mathlib.h
   24669  2 Jul  1996 modelgen.c
    2282  2 Jul  1996 modelgen.h
    1345  2 Jul  1996 pakpatch.c
    4832  2 Jul  1996 qlumpy.c
     313  2 Jul  1996 qlumpy.h
    8692  2 Jul  1996 quakegrb.c
    1326  2 Jul  1996 readme.txt
    2896  2 Jul  1996 scriplib.c
     368  2 Jul  1996 scriplib.h
    9900  2 Jul  1996 sprgen.c
    2016  2 Jul  1996 spritegn.h
    7447  2 Jul  1996 texmake.c
    3857  2 Jul  1996 trilib.c
     283  2 Jul  1996 trilib.h
    2403  2 Jul  1996 unpack.c
    5543  2 Jul  1996 wadlib.c
    1089  2 Jul  1996 wadlib.h
```

Readme snippet:

```text
Here are the miscellaneous utilities from quake:

dirpack:  This collapses a directory hierarchy into a pak file.  We don't really use this anymore after the functionality was built into qcc.

unpack:  Unpacks a pak file into a directory tree.  I don't think I ever used this, so I'm not even sure it works.  Trivial code, in any case.

qlumpy: Grabs graphics off of lbm screens.  Has the colormap calculation code and the error-diffused mip map generation code.  It generates either individual files, or a combined wad file (barely used at all in Quake now).

texmake:  Takes an alias/wavefront .tri file and generates a wireframe outline on an lbm page for artists to draw in.

modelgen: Takes a directory of alias/wavefront .tri files for all of the animations of a character, combines with one or more skins colored over texmake frames, and outputs a .mdl file.  Modelgen parses the same source as qcc, so frame indexes keep their symbolic names when compiled into prog code.

sprgen: Grabs sprite data.  We coded lots of ways for sprites to behave (allways perpendicular, pivot along Z to face origin, pivot on Z to be parallel to view plane, fixed orientation), but we wound up only having three sprites in the entire game:  explosions, drowning bubble, and a gold ball light in the registered version....

John Carmack
```

-- readme.txt

Locations:

* ftp://ftp.idsoftware.com/idstuff/source/qutils.tar.gz
* http://reality.sgi.com/rae/quake/idfiles/qutils.tar.gz
* http://reality.sgi.com/rae_aw/quake/idfiles/qutils.tar.gz


## qcc.tar.gz

Released as `qcc.tar.gz`.

Announcements:

```text
July 25th
Quake C Released
True to their word, hot on the heels of releasing the registered Quake, id has also released the Quake C source and compiler. They can be downloaded from id's FTP Site. For you literate types, here's the text file (qcc.txt).
```

-- https://www.bluesnews.com/archives/july96.html

Links:

* ftp://206.86.8.31/idstuff/source/
* https://www.bluesnews.com/archives/qcc.txt



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

-- [rec.games.computer.quake.misc](https://groups.google.com/g/rec.games.computer.quake.misc/c/m_SOUEe39Mo/m/_dbg7CDn_HAJ)


```text
7-25-96, Thursday, 8:30PM EST

...

The Quake C compiler has been released by id. You can get the tar/gzipped source from id's FTP site, and this even includes a DOS executable. This stuff looks complicated, but extremely powerful.
```

-- [http://www.canvasnet.com/quake/old/july.htm](https://web.archive.org/web/20010719125231/http://www.canvasnet.com/quake/old/july.htm)

Links:

* ftp://ftp.idsoftware.com/idstuff/source/qcc.tar.gz


Archive content:

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

Tree:

```text
.
├── builtin.c
├── cmdlib.c
├── cmdlib.h
├── cwsdpmi.exe
├── makefile
├── pr_comp.c
├── pr_comp.h
├── pr_lex.c
├── progdefs.h
├── qcc.c
├── qcc.h
├── qccdos.exe
├── readme.txt
└── v101qc
    ├── ai.qc
    ├── amtest.qc
    ├── boss.qc
    ├── buttons.qc
    ├── client.qc
    ├── combat.qc
    ├── defs.qc
    ├── demon.qc
    ├── dog.qc
    ├── doors.qc
    ├── enforcer.qc
    ├── fight.qc
    ├── fish.qc
    ├── hknight.qc
    ├── items.qc
    ├── jctest.qc
    ├── knight.qc
    ├── misc.qc
    ├── models.qc
    ├── monsters.qc
    ├── ogre.qc
    ├── oldone.qc
    ├── plats.qc
    ├── player.qc
    ├── progs.src
    ├── shalrath.qc
    ├── shambler.qc
    ├── soldier.qc
    ├── sprites.qc
    ├── subs.qc
    ├── tarbaby.qc
    ├── triggers.qc
    ├── weapons.qc
    ├── wizard.qc
    ├── world.qc
    └── zombie.qc
```

Readme snippet:

```text
This is the last major component of the quake utilities to be released.  To be honest, I have been a little reticent to release this because most of the actual qc code is basically rather embarassing crap.  The time never became available to even give it a good top to bottom going over.  I never spent any quality engineering time on my parts, American wrote a lot of qc code, and even Romero has a bit of work in there.  It is a mess.  If you look through the code and occasionally think "This is stupid!", you are probably right...
...
```

-- readme.txt


Locations

* ftp://ftp.idsoftware.com/idstuff/source/qcc.tar.gz
* http://darkskye.home.mindspring.com/files/qcc.tar.gz
* http://ftp.mancubus.net/pub/idgames2/idstuff/source/qcc.tar.gz
* http://gamers.org/pub/3dgamers/00archives/doom2/addons/idstuff/source/qcc.tar.gz
* http://gamers.org/pub/games/idgames/idstuff/source/qcc.tar.gz
* http://public.planetmirror.com/pub/idgames2/quakec/utils/qcc.tar.gz
* http://reality.sgi.com/rae/quake/idfiles/qcc.tar.gz
* http://reality.sgi.com/rae_aw/quake/idfiles/qcc.tar.gz
* http://www.bluesnews.com/files/qcc_tar.gz
* http://www.gamers.org/pub/games/idgames/idstuff/source/qcc.tar.gz
* http://www.gamers.org/pub/games/idgames2/idstuff/source/qcc.tar.gz
* http://www.gamers.org/pub/games/idgames2/quakec/utils/qcc.tar.gz
* http://www.gamers.org/pub/games/idgames2/utils/quakec/qcc.tar.gz
* http://www.gamers.org/pub/idgames/idstuff/source/qcc.tar.gz
* http://www.gamers.org/pub/idgames2/idstuff/source/qcc.tar.gz
* http://www.gamers.org/pub/idgames2/quakec/utils/qcc.tar.gz
* http://www.gamers.org/pub/idgames2/utils/quakec/qcc.tar.gz
* http://www.gamesmania.com/english/../common/quake/qcc_tar.gz
* http://www.gamesmania.com/german/../common/quake/qcc_tar.gz
* http://www.gamesmania.com/italian/../common/quake/qcc_tar.gz
* http://www.gamesmania.com/japanese/common/quake/qcc_tar.gz
* http://www.idsoftware.com/ftp/source/qcc.tar.gz
* https://www.quaddicted.com/files/idgames/idstuff/source/qcc.tar.gz
* https://www.quaddicted.com/files/idgames2/idstuff/source/qcc.tar.gz
* https://www.quaddicted.com/files/idgames2/quakec/utils/qcc.tar.gz
* https://www.quaddicted.com/files/idgames2/utils/quakec/qcc.tar.gz
* https://www.quaddicted.com/files/tools/idgames2_utils/quakec/qcc.tar.gz


## qbsp_29.tar.gz

Released as `qbsp_29.tar.gz`, at the same time as the above `qcc.tar.gz`.

Announcements:

```text
###############################################################################
#
# -- DIR, 26-Jul-1996
# dir /mirrors/idsoft/idstuff/source

#
# -- 386k, 26-Jul-1996
get /mirrors/idsoft/idstuff/source/qbsp_29.tar.gz

#
# -- 5.3k, 26-Jul-1996
read /mirrors/idsoft/idstuff/source/qbsp_29.txt

#
# -- 199k, 26-Jul-1996
get /mirrors/idsoft/idstuff/source/qcc.tar.gz

#
# -- 3.0k, 26-Jul-1996
read /mirrors/idsoft/idstuff/source/qcc.txt
```

-- [relcom.archives](https://groups.google.com/g/relcom.archives/c/P1ML15kt8bU/m/XDS-pfsVPh4J)


Archive content:

```text
   16815 26 Jul  1996 brush.c
    7410 26 Jul  1996 bsp5.h
    9489 26 Jul  1996 bspfile.c
    5230 26 Jul  1996 bspfile.h
     453 26 Jul  1996 bspinfo.c
    8436 26 Jul  1996 cmdlib.c
    1651 26 Jul  1996 cmdlib.h
    8757 26 Jul  1996 csg4.c
  547656 27 Jun  1996 dm1.bsp
   86732 27 Jun  1996 dm1.h1
   57419 27 Jun  1996 dm1.h2
  266217 26 Jul  1996 dm1.map
   84567 27 Jun  1996 dm1.prt
    6728  9 Jul  1996 draw.m
    5552 26 Jul  1996 entities.c
     694 26 Jul  1996 entities.h
    5851 26 Jul  1996 entmap.c
    9689 26 Jul  1996 flow.c
    2029 26 Jul  1996 light.c
     775 26 Jul  1996 light.h
   11667 26 Jul  1996 ltface.c
     944 27 Jun  1996 makefile_alpha
    1785 27 Jun  1996 makefile_irix
    1049 27 Jun  1996 makefile_next
     958 27 Jun  1996 makefile_nt
   10235 26 Jul  1996 map.c
     936 26 Jul  1996 map.h
    1711 26 Jul  1996 mathlib.c
    1113 26 Jul  1996 mathlib.h
    5267 26 Jul  1996 merge.c
     486 26 Jul  1996 nodraw.c
    4798 26 Jul  1996 outside.c
   11442 26 Jul  1996 portals.c
   19864 26 Jul  1996 qbsp.c
    5451 26 Jul  1996 readme.txt
    9061 26 Jul  1996 region.c
   13609 26 Jul  1996 solidbsp.c
    2767 26 Jul  1996 soundpvs.c
   10801 26 Jul  1996 surfaces.c
    1343 26 Jul  1996 threads.c
     333 26 Jul  1996 threads.h
    9149 26 Jul  1996 tjunc.c
    3567 26 Jul  1996 trace.c
   18456 26 Jul  1996 vis.c
    2341 26 Jul  1996 vis.h
    9507 26 Jul  1996 writebsp.c
```

Readme snippet:

```text
version 29 chnages:  the lighting calculations were changed to allow the overbrighting added in quake 1.0, and some restrictions on maximum face count in qbsp were removed.  A little memory was also saved in qbsp.
...
```

-- readme.txt

Locations:

* http://reality.sgi.com/rae/quake/idfiles/qbsp_29.tar.gz
* http://reality.sgi.com/rae_aw/quake/idfiles/qbsp_29.tar.gz


## qutils.zip

Released as `qutils.zip`.

Announcements:

```text
-----------------------------------------
John Carmack's .plan for Sep 13, 1996
-----------------------------------------

...

There is new source code available. ftp://ftp.idsoftware.com//idstuff/source/qutils.zip has win-32 compiled versions and VC++ projects for all of the quake command line utilities. The qbsp/light/vis programs have not been tested all that well here, because we still use a dec alpha running unix for most of our work, but it has been converted from doubles to floats, which should reduce the memory requirements quite a bit (and possibly cause more numeric instabilities...).
...

```

-- [Johnc .plan archive](https://github.com/ESWAT/john-carmack-plan-archive/blob/master/by_year/johnc_plan_1996.txt)

```text
September 13th

Quake 1.05!
Thanks to Kristopher S Ray for dropping me a line to let me know that John Carmack updated his plan to include info on the next release of Quake!:

	"There is new source code available. ftp.idsoftware.com : /idstuff/source/qutils.zip has win-32 compiled versions and VC++ projects for all of the quake command line utilities. The qbsp/light/vis programs have not been tested all that well here, because we still use a dec alpha running unix for most of our work, but it has been converted from doubles to floats, which should reduce the memory requirements quite a bit (and possibly cause more numeric instabilities...).

	I also uploaded the DOOM ipxsetup / sersetup source code, which we haven't had on our ftp site before.

	We are going to begin internal testing of a 1.05 Quake release tomorrow. When we upload for general release, we will also upload the current .qc source. The old qcc.tar.gz file is still present on the ftp site for the original .qc files for now. "
```

-- https://www.bluesnews.com/archives/sept96-2.html

```text
==September 13== 12:40a.m. CDT

John Carmack's .plan update:

	There is new source code available. ftp.idsoftware.com : /idstuff/source/qutils.zip has win-32 compiled versions and VC++ projects for all of the quake commandline utilities.
	The qbsp/light/vis programs have not been tested all that well here, because we still use a dec alpha running unix for most of our work, but it has been convertedfrom doubles to floats, which should reduce the memory requirements quite a bit (and possibly cause more numeric instabilities...).

	I also uploaded the DOOM ipxsetup / sersetup source code, which we haven't had on our ftp site before.

	We are going to begin internal testing of a 1.05 Quake release tomorrow. When we upload for general release, we will also upload the current .qc source. The oldqcc.tar.gz file is still present on the ftp site for the original .qc files for now.

Cool...v1.05....I can't wait (I'm assuming that's a full Quake release and not just the Win32 server version).:) Get some sleep John...it's too late for work. I need sleep...I think I'm getting sick on top of everything else that's happened this week. Life's great.
```

-- [http://redwood.stomped.com/996.html](https://web.archive.org/web/20010619143518/http://redwood.stomped.com/996.html) (archived)



Archive content:

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

Tree:

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

Readme snippet:

```text

This is the readme from our most recent licensed developer CD.  Not all of it is applicable to this source upload, because the map editor, source data, and game source code have not been made freely available (gotta have some reason to charge lots of $$$ for it...), but it is the best documentation I have.

-- John Carmack




Quake Development CD 9/4/96
---------------------------

Included is all of the source data and utilities necessary to generate all of the data distributed with quake, and the main executable itself.  You can modify the data in place, or copy the data you wish to modify to an addon directory and work from there.

The win-32 tools have not been extensively tested yet, because we still do most of our work on unix.
...
```

-- README.TXT

Locations:

* ftp://ftp.idsoftware.com/idstuff/source/qutils.zip
* ftp://ftp.stomped.com/pub/redwood/idstuff/qutils.zip
* http://bluesnews.com/files/qutils.zip
* http://ftp.mancubus.net/pub/idgames2/idstuff/source/qutils.zip
* http://gamers.org/pub/3dgamers/00archives/doom2/addons/idstuff/source/qutils.zip
* http://gamers.org/pub/games/idgames/idstuff/source/qutils.zip
* http://redwood.gatsbyhouse.com/files/idstuff/qutils.zip
* http://www.bluesnews.com/files/qutils.zip
* http://www.cdrom.com/pub/idgames2/planetquake/qng/qutils.zip
* http://www.fortunecity.com/underworld/darkforces/68/qutils.zip
* http://www.gamers.org/pub/games/idgames/idstuff/source/qutils.zip
* http://www.gamers.org/pub/games/idgames2/idstuff/source/qutils.zip
* http://www.gamers.org/pub/games/idgames2/planetquake/qng/qutils.zip
* http://www.gamers.org/pub/idgames/idstuff/source/qutils.zip
* http://www.gamers.org/pub/idgames2/idstuff/source/qutils.zip
* http://www.gamers.org/pub/idgames2/planetquake/qng/qutils.zip
* http://www.gamesmania.com/common/quake/qutils.zip
* http://www.gamesmania.com/english/../common/quake/qutils.zip
* http://www.gamesmania.com/german/../common/quake/qutils.zip
* http://www.gamesmania.com/italian/../common/quake/qutils.zip
* http://www.idsoftware.com/ftp/source/qutils.zip
* http://www.visi.com/~jlowell/basebench/qutils.zip
* https://www.quaddicted.com/files/idgames/idstuff/source/qutils.zip
* https://www.quaddicted.com/files/idgames2/idstuff/source/qutils.zip
* https://www.quaddicted.com/files/idgames2/planetquake/qng/qutils.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/qng/qutils.zip



## Scourge of Armagon Tools

Released as:

* `all.zip`
* `docs.zip`
* `maps.zip`
* `newexes.zip`
* `qc.zip`
* `qcc.zip`
* `utilsrc.zip`

Announcements:

```text
March 12, 1997

More Hipnotic Quake C
The QC Source and .exe's are now up on Hipnotic's Page (Thanks Jeff McCall ). Here are the files that they are issuing as an unsupported release:

Utilsrc.zip (114 KB)	Source code for qbsp and light
Newexes.zip (93 KB)	qbsp and light
Docs.zip (8 KB)	Text files of the QC changes
Qc.zip (170 KB)	all the new .qc files
Maps.zip (222 KB)	3 .map files utilizing the new QC
All.zip (559 KB)	All 5 files in one zip
```

-- https://www.bluesnews.com/archives/march97-2.html

Links:

* https://www.bluesnews.com/files/utilsrc.zip
* https://www.bluesnews.com/files/newexes.zip
* https://www.bluesnews.com/files/docs.zip
* https://www.bluesnews.com/files/qc.zip
* https://www.bluesnews.com/files/maps.zip
* https://www.bluesnews.com/files/all.zip
* http://www.hipnotic.com/qc107.htm


Is there a need to dig into this?


## q1tools_gpl.tgz

Released as `q1tools_gpl.tgz`.

Announcements:


```text
Tuesday · May 9 · 2000

More Quake 1 source code released
JCal @  10:58 PM Your Time

id Software's John Carmack updated his .plan file with news on more source code for Quake 1:

And the Q1 utilities are now also available under the GPL in source/q1tools_gpl.tgz.

id's FTP site is located at ftp://ftp.idsoftware.com.
```

-- [http://www.stomped.com/news/arc4-2000.shtml](https://web.archive.org/web/20000816002131/http://www.stomped.com/news/arc4-2000.shtml) (archived)

Links:

* http://finger.stomped.com/users.php3?user=johnc@idsoftware.com
* ftp://ftp.idsoftware.com/

```text
5/9/00
------
And the Q1 utilities are now also available under the GPL in
source/q1tools_gpl.tgz.
```

-- [Johnc .plan archive](https://www.bluesnews.com/cgi-bin/finger.pl?id=1&time=20000509143539)

```text
Tuesday, May 09, 2000

Quake Utilities Code Released [May 09, 2000, 3:27 pm ET] – Post a Comment
id Software's John Carmack made an update to his .plan with word that he has released the source code to the Quake 1 tools under the GPL license. Here's a local copy, and while we're at it, here's a local copy of the Quake/QuakeWorld .qc files that were released yesterday (story).
```

-- https://www.bluesnews.com/s/13102/quake-utilities-code-released

Links:

* https://www.bluesnews.com/cgi-bin/finger.pl?id=1&time=20000509143539
* https://www.bluesnews.com/files/idstuff/quake/source/q1tools_gpl.shtml
* https://www.bluesnews.com/files/idstuff/quake/source/qw-qc.shtml


Archive content:

```text
   96  9 May  2000 qcc
  544  9 May  2000 qutils
```

Tree:

```text
.
├── qcc
│   └── send
│       ├── COPYING
│       ├── builtin.c
│       ├── cmdlib.c
│       ├── cmdlib.h
│       ├── cwsdpmi.exe
│       ├── makefile
│       ├── pr_comp.c
│       ├── pr_comp.h
│       ├── pr_lex.c
│       ├── progdefs.h
│       ├── qcc.c
│       ├── qcc.h
│       ├── qccdos.exe
│       ├── readme.txt
│       └── v101qc
│           ├── ai.qc
│           ├── amtest.qc
│           ├── boss.qc
│           ├── buttons.qc
│           ├── client.qc
│           ├── combat.qc
│           ├── defs.qc
│           ├── demon.qc
│           ├── dog.qc
│           ├── doors.qc
│           ├── enforcer.qc
│           ├── fight.qc
│           ├── fish.qc
│           ├── hknight.qc
│           ├── items.qc
│           ├── jctest.qc
│           ├── knight.qc
│           ├── misc.qc
│           ├── models.qc
│           ├── monsters.qc
│           ├── ogre.qc
│           ├── oldone.qc
│           ├── plats.qc
│           ├── player.qc
│           ├── progs.src
│           ├── shalrath.qc
│           ├── shambler.qc
│           ├── soldier.qc
│           ├── sprites.qc
│           ├── subs.qc
│           ├── tarbaby.qc
│           ├── triggers.qc
│           ├── weapons.qc
│           ├── wizard.qc
│           ├── world.qc
│           └── zombie.qc
└── qutils
    ├── COPYING
    ├── bin
    │   ├── bspinfo.exe
    │   ├── light.exe
    │   ├── modelgen.exe
    │   ├── qbsp.exe
    │   ├── qcc.exe
    │   ├── qfiles.exe
    │   ├── qlumpy.exe
    │   ├── sprgen.exe
    │   ├── texmake.exe
    │   └── vis.exe
    ├── bspinfo
    │   ├── bspinfo.c
    │   ├── bspinfo.mak
    │   ├── bspinfo.mdp
    │   └── bspinfo.ncb
    ├── common
    │   ├── bspfile.c
    │   ├── bspfile.h
    │   ├── cmdlib.c
    │   ├── cmdlib.h
    │   ├── lbmlib.c
    │   ├── lbmlib.h
    │   ├── mathlib.c
    │   ├── mathlib.h
    │   ├── polylib.c
    │   ├── polylib.h
    │   ├── scriplib.c
    │   ├── scriplib.h
    │   ├── threads.c
    │   ├── threads.h
    │   ├── trilib.c
    │   ├── trilib.h
    │   ├── wadlib.c
    │   └── wadlib.h
    ├── install.bat
    ├── light
    │   ├── entities.c
    │   ├── entities.h
    │   ├── light.c
    │   ├── light.h
    │   ├── light.mak
    │   ├── light.mdp
    │   ├── light.ncb
    │   ├── ltface.c
    │   ├── threads.c
    │   ├── threads.h
    │   └── trace.c
    ├── modelgen
    │   ├── anorms.h
    │   ├── modelgen.c
    │   ├── modelgen.h
    │   ├── modelgen.mak
    │   ├── modelgen.mdp
    │   └── modelgen.ncb
    ├── qbsp
    │   ├── brush.c
    │   ├── bsp5.h
    │   ├── csg4.c
    │   ├── makefile
    │   ├── map.c
    │   ├── map.h
    │   ├── merge.c
    │   ├── nodraw.c
    │   ├── outside.c
    │   ├── portals.c
    │   ├── qbsp.c
    │   ├── qbsp.mak
    │   ├── qbsp.mdp
    │   ├── qbsp.ncb
    │   ├── region.c
    │   ├── solidbsp.c
    │   ├── surfaces.c
    │   ├── tjunc.c
    │   └── writebsp.c
    ├── qcc
    │   ├── makefile
    │   ├── pr_comp.c
    │   ├── pr_comp.h
    │   ├── pr_lex.c
    │   ├── qcc
    │   ├── qcc.c
    │   ├── qcc.h
    │   ├── qcc.mak
    │   ├── qcc.mdp
    │   ├── qcc.ncb
    │   ├── qcc.pdb
    │   └── vc40.pdb
    ├── qfiles
    │   ├── qfiles.c
    │   ├── qfiles.mak
    │   ├── qfiles.mdp
    │   └── qfiles.ncb
    ├── qlumpy
    │   ├── qlumpy.c
    │   ├── qlumpy.h
    │   ├── qlumpy.mak
    │   ├── qlumpy.mdp
    │   ├── qlumpy.ncb
    │   └── quakegrb.c
    ├── readme.txt
    ├── sprgen
    │   ├── s_bubble.spr
    │   ├── s_explod.spr
    │   ├── s_light.spr
    │   ├── sprgen.c
    │   ├── sprgen.mak
    │   ├── sprgen.mdp
    │   ├── sprgen.ncb
    │   └── spritegn.h
    ├── texmake
    │   ├── texmake.c
    │   ├── texmake.mak
    │   ├── texmake.mdp
    │   └── texmake.ncb
    └── vis
        ├── flow.c
        ├── soundpvs.c
        ├── vis.c
        ├── vis.h
        ├── vis.mak
        ├── vis.mdp
        └── vis.ncb
```

Locations:

* ftp://ftp.idsoftware.com/idstuff/source/q1tools_gpl.tgz
* http://3ddownloads.com/telefragged/quake/source/q1tools_gpl.tgz
* http://ftp.mancubus.net/pub/idgames2/idstuff/source/q1tools_gpl.tgz
* http://ftp.netc.pt/pub/idgames/idstuff/source/q1tools_gpl.tgz
* http://ftp.sunet.se/pub/pc/games/idgames/idstuff/source/q1tools_gpl.tgz
* http://gamers.org/pub/games/idgames/idstuff/source/q1tools_gpl.tgz
* http://mirrors.xmission.com/idsoftware/source/q1tools_gpl.tgz
* http://public.planetmirror.com/pub/idgames/idstuff/source/q1tools_gpl.tgz
* http://sunsite.org.uk/packages/idgames/idstuff/source/q1tools_gpl.tgz
* http://sunsite.org.uk/packages/idgames2/idstuff/source/q1tools_gpl.tgz
* http://www.3ddownloads.com/telefragged/quake/source/q1tools_gpl.tgz
* http://www.gamers.org/pub/games/idgames/idstuff/source/q1tools_gpl.tgz
* http://www.gamers.org/pub/games/idgames2/idstuff/source/q1tools_gpl.tgz
* http://www.gamers.org/pub/idgames/idstuff/source/q1tools_gpl.tgz
* http://www.gamers.org/pub/idgames2/idstuff/source/q1tools_gpl.tgz
* https://www.quaddicted.com/files/idgames/idstuff/source/q1tools_gpl.tgz
* https://www.quaddicted.com/files/idgames2/idstuff/source/q1tools_gpl.tgz
* https://www.quaddicted.com/files/mirrors/ftp.telefragged.com/quake/source/q1tools_gpl.tgz




