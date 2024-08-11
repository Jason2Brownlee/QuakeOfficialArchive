# DEC Alpha Linux Quake History

Alpha or Alpha AXP is a platform by Digital Equipment Corporation (DEC), typically referred to as simply "[DEC Alpha](https://en.wikipedia.org/wiki/DEC_Alpha)". It ran various flavors of UNIX and Linux.

The Quake client was ported to this platform for Alpha Linux and was referred to as "DEC Alpha Quake".

Releases:

* 1996 Aug 12, DEC Alpha Linux Quake (Dave Taylor)
* 1996 Oct 04, alpha-ELF-xquake.gz
* 1996 Nov 13, alpha-ELF-xquake-1.06.gz
* 1996 Nov 22, i386-ELF-xquake-1.06.gz
* 1997 Sep 22, xquake-1.06-alpha-bin.gz

## DEC Alpha Linux Quake (Dave Taylor)

Developed by Dave Taylor.

Perhaps not released publicly by Dave?

Announcement and discussion:

```text
Date: Mon, 12 Aug 1996 19:13:05 -0500 (CDT)
From: Dave Taylor <ddt at crack.crack.com>
To: linux-alpha at vger.rutgers.edu, axp-list at redhat.com
Subject: Alpha Linux Quake


Quake 1.01 (a nifty game) for Alpha/Linux is available on
ddt.is.not.lame.org:/linux.  The xf86quake version is slower and crashes
some Alpha's.  Don't really recommend it.  Kind of a stillborn idea
after I thought about it.  Can't do byte-access to the framebuffer
without reading each pixel you write.  Sigh.

Linus, sorry I couldn't port Doom to the Alpha.  Plz accept this instead.
I think you will dig.

	=-ddt->

- ------- Forwarded Message

On 13 Aug 1996, Martin Ostermann wrote:
>
> Linus Torvalds <torvalds at cs.Helsinki.FI> writes:
>
> > Does anybody have the quake files unpacked somewhere? I really simply
> > don't _have_ any DOS box to unpack things on, and I don't even have
> > dosemu or anything like that installed anywhere.. I'd love ot try quake
> > out on my home alpha.
> >
> > 		"Desperate"
>
> You don't need them -- the README of the alpha-quake package
> describes how to catenate the data-files together to an 'quakedate.exe'
> file, that can be extracted by lha, which is available for Unix. Even
> comes with RedHat, as far as I remember.

Duh. I _did_ that, and it didn't work. It turns out that the filename
actually makes a difference: it _has_ to end with ".exe" or lha won't
work.

Oh, well. After renaming the file lha worked perfectly and I can shoot
monsters to my hearts delight. Perfectly playable even at largish screen
sizes (700+ x 500+). Certianly a lot better than doom, which I had to
play with the picture coming over the network from a x86 machine..

> I just did that, I am know waiting for alpha-quake to arrive -- about
> 80% done during the last 3 hour's !

Indeed, know what you mean..

		"Sated"
```
-- https://blu.org/pipermail/discuss/1996-August/001053.html



## alpha-ELF-xquake.gz (Linus Torvalds)

Released as `alpha-ELF-xquake.gz`, likely by Linus Torvalds as a bug fix for Dave Taylor's August version or perhaps the August version as-is.

We know little.

Announcement and discussion:


