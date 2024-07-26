Quake Utils Research
====================
Investigation into what tools/src were released, and when.

This is hard because it is July 1996, and internet archive started in this month. Most of the news sites were not captured until much later. There is scant evidence and files.


## Files

* qbsp.tar.gz
* qbsp.txt
* qbsp_29.tar.gz
* qbsp_29.txt
* qutils.tar.gz
* qutils.zip
* qutils.txt
* qcc.tar.gz
* qcc.zip
* qcc.txt


## News


map compile tools were released around the time of the retail cd (early-mid july)

people compiling maps, e.g.:


https://web.archive.org/web/19970523110440/http://web.inter.nl.net/users/L.J.Noordsij/index.html

> July 18th, 21:03 CEST
>
> After trying a lot of map editing (sorry, no editor, just a text editor) I tried if I could simulate raising and lowering water. And it worked! I've seen the topic in the newsgroups lately, and here is a working example that shows it IS possible to have a water level raise, sink. Click here to get the level. You can compile it with QBSP and LIGHT, it will only take one sec. Also, read the text file in it about why I distribute a map for the SW version (although it actually just IS a text file). Have fun, let me know if you can do something cool with it (or something else).


qcc was released at the end of july, people using it:

https://web.archive.org/web/19970523110440/http://web.inter.nl.net/users/L.J.Noordsij/index.html


> July 27th, 18:01 CEST
>
> As you can see there isn't much news added to this page anymore, well, that's because I find it too little to update every time, so I will not be focused on news a lot anymore. Right now people don't really need real NEWS pages, so I'll be focusing on other features:
> ****** QUAKEC - As you probably know Quake C was released! (Compiler plus the used .QC files) I don't have Quake registered yet, but when I visit Florida next week I'll call 1-800-idgames and hope they deliver it to the vacation address within 2 weeks :) But from what I've seen so far it is a *very* powerful language! I've already seen code that will make a missile circle around you until it hits something, and the code used by/for the weapons is all QCC too! So adding new weapons will be easy! You can also implement interconnected servers, we're working on that right now :) In r.c.g.q.e I saw a post from someone who has 1) Made the corpses SOLID, > 2) Made them last forever (that would kick ass after an hour of DM, bodies stacked everywhere :) And we could add some extra ThrowGibs('progs/gib1.mdl') (or something :) in the death scenes to have a more bloody effect! And best of all... in MP games only the CODE ON THE SERVER WILL BE USED! If you change your code so the cheats will work (very easy) and connect to a server, you will use the SERVER code, so no cheating! And if the server has new weapons, then you need to get the new .MDL files, but the CODE will be straight from the server! So if they enhance the weapon (make it smarter) you will get that code instantly. If the server removes the "if (deathmatch || coop) return" before the cheating routine (which means "STOP HERE if Coop or DM game") then all players can cheat, regardless of the code they have on their machine. So each server has it's own rules, which the server 'masters' can improve and improve withouth you requiring to have the same .QC files for every server (Duke3D?? :). Really, QuakeC is AWESOME!
****** I am now a member of a group of people that will be creating the coolest stuff (levels/qc/weapons) for you! Our artist already made a load of new textures that we can use to create a beautiful city environment, we have some new sounds and we are working on a theme for the project. Anyway, there will be (a) page(s) devoted to that, one instead of this one, and some on the other guys' ISP's. So maybe a QuakeC section here, a Level rating section 500 km from here, a Weapons section on the other side of the atlantic. Really, we've got big plans AND some amazingly cool art for those pages already. Keep watching, and enjoy Quake


## Blues News

### News

https://www.bluesnews.com/archives/july96.html

> July 5th
> Early linux version of v0.91
>
> Linux Quake Released
>Dave Taylor's eagerly awaited Linux port of Quake 0.91 (303 KB) has been released, and can be found on LEK Internet Services's FTP site.

ftp://ftp.lek.net/pub/linux/quake/

what is the filename?

id FTP site:

ftp://206.86.8.31/idstuff/quake/


> July 25th
>
> Quake C Released
> True to their word, hot on the heels of releasing the registered Quake, id has also released the Quake C source and compiler. They can be downloaded from id's FTP Site. For you literate types, here's the text file (qcc.txt).


ftp://206.86.8.31/idstuff/source/
https://www.bluesnews.com/archives/qcc.txt


### Files

https://web.archive.org/web/19970204063238fw/http://bluesnews.com/q-files.html

