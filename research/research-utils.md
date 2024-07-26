Quake Utils Research
====================
Investigation into what tools/src were released, and when.

This is hard because it is July 1996, and internet archive started in this month. Most of the news sites were not captured until much later. There is scant evidence and files.


## Files

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


