# Quake Map History

Release history of additional maps (.bsp) and map sources (.map).

Releases:

* 1995 Jul ??, test1.map
* 1996 Apr 04, johnc99.map
* 1996 May 19, jrbase1.map (QuakeEd.tar.gz)
* 1996 Jul 02, dm1.map, dm1.bsp (qbsp.tar.gz)
* 1996 Jul 25, dm1.map, dm1.bsp (qbsp_29.tar.gz)
* 1996 Dec 30, idctf1.zip
* 1997 Mar 14, maps.zip (Scourge of Armagon)
* 1997 Mar 09, base32.zip
* 1997 Apr 02, death32.zip
* 1997 Apr 09, death32a.zip
* 1997 Jul 02, deathpack1.zip and dm3.zip
* 1997 Jul 06, deathpack1u.zip
* 1997 Aug 25, dm7.zip
* 1999 Mar 18, q1edge.zip
* 2001 Jun 23, e2m10.zip
* 2006 Oct 11, quake_map_source.zip


## test1.map

Posted to IRC in July 1995, referred to as `test1.map`.


IRC logs:

```text
an abbridged log from a stay of dave taylor ('iddt') on #doom,
late jul 95:

...
<calabraun> iddt: okay.. lets see.. are the text files for quake levels in
            an ascii map format, or lines of code which translate to a map?
<iddt>      cala, here's some lines from a map file...
<iddt>      4 wall14_5 0 0 0 0 0 0
<iddt>      (0,912,176,144) (0,928,176,144) (16,928,176,144) (16,912,176,144)
<iddt>      4 wall14_5 0 0 0 0 0 0
<iddt>      (192,928,144,0) (192,1040,144,0) (208,1040,144,0) (208,928,144,0)
<iddt>      it's like coordinates specifying a brush and a texture and some
            other stuff.
...
```