> Quake C Source	Go forward, be bold (qcc.txt)...	qcc.tar.gz (199 KB)

https://web.archive.org/web/19970204063238fw/http://bluesnews.com/files/qcc.txt
https://web.archive.org/web/19970204063238fw/http://bluesnews.com/files/qcc.tar.gz

> Quake Utilities	Unsupported software from id (qutils.txt)	qutils.zip (700 KB)

https://web.archive.org/web/19970204063238fw/http://bluesnews.com/files/qutils.txt
https://web.archive.org/web/19970204063238fw/http://bluesnews.com/files/qutils.zip


## Usenet

## qutils.tar.gz

27 june: bsp utils
	no confirmation elsewhere of this yet...
	no idea of what files
2 july qutils.tar.gz and qutils.zip
25 july qcc

https://groups.google.com/g/fido7.game.doom/c/-RwtQ-1o3lk/m/KSikAEq9Bl8J

> 7/25 id Software has released the Quake C Compiler (qcc), along with
accompanying source code. Although John Carmack calls it "sloppy", Quake players
will be eager to try it out for themselves. You can download it directly f rom
Stomped, or from id Software themselves. If you are a MS-DOS user and cannot
extract the archive, Download the .zip version here.

> 7/2 id released more source code for their editing utilities. You can get the
source here as qutils.tar.gz or qutils.zip, but I personally am waiting on the
full editors to come out.


> 6/27 John Carmack has released the source code for Quake's QBSP/VIS/LIGHT
routines which should now make creation of Quake maps a reality.
>
> John has included makefiles for Alpha, Irix, Next and Windows NT platforms.
Being the NT freak that I am, I have compiled all the modules into Windows NT
Executables using MSVC++ 4.0 (Except for vis.exe, I had an error in compiling
it. I will recompile it soon).
>
> Programmers Note: John Carmack was NOT kidding around when he said that they
used high-end four processor Alpha 4/275's to run QBSP. On my measly Pentium 100
with 24megs of RAM, running QBSP on dm1.map brought Windows NT to it's knees.
Forget about running QBSP and doing something else in the background. QBSP is a
PIG on system resources.



https://groups.google.com/g/nctu.ccca.mirror/c/h_TU5m7gut0/m/uD1Oeqt_MgwJ

> 30,339 /PC/games/id/id-mirror/idstuff/source/qutils.tar.gz
> 736 /PC/games/id/id-mirror/idstuff/source/qutils.txt

is this the path on id ftp and cdrom.com?



https://groups.google.com/g/relcom.archives/c/sGqPkAIlG64/m/9OTadMAzTKsJ

> ----------------------------------------------------------
> каталог /gamesdomain/idsoftware/source
> ----------------------------------------------------------
>
> QuakeEd.tar.gz 394767 May-19-1996 * -
> QuakeEd.txt 2232 May-19-1996 * -
> qbsp_29.tar.gz 395452 Jul-25-1996 * -
> qbsp_29.txt 5451 Jul-25-1996 * -
> qcc.tar.gz 204053 Jul-25-1996 * -
> qcc.txt 3081 Jul-25-1996 * -
> qutils.tar.gz 30339 Jul-1-1996 * -
> qutils.txt 1326 Jul-1-1996 * -
> wolfsrc.txt 7276 Oct-19-1995 * -
> wolfsrc.zip 576904 Oct-19-1995 * -


The first release was a txt and tar.gz perhaps
qcc was july 25 as we expect
qbsp_29.txt also released on july 25th

QuakeEd may 1996

file timestamps in modern source/ are wrong.
files must have been moved in oct 1996



https://groups.google.com/g/nctu.ccca.mirror/c/c5ZTeDaZ8tI/m/dn6A3xg259cJ


> 30,339 /PC/games/DOOM/idstuff/source/qutils.tar.gz
> 736 /PC/games/DOOM/idstuff/source/qutils.txt


https://groups.google.com/g/relcom.archives/c/2UHFQOFjbYI/m/XGkEKVooMzYJ


> #
> # -- 29k, 03-Jul-1996
> get /mirrors/idsoft/idstuff/source/qutils.tar.gz
>
> #
> # -- 1.2k, 03-Jul-1996
> read /mirrors/idsoft/idstuff/source/qutils.txt



https://groups.google.com/g/relcom.games/c/WqbJHOyIAYw/m/cMhxZGhRi6oJ

> #
> # -- 29k, 02-Jul-1996
> get /mirrors/idsoft/tonsmore/idstuff/source/qutils.tar.gz
>
> #
> # -- 1.2k, 02-Jul-1996
> read /mirrors/idsoft/tonsmore/idstuff/source/qutils.txt