```text
...
bme...@bruce.cs.monash.edu.au
13 Oct 1996

They gave Linus himself a source code license. And he has released a bugfixed
version of Quake for linux/ALPHA. Bummer the man himself has an ALPHA,
isn't it?
...


bme...@bruce.cs.monash.edu.au

15 Oct 1996

It's in

ftp://ftp.azstarnet.com/pub/linux/axp/misc/alpha-ELF-xquake.gz

(among other places). However, this is _not_ for linux/Intel, but for
linux/ALPHA, running on DEC ALPHA RISC processors. If you have one of them,
fine (although you should be on the mailing list if you did), if not,
it is of no use to you whatsoever (and bandwidth is limited enough
already, so don't download it ;-)
```
-- [rec.games.computer.quake.misc](https://groups.google.com/g/rec.games.computer.quake.misc/c/cKGT0uqJP5Y/m/4C8Z5ciyisgJ)


Locations:




## alpha-ELF-xquake-1.06.gz (Linus Torvalds)

Released as `alpha-ELF-xquake-1.06.gz`.

Announcement and discussion:


```text
Bergen Friundervisningen
16 Nov 1996

I believe there is an ALPHA version at ftp.cs.helsinki.fi
in the directory /pub/Software/Linux/Kernel/testing/alpha-ELF-xquake-1.06.gz

Kjartan Maraas

...

Ravi K. Swamy
18 Nov 1996

Linus really does have the source to Quake and has fixed a few bugs
with the Alpha port. Read the alpha mailing list and you'll see posts
from him mentioning it from time to time.

Ravi
```
-- [rec.games.computer.quake.misc](https://groups.google.com/g/rec.games.computer.quake.misc/c/xVvxzFgADW0/m/UvlJd-td0FIJ)

* ftp://ftp.stomped.com/pub/redwood/ports/alpha-ELF-xquake-1_06.gz
* http://redwood.gatsbyhouse.com/files/ports/alpha-ELF-xquake-1_06.gz
* http://www.planetquake.com/threewave/htdocs/linux/files/alpha-ELF-xquake-1.06.gz


## i386-ELF-xquake-1.06.gz (Linus Torvalds)

Released as `i386-ELF-xquake-1.06.gz` and perhaps repackaged as `i386-ELF-xquake-1.06.tar.gz`.

Announcement and discussion:

```text
==November 1== 11:15p.m. CST
John Cash updated his .plan today (thanks to RIDE-MY-ROCKET) with this :

	11/1:
	*Sent off source to get the 1.06 Linux version done.
	Tim just got a Mortal Kombat II machine.  Productivity may suffer.
```
-- [http://redwood.gatsbyhouse.com/quake/1196.html](https://web.archive.org/web/19970327200928/http://redwood.gatsbyhouse.com/quake/1196.html) (archived)

```text
==November 25== 11:30p.m. CST

Thanks to Russ Ringer for pointing out Linux Quake 1.06 is available. I got it from that guy's ftp site that created Linux (I think...ftp://ftp.cs.Helsinki.FI/pub/People/Torvalds_Linus/) in a testing directory on a Finnish ftp site so I can't guarantee it's finished but Russ said it got rid of some errors he was having in 1.01 Linux Quake. Anyway, here is i386-ELF-xquake-1_06.gz. Also while I was there I noticed alpha-ELF-xquake-1_06.gz which I'm guessing is for DEC Alpha processors.
```
-- [http://redwood.gatsbyhouse.com/quake/1196.html](https://web.archive.org/web/19970327200928/http://redwood.gatsbyhouse.com/quake/1196.html) (archived)

Links:

* ftp://ftp.cs.helsinki.fi/pub/People/Torvalds_Linus/
* http://redwood.gatsbyhouse.com/quake/files/i386-ELF-xquake-1_06.gz
* http://redwood.gatsbyhouse.com/quake/files/alpha-ELF-xquake-1_06.gz


```text
1.06 Linux X
This is the version of quake as produced by 'id' games and compiled by Linus Torvalds of Linux fame now working on his Thesis. This is only an executable - X-Windows libs are required to run it as a server.
```
-- [http://www.cms.dmu.ac.uk/~rl/Quake/](https://web.archive.org/web/19980114151448/http://www.cms.dmu.ac.uk/~rl/Quake/) (archived)

Links:

* http://www.cms.dmu.ac.uk/~rl/Quake/i386-ELF-xquake-1.06.tar.gz


```text
Phil Ross
23 Nov 1996

Well, when I was looking for kernel 2.0.26, I found these in the
testing directory:
Current directory is /pub/People/Torvalds_Linus/testing

Up to higher level directory
alpha-ELF-xquake-1.06.gz 242 Kb Wed Nov 13 14:52:00 1996
alpha-ELF-xquake.gz 239 Kb Fri Oct 4 12:01:00 1996
axp-bash.gz 380 Kb Fri Mar 10 00:00:00 1995
axp-net.tar.gz 277 Kb Mon Jul 10 00:00:00 1995
axp-patch-e2fsprog.gz 17 Kb Sun Mar 12 00:00:00 1995
axp-uemacs.gz 116 Kb Thu Mar 23 00:00:00 1995
e2fsprogs-0.5a.tar.gz 222 Kb Sun Mar 12 00:00:00 1995
i386-ELF-xquake-1.06.gz 145 Kb Fri Nov 22 15:43:00 1996


Is the i386-ELF-xquake-1.0.6.gz not really 1.06???

I downloaded it and it worked and when I start it it says 1.06.

*shrug*


-Phil
```
-- [comp.os.linux.misc](https://groups.google.com/g/comp.os.linux.misc/c/0ItwknxKHn8/m/5zm_21fbY-cJ)


```text
...
FR-- 248083 1996/11/13 00:00 testing/alpha-ELF-xquake-1.06.gz
FR-- 244942 1996/10/03 00:00 testing/alpha-ELF-xquake.gz
...
FR-- 148856 1996/11/22 00:00 testing/i386-ELF-xquake-1.06.gz
...
FR-- 248659 1997/09/22 00:00 testing/xquake-1.06-alpha-bin.gz
...
```
- [muc.archive.update](https://groups.google.com/g/muc.archive.update/c/_mq5lH5H8oc/m/kz2hPjNF_lsJ)

Locations:

* ftp://ftp.stomped.com/pub/redwood/ports/i386-ELF-xquake-1_06.gz
* http://ftp.sun.ac.za/sites/sunsite.unc.edu/pub/Linux/games/quake/i386-ELF-xquake-1.06.gz
* http://redwood.gatsbyhouse.com/files/ports/i386-ELF-xquake-1_06.gz
* http://sunsite.unc.edu/pub/Linux/Incoming/i386-ELF-xquake-1.06.gz
* http://www.planetquake.com/threewave/htdocs/linux/files/i386-ELF-xquake-1.06.gz
* https://www.quaddicted.com/files/engines/i386-ELF-xquake-1.06.gz




## xquake-1.06-alpha-bin.gz (Linus Torvalds)

Released as `xquake-1.06-alpha-bin.gz` by Linus Torvalds.


```text
xquake binary update
Linus Torvalds
22 Sept 1997

I was asked to show xquake on my alpha yesterday, and noticed that my
xquake binary no longer worked on my machine. It core-dumped when
trying to start a new game. Panic. Embarrassment.

I don't know if anybody else has seen this problem, or if anybody cares,
but I decided I might as well make a new test binary available in case
others see the same thing with the old binary.

The problem was due to the newer 'malloc()' implementation that no
longer allocated contiguous memory (it uses anonymous mmap() for large
memory allocations). Quake uses some 32-bit offsets internally, and the
offsets between different allocations no longer fit into 32 bits with
the new malloc.

The new binary is available on

ftp://ftp.kernel.org/pub/linux/kernel/testing/xquake-1.06-alpha-bin.gz

but if the old binaries work for you the new one shouldn't have any new
features, so this is relevant only if you have had problems with quake
on the alpha.

Linus
```
-- [comp.os.linux.alpha](https://groups.google.com/g/comp.os.linux.alpha/c/LoNOegYW5vY/m/rPktwwmMxcEJ)


Locations:

* https://cdn.kernel.org/pub/linux/kernel/testing/old/quake/xquake-1.06-alpha-bin.gz
* https://mirror.ihost.md/kernel/testing/old/quake/xquake-1.06-alpha-bin.gz
* https://kebo.pens.ac.id/linux/testing/old/quake/xquake-1.06-alpha-bin.gz




## References

* https://en.wikipedia.org/wiki/DEC_Alpha
* https://www.ibiblio.org/pub/historic-linux/ftp-archives/tsx-11.mit.edu/Oct-07-1996/sources/system/testing/
* https://cdn.kernel.org/pub/linux/kernel/testing/old/quake/
* http://31.131.0.222/?dir=kernel/testing/old/quake
* http://ftpkernel.metu.edu.tr/linux/kernel/testing/old/quake/
* https://web.archive.org/web/19970617190706/http://www.planetquake.com/threewave/htdocs/linux/
* https://web.archive.org/web/19980114151448/http://www.cms.dmu.ac.uk/~rl/Quake/