-- [QuakeTalk](https://www.gamers.org/games/quake/quaketalk.txt)


```text
Quote from Dave Taylor (IRC, 1995)
You will note that this is different from the current MAP file format. Guessing, the number of vertices and the texture is given, followed by texture mapping parameters, and the vertices. While four vertices are sufficient to define a (sheared, rotated) cube, I guess each line defines a plane. However, this format, while quoted on some pages, is obviously not used anymore.
here's some lines from a map file...

   4 WALL14_5 0 0 0 0 0 0
     (0,912,176,144) (0,928,176,144) (16,928,176,144) (16,912,176,144)
   4 WALL14_5 0 0 0 0 0 0
     (192,928,144,0) (192,1040,144,0) (208,1040,144,0) (208,928,144,0)

it's like coordinates specifying a brush and a texture and some other
stuff.
```

-- https://www.gamers.org/dEngine/quake/QuakeEd/map_example.html


Locations

* https://www.gamers.org/dEngine/archive/maps/test1.map


## johnc99.map

Sample map content emailed by John Carmack referred to as `johnc99.map`.

Discussion:

> Example from John Carmack (e-mail, april/04/96)
>
> Here is the contents of johnc99.map, a simple box room consisting of six brushes on the world (the entity #0), and three other entities without brushes ("info_player_start", "light", and "info_player_deathmatch"). Note that it takes six cubes (brushes or building blocks) to define on box volume, and each brush has six planes, the intersections of which define the surface of the brush.

-- https://www.gamers.org/dEngine/quake/QuakeEd/map_example.html

```text
MAP file format...brushes?
Chris Carollo
18 Apr 1996

I've been perusing Carmack's info on their method of defining
surfaces in the map with brushes, and then using qbsp to do the
intersection calculating/BSP building/etc.
My initial question is...why? I'm assuming that qbsp performs some
sort of CSG calculations, and is that really necessary? I'm not
seeing the advantages this type of representation has over simply
listing the surfaces.

For example, in johnc99.map, why are 36 planes used to define a
map with only 6 used surfaces? Why not simply define 6 planes
and be done with it? Or am I missing something about this map?

I'm sure id has a valid reason for using this method (they certainly
aren't short on programming gods)...could anyone explain this?

-Chris
```

-- [rec.games.computer.quake.editing](https://groups.google.com/g/rec.games.computer.quake.editing/c/B0cTu7Bz6tQ/m/5qZ1AUZdikAJ)


Locations:

* https://www.gamers.org/dEngine/archive/maps/johnc99.map


## jrbase1.map (QuakeEd.tar.gz)

The `jrbase1.map` example map was provided with the QuakeEd source code released as `QuakeEd.tar.gz`.

Archive snippet:

```text
...
  671282 19 May  1996 jrbase1.map
...
```

Readme snippet:

```text
...
I included some sample data to help you follow the code:

quake.qpr : our current project file
jrbase1.map : a sample map
triggers.qc : a sample qc source file that includes some /*QUAKED comments
...
```

-- readme.txt

Locations of independent `jrbase1.map`:

* https://www.gamers.org/dEngine/archive/maps/jrbase1.map

## dm1.map, dm1.bsp (qbsp.tar.gz)

The `dm1.map` and `dm1.bsp` files were included with the `qbsp.tar.gz` release.

Archive snippet:

```text
...
  547656 27 Jun  1996 dm1.bsp
   86732 27 Jun  1996 dm1.h1
   57419 27 Jun  1996 dm1.h2
  266217 27 Jun  1996 dm1.map
   84567 27 Jun  1996 dm1.prt
...
```



## dm1.map, dm1.bsp (qbsp_29.tar.gz)

The `dm1.map` and `dm1.bsp` files were included with the `qbsp_29.tar.gz` release.

Archive snippet:

```text
...
  547656 27 Jun  1996 dm1.bsp
   86732 27 Jun  1996 dm1.h1
   57419 27 Jun  1996 dm1.h2
  266217 26 Jul  1996 dm1.map
   84567 27 Jun  1996 dm1.prt
...
```

## idctf1.zip

```text
==December 30==
11:25p.m. CST
Full update to come within hours...but for now, my favorite level designer at id (Tim Willits, if you didn't already know) has released a very cool Capture the Flag level. You can get idctf1.zip (772k)from here. I'm working on a small file section right now. All the files are there, I just need to make the page *grin*. BTW, I got the file from blue's but saw the link on that cool page, The Void because blue's page is screwed again like it was Saturday. According to Quakeholio, a non-QW server is running it at 192.246.40.121 (that's at id btw). It is up, I just checked it, but nobody's there. :(. Those shelves are very cool looking. Happiness is find one Shiner Bock in the fridge and a frosted mug in the freezer to pour it in.
```

-- [http://redwood.stomped.com/1296.html](https://web.archive.org/web/20011121183249/http://redwood.stomped.com/1296.html)

Links:

* http://redwood.stomped.com/files/ctf/idctf1.zip

```text
December 30, 1996
Tim Willits' CTF Map
Tim Willits just sent along his CTF map (772 KB) designed to work with Threewave CTF (here's the read me). This is a real treat, as Tim is a brilliant level designer. If you want to try it, he is running a server at id at:

	192.246.40.121

He also wants to be sure to note that this is not an official id product, just a map compatible with Zoid's modifications.

While he was at it, Tim also set the record straight about his odd plan update:

	"I did not update my .plan, American did that crap about me liking WOOD"
```

-- https://www.bluesnews.com/archives/dec96-4.html

Links:

* https://www.bluesnews.com/files/idctf1.zip
* https://www.bluesnews.com/files/idctf1.txt
* https://www.bluesnews.com/archives/dec96-4.html#True%20Confessions%20of%20Tim%20Willits


Archive content:

```text
  1773560 30 Dec  1996 idctf1.bsp
     1319 30 Dec  1996 idctf1.txt
```

Readme snippet:

```text
12-30-1996

=================================================
Title:          idctf1
File:           idctf1.bsp
Author:         Tim Willits
Email Address:  twillits@idsoftware.com
URL:            www.idsoftware.com
Description:    This map is e1m5 converted into a capture the flag level.
```

-- idctf1.txt

Locations:

* ftp://ftp.canvasnet.com/quake/levels/bsp/idctf1.zip
* ftp://ftp.stomped.com/pub/redwood/ctf/idctf1.zip
* http://bluesnews.com/files/idctf1.zip
* http://bluesnews.com/files/maps/idctf1.zip
* http://ftp.mancubus.net/pub/idgames2/idstuff/unsup/idctf1.zip
* http://gamers.org/pub/3dgamers/00archives/doom2/addons/idstuff/unsup/idctf1.zip
* http://quakemecca.simplenet.com/files/maps/idctf1.zip
* http://redwood.gatsbyhouse.com/files/ctf/idctf1.zip
* http://www.bluesnews.com/files/idctf1.zip
* http://www.gameaholic.com/deicide/download.cgi?/idstuff/unsup/idctf1.zip
* http://www.gamers.org/pub/games/idgames/idstuff/unsup/idctf1.zip
* http://www.gamers.org/pub/games/idgames2/idstuff/unsup/idctf1.zip
* http://www.gamers.org/pub/idgames/idstuff/unsup/idctf1.zip
* http://www.gamers.org/pub/idgames2/idstuff/unsup/idctf1.zip
* http://www.planetquake.com/koc/files/idctf1.zip
* http://www.planetquake.com/quakex/threewave/idctf1.zip
* http://www.quakehole.com/files/bsp/idctf1.zip
* https://www.quaddicted.com/files/idgames/idstuff/unsup/idctf1.zip
* https://www.quaddicted.com/files/idgames2/idstuff/unsup/idctf1.zip
* https://www.quaddicted.com/files/idgames2/planetquake/threewave/ctf/misc/idctf1.zip
* https://www.quaddicted.com/files/maps/multiplayer/ctf/idctf1.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/threewave/ctf/misc/idctf1.zip
* https://www.quaddicted.com/files/mirrors/quakerepo.net/ctf/maps/idctf1.zip

## maps.zip (Scourge of Armagon)


Do we need to dig into this?


## base32.zip

The archive `base32.zip` contains `base32.bsp`.

```text
-rw-rw-r--  0 0      0     3066724  9 Mar  1997 base32.bsp
```

Release details?

Maybe released:

```text
March 11, 1997
32 Player QuakeWorld Project
The project to create quality maps for the upcoming QuakeWorld (which supports up to 32 players) has moved to http://stomped.com/quakeworld32/.

```

-- [https://www.bluesnews.com/archives/march97-2.html](https://www.bluesnews.com/archives/march97-2.html)


The `http://stomped.com/quakeworld32/` URL was not archived.

Locations:

* ftp://ftp.stomped.com/pub/redwood/qw/maps/base32.zip
* http://bluesnews.com/files/base32.zip
* http://quake.shiny.it/archive/base32.zip
* http://redwood.stomped.com/files/qw/maps/base32.zip
* http://www.bluesnews.com/files/idstuff/quakeworld/maps/base32.zip
* http://www.frag.com/files/qw/base32.zip
* http://www.frag.com/quakeworld/files/base32.zip
* http://www.gamers.org/pub/games/idgames/levels/doom2/Ports/a-c/base32.zip
* http://www.imaxx.net/~dakota/capture/FILES/base32.zip
* https://www.quaddicted.com/files/idgames/levels/doom2/Ports/a-c/base32.zip
* https://www.quaddicted.com/files/mirrors/quakerepo.net/deathmatch/maps/base32.zip

## death32.zip

Released as `death32.zip`.

```text
April 2, 1997
11:40p.m. CST

Download death32.zip (786k). This combines DM2, DM4, and DM6. I'm now running it on quakeworld.insync.net (206.222.163.150).

Disruptor .plan update:

	I've released a deathmatch map compilation I've done for QuakeWorld called Death32 which is a mix of DM2, DM4 and DM6. It's available on;

	ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/death32.zip

	I'll probably have another release later on this week as I recieve comments from the players.

11:15p.m. CST
Look for a new QW client "soon" as well as a new server. The 1.54 server running at quakeworld.insync.net IS compatible with the older client. death32.bsp, a 32 player combo level consisting of DM2, DM4, and DM6, by Christian 'Disruptor' Antkow should be out fairly soon. It rocks, but it will be even more confusing when you first get in it than base32.

9:00p.m. CST
Oops, got distracted playing the upcoming death32 level that Disruptor is making (combines dm2, dm4, and dm6). Anyway, my computer is fixed (I had problems earlier that prevented me from updating...thanks to Qspy Joe for helping me). Quake Spy 5.1b is available. It gets rid of the whole DLL thing so this should work for everybody. It's much smaller too. Download qspyinst.exe (735k).
```

-- [http://redwood.stomped.com/497.html](https://web.archive.org/web/20011031111944/http://redwood.stomped.com/497.html) (archived)

Links:

* http://redwood.stomped.com/files/qw/maps/death32.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/death32.zip


```text
April 3, 1997
Death 32

Disruptor has combined American McGee's DM2, DM4, and Tim Willits' DM6 (three of my favorites) into Death32 (785 KB), the second 32 Player QuakeWorld Map. This is a beta version of the map, so it's possible a revision will follow. Disruptor also updated his .plan to commemorate the occasion.
```

-- https://www.bluesnews.com/archives/march97-5.html

Links:

* https://www.bluesnews.com/files/death32.zip
* http://www.bluesnews.com/cgi_bin/idfinger.cgi?who=xian

The archive `death32.zip` contains `death32.bsp`.

```text
-rw-rw-r--  0 0      0     1834696  2 Apr  1997 death32.bsp
```

Locations:

* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/death32.zip
* http://bluesnews.com/files/death32.zip
* http://quake.shiny.it/archive/death32.zip
* http://quakemecca.simplenet.com/files/maps/death32.zip
* http://www.bluesnews.com/files/death32.zip
* http://www.i-55.com/ninvaderz/server/death32.zip
* http://www.quake.shiny.it/archive/death32.zip

## death32a.zip

Released as `death32a.zip`.


```text
April 9, 1997

New Death32
Thanks El Tigre]3[ for the word that a new version of Death32 (785 KB), the 32 player Deathmatch map, has been released on id's FTP site. As is his way, Disruptor updated his .plan to celebrate.

	I've released an updated version of my death32 compilation for QuakeWorld. It contains some bugfixes and other updates to the map. It's available on;

	ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/death32a.zip

	It's running on Underworld, my server here at id at 192.246.40.169:27500
```

-- https://www.bluesnews.com/archives/april97-1.html

Links:

* https://www.bluesnews.com/files/death32a.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/


```text
April 9, 1997

Thanks to scorpio for letting me know that death32a.zip (785k), the updated death32. Disruptor's made some cool changes to it. I'm now running it on my server, so you will have to download it to play on there. Here's what Disruptor had to say in his .plan:

	I've released an updated version of my death32 compilation for QuakeWorld. It contains some bugfixes and other updates to the map. It's available on;

	ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/death32a.zip
```

-- [http://redwood.stomped.com/497.html](https://web.archive.org/web/20011031111944/http://redwood.stomped.com/497.html) (archived)

Links:

* ftp://ftp.stomped.com/pub/redwood/qw/maps/death32a.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/death32a.zip


The archive `death32a.zip` contains `death32a.zip`.

```text
-rw-rw-r--  0 0      0     1847840  8 Apr  1997 death32a.bsp
```

Locations:

* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/death32a.zip
* ftp://ftp.stomped.com/pub/redwood/qw/maps/death32a.zip
* http://bluesnews.com/files/death32a.zip
* http://quake.shiny.it/archive/death32a.zip
* http://web.ukonline.co.uk/blue.s/levels/quake/death32a.zip
* http://www.bluesnews.com/files/death32a.zip
* http://www.bluesnews.com/files/idstuff/quakeworld/maps/death32a.zip
* http://www.frag.com/files/qw/death32a.zip
* http://www.frag.com/quakeworld/files/death32a.zip
* http://www.imaxx.net/~dakota/capture/FILES/death32a.zip
* http://www.quake.shiny.it/archive/death32a.zip
* https://www.quaddicted.com/files/mirrors/quakerepo.net/deathmatch/maps/death32a.zip

## deathpack1.zip and dm3.zip

Released as `deathpack1.zip` and dm3.zip.

```text
July 2, 1997
The DeathPack
The final version of Death32B has been released in a compilation zip. DeathPack1.zip contains the QRAD version of Death32, along with a new version of Base32. Both maps have been compiled for transparent water as well. The file is 2.5 megs. Also there is a transparent water VIS'd DM3 as well from id. Download dm3.zip. My normal QuakeWorld server is running death32b right now and can run the other 2 on request.
```
-- [http://redwood.stomped.com/797.html](https://web.archive.org/web/20011125210253/http://redwood.stomped.com/797.html)

Links:

* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/deathpack1.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/dm3.zip


```text
Wednesday, July 2, 1997
New Death 32, Base32 and DM3

Disruptor has released the final new versions of Death32 and Base32 (2.1 MB) with radiant lighting and transparent water support in Death32 and transparent water in Base32 on id's FTP site (thanks to the good Doctor, DR_Zith). And a version of DM3 (433 KB) re-vized for transparent water support has also appeared on id's FTP site. Thanks Richard H. Pistole. Disruptor updated his .plan accordingly:

	I've uploaded deathpack1.zip to;

	ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/deathpack1.zip

	It's death32b (which features subtle QRAD lighting and watervis)
	and base32a (which features watervis) running in a loop.

	As usual, these maps are running on inferno.

The IP address for Inferno is 192.246.40.250:27500.
```

-- https://www.bluesnews.com/archives/june97-4.html

Links:

* https://www.bluesnews.com/files/idstuff/quakeworld/maps/deathpack1.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/deathpack1.zip
* https://www.bluesnews.com/files/idstuff/quakeworld/maps/dm3.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/

Archive `deathpack1.zip` content:

**We do not have a copy of deathpack1.zip at this time**

Archive `dm3.zip` content:

**We do not have a copy of deathpack1.zip at this time**


Locations for `deathpack1.zip`:

* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/deathpack1.zip
* http://bluesnews.com/files/idstuff/quakeworld/maps/deathpack1.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/deathpack1.zip

Locations for `dm3.zip`:

* http://bluesnews.com/files/idstuff/quakeworld/maps/dm3.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/dm3.zip

## deathpack1u.zip

```text
July 6, 1997

Final Deathpack
Disruptor updated his plan to assure people that this is the final Deathpack zip. Deathpack includes an enhanced version of Death32, which uses QRAD for superior lighting, and it also includes a new version of Base32, vis'd for transparent water.

	I didn't get a chance to update my .planfile last night, but just wanted to let everyone know that;

	ftp://ftp.idsoftware.com/idstuff/quakeworld/deathpack1u.zip is *the final* bugfixed version.

	I just wanted to apologize to everyone that downloaded deathpack1.zip. It had a bad vis error that I somehow didn't catch on the first pass. Death32 was also brightened up quite a bit.


Alternately, you can get it at ftp://ftp.stomped.com/pub/redwood/qw/maps/deathpack1u.zip.
```

-- [http://redwood.stomped.com/797.html](https://web.archive.org/web/20011125210253/http://redwood.stomped.com/797.html)

Links:

* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/deathpack1u.zip
* ftp://ftp.stomped.com/pub/redwood/qw/maps/deathpack1u.zip

Archive content:

```text
-rw-rw-r--  0 0      0     3085724  4 Jul  1997 base32b.bsp
-rw-rw-r--  0 0      0     1925640  3 Jul  1997 death32c.bsp
```

Locations

* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/deathpack1u.zip
* ftp://ftp.stomped.com/pub/redwood/qw/maps/deathpack1u.zip
* http://bluesnews.com/files/idstuff/quakeworld/maps/deathpack1u.zip
* http://www.bluesnews.com/files/idstuff/quakeworld/maps/deathpack1u.zip
* http://www.frag.com/files/qw/deathpack1u.zip
* http://www.gameaholic.com/deicide/download.cgi?/idstuff/quakeworld/maps/deathpack1u.zip
* http://www.gamers.org/pub/games/idgames/idstuff/quakeworld/maps/deathpack1u.zip
* http://www.gamers.org/pub/idgames/idstuff/quakeworld/maps/deathpack1u.zip
* http://www.gamers.org/pub/idgames2/idstuff/quakeworld/maps/deathpack1u.zip
* http://www.idsoftware.com/ftp/quakeworld/maps/deathpack1u.zip
* https://www.quaddicted.com/files/idgames/idstuff/quakeworld/maps/deathpack1u.zip
* https://www.quaddicted.com/files/idgames2/idstuff/quakeworld/maps/deathpack1u.zip
* https://www.quaddicted.com/files/idgames2/planetquake/chopshop/maps/quake/deathmatch/deathpack1u.zip
* https://www.quaddicted.com/files/maps/multiplayer/deathpack1u.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/chopshop/maps/quake/deathmatch/deathpack1u.zip

## dm7.zip

Released as `dm7.zip`.

```text
Monday, August 25, 1997
I received an okay from id to post the new deathmatch map DM7 (263 KB), that was recently released on the UK's PC Format (not PC Zone as I said originally, thanks Spike).  Ion Storm's Cleaner sent along the text file which was omitted (I've included it with my zip), as well as an explanation of the map's odd history :

	Here at IonStorm I have access to all the original id maps. On this cd was a map call DM7, being the curious bastard I am I tried to load it. The original map was screwed up (some type of texture problem). I fixed that textured and begun to play with it and revise it a little, more to my liking for a deathmatch map. What came out was Acrophobia - DM7. So for the most part it is an one of the original quake deathmatch levels.

As for servers, there is QuakeWorld server in the UK at 158.143.100.69:27500. Thanks James. Also Redwood is running it on his server at 204.52.135.50:27500.
```

-- https://www.bluesnews.com/archives/aug97-4.html

Links:

* https://www.bluesnews.com/files/maps/dm7.zip
* https://www.bluesnews.com/files/maps/dm7.txt


```text
Sunday, August 24, 1997

According to Jim McCauley, Features Editor of PC Format (UK), the CD included with their September issue (due out August 28) will have DM7, the oft-rumored follow-up to the six original id DM levels.
```

-- https://www.bluesnews.com/archives/aug97-4.html

```text
August 25, 1997

DM7 Part II
All of those people downloading DM7 from my server is lagging the play for those of us in the game. I'm turning off the downloads, but Blue gave me permission to use his dm7.zip (263k). Download that, then unzip to the quake\id1\maps directory (make a maps directory if you don't have one already).

...

DM7
I saw on sCary's that DM7 was released on a CD with a UK games magazine, much to the chagrin of id. It's running on my server at 204.52.135.50 or quake.hal-pc.org (located in Houston, Texas). I've been told it is also running on 158.143.100.69:27500. I kinda like the level, but it seriously lags in GL (high r_speeds) and is a camper's heaven.
```

-- [http://redwood.stomped.com/897.html](https://web.archive.org/web/20011125200502/http://redwood.stomped.com/897.html) (archived)

Links:

* ftp://ftp.stomped.com/pub/redwood/levels/dm7.zip

Archive content:

```text
-rw-rw-r--  0 0      0      587644 25 Aug  1997 dm7.bsp
-rw-rw-r--  0 0      0        1227 25 Aug  1997 dm7.txt
```

Readme snippet:

```text
Here is a copy of the info file that was to go with DM7.

5/12/97		DM7.TXT
================================================================
TITLE: 		 "Archophobia"

================================================================
Authors         : American McGee - Original Map design
		: Cleaner - David Namaksy - Map revision
			Small ledges around the map
			Revised lighting
			Revised item Placement
			Stairs out of water
			Some of the main walkways around the level
			Some other small changes
			Intermission camera
			Deathmatch Starts
		: Tom Hall - Map Name
...
```

-- dm7.txt

Locations:

* ftp://ftp.stomped.com/pub/redwood/levels/dm7.zip
* http://bluesnews.com/files/maps/dm7.zip
* http://lavite.net/maps/q1/dm7.zip
* http://www.gamers.org/pub/games/idgames2/planetquake/5thD/dm7.zip
* http://www.gamers.org/pub/games/idgames2/planetquake/bastard/dm7.zip
* http://www.gamers.org/pub/games/idgames2/planetquake/talon/dm7.zip
* http://www.gamers.org/pub/idgames2/planetquake/5thD/dm7.zip
* http://www.gamers.org/pub/idgames2/planetquake/bastard/dm7.zip
* http://www.gamers.org/pub/idgames2/planetquake/talon/dm7.zip
* https://www.quaddicted.com/files/idgames2/levels/deathmatch/d-f/dm7.zip
* https://www.quaddicted.com/files/idgames2/planetquake/5thD/dm7.zip
* https://www.quaddicted.com/files/idgames2/planetquake/bastard/dm7.zip
* https://www.quaddicted.com/files/idgames2/planetquake/chopshop/maps/quake/deathmatch/dm7.zip
* https://www.quaddicted.com/files/idgames2/planetquake/lvl/quake1_files/dm7.zip
* https://www.quaddicted.com/files/idgames2/planetquake/talon/dm7.zip
* https://www.quaddicted.com/files/maps/multiplayer/dm7.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/5thD/dm7.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/bastard/dm7.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/chopshop/maps/quake/deathmatch/dm7.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/lvl/quake1_files/dm7.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/talon/dm7.zip
* https://www.quaddicted.com/files/mirrors/quakerepo.net/deathmatch/maps/dm7.zip

## q1edge.zip

Released as `q1edge.zip`.

It is possible that two versions of the map were published, one day apart.


```text
March 18, 1999
New id Quake 1 Map

Tim Willits updated his .plan to release a new Quake 1 map. Check out what he said below.

	New Quake 1 map

	I had an old Quake 1 map lying around so I thought I would release it.

	This map was originally built for the Quake 1 arcade game, a conversion of "The Edge" for Quake2. I added some teleporters to it in hopes of speeding up gameplay and help prevent camping.

	For those of you who like to play Quake 1 I hope you enjoy this.

	Thanks, Tim

	ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/q1edge.zip
```

-- [http://redwood.stomped.com/399.html](https://web.archive.org/web/20011122033314/http://redwood.stomped.com/399.html) (archived)


```text
March 19, 1999
Q1Edge Fix

Tim Willits updated his .plan to say that you should get the latest version at ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/q1edge.zip
```

-- [http://redwood.stomped.com/399.html](https://web.archive.org/web/20011122033314/http://redwood.stomped.com/399.html) (archived)

```text
Friday, Mar 19, 1999
Fixed Q1Edge [05:37 am ET] – Share – Post a Comment
id Software's Tim Willits updated his .plan with word that he's posted a fixed version of his Q1Edge conversion of Q2DM1 for Quake 1. Here's the update:

	New Quake 1 map FIXED!

	I fixed the clipping problem I had with the old map and replaced the file on the FTP site.

	Please re-download it for the fixed version.

	Q1edge Conversion

	I had an old Quake 1 map lying around so I thought I would release it.

	This map was originally built for the Quake 1 arcade game, a conversion of "The Edge" for Quake2. I added some teleporters to it in hopes of speeding up gameplay and help prevent camping.

	For those of you who like to play Quake 1 I hope you enjoy this.

	Thanks, Tim

	ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/q1edge.zip
```

-- https://www.bluesnews.com/s/801/fixed-q1edge

Links:

* https://www.bluesnews.com/cgi-bin/finger.pl?id=11&time=19990317205412
* https://www.bluesnews.com/cgi-bin/finger.pl?id=11&time=19990318201510

Archive content:

```text
-rw-rw-r--  0 0      0     1221260 18 Mar  1999 q1edge.bsp
-rw-rw-r--  0 0      0         530 18 Mar  1999 readme.txt
```

Readme snippet:

```text
Map:  Q1EDGE
Author:  Tim Willits
Company:  id Software
Game: Quake 1
Single Player: No
Deathmatch: Yes

Unzip into your quake1\id1\maps directory.

Description:  This map was originally built for the Quake 1 arcade game, a conversion
of "The Edge" for Quake2. I added some teleporters to it in hopes of speeding up
gameplay and help prevent camping.

For those of you who like to play Quake 1 I hope you enjoy this map.

****This is a fixed version of the map. The map name is now The Edge Conversion.
```

-- readme.txt

Locations:

* ftp://ftp.idsoftware.com/idstuff/quakeworld/maps/q1edge.zip
* http://gocompupro.com/cqf/maps/q1edge.zip
* http://quake.crimea.ua/files/quake/maps/q1edge.zip
* http://quake.tronet.troitsk.ru/download/q1edge.zip
* http://www.gamers.org/pub/games/idgames/idstuff/quakeworld/maps/q1edge.zip
* http://www.gamers.org/pub/games/idgames2/planetquake/Fargo/q1edge.zip
* http://www.gamers.org/pub/idgames/idstuff/quakeworld/maps/q1edge.zip
* http://www.gamers.org/pub/idgames2/idstuff/quakeworld/maps/q1edge.zip
* http://www.gamers.org/pub/idgames2/planetquake/Fargo/q1edge.zip
* https://www.quaddicted.com/files/idgames/idstuff/quakeworld/maps/q1edge.zip
* https://www.quaddicted.com/files/idgames2/idstuff/quakeworld/maps/q1edge.zip
* https://www.quaddicted.com/files/idgames2/planetquake/Fargo/q1edge.zip
* https://www.quaddicted.com/files/mirrors/ftp.planetquake.com/Fargo/q1edge.zip
* https://www.quaddicted.com/files/mirrors/quakerepo.net/deathmatch/maps/q1edge.zip


## e2m10.zip

Released as `e2m10.zip`

```text
Quake Birthday Surprise -  Saturday - June 23, 2001

Well, what more is there to say about Quake?  I love 'im like a son.  And I have some great memories of his birth, of his growing up, out in the world.  All the LAN parties, all the levels, all the demos and speed-running contests and challenges... it's been a great 5 years for good ole Quake.  So good, in fact, that he got two brothers: Quake II and Quake III, who made their own way in the world; established their own unique identities and accomplished their own goals.
But to me, there's just something about Quake 1, the original, that keeps pulling me back into its dark embrace.  I think... it's the rawness, the edgy violence and the unsettling, menagerie of wild creatures we pulled from the nethercore of our mind's eye and then placed among the tattered ruins and ancient walkways of Quake's wind-blown crevices and scenic vistas.

Creating those fantastic and impossible environments was a challenge from the very beginning.  We were accustomed to having the editor, or at least the graphics engine, take care of such trivial things as connecting walls to floors, evenly lighting entire rooms, and making it easy to create doors and doorways.  That was the familiar universe of our baby, DOOM.  We were in the new universe of Quake, where once again we were inventing our own rules and trying to play by them, or at least create by them.

It took a while to get used to the freedom of creation in the new engine and to get the right feel for scale and space.  Countless maps were worked on and discarded.  I remember many maps that I thought were going to turn out great, but just didn't make the cut in the end.  I wish I had copies of those old guys -- I spent a lot of time in them, thinking about them during their creation, learning how to create spaces with them.  Really, the only visible remnant of my early, slightly-off perception of Quake-space is in e2m6, The Dismal Oubliette.  In the area where you take the elevator through the three floors, the hallways are very cramped and dangerous -- I didn't have the right scale in there and didn't have time to correct it before release, but I knew it was wrong.  Ah, well.  A defective gene was left in, but it's not the only one, thankfully.

For a long time now, I've kept one remnant of Quake's creation that I had to cut out.  It's the Lost Entrance of the Dismal Oubliette.  Yes, there used to be a much more interesting beginning to that area of Quake, but I had to amputate the guy and cauterize the wound into its current state, the starting point of e2m6.  I remember spending many hours trying to get it just right, to create the feeling of an awful, cavernous pit for the player to get out of and into the real horror of the Oubliette.  It added a nice bit of gameplay time and I'm sorry that it had to go, but we set the .BSP file size at 1.4Mb and had to be strict about it.

But today, on Quake's 5th Birthday, I will give you a personal piece of Quake's creation that I treasure.  Be careful with it, it's fragile and one of a kind and was created back in the mists of time around QTest's release.  I've named the map E2M10.BSP and am including the E2M10.MAP that chronicles its creation.  Looking closely at the .map file will reveal some long-lost entities that we had in Quake and I'm not sure if I even remember what they did...

The Lost Entrance to the Dismal Oubliette

e2m10.zip

Unzip all the files in your quake\id1\maps directory, run Quake, pull up the console and type map e2m10 and spend a little time in a creation that was destined for release, but didn't make the cut.
```

-- [http://rome.ro/archive/news/news_05_12_2001_to_06_27_2001.htm](https://web.archive.org/web/20020604182126/http://rome.ro/archive/news/news_05_12_2001_to_06_27_2001.htm) (archived)

Links:

* http://rome.ro/downloads/e2m10.zip


```text
Romero's "Lost" Quake Map [Jun 24, 2001, 08:12 am ET] – 12 Comments
An update to Planet Romero in honor of Quake's fifth birthday the other day offers "Lost Entrance of the Dismal Oubliette," a map that at one point was intended for inclusion in Quake that was cut for exceeding their file size for .bsps. Here's a bit from the accompanying update that fills us in on the history of this map:

	Yes, there used to be a much more interesting beginning to that area of Quake, but I had to amputate the guy and cauterize the wound into its current state, the starting point of e2m6. I remember spending many hours trying to get it just right, to create the feeling of an awful, cavernous pit for the player to get out of and into the real horror of the Oubliette. It added a nice bit of gameplay time and I'm sorry that it had to go, but we set the .BSP file size at 1.4Mb and had to be strict about it.

	But today, on Quake's 5th Birthday, I will give you a personal piece of Quake's creation that I treasure. Be careful with it, it's fragile and one of a kind and was created back in the mists of time around QTest's release. I've named the map E2M10.BSP and am including the E2M10.MAP that chronicles its creation. Looking closely at the .map file will reveal some long-lost entities that we had in Quake and I'm not sure if I even remember what they did...
```

-- https://www.bluesnews.com/s/26231/romero_s-lost-quake-map

Links:

* http://www.johnromero.com/


Archive content:

```text
-r--r--r--  0 0      0      282987 19 Jun  1998 e2m10.map
-rw-rw-r--  0 0      0        2306 23 Jun  2001 e2m10.txt
-r--r--r--  0 0      0      574308 19 Jun  1998 e2m10.bsp
```

Readme snippet:

```text
February 1996
================================================================
Title                   : Lost Entrance of the Dismal Oubliette
Filename                : e2m10.bsp
Author                  : John Romero
Email Address           : john@rome.ro
Description             : Winding, dripping cave entrance

         More Quake History and tidbits might be found on:
                           http://rome.ro
================================================================
...
```

Locations:

* http://quake.crimea.ua/files/quake/maps/e2m10.zip
* http://www.quaddicted.com/filebase/e2m10.zip
* https://www.quaddicted.com/filebase/e2m10.zip
* https://www.quaddicted.com/files/maps/multiplayer/e2m10.zip
* https://www.quaddicted.com/files/maps/singleplayer/e2m10.zip
* https://www.quaddicted.com/files/mirrors/quakerepo.net/singleplayer-deathmatch/maps/e2m10.zip
* https://www.quaddicted.com/reviews/e2m10.html

## quake_map_source.zip

Released as `quake_map_source.zip`.


```text
wednesday, october 11, 2006
Quake Map Sources Released!

Since it's Quake 1's tenth anniversary this year (starting June 22nd) I thought I'd dig up and release all of Quake's original map sources. For all these years the only possible way to glean any information from Quake's internal format was from BSP deconstruction programs - but those had problems with tons of brushes generated from insane BSP splits. So finally, here are the originals with the dust blown off of them, shined-up and zipped up. Have fun, mappers!
```

-- [http://rome.ro/2006/10/quake-map-sources-released.html](https://web.archive.org/web/20061022171208/http://rome.ro/2006/10/quake-map-sources-released.html) (archived)

Link:

* http://www.mediamax.com/theromero/Hosted/quake/quake_map_source.zip


```text
Quake Maps Source [Oct 12, 2006, 09:57 am ET] – 8 Comments
Planet rome.ro (thanks Daz) now offers the release of the source code for the maps in the original Quake. Here's the accompanying word from John Romero:
Since it's Quake 1's tenth anniversary this year (starting June 22nd) I thought I'd dig up and release all of Quake's original map sources. For all these years the only possible way to glean any information from Quake's internal format was from BSP deconstruction programs - but those had problems with tons of brushes generated from insane BSP splits. So finally, here are the originals with the dust blown off of them, shined-up and zipped up. Have fun, mappers!
```

-- https://www.bluesnews.com/s/71823/quake-maps-source

```text
Thursday, 12 October, 2006 – Planet Quake News	Planet Quake
John Romero's Quake Map Source Release
5:57 PST | jube | Print News | Mail News
In honour of Quake's 10th year, John Romero went on the hunt for Quake's original map sources, and has released them to the public. I guess time will tell if Quake mappers come up with anything spiffy to do with them. In the meantime grab the Quake Map Sources from the PQ Files.
```
-- [http://planetquake.gamespy.com/quake1/](https://web.archive.org/web/20061022160540/http://planetquake.gamespy.com/quake1/)


Archive content:

```text
-r--r--r--  0 0      0      512159  4 Sep  1996 E4M8.MAP
-r--r--r--  0 0      0      202265  4 Sep  1996 END.MAP
-rw-rw-r--  0 0      0        1046 11 Oct  2006 release_readme.txt
-r--r--r--  0 0      0      669185  4 Sep  1996 START.MAP
-r--r--r--  0 0      0         590  4 Sep  1996 B_ARMOR1.MAP
-r--r--r--  0 0      0         590  4 Sep  1996 B_ARMOR2.MAP
-r--r--r--  0 0      0         590  4 Sep  1996 B_ARMOR3.MAP
-r--r--r--  0 0      0         577  4 Sep  1996 B_BACKPK.MAP
-r--r--r--  0 0      0        3574  4 Sep  1996 B_BARREL.MAP
-r--r--r--  0 0      0         689  4 Sep  1996 B_BATT0.MAP
-r--r--r--  0 0      0         697  4 Sep  1996 B_BATT1.MAP
-r--r--r--  0 0      0         602  4 Sep  1996 B_BH10.MAP
-r--r--r--  0 0      0         618  4 Sep  1996 B_BH25.MAP
-r--r--r--  0 0      0         587  4 Sep  1996 B_BH100.MAP
-r--r--r--  0 0      0         923  4 Sep  1996 B_BOMB.MAP
-r--r--r--  0 0      0         684  4 Sep  1996 B_EXBOX2.MAP
-r--r--r--  0 0      0         688  4 Sep  1996 B_EXPLOB.MAP
-r--r--r--  0 0      0        4770  4 Sep  1996 B_KEY1.MAP
-r--r--r--  0 0      0        4764  4 Sep  1996 B_KEY2.MAP
-r--r--r--  0 0      0         605  4 Sep  1996 B_NAIL0.MAP
-r--r--r--  0 0      0         610  4 Sep  1996 B_NAIL1.MAP
-r--r--r--  0 0      0         513  4 Sep  1996 B_NAIL2.MAP
-r--r--r--  0 0      0         694  4 Sep  1996 B_ROCK0.MAP
-r--r--r--  0 0      0         664  4 Sep  1996 B_ROCK1.MAP
-r--r--r--  0 0      0         606  4 Sep  1996 B_SHELL0.MAP
-r--r--r--  0 0      0         610  4 Sep  1996 B_SHELL1.MAP
-r--r--r--  0 0      0      270971  4 Sep  1996 DM1.MAP
-r--r--r--  0 0      0      668496  4 Sep  1996 DM2.MAP
-r--r--r--  0 0      0      376408  4 Sep  1996 DM3.MAP
-r--r--r--  0 0      0      364922  4 Sep  1996 DM4.MAP
-r--r--r--  0 0      0      215038  4 Sep  1996 DM5.MAP
-r--r--r--  0 0      0      250581  4 Sep  1996 DM6.MAP
-r--r--r--  0 0      0      212798  4 Sep  1996 DM7.MAP
-r--r--r--  0 0      0       26184  4 Sep  1996 DM8.MAP
-r--r--r--  0 0      0      673520  4 Sep  1996 E1M1.MAP
-r--r--r--  0 0      0      593657  4 Sep  1996 E1M2.MAP
-r--r--r--  0 0      0      648687  4 Sep  1996 E1M3.MAP
-r--r--r--  0 0      0      738630  4 Sep  1996 E1M4.MAP
-r--r--r--  0 0      0      741571  4 Sep  1996 E1M5.MAP
-r--r--r--  0 0      0      655639  4 Sep  1996 E1M6.MAP
-r--r--r--  0 0      0      242674  4 Sep  1996 E1M7.MAP
-r--r--r--  0 0      0      428752  4 Sep  1996 E1M8.MAP
-r--r--r--  0 0      0      838179  4 Sep  1996 E2M1.MAP
-r--r--r--  0 0      0      653363  4 Sep  1996 E2M2.MAP
-r--r--r--  0 0      0      728778  4 Sep  1996 E2M3.MAP
-r--r--r--  0 0      0      632224  4 Sep  1996 E2M4.MAP
-r--r--r--  0 0      0      691587  4 Sep  1996 E2M5.MAP
-r--r--r--  0 0      0      713587  4 Sep  1996 E2M6.MAP
-r--r--r--  0 0      0      836821  4 Sep  1996 E2M7.MAP
-r--r--r--  0 0      0      282987 19 Jun  1998 e2m10.map
-rw-rw-r--  0 0      0        2306 23 Jun  2001 e2m10.txt
-r--r--r--  0 0      0      675637  4 Sep  1996 E3M1.MAP
-r--r--r--  0 0      0      591388  4 Sep  1996 E3M2.MAP
-r--r--r--  0 0      0      660964  4 Sep  1996 E3M3.MAP
-r--r--r--  0 0      0      920837  4 Sep  1996 E3M4.MAP
-r--r--r--  0 0      0     1118684  4 Sep  1996 E3M5.MAP
-r--r--r--  0 0      0     1007883  4 Sep  1996 E3M6.MAP
-r--r--r--  0 0      0      873225  4 Sep  1996 E3M7.MAP
-r--r--r--  0 0      0      897145  4 Sep  1996 E4M1.MAP
-r--r--r--  0 0      0      513617  4 Sep  1996 E4M2.MAP
-r--r--r--  0 0      0      545731  4 Sep  1996 E4M3.MAP
-r--r--r--  0 0      0      544892  4 Sep  1996 E4M4.MAP
-r--r--r--  0 0      0      557818  4 Sep  1996 E4M5.MAP
-r--r--r--  0 0      0      443111  4 Sep  1996 E4M6.MAP
-r--r--r--  0 0      0      602908  4 Sep  1996 E4M7.MAP
```

Readme snippet:

```text
**************************************************
The Original Quake Map Sources
by id Software (C) 1996
Released October 2006 during Quake's 10th Anniversary
**************************************************

These are the original Quake map source files as of Quake v1.06.  I've included the chopped-off
beginning to E2M6 (The Dismal Oubliette) as well, named E2M10.MAP.  The majority of these maps
were created during the last 7 months of Quake's development cycle when we had decided on the
final direction of the game.  For a comprehensive listing of each map, its name, author and
place in the final game please visit the Wikipedia (http://en.wikipedia.org/wiki/Quake).

Also included with the full map sources are the map sources created for the game's items (armor,
ammo, etc.) which were needed to light the BSP files so the items could be viewed in the game.

You can open these .MAP files with a Quake map editor such as Qoole 99.

Have fun and Happy Birthday, Quake!


John Romero
john@rome.ro
http://rome.ro
```

Locations:

* http://www.inside3d.com/idmapsources/quake_map_source.zip
* http://www.quake-1.com/files/maps/quake_map_source.zip
* http://www.quaketastic.com/files/single_player/maps/quake_map_source.zip
* https://www.quaddicted.com/files/maps/sources/quake_map_source.zip
* https://www.quaddicted.com/files/quake_map_source.zip
* https://www.quaddicted.com/files/tools/quake_map_source.zip


## References

* https://www.gamers.org/dEngine/archive/maps/
* https://www.gamers.org/dEngine/quake/QuakeEd/map_example.html