Lots of confirmation of the july 02 1996 release.
No confirmation of the June 27 release...




### qutils.zip


https://groups.google.com/g/fido.ger.spiele/c/V8go2Lt31aU/m/Lg2bkgngh30J

carmack plan file


> Sept 13:
>
> There is new source code available. ftp.idsoftware.com : /idstuff/source/qutils.zip has win-32 compiled versions and VC++ projects for all of the quake command line utilities.
>
> The qbsp/light/vis programs have not been tested all that well here, because we still use a dec alpha running unix for most of our work, but it has been converted from doubles to floats, which should reduce the memory requirements quite a bit (and possibly cause more numeric instabilities...).

This date matches the final release of qutils.


https://groups.google.com/g/relcom.archives/c/LaiINsjwS5s/m/4UEQAZ_XSt4J

> #
> # -- 355, 13-Sep-1996
> read /mirrors/idsoft/idstuff/source/qutils.txt
>
> #
> # -- 700k, 13-Sep-1996
> get /mirrors/idsoft/idstuff/source/qutils.zip


looks like the .tar.gz was removed later...



https://groups.google.com/g/relcom.archives/c/OdfZraIXLHY/m/N98jNQ-kadkJ

> #
> # -- 355, 13-Sep-1996
> read /mirrors/idsoft/tonsmore/idstuff/source/qutils.txt
>
> #
> # -- 700k, 13-Sep-1996
> get /mirrors/idsoft/tonsmore/idstuff/source/qutils.zip


### qbsp_29.tar.gz


https://groups.google.com/g/rec.games.computer.quake.editing/c/m_SOUEe39Mo/m/_dbg7CDn_HAJ

> Frans P. de Vries July 25 1996
>
> John Carmack today released the Quake C compiler QCC, as well as an updated version (v29) of QBSP:
> ftp://ftp.idsoftware.com/idstuff/source/qcc.tar.gz
f> tp://ftp.idsoftware.com/idstuff/source/qbsp_29.tar.gz
>
> They have already been mirrored to the primary Quake archive:
>
> ftp://ftp.cdrom.com/pub/idgames2/idstuff/source/qcc.tar.gz
> ftp://ftp.cdrom.com/pub/idgames2/idstuff/source/qbsp_29.tar.gz
>
> and should appear on all idgames[2] mirrors within a day or two.
>
> QCC includes a DOS executable, the source code of the compiler, lots of Quake C examples by way of the QC files for the monsters and various other items, and hardly any documentation ;) Hackers, eat your heart out! :-)


released on the 25th


https://groups.google.com/g/relcom.archives/c/oTFQtmcEnsU/m/1GOKiMp3nrQJ

> #
> # -- 386k, 26-Jul-1996
> get /mirrors/idsoft/tonsmore/idstuff/source/qbsp_29.tar.gz
>
> #
> # -- 5.3k, 26-Jul-1996
> read /mirrors/idsoft/tonsmore/idstuff/source/qbsp_29.txt


https://groups.google.com/g/relcom.archives/c/P1ML15kt8bU/m/XDS-pfsVPh4J


> # -- DIR, 26-Jul-1996
> # dir /mirrors/idsoft/idstuff/source
>
> #
> # -- 386k, 26-Jul-1996
> get /mirrors/idsoft/idstuff/source/qbsp_29.tar.gz
>
> #
> # -- 5.3k, 26-Jul-1996
> read /mirrors/idsoft/idstuff/source/qbsp_29.txt
>
> #
> # -- 199k, 26-Jul-1996
> get /mirrors/idsoft/idstuff/source/qcc.tar.gz
>
> #
> # -- 3.0k, 26-Jul-1996
> read /mirrors/idsoft/idstuff/source/qcc.txt




https://groups.google.com/g/nctu.ccca.mirror/c/Y7A11OBaKvM/m/yHz0dc85IiwJ

> 395,452 /PC/games/id/id-mirror/idstuff/source/qbsp_29.tar.gz
> 2,479 /PC/games/id/id-mirror/idstuff/source/qbsp_29.txt
> 1,532 /PC/games/id/id-mirror/idstuff/source/qcc.txt
> 204,053 /PC/games/id/id-mirror/idstuff/source/qcc.tar.gz



https://groups.google.com/g/relcom.archives/c/sGqPkAIlG64/m/9OTadMAzTKsJ

