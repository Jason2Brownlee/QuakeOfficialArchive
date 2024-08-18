# Amiga Quake History

## Releases

* QuakePPC (based on leaked src)
	* 1998 Sep 09, QuakePPC9.LhA
	* 1998 Sep 16, QuakePPC.lha
	* 1998 Sep 16, QuakePPC10.lha

## Amiga Quake Alpha aka "QuakePPC" (Leak)

A port of Quake to Amiga was made using the leaked Linux Quake v1.01 source code.

There were at least two alpha versions (e.g. one using the v1.01 source and an update with 1.06 changes).

Perhaps distributed as:

* Quake.lha
* QuakePPC.lha
* QuakePPC9.LhA
* QuakePPC10.lha


```text
Sca
5 Nov 1998

Err. i just peeked at Clickbooms site, and i said
Quote:
So called "Quake PPC" on Aminet is illegal and not coming from clickBOOM.
This idiotic move by some no-brain imbecil now made it official there will
be no Quake PPC coming from clickBOOM.
No one better even think about flaming us for this decision.
end quote:

...

Bablos
5 Nov 1998

The QuakePPC.lha archive on Paderborn Aminet isn't the real thing -
sure, the readme file might claim that it's an official patch from
ClickBOOM, but it ain't - it's just one of the FastQuake pirate
releases. It's identical to either FQ 3 or 4 - same datestamp, same
file size, even same README in the archive. Certainly no patch.


Bablos.
```
-- [comp.sys.amiga.games](https://groups.google.com/g/comp.sys.amiga.games/c/RU1Uf7dsiIc/m/zmQUcl4t4LcJ)


```
@BEGIN_FILE_ID.DIZ .________________
____Ś____ ( _____/__ - -------------
_/ ___/ _/\_ T Ź\_ ˇ diGiTAL ˇ
.-\ Ś/ 7--7 l / ˇ cORRUPTiON ˇ
| \____.-----Ś Ś----.____/------- - - -
| ŻŻŻŻŻ ŻŻŻŻŻ
| AMIGA QUAKE Alpha 0.2
| Requires CyberGFX & 8 megs
| Ported & Coded on Amiga by MAX
`----------------------------- Design: sTORM
@END_FILE_ID.DIZ

******************************************************************************
* Description *
******************************************************************************


Direct port of the original Quake v1.01 from ID Software.


******************************************************************************
* Requirements *
******************************************************************************

Amiga Computer.
68020/30/40/60 processor.
CyberGraphX graphic board with 320x200x256 screemode.
8-10 Megz of free memory.
ShareWare or Registered Quake.

******************************************************************************
* How to Use *
******************************************************************************

Smash this executable over the Quake installed directory. (You have to install
Quake shareware or Quake registered on a PC, then copy the entire Quake
directory to your Amiga).

Type in the cli or shell

stack 300000
AmigaQuake


******************************************************************************
* History *
******************************************************************************


v0.1 - First Released version.

v0.2 - Removed lottsa bugs. (too much).
- Lottsa stable version (NO MORE GURUS). (I HOPE)
- Full multitask.
- Little faster engine.
- Reduced stack requirements.
- Added CleanUp code (You can quit now!).

******************************************************************************
* To Do *
******************************************************************************


- Add Sound
- Add multiple Graphics resolutions 640x480, 800x600, etc.
- Add AGA and ECS graphics modes.
- Add v1.06 bullshit.
- ReCode whole draw, light, sprites and models routines in 100 % assembler.
- AmigaStylize.
- Add 16 and 24 Bit support.

Yepz the options are in order.
```
-- [comp.sys.amiga.games](https://groups.google.com/g/comp.sys.amiga.games/c/JaSZlQlMO9Y)


A version named `QuakePPC.lha`, content:

```text
  877320 16 Sep  1998 QuakePPC
    1260  1 Jan  1980 QuakePPC.info
    3489 11 Sep  1998 READMEPPC
     578  1 Jan  1980 READMEPPC.info
```

Readme snippet:

```text
Quake for PPC-Amiga
-------------------

You need v46 ppc.library, get it from phase5 site if you don't have it.
And of course you also need the normal Quake data files, PAK0.PAK and
PAK1.PAK. These should be in id1/ subdirectory.

...

This version is almost completely compiled with EGCS.

     - the anonymous author. :)


---
Little update history, latest additions on bottom:

-Added direct gfx card access. Quake renders directly to gfx card, no
 chunky buffer in fastram!
