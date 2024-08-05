# SGI Quake / IRIX Quake

SGI stands for "Silicon Graphics, Inc", a company responsible for the "Silicon Graphics Computer Systems", a high-end workstation capable of 3D graphics in 1996.

Quake was ported to this platform officially (Ed Hutchins and John Carmack) and was called "SGI Quake", "SGIQuake", or "IRIX Quake", after the name of the SGI operating system IRIX.

> Id software bears _NO_ support responsibility for the SGI versions of Quake (either .gl or .sw) whatsoever! Likewise, SGI is releasing these versions of Quake as-is, and is not responsible for support. These executables are being made available in a large part through the efforts of individual employees of SGI, and to the extent that we can we'll be happy to answer questions on the appropriate SGI newsgroups (comp.sys.sgi.\*). Please help ensure further Quake-related progress by limiting your questions to this channel.

-- https://www.siliconbunny.com/mirrors/ftp.sgi.com/sgi/quake/doc/quake1.html

Releases:

* 1996 Oct 24, GLQuakeV0_3.tar.Z, GLQuakeV0_3src.tar.Z, libutil.tar.Z
* 1997 Feb 12, sgiquake.tar.Z or sgiquake.tar.gz.pre_040997
* 1997 Mar 25, quake.gl
* 1997 Apr 09, sgiquake-1997-04.tar.gz
* 1997 May 02, sgiquake-1997-05-02.tar.gz
* 1997 May 14, sgiquake-1997-05-13.tar.gz
* 1997 May 22, sgiquake-1997-05-21.tar.gz
* 1997 Sep 24, sgiquake.tar.gz


## Custom Quake Renderer (early SGI Quake?)

Not a port of Quake, but a Quake renderer/server written for SGI.

Comment on Edward Hutchins aka "Ed Hutchins" project:

```text
Ed Hutchins
6 Sept 1996

> Author: Matt Pharr <m...@graphics.stanford.edu>
> Date: 05 Sep 1996 16:08:49 -0700

>
> r...@fangio.asd.sgi.com (Robert Keller) writes:
> > Ian CR Mapleson <mapl...@cee.hw.ac.uk> wrote:
> > >I doubt any port would take advantage of any hw texture mapping that some
> > >SGI machines have though - too much work to write such a complex port.
> >
> > perhaps for id software, but I know of someone who is using the bits of
> > freely available id quake code and databases to make a quake-equivalent
> > come to life on InfiniteReality...
Thanks for spilling the beans on project MooseHead! (I hope I have as much
fun on my sabbatical as you apparently are :-).

> Sounds like they're opening a bit of a can of worms there. It's not going
> to look _that_ much better on the $200,000 IR than it does on a $3000 PC;
> while higher resolution better texture sampling, etc. would be nice, I
> don't think that it's going to look 70x better...

I mainly did it because I hadn't written a decent OpenGL app before.
The biggest problem is that all the artwork comes from 256 color palettes.
Things look amazingly good considering the game's target platform, but I'd
agree it isn't worth 70x (1280x1024 instead of 640x480 is about 4x,
multisampling is another 4x, real mip-mapping and 60Hz is worth 2x, so
I'd give it a 32x rating). Lighting is the biggest problem so far (I've done
a sleazy hack that lets you independently turn lightmaps on or off, but
the real game incrementally blends contributions from each lightmap which
means host side fiddling and subtex loads are needed...). The QuakeC
interpreter is up and running, entities initialize themselves... all
that's really left is doing the simulation loop. Wish me luck.

(note that running @ film resolution (2048x1200) gives you 8 x 4 x 2 x
an extra 2 because face it, film-res is way cool, for a grand total of
128x better than the PC).

Oh, I should pick up another 2x just because I disprove a Michael Abrash
quote from one of his Quake talks:

"It would be nice to be able to chuck all the polygons at a rasterizer that
was so fast that we didn't have to think any further.
Problem: no such rasterizer."

I render whole levels (no sw culling) at 1280x1024 at 10+fps, as fast as a
$3k PC renders at 640x480. Rendering using the PVS and view direction to
perform culling hits 60fps.

> -matt
> --
> Matt Pharr | m...@lux.stanford.edu | <URL:http://www-graphics.stanford.edu/~mmp>

P.S. if any id guys out there are interested in supplying the server
side IRIX executable + specs on the communication interface to the client,
I'd be happy to provide an Infinite Reality tuned client-side renderer :-)

- Ed
```