> ----------------------------------------------------------
> каталог /gamesdomain/idsoftware/source
> ----------------------------------------------------------
>
> QuakeEd.tar.gz 394767 May-19-1996 * -
> QuakeEd.txt 2232 May-19-1996 * -
> qbsp_29.tar.gz 395452 Jul-25-1996 * -
> qbsp_29.txt 5451 Jul-25-1996 * -
> qcc.tar.gz 204053 Jul-25-1996 * -
> qcc.txt 3081 Jul-25-1996 * -
> qutils.tar.gz 30339 Jul-1-1996 * -
> qutils.txt 1326 Jul-1-1996 * -
> wolfsrc.txt 7276 Oct-19-1995 * -
> wolfsrc.zip 576904 Oct-19-1995 * -


### qbsp.tar.gz


http://www.gamesmania.com/common/quake/qbsp_tar.gz

content date is june 27


date 27 June 1996

I think this is the missing file...


https://www.gamers.org/dEngine/quake/archive/current/0137.html

Date: Wed, 26 Jun 1996 20:39:02 +0100 (BST)

ftp://ftp.idsoftware.com/idstuff/source/qbsp.tar.gz



https://groups.google.com/g/rec.games.computer.quake.editing/c/XYbXm5qR-nk/m/Tm8piwydCH0J

> /idstuff/source/qbsp.tar.gz.
...
> ftp://ftp.stomped.com/pub/quake_sw/level_editors/qbsp.zip, qbsp_nt.zip


https://groups.google.com/g/relcom.games/c/5dinwt7y9jM/m/DPbvC1ZIJ7kJ

> # dir /mirrors/idsoft/tonsmore/idstuff/source
>
> #
> # -- 385k, 27-Jun-1996
> get /mirrors/idsoft/tonsmore/idstuff/source/qbsp.tar.gz
>
> #
> # -- 5.0k, 27-Jun-1996
> read /mirrors/idsoft/tonsmore/idstuff/source/qbsp.txt



https://groups.google.com/g/relcom.games/c/vz_KbGRbtQ4/m/vtAEvnIcWogJ

> #
> # -- DIR, 27-Jun-1996
> # dir /mirrors/idsoft/idstuff/source
>
> #
> # -- 385k, 27-Jun-1996
> get /mirrors/idsoft/idstuff/source/qbsp.tar.gz
>
> #
> # -- 5.0k, 27-Jun-1996
> read /mirrors/idsoft/idstuff/source/qbsp.txt


https://groups.google.com/g/rec.games.computer.quake.misc/c/10byqP-YgFs/m/y5n-tph74j4J

> Jon Sprake
> unread,
> 28 June 1996, 5:00:00 pm
> to
> >The first level of qtest is available for Quake SW now. It's called dm1.bsp, and is
> >available in the qbsp/vis/light source archive from id Software. Download it from
> >ftp://ftp.idsoftware.com/idstuff/source/qbsp.tar.gz
> Hurray...


https://groups.google.com/g/nctu.ccca.mirror/c/4FNQFGdVgNE/m/DEPyxiRRHJkJ

> 395,115 /PC/games/id/id-mirror/idstuff/source/qbsp.tar.gz
> 2,373 /PC/games/id/id-mirror/idstuff/source/qbsp.txt


## Other

Maybe files are wrapped up in other releases, e.g. ports of tools


### QUTILDOS

https://www.quaddicted.com/files/idgames2/utils/graphics_edit/id_utils/qutildos.txt
https://www.quaddicted.com/files/idgames2/utils/graphics_edit/id_utils/qutildos.zip

qutildos.txt	1996-Jul-24 00:00:00	1.4K	text/plain
qutildos.zip	1996-Jul-24 00:00:00	396.0K	application/zip

So, this release uses stuff from the 1996 Jul 02 release of qutils.

   0 27 Jul 07:24 DIRPACK.EXE
   0 27 Jul 07:25 MODELGEN.EXE
   0 27 Jul 07:25 QLUMPY.EXE
1437 24 Jul  1996 QUTILDOS.TXT
1341  2 Jul  1996 README.TXT
   0 27 Jul 07:25 SPRGEN.EXE
   0 27 Jul 07:25 TEXMAKE.EXE
   0 27 Jul 07:25 UNPACK.EXE

Contains a readme from carmack

the readme is dated 2 Jul 1996

on the mis utils from quake, not light and vis and stuff, the others.

maybe the qutils.txt or a file within the release from that time.



### Quake Development CD