-Compiled with EGCS
-Removed 68k startup code, everything in ELF
-New c2p system, no more 68k render task, just PPCCallM68k()
-C2P only the modified parts of screen
-Chunky bitmap can have a modulo. This means that width doesn't need to be
 aligned to 64 pixels anymore, and direct cgx access should work with CV64.
-Rewrote render code, it's a bit faster.
-Multiplayer menu doesn't crash anymore if no networking is available.
-Minor optimizations
-Screenmode can be changed on the fly..
-Added Quake v1.06 stuff! This is entirely based on Q101-106.TXT which can
 be found from www.idsoftware.com. I included the text file in this
 release, check the modifications there. Note that there probably are some
 internal changes too which are not listed there, and thus are not present
 in my version either. However, I still decided to bump the version to 1.06. :)
```
-- READMEPPC


Locations:

* https://eab.abime.net/attachment.php?attachmentid=65013&d=1572573684
* https://mirrors.xmission.com/aminet/game/patch/QuakePPC.lha
* https://eab.abime.net/attachment.php?attachmentid=65359&d=1575015698
* https://eab.abime.net/attachment.php?attachmentid=65360&d=1575015721
* https://eab.abime.net/attachment.php?attachmentid=65361&d=1575015744

## Coolquake

Subsequent port based on leaked code?

## Fastquake

Subsequent port based on leaked code?

related?
https://aminet.net/package/game/patch/FastPatchQuake
https://web.archive.org/web/19980117191317/http://www.fragzone.se/fastquake/

## ClickBoom

The official Quake port for Amiga was created by ClickBoom.

Releases:

* binary
	* quake060.lha
* quakeplayer (demo player)
	* quakeplayer.lha
	* QuakePlayer096.lha
	* QuakeP-096code.LZX
* demos
	* quakedemos.lha



```text
Hot on the heels of Myst is Quake, the next game to receive the porting treatment from ClickBOOM. Interestingly, Quake came 2nd in the voting by Amiga users, with Monkey Island 3 coming first. But I don't mind, as I would rather see Quake.

They expect to release Amiga Quake in February 1998. This suprised me; okay, it may slip a month or two, but it is soon, considering how long it took to port Myst.
...
```
-- https://members.tripod.com/doubleclick_mag/quake.html


```text
update	Quake 060 main exe (optimized for 060 CPU)	Amiga	0.3Mb	DOWNLOAD
demo	Quake player v0.96	Amiga	6Mb	DOWNLOAD
demo	Misc. demos for Quake and QuakePlayer	Amiga	0.4Mb	DOWNLOAD
```
-- [http://www.clickboom.com/download.shtml](https://web.archive.org/web/20030808082427/http://www.clickboom.com/download.shtml)

Links:
* https://web.archive.org/web/20030808082427/http://65.95.96.20/ftp/updates/amiga/quake060.lha
* https://web.archive.org/web/20030808082427/http://65.95.96.20/ftp/demos/amiga/quakeplayer.lha
* https://web.archive.org/web/20030808082427/http://65.95.96.20/ftp/demos/amiga/quakedemos.lha








## References

* https://eab.abime.net/showthread.php?p=1411641
* http://www.oldgamesfinder.com/?m=2&q=Quake
* https://quake.fandom.com/wiki/Quake_(Amiga_version)
* https://www.amigareviews.leveluphost.com/quake1.htm
* https://www.quakeworld.nu/forum/topic/1411/16501/amiga-quake
* http://www.clickboom.com/download.shtml
* http://obligement.free.fr/articles/quake_amiga_bonne_id.php
* https://web.archive.org/web/20000422214419/http://devnull.owl.de/~frank/quake_e.html
* http://apollo-core.com/knowledge.php?b=3&note=10191&x=1&z=pt0bbx
* http://www.clickboom.com/quake/
* https://members.tripod.com/doubleclick_mag/quake.html
* https://www.pouet.net/topic.php?which=12222&page=1
* https://eab.abime.net/showthread.php?t=99433
* https://web.archive.org/web/20010119135000/http://home3.swipnet.se:80/~w-32234/ppcrulez/software/quake.html
* https://www.lemonamiga.com/games/details.php?id=2355
* https://amiga.abime.net/games/view/quake-clickboom-pxl

Later ports:

* https://aminet.net/package/game/shoot/WarpQuake
* https://aminet.net/package/game/shoot/Awinquake