-- [comp.sys.sgi.misc](https://groups.google.com/g/comp.sys.sgi.misc/c/9wcQU8XNVVE/m/vAr6MWV8K8sJ)

And later:

```text
GLQuake v0.3 available
Ed Hutchins
24 Oct 1996

I've made the source to my OpenGL Quake walkthrough available on my
homepage at: http://reality.sgi.com/employees/hutchins_asd
I'm hoping others will want to pitch in and get it running as
a client (and possibly a full game server) on SGI machines. This
is my first OpenGL program and should in no way be construed as
a benchmark of what SGI machines can do :-)
- Ed
```

-- [comp.sys.sgi.announce](https://groups.google.com/g/comp.sys.sgi.announce/c/qBpfTShJ8E4/m/-RDNLwsnauQJ)


```text
January 17, 1997

Here's an interesting GL Quake link for those with SGI machines from an SGI employee.
```

-- [http://redwood.stomped.com/197.html](https://web.archive.org/web/20011031111652/http://redwood.stomped.com/197.html) (archive)

Link:

* http://reality.sgi.com/employees/hutchins_asd/

```text
* GLQuake v0.3 - GLQuake executable
* GLQuake v0.3 source - Quake walkthrough in OpenGL (was IRQuake)
* libutil.a sources (now also included in GLQuake distribution)

These links should work again, but some browsers have trouble with relative links (all browsers had trouble with the absolute path).
GLQuake has the majority of rendering code and the QuakeC interpreter needed for getting a full Quake server running, but someone out there will have to work on replicating Quake's main world-simulation loop. Writing a client-side quake terminal should be possible since most of the client-server protocol has been documented in the Quake specs.
Note that you need IRIX 6.2 or later to compile GLQuake, and that you'll need the PAK files from the game. I'd recommend buying it outright, but you can also get the shareware levels from id software's site. I haven't tried running with the v1.06 PAK files yet, but I assume the changes aren't too drastic (GLQuake works with v1.01). If anyone ports GLQuake to other platforms, I'd be happy to put pointers or distribute copies from here.
```

-- [http://reality.sgi.com/employees/hutchins_asd/](https://web.archive.org/web/19980220092553/http://reality.sgi.com/employees/hutchins_asd/) (archived)

Links:

* ftp:ftp/GLQuakeV0_3.tar.Z
* ftp:ftp/GLQuakeV0_3src.tar.Z
* ftp:ftp/libutil.tar.Z

I suspect these links were supposed to be something like the following (based on sgiquake links below):

* http://reality.sgi.com/employees/hutchins_asd/ftp/GLQuakeV0_3.tar.Z
* http://reality.sgi.com/employees/hutchins_asd/ftp/GLQuakeV0_3src.tar.Z
* http://reality.sgi.com/employees/hutchins_asd/ftp/libutil.tar.Z




## Early Interest and Requests

Early testing by John Carmack:

```text
-----------------------------------------
John Carmack's .plan for Mar 02, 1996
-----------------------------------------

* wrote sgi test demo
```

-- [johnc .plan archive](https://github.com/ESWAT/john-carmack-plan-archive/blob/master/by_year/johnc_plan_1996.txt)

Dave Taylor references this in his email below.


Request of Dave Taylor by Piotr Marek Jr. aka "YoonioR":

```text
10/29/1996
I got a reply from Dave Taylor <ddt;@crack.com> (former programmer and co-founder of id Software), now co-owner of the UNIX-oriented company crack dot com (who wrote the game Abuse, among other things). I asked him about the next versions of Quake for the Intel/Linux platform and - something that interests me and a few other people very much - a port to SGI/IRIX. Bad news, my friends. Read the letter carefully...
```

-- [http://www.pk.edu.pl/~pmj/quake/news_old1.html](https://web.archive.org/web/19981206044920/http://www.pk.edu.pl:80/~pmj/quake/news_old1.html) (archived, google translate)

Email:

```text
Subject:
        Re: Quake ports to SGI?
  Date:
        Mon, 28 Oct 1996 22:15:18 -0600 (CST)
  From:
        Dave Taylor
    To:
        "Piotr Marek Jr."


>       I have two quick questions.
> First - are You planning to make Linux port based on 1.06 progs?
> Currently available 1.01 makes impossible (as far as for myself)
> to run it with modified ServerModules as they're based on 1.06 progs.

I can't, but Linus might be able to.  Ask (beg) him.

> Second, more important: have You heard any rumors regarding
> IRIX port to Quake?

I can't do it.  You can beg id Software.  Carmack made an OpenGL version
which screamed on a loaner Maximum Impact we had.  It made my dick hard.
But I know he didn't maintain the source.  Would take some serious convincing.
There are buttloads of reasons not to do it.

        =-ddt->
```

-- [http://www.pk.edu.pl/~pmj/quake/taylor.html](https://web.archive.org/web/19991118001510/http://www.pk.edu.pl/~pmj/quake/taylor.html) (archived)

Follow-up with John Carmack:

```
31.10.1996

New news from the Quake porting front to other platforms. John Carmack replied to my question about a Quake port to IRIX. Details in the mail!
```

-- [http://www.pk.edu.pl/~pmj/quake/news_old1.html](https://web.archive.org/web/19981206044920/http://www.pk.edu.pl:80/~pmj/quake/news_old1.html) (archived, google translate)

Email:

```text
From: John Carmack
Date: Wed, 30 Oct 96 11:31:23 -0600
To: "Piotr Marek Jr."
Subject: Re: IRIX port to Quake? Ever?

A server port to irix would be very easy, but a proper
client would take more time than we are likely to have.

We are probably going to do an open-gl version of quake
on NT, which would be the interesting thing to run on
SGI hardware, but that is quite some time off.

If you know anyone at sgi, I will make this offer:

If sgi is willing to provide an r10000 based machine
(for us to keep) and an engineer to work on sight here
at id, I will provide them with assistance in fully
porting the linux version of quake over to irix.

John Carmack
```

-- [http://www.pk.edu.pl/%7Epmj/quake/carmacksgi.html](https://web.archive.org/web/19991011003832/http://www.pk.edu.pl/%7Epmj/quake/carmacksgi.html) (archived)


The exchange outlined in the email looks like to have paid off one month later:

```text
-----------------------------------------
John Carmack's .plan for Nov 23, 1996
-----------------------------------------

...

IRIX-GLQuake: In two weeks, Ed Hutchins from SGI is coming down and we are going to port glQuake to irix. This will only run (reasonably) on systems with hardware texture mapping: O2, impact, RE2, and IR. No indys, extremes, etc. You could probably use them as dedicated servers, though.
```

-- [johnc .plan archive](https://github.com/ESWAT/john-carmack-plan-archive/blob/master/by_year/johnc_plan_1996.txt)

This suggests that the port by Ed Hutchins was official.


## SGI Quake (Ed Hutchins) v1

Released as `sgiquake.tar.Z`, later distributed as `sgiquake.tar.gz.pre_040997`.

Work on the port was announced on http://www.webcom.com/phantasm/QUSI/ which was not archived:

```text
Joel Baxter
31 Jan 1997

Yah, we're pretty bummed about that too. I've been following the progress
of SGIQuake via this site:

http://www.webcom.com/phantasm/QUSI/

For a while it was cool. They're posting SGI/glquake screenshots! They're
posting SGI/xquake screenshots! They have servers and clients running!
They're playing CTF! At about that point I felt like tapping gently on the
window and saying "Uhh... guys... there's folks out here too..." And then
no more updates. I think they've locked themselves in a room to "test" the
thing a little more.

Now even the QUSI page author has posted a little paragraph saying that he's
puzzled at the sudden Informational Black Hole that has engulfed the
project. If I were you, I'd still maintain some optimism. In all
seriousness, they're probably just wanting to polish the thing up before
releasing it. Also, I heard from another source that SGIQuake was
stimulating some hardware bug on the machine they were testing it on, and
they were trying to chase that down (although that was a while ago). Not a
design flaw, but an actual malf in that particular machine; still you could
see how figuring that out might take priority (after all, they are SGI
employees, not id employees).


Keep the faith, brother.


--
Joel Baxter jba...@lemur.stanford.edu http://lemur.stanford.edu/~jbaxter/
aka lemurboy Clan 9 From Outer Space http://lemur.stanford.edu/clan9/
```

-- [rec.games.computer.quake.misc](https://groups.google.com/g/rec.games.computer.quake.misc/c/C_Bich6jUOo/m/p_fhL-ZZ3L4J)



(Pre)Launch announcement:

```text
SGI Quake
Ed Hutchins
12 Feb 1997

The SGI port of idsoftware's Quake should be available from:
http://www.sgi.com/Fun/Free_games.html
sometime tomorrow (Wednesday).
For those who really can't wait, you can grab copies now from:
http://reality.sgi.com/employees/hutchins_asd

- Ed
```

-- [comp.sys.sgi.apps](https://groups.google.com/g/comp.sys.sgi.apps/c/YAdEZ-z2CA8/m/P9igx7lW4WwJ)


Announced:

```text
February 12, 1997

SGI Quake
It's not one of Zoid's ports, but there's an SGI Quake avaiilable at Ed's Homely Page (which is part of the SGI site). I don't know if it works or anything, but if anyone want to send me a Silicon Graphics workstation to test it with, I'll be glad to. Thanks CareTaker.
```

-- https://www.bluesnews.com/archives/feb97-2.html
-- https://www.bluesnews.com/cgi-bin/blammo.pl?mode=archive&display=19970412&oneday=true

Links:

* http://reality.sgi.com/employees/hutchins_asd/

```text
February 12, 1997

I saw at Blue's that the SGI Quake that I mentioned here a few weeks ago has been released as a full version.
```

-- [http://redwood.stomped.com/297.html](https://web.archive.org/web/20010422160347/http://redwood.stomped.com/297.html) (archived)

Links:

* http://reality.sgi.com/employees/hutchins_asd/



Suggestion of a prior version, or perhaps this references his two versions (e.g. Feb and April 1997).

```text
SGI Quake!
The port of idsoftware's Quake to SGI platforms is finally ready for prime-time!

sgiquake.tar.Z - SGI quake executables for all platforms

Here's the README.TXT file included in sgiquake.tar.Z.
I couldn't resist putting these out early here, the more kosher location for SGI quake will be here.
Note: there was a slightly broken version here for a while (savegame didn't work), get the latest version if you notice this problem.
```

-- [http://reality.sgi.com/employees/hutchins_asd/](https://web.archive.org/web/19980220092553/http://reality.sgi.com/employees/hutchins_asd/) (archived)


Links:

* http://reality.sgi.com/employees/hutchins_asd/ftp/sgiquake.tar.Z
* http://reality.sgi.com/employees/hutchins_asd/README.TXT
* http://www.sgi.com/Fun/Free_games.html


```text
Welcome to the SGI port of Id Software, Inc's Quake!
Disclaimer:
Id Software, Inc bears NO support responsibility for the SGI versions of Quake (either .gl or .sw) whatsoever!
Likewise, SGI is releasing these versions of Quake as-is, and is not responsible for support.

These executables are being made available in a large part through the efforts of individual employees of SGI, and we refer any questions on the appropriate SGI newsgroups (comp.sys.sgi.*).
```

-- [http://www.sgi.com/Fun/free/sgi-quake.html](https://web.archive.org/web/19980701023059/http://www.sgi.com/Fun/free/sgi-quake.html) (archived)

Link:

* http://reality.sgi.com/employees/hutchins_asd/ftp/sgiquake.tar.Z

Screenshots taken of SGI Quake:

* https://web.archive.org/web/19970315085554/http://reality.sgi.com/rae/quake/pics/sgiquake/

Archive content:

```text
   3934 12 Feb  1997 LICINFO.TXT
  43292 12 Feb  1997 MANUAL.TXT
   3766 12 Feb  1997 ORDER.TXT
   7951 12 Feb  1997 README.TXT
   1406 12 Feb  1997 quake
 582564 12 Feb  1997 quake.gl
 668456 12 Feb  1997 quake.gl.r10k
 582564 12 Feb  1997 quake.sw
 667916 12 Feb  1997 quake.sw.r10k
```

Readme snippet:

```text
Welcome to the SGI port of idsoftware's Quake!
...
- Ed Hutchins
2/11/1997
```

On the day of release, Philip Nemec (who later takes over support of the port) is offering technical support on USENET:

```text
Philip Nemec
12 Feb 1997
to Phillip George Geiger

I'm not sure if 5.2 works at all. But since you're running a < 6.3 OS
you need to run without sound (-nosound) - I think that will fix that
unresolvable symbol problem.
The glxinfo not being found will mess up the autodetection so you should
manually run the correct binary (in your case I think that would be
./quake.sw -nosound).
```

-- [comp.sys.sgi.misc](https://groups.google.com/g/comp.sys.sgi.misc/c/82Zxr0wbPXs/m/CT7uIY1SZcgJ)



Additional Links:

* https://web.archive.org/web/19970409141001/http://www.frag.com/files/ports/sgiquake_tar.Z
* https://web.archive.org/web/19970327191450/http://redwood.gatsbyhouse.com/files/ports/sgiquake_tar.Z


## SGI Quake Binary (Ed Hutchins) v???

Perhaps released as `quake.gl`.

Found in a directory titled `1997-03-25/` suggesting a release date.

binary

md5sum does not match other Ed versions.

Link:

* https://www.siliconbunny.com/mirrors/ftp.sgi.com/sgi/quake/download/quake1/1997-03-25/


## SGI Quake (Ed Hutchins) v2


`sgiquake-1997-04.tar.gz`

Announced?

```text
New SGI Quake [Apr 12, 1997, 12:00 pm ET] – Post a Comment
Saw on the Void that there's a new version of SGI Quake available on Quake Utils for SGI Irix.
```

-- https://www.bluesnews.com/s/226446/new-sgi-quake

Links:

* http://www.organism.com/void/
* http://www.webcom.com/phantasm/QUSI/



Archive content:

```text
   3934  9 Apr  1997 LICINFO.TXT
  43292  9 Apr  1997 MANUAL.TXT
   3766  9 Apr  1997 ORDER.TXT
   7951  9 Apr  1997 README.TXT
   1461  9 Apr  1997 quake
 844860  9 Apr  1997 quake.gl
 926212  9 Apr  1997 quake.gl.r10k
 846784  9 Apr  1997 quake.sw
 948212  9 Apr  1997 quake.sw.r10k
```

Readme snippet:

```text
Welcome to the SGI port of idsoftware's Quake!
...
- Ed Hutchins
2/11/1997
```

-- sgiquake-1997-04.tar.gz/README.TXT



## SGI Quake v1.08

Perhaps released as `sgiquake-1997-05-02.tar.gz`.

Announced:

```text
May 2, 1997

SGI Quake 1.08
SGI Quake 1.08 has been released on Quake Utils for SGI Irix. Thanks Thomas Winzig.
```

-- https://www.bluesnews.com/archives/april97-4.html

Links:

* http://www.webcom.com/phantasm/QUSI/



Archive content:

```text
    3934 19 Apr  1997 LICINFO.TXT
   43292 19 Apr  1997 MANUAL.TXT
    3766 19 Apr  1997 ORDER.TXT
    9698 30 Apr  1997 README.TXT
    1461 30 Apr  1997 quake
 1167008 30 Apr  1997 quake.gl
 1191392 30 Apr  1997 quake.gl.r10k
  765020 30 Apr  1997 quake.sw
  857856 30 Apr  1997 quake.sw.r10k
```

Readme snippet:

```text
1.08:	* Fixed R10k executables to load libaudio.so dynamically
	* Optimized all executables (all executables now -n32)
	  This may require some software installation on 6.2 machines
	  as n32 libraries are not installed by default on 6.2.
	  The speedup is well worth it though (5-25%)!
	* Stripped binaries for smaller distribution.
...
- Philip Nemec
4/30/1997
```


## SGI Quake v1.09

Perhaps released as `sgiquake-1997-05-13.tar.gz`.


```text
Wednesday, May 14, 1997

SGI Quake 1.09
SGI Quake 1.09 has been released by Philip Nemec. The new version includes support for Wingman Warrior joysticks, among other things. Available on Quake Utils for SGI Irix. Thanks Thomas Winzig.
```

-- https://www.bluesnews.com/archives/may97-2.html

Links:

* http://www.webcom.com/phantasm/QUSI/



Archive content:

```text
    3934 13 Feb  1997 LICINFO.TXT
   43292 13 Feb  1997 MANUAL.TXT
    3766 13 Feb  1997 ORDER.TXT
   10815 14 May  1997 README.TXT
    1461  9 Apr  1997 quake
 1176144 14 May  1997 quake.gl
  598948 14 May  1997 quake.gl.o32
 1204712 14 May  1997 quake.gl.r10k
  822028 14 May  1997 quake.sw
  590756 14 May  1997 quake.sw.o32
 1286808 14 May  1997 quake.sw.r10k
   24748 13 May  1997 test_wingman_warrior
```

Readme snippet:

```text
1.09:	* Added support for Logitech's WingMan Warrior (serial joystick).
	* Included a WingMan Warrior test program.
	* Included o32 versions for 5.3 and machines missing libraries, etc.
...
```


## SGI Quake v1.10

Perhaps released as `sgiquake-1997-05-21.tar.gz`.


```text
SGI Quake 1.10 [May 22, 1997, 12:00 pm ET] – Post a Comment

Thanks Thomas Winzig for word that Philip Nemec has released SGI Quake 1.10, fixing the bug with lookspring, which didn't work. Available from Quake Utils for SGI Irix.
```

-- https://www.bluesnews.com/s/227017/sgi-quake-1-10

Links:

* http://www.webcom.com/phantasm/QUSI/


Archive content:

```text
    3934 15 May  1997 LICINFO.TXT
   43292 15 May  1997 MANUAL.TXT
    3766 15 May  1997 ORDER.TXT
   11004 22 May  1997 README.TXT
    1461 15 May  1997 quake
 1181320 22 May  1997 quake.gl
  598948 22 May  1997 quake.gl.o32
 1205712 22 May  1997 quake.gl.r10k
  773416 22 May  1997 quake.sw
  590756 22 May  1997 quake.sw.o32
 1287684 22 May  1997 quake.sw.r10k
   24748 15 May  1997 test_wingman_warrior
```

Readme snippet:

```text
1.10:   * Fixed lookspring bug (lookspring value was ignored).
        * Packaged correct binaries (WingMan Warrior support).
...
```

Additional Links:

* https://web.archive.org/web/19980511165728/ftp://ftp.stomped.com/pub/redwood/ports/sgiquake1_10_tar.Z


## SGI Quake v1.11

Perhaps released as `sgiquake.tar.gz`.






Archive content:

```text
    3934  9 Apr  1997 LICINFO.TXT
   43292  9 Apr  1997 MANUAL.TXT
    3766  9 Apr  1997 ORDER.TXT
   11367 24 Sep  1997 README.TXT
    1461  9 Apr  1997 quake
 1180676 24 Sep  1997 quake.gl
  598948 24 Sep  1997 quake.gl.o32
 1205124 24 Sep  1997 quake.gl.r10k
  773436 24 Sep  1997 quake.sw
  590756 24 Sep  1997 quake.sw.o32
 1292052 24 Sep  1997 quake.sw.r10k
   24748 22 May  1997 test_wingman_warrior
```

Readme snippet:

```text
1.11:	* Added support for -heapsize parameter - make more add-on levels work.
	* Updated patch information
...
```


## Afterward

Ed Hutchins may have still been involved, e.g. adding the "heapsize parameter" mentioned in the changelog of v1.11:

```text
Edward Hutchins
2 Oct 1997

I sent the changes to ne...@sgi.com that should allow you to
specify -heapsize 16000 and play with the more demanding add-ons.
(8M was fine for the shareware and registered versions).
Check out http://reality.sgi.com/nemec/quake/... version 1.10 is
what you want.

- Ed
```

-- [comp.sys.sgi.misc](https://groups.google.com/g/comp.sys.sgi.misc/c/V87GwtinZzw/m/jjsV_zxixkkJ)


Comments on many optimizations and 3DFX being faster than SGI hardware:

```text
Edward Hutchins
2 Oct 1997

> Author: Ben Cannon <b...@cartsys.com>
> Date: Tue, 30 Sep 1997 18:36:09 -0700

>
> Kristoffer Lawson wrote:
> >
> > Brian A. Higgins (higg...@falcon.jmu.edu) wrote:
> > : > Expect a lot less for a PC machine
> >
> > : Heheh...when I first read this, I thought you meant PC as in "personal
> > : computer running Windows." :)
> >
> > I happen to have a R5000PC machine as that's what I got with the bundle
> > I purchased. How much would a SC processor upgrade cost? Is just switching
> > the processor enough? Atm. Quake runs quite nice in 640x480x32+32 mode
> > except for a lot of swapping but I also heard 3dfx Quake is actually faster..
>
> I've heard that my Cat (Sylvester) is the Pope. Dosen't mean it's true
> :)
Better get a pointy hat for that cat...

> O2 is faster than 3Dfx. (though 3dfx is pretty good, when you can get
> their mess of drivers and crap to work.)

No, at 640x480 3Dfx is faster than an R10K O2. Period. I've benchmarked
them both. Even with dynamic lightmapping enabled the 3Dfx on a fast
Pentia wins. At 800x600 and above, the O2 is infinitely faster than the 3Dfx
because the 3Dfx can't do double-buffered/Z visuals of the right type for
Quake at that rez (unless they've tweaked their drivers since I last
checked). At 1280x1024 an R5k O2 runs neck-and-neck with carmack's $30k
Intergraph workstation, because while the CPU is a bit choked the O2 does
have a pretty good fill rate. If you want to brag, I believe the O2 has
the fastest glDrawPixels rate on the planet (it beats the IR!). Video
apps of all kinds are pretty much top-of-class too (due to UMA and VICE).
Not to mention the fact that my little O2 kick's a Sun ES3000's butt at
IO (at least for a database app that I've run on both systems).

> > Well, I know the SGI port hasn't exactly been very finely optimized (?)
>
> It's been ported to a MIPS chip, that's about it!

Thanks a lot... actually, a lot of the optimizations that I did for
the SGI version wound up back in the main Quake sources (things like
lookup tables for sin/cos). There was more time spent on optimization
than on the actual porting effort. Some tradeoffs were made so that
the Onyx2 IR (which was used for a lot of the profiling) could hit
60Hz at 1280x1024, but basically I don't think there are any easy
pickin's left in the optimization realm. Possibly as the MIPS compiler
gets smarter (which all compilers do over time), there might be some
incremental improvements. Also, eliminating some of the round-trips
to the Xserver for things like glViewport (on the O2) would help quite
a bit.

> > but it's still annoying have some 3dfx ppl brag about their card :-P

They deserve to, for what it was designed for it's a good card. If SGI
management ever gets it's act together and gets the respun R10K interface
out the door, the O2 might be able to beat the 3Dfx. Of course, I'd be
more worried about chips like the NVidia Riva128 and follow-ons at that
point (once they clean up their drivers). That chipset is a full 2D/3D
solution too...

> > I tried running Quake in 16+16bit mode where it's definitely a good bit
> > faster.

Yup, but dithering looks kinda sucky in my opinion. 32+32 is only slightly
slower and looks tons better, but you need at least 128M.

> You need more RAM.
> Quake (all by itself) on an O2 likes over 80MB of RAM.
> (!!!!!!!!!!!!!!)

Textures are tiled on rather large boundaries, and unfortunately
there are still a lot of small textures in Quake (so you end up
with tons of pages pinned down and wasted because of internal
fragmentation). I don't know what happened to the suggestion that
small textures release unused pages so that they can at least
be used for code and data... it would probably allow Quake to
run with all features on on a 64M O2.

Don't get me wrong, I'm posting this from an O2 and I find them
one of the most useful and powerful machines for the price (well
worth 2X the Dell NT system sitting beside me), but it isn't top
dog in every category, and it's beginning to show it's age (the
PC realm is moving much faster than Moor's law for the time being
because they're playing catch-up with the workstation market).

- Ed

P.S. Just thought of something... I've not benchmarked the 1M SC
200MHz R5k O2... that one might be a bit faster.
```

-- [comp.sys.sgi.misc](https://groups.google.com/g/comp.sys.sgi.misc/c/5uDvc-ooKmg/m/nk0Ghb_stloJ)


## References

* https://en.wikipedia.org/wiki/Silicon_Graphics
* https://en.wikipedia.org/wiki/IRIX
* https://web.archive.org/web/20210310142150/https://sgifiles.irixnet.org/sgi/quake/
* https://www.siliconbunny.com/mirrors/ftp.sgi.com/sgi/quake/
* https://www.siliconbunny.com/mirrors/ftp.sgi.com/sgi/quake/doc/quake1.html
* https://www.siliconbunny.com/mirrors/ftp.sgi.com/sgi/quake/download/quake1/
* http://www.sgidepot.co.uk/quake1bench.html
* https://web.archive.org/web/19980220092553/http://reality.sgi.com/employees/hutchins_asd/
* https://web.archive.org/web/19980701023059/http://www.sgi.com/Fun/free/sgi-quake.html
* https://www.betaarchive.com/forum/viewtopic.php?t=22492
* https://web.archive.org/web/19970617005422/http://reality.sgi.com/hutchins_asd/
* https://web.archive.org/web/19970526005454/http://reality.sgi.com/sgiquake/
* https://ftp.zx.net.nz/pub/archive/ftp.sgi.com/sgi/quake/download/quake1/
* https://ftp.jurassic.nl/mirrors/ftp.sgi.com/sgi/quake/download/quake1/
* https://discmaster.textfiles.com/browse/17621/sgi.tar/ftp.sgi.com/sgi/quake/download/quake1
* https://web.archive.org/web/19970315044841/http://reality.sgi.com/rae/quake/
* https://web.archive.org/web/19970315085554/http://reality.sgi.com/rae/quake/pics/sgiquake/