qutils/README.txt

> Quake Development CD 9/4/96

Maybe a copy of this cd was leaked....


https://www.betaarchive.com/forum/viewtopic.php?t=22492&hilit=quake

> * Qtest (or Qtest1)
> * Quake 0.8 (called Beta3 in the readme. Probably a leftover from a previous version for Q&A)
> * Quake Press Release (almost exactly the same as 0.8)


Request for Quake 1.01 source and NextStep 3.3 Developer CD.
https://www.betaarchive.com/forum/viewtopic.php?t=30195

> This code was leaked back in 1997

> By mere chance I had found this rare piece of gaming history. It was the source to the 1.01 build of Linux Quake. Dave Taylor was porting Quake to Linux and their (crack.com) web server was hacked. It was a notable incident. Now that the engine is OSS, I don't think it would be an issue to have though it is great for story telling.

### Quake leak

Infamous source leak of Linux Quake 1.01
https://www.betaarchive.com/forum/viewtopic.php?t=22882

> This is the source code to the Linux build of Quake 1.01 that Dave Taylor was porting. It was taken during an infamous server break in at Crack.com. Back in those days , this was a huge incident. The incident is mentioned in this interview (March of 1997)

http://web.archive.org/web/20070711074820/http://voretimes.planetquake.gamespy.com/inter23.htm

http://www.megaupload.com/?d=2G2297SE



### test1.map

QuakeEd 1.2 upload/test1.map

https://www.gamers.org/dEngine/quake/archive/current/0009.html

> In addition, John Carmack released the test1.map source as used in
the Quake qtest1 release. This offers every BSP builder out there
a chance to compare the results on test1.map against the BSP file
in qtest1.

when was this released?

http://www.gamers.org/dEngine/archive/

https://www.gamers.org/dEngine/archive/QuakeEd/QuakeEd-1.2.map.tgz

  3295  6 Jun  1996 johnc99.map
671270  6 Jun  1996 jrbase1.map
231833  7 Jun  1996 test1.map

these are after quakeed was released and after utils were released...


Quakeed:

-rw-rw-rw-@ 1 jasonb  staff  671282 19 May  1996 jrbase1.map



https://groups.google.com/g/rec.games.computer.quake.editing/c/B0cTu7Bz6tQ/m/5qZ1AUZdikAJ

> 18 Apr 1996, 5:00:00 pm
...
> For example, in johnc99.map, why are 36 planes used to define a
map with only 6 used surfaces? Why not simply define 6 planes
and be done with it? Or am I missing something about this map?


So, this file was available at least mid april....
before quakeed..., after development cd


https://quake.fandom.com/wiki/JOHNC99

https://www.gamers.org/dEngine/quake/QDP/QPrimer.html

johnc99.map

Released with qtest1 are the test1/test2/test3 levels, but only the test1 MAP files is available.
	not in test1.zip... or the pak


https://www.gamers.org/dEngine/quake/QuakeEd/map_example.html


Example from John Carmack (e-mail, april/04/96)
Here is the contents of johnc99.map, a simple box room consisting of six brushes on the world (the entity #0), and three other entities without brushes ("info_player_start", "light", and "info_player_deathmatch"). Note that it takes six cubes (brushes or building blocks) to define on box volume, and each brush has six planes, the intersections of which define the surface of the brush.





### qbsp29.zip

https://www.quaddicted.com/files/idgames2/planetquake/thunder/bsp/qbsp29.zip

just compiled files

dates match though (24 Jul  1996), probably qbsp_29.tar.gz or a subset


  59904 24 Jul  1996 BSPINFO.EXE
  47104 24 Jul  1996 ENTMAP.EXE
  86016 24 Jul  1996 LIGHT.EXE
 138752 24 Jul  1996 QBSP.EXE
  87552 24 Jul  1996 VIS.EXE

don't know....


### beta 3

https://quake.fandom.com/wiki/Beta3

https://archive.org/download/quakeprototypes
https://archive.org/download/quakeprototypes/Quake%20Prototypes/Quake/

TEST1M.7z (View Contents)	17-Oct-2019 22:40	187.0K
q1prerelease.zip (View Contents)	17-Oct-2019 22:39	20.9M
qtest1.zip (View Contents)	17-Oct-2019 22:40	4.1M


https://www.celephais.net/board/view_thread.php?id=60410


TEST1M.7z
	modified version of test level...
	released after test1

q1prerelease.zip
	Quake BETA3
	Tuesday, June 11th, 1996


