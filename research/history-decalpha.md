# DEC Alpha Linux Quake History

Alpha or Alpha AXP is a platform by Digital Equipment Corporation (DEC), typically referred to as simply "[DEC Alpha](https://en.wikipedia.org/wiki/DEC_Alpha)". It ran various flavors of UNIX and Linux.

The Quake client was ported to this platform for Alpha Linux and was referred to as "DEC Alpha Quake".

Releases:

* 1996 Aug 12, alpha-ELF-xquake.gz
* xquake-1.06-alpha-bin.gz
* i386-ELF-xquake-1.06.gz
* alpha-ELF-xquake-1.06.gz




## alpha-ELF-xquake.gz

Developed and released by Dave Taylor.

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


Archive contents:

```text
defla d7416de7 Aug 12 05:25       244942       645048  62.0% ./alpha-ELF-xquake
```



## References

* https://en.wikipedia.org/wiki/DEC_Alpha
* https://www.ibiblio.org/pub/historic-linux/ftp-archives/tsx-11.mit.edu/Oct-07-1996/sources/system/testing/
* https://cdn.kernel.org/pub/linux/kernel/testing/old/quake/
* http://31.131.0.222/?dir=kernel/testing/old/quake
* http://ftpkernel.metu.edu.tr/linux/kernel/testing/old/quake/