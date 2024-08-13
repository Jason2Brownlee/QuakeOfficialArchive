# QuakeWorld History

History of QuakeWorld client (QWCL) and server (QWSV) releases.


## Releases

* 1996 Dec 13, qwsv1213.zip
* 1996 Dec 17, qwcl1217.zip
* 1997 Mar 30, qwsv3_29.zip
* 1997 Apr 01, qwinst150.exe
* 1997 Apr 01, qwqc150.zip
* 1997 Apr 03, qwinst150b.exe
* 1997 Apr 03, qwcl1.54-i386-unknown-linux2.0.tar.gz, qwsv1.54-i386-unknown-linux2.0.tar.gz


## QuakeWorld Server (QWSV) v(1213)

Released as `qwsv1213.zip`.


```text
December 13, 1996
QuakeWorld Server Distribution Plan
Disruptor (Christian Antkow), the QuakeWorld main man, and master of the master-server, let me know that the Revco page has a very significant update: The news that the Server software would be distributed in advance of the client software ("soon"). This of course only makes sense, otherwise five minutes after the client is released we'll have 5,000,000 users trying to log into two servers. Shortly after that I got word from the source of the distribution (who'll remain nameless, not that anyone around here likes to hound people), filling me in on the plan, and I am comfortable that this is going to work out with a minimum of bloodshed. Stay tuned for further details...
```

-- https://www.bluesnews.com/archives/dec96-1.html

```text
QuakeWorld Newsflash Part III
There's a new update to the RevCo page pointing out that the first batch of clan skins have been released (also available on on Stomped). Thanks for that to Ozzie.

The RevCo page was updated earlier with Disruptor's QuakeWorld server docs and this note (thanks Greg_Gibson aka angryHelmut):

Expect the server to be uploaded "shortly"

Here are the server documents in text and HTML formats.
```
-- https://www.bluesnews.com/archives/dec96-1.html

```text
QuakeWorld Server Released
Get qwsv1213.zip here or from id's ftp site or Stomped, and the first batch of clan skins right here. Here are the server documents in text and HTML formats. (Thanks to Don Peterson and Benjamin Alexander for spotting the screwed links). To install the skins, create a \quake\qw\skins\ subdirectory and unzip this file into it.
```
-- https://www.bluesnews.com/archives/dec96-1.html

Links:

* https://www.bluesnews.com/files/qwsv1213.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/qwsv1213.zip
* ftp://ftp.stomped.com/pub/quake/quakeworld/qwsv1213.zip
* https://www.bluesnews.com/archives/qwserver.txt
* https://www.bluesnews.com/archives/qwserver.html


Archive content:

```text
drwxrwxr-x  0 0      0           0 13 Dec  1996 PROGS/
-rw-rw-r--  0 0      0      158720 13 Dec  1996 QWSV.EXE
-rw-rw-r--  0 0      0      183444 13 Dec  1996 PROGS.DAT
-rw-rw-r--  0 0      0        9104 13 Dec  1996 QWSV.TXT
-rw-rw-r--  0 0      0       17557  5 Dec  1996 PROGS/PLAYER.QC
-rw-rw-r--  0 0      0        2910  5 Dec  1996 PROGS/BUTTONS.QC
-rw-rw-r--  0 0      0       28425 13 Dec  1996 PROGS/CLIENT.QC
-rw-rw-r--  0 0      0        6284 13 Dec  1996 PROGS/COMBAT.QC
-rw-rw-r--  0 0      0       17648  5 Dec  1996 PROGS/DEFS.QC
-rw-rw-r--  0 0      0       17028 13 Dec  1996 PROGS/DOORS.QC
-rw-rw-r--  0 0      0        6056 13 Dec  1996 PROGS/FILES.DAT
-rw-rw-r--  0 0      0       28634 13 Dec  1996 PROGS/ITEMS.QC
-rw-rw-r--  0 0      0         222  5 Dec  1996 PROGS/JCTEST.QC
-rw-rw-r--  0 0      0       16303  5 Dec  1996 PROGS/MISC.QC
-rw-rw-r--  0 0      0        9788  5 Dec  1996 PROGS/MODELS.QC
-rw-rw-r--  0 0      0        7693  5 Dec  1996 PROGS/PLATS.QC
-rw-rw-r--  0 0      0        1697  5 Dec  1996 PROGS/AMTEST.QC
-rw-rw-r--  0 0      0        2541 13 Dec  1996 PROGS/PROGDEFS.H
-rw-rw-r--  0 0      0         149  5 Dec  1996 PROGS/PROGS.SRC
-rw-rw-r--  0 0      0        2368  5 Dec  1996 PROGS/SERVER.QC
-rw-rw-r--  0 0      0         486  5 Dec  1996 PROGS/SPRITES.QC
-rw-rw-r--  0 0      0        5542 13 Dec  1996 PROGS/SUBS.QC
-rw-rw-r--  0 0      0       14106  5 Dec  1996 PROGS/TRIGGERS.QC
-rw-rw-r--  0 0      0       24696 13 Dec  1996 PROGS/WEAPONS.QC
-rw-rw-r--  0 0      0       11188  5 Dec  1996 PROGS/WORLD.QC
```

Readme snippet:

```text
============================
= QuakeWorld Server (QWSV) =
============================
Released: Friday, December 13th, 1996

...

====================================
= 4. QuakeWorld Master Server 1.03 =
====================================
Last Updated: Thursday, December 12th, 1996

...
```
-- QWSV.TXT


## QuakeWorld Client (QWCL) v1.25

Released as `qwcl1217.zip`.

```text
December 17, 1996

QuakeWorld Client Released
Here's the moment you've been waiting for, the QuakeWorld Client (1.4 MB). Here's the read me, the server (202 KB), the server read me, the new base skin file (17 KB), and the new skins file (1.4 MB). By the way, everyone who couldn't stand waiting a second longer for the client owes a large debt to Christian (and others I'm sure), who toiled all the way through the night on this.

Here is the lowdown from id Software's Michael Abrash on the "Cannot load wdirxxf.dll" message.

	"Unless you want to run -dibonly (which is usually slower, and is a lot slower at low-res such as 320x200), you *must* have all 6 files (wdir62.dll, wdir62f.dll, pmpro62.dll, pmpro62f.dll, wdirnop.com, and wdirnop.pif. You must also have the latest versions, dated 12/9/96."

Michael asks that everyone avoid distributing just qwcl.exe (or at least, if you do, not to send him or John Carmack mail asking why things aren't working).
```
-- [http://bluesnews.com/dec2.html](https://web.archive.org/web/19970204064637fw/http://bluesnews.com/dec2.html)


Links:

* http://bluesnews.com/files/qwcl1217.zip
* http://bluesnews.com/files/qwreadme.txt
* http://bluesnews.com/files/qwsv1213.zip
* http://bluesnews.com/files/qwsv.txt
* http://bluesnews.com/files/skinbase.zip
* http://bluesnews.com/files/qw_skins.zip


Archive content:

```text
-rw-rw-r--  0 0      0      374882 16 Dec  1996 QW.HLP
drwxrwxr-x  0 0      0           0 14 Dec  1996 QW/
-rw-rw-r--  0 0      0      219648 17 Dec  1996 QW.EXE
-rw-rw-r--  0 0      0        8628  5 Dec  1996 QW.GID
-rw-rw-r--  0 0      0      524288 13 Dec  1996 QWCL.EXE
-rw-rw-r--  0 0      0       40724  5 Dec  1996 welcome to quakeworld.wav
-rw-rw-r--  0 0      0        3889  5 Dec  1996 qwfe readme.txt
-rw-rw-r--  0 0      0       47040  5 Dec  1996 abort.wav
-rw-rw-r--  0 0      0          83  7 Jan  1997 master.dat
-rw-rw-r--  0 0      0       35908  5 Dec  1996 gdy2die2.wav
-rw-rw-r--  0 0      0       21566  5 Dec  1996 complete.wav
-rw-rw-r--  0 0      0       24480 13 Dec  1996 qw-win.txt
-rw-rw-r--  0 0      0         995 15 Dec  1996 WDIRNOP.PIF
-rw-rw-r--  0 0      0           5  9 Dec  1996 WDIRNOP.COM
-rw-rw-r--  0 0      0       36864  9 Dec  1996 WDIR62F.DLL
-rw-rw-r--  0 0      0       24216  9 Dec  1996 WDIR62.DLL
-rw-rw-r--  0 0      0       28672  9 Dec  1996 PMPRO62F.DLL
-rw-rw-r--  0 0      0       28672 23 Oct  1996 PMPRO61F.DLL
-rw-rw-r--  0 0      0       18890 23 Oct  1996 PMPRO61.DLL
-rw-rw-r--  0 0      0       18890  9 Dec  1996 PMPRO62.DLL
-rw-rw-r--  0 0      0       13700 16 Dec  1996 qwsv.txt
-rw-rw-r--  0 0      0        2068 17 Dec  1996 readme.txt
-rw-rw-r--  0 0      0        9275 17 Dec  1996 qwcl.txt
-rw-rw-r--  0 0      0      769024 17 Sep  1996 mfcinst.exe
```

Readme snippets:



```text
==================================
= QuakeWorld Client (QWCL) v1.25 =
==================================
Released: Tuesday, December 17th, 1996
```
-- qwcl.txt


## QuakeWorld Server (QWSV) v(0329) v1.51

Released as `qwsv3_29.zip`.

```text
March 30, 1997
New QuakeWorld Server
The new version of the Quake World server, has been released on id's FTP site. A different version, with the same filename was uploaded shortly after the original, so if you downloaded it early on, you should get it again. Once again, in advance of the client to allow servers to be online when the client is released. Also now available is QPlug, the browser plug-in that accompanied the new QW. Unfortunately, the new master is not compatible with the current masters/clients, so this should be kept in mind when switching over. More information can be found on QuakeWorld Central "The Official Home of QuakeWorld" which is now open for business.
```
-- https://www.bluesnews.com/archives/march97-5.html

```text
March 30, 1997
QuakeWorld Central Update II
The reference to a new QuakeWorld server on QuakeWorld Central is the second version that was uploaded last night. To make sure you have the right one, simply verify that you have version 1.51. From earlier, thanks kolinahr for pointing out there was an update answering the many frequently asked questions about the new QuakeWorld.
```
-- https://www.bluesnews.com/archives/march97-5.html

Links:

* https://www.bluesnews.com/files/qwsv3_29.zip
* ftp://ftp.idsoftware.com/idstuff/quakeworld/qwsv3_29.zip
* https://www.bluesnews.com/files/qp3_29.zip


Archive content:

```text
-rw-rw-r--  0 0      0      184320 30 Mar  1997 QWSV.EXE
-rw-rw-r--  0 0      0      187452 29 Mar  1997 PROGS.DAT
-rw-rw-r--  0 0      0         265 30 Mar  1997 QWSV.TXT
```

Readme:

```text
QWSV Notes (March.29.1997 Release)
----------------------------------

 Please refer to

 http://qwcentral.stomped.com

 for documentation.

 Server operators wishing to link to our master server at id, please use;

 qwsv +setmaster 192.246.40.12.
 ```

## QuakeWorld Client (QWCL) v1.50

Released as `qwinst150.exe`.


```text
April 1, 1997
New QuakeWorld Client/QSpy Release
Hot off the presses is the new QuakeWorld Client and QuakeSpy (1.6 MB) all rolled into one. The new QuakeWorld is version 1.50, and is only compatible with the new servers (currently version 1.51). The new program is an installer that will install everything for you. Hint of the day: if the installation suggests rebooting, believe it. In honor of the event, Disruptor's .plan and the RevCo page have been updated. My old buddy Moogle wrote in to point out the most recent addition to Dis' .plan to save a little wear and tear in Dis' mailbox:

	- U_REMOVE on full update: We know about this. It shouldn't be a serious
	error. We'll try to fix it.
```
-- https://www.bluesnews.com/archives/march97-5.html

Links:

* https://www.bluesnews.com/files/qwinst150.exe


**Cannot unzip on a POSIX box, yet.**


## QuakeWorld QuakeC v1.50

Released as `qwqc150.zip` and qwqc150.txt.

```text
April 2, 1997
QuakeWorld QC
Disruptor released the new QuakeWorld Quake C files yesterday.
```
-- https://www.bluesnews.com/archives/march97-5.html

Links:

* https://www.bluesnews.com/files/qwqc150.zip


Archive content:

```text
-rw-rw-r--  0 0      0        1697  5 Dec  1996 amtest.qc
-rw-rw-r--  0 0      0        2910  5 Dec  1996 buttons.qc
-rw-rw-r--  0 0      0       30162 27 Mar  1997 client.qc
-rw-rw-r--  0 0      0        7578 29 Mar  1997 combat.qc
-rw-rw-r--  0 0      0       24717 27 Mar  1997 defs.qc
-rw-rw-r--  0 0      0       17076 26 Feb  1997 doors.qc
-rw-rw-r--  0 0      0       31876 29 Mar  1997 items.qc
-rw-rw-r--  0 0      0         222  5 Dec  1996 jctest.qc
-rw-rw-r--  0 0      0       16413 19 Feb  1997 misc.qc
-rw-rw-r--  0 0      0        9788  5 Dec  1996 models.qc
-rw-rw-r--  0 0      0        7741 26 Feb  1997 plats.qc
-rw-rw-r--  0 0      0       20596 28 Mar  1997 player.qc
-rw-rw-r--  0 0      0        2368  5 Dec  1996 server.qc
-rw-rw-r--  0 0      0         486  5 Dec  1996 sprites.qc
-rw-rw-r--  0 0      0        5542 13 Dec  1996 subs.qc
-rw-rw-r--  0 0      0       14140 19 Feb  1997 triggers.qc
-rw-rw-r--  0 0      0       27741 27 Mar  1997 weapons.qc
-rw-rw-r--  0 0      0       11188  5 Dec  1996 world.qc
-rw-rw-r--  0 0      0         149  5 Dec  1996 progs.src
```

Readme:

```text
The latest id source code to QuakeWorld progs.dat.
```
-- qwqc150.txt


## QuakeWorld Client (QWCL) v1.50 v2

Released as `qwinst150b.exe`.

```text
April 3, 1997
QW Installer
Here is the new installer (1.1 MB) for the QuakeWorld client that has the lean, DLL-less install of QSpy 5.1b. morbid says that if you haven't already gotten the new smaller QSpy, you really ought to do so, among other things it apparently operates faster.
```
-- https://www.bluesnews.com/archives/march97-5.html

Links:

* https://www.bluesnews.com/files/qwinst150b.exe

**Cannot unzip on a POSIX box, yet.**


## Linux QuakeWorld Client (QWCL) and Server (QWSV) v1.54

Released as:

* `qwcl1.54-i386-unknown-linux2.0.tar.gz`
* `qwsv1.54-i386-unknown-linux2.0.tar.gz`


```text
April 3, 1997
Linux QuakeWorld
Well that was Quick... I mentioned that Zoid said soon for the Linux QuakeWorld files, but I didn't realize that meant hours. While I was at the QuakeCast, Zoid released the Linux Server, and the Linux Client (shift-click on the links), thanks moogle.
```
-- https://www.bluesnews.com/archives/march97-5.html

Links:

* https://www.bluesnews.com/files/qwsv1_54-i386-unknown-linux2_0_tar.gz
* https://www.bluesnews.com/files/qwcl1_54-i386-unknown-linux2_0_tar.gz


The `qwcl1_54-i386-unknown-linux2_0_tar.gz` content:

```text
-rwsr-xr-x  0 root   root   271952  4 Apr  1997 qwcl
-rw-------  0 zoid   users    4131  4 Apr  1997 qwcl.txt
```

The `qwsv1.54-i386-unknown-linux2.0.tar.gz` content:

```text
drwx------  0 zoid   users       0  4 Apr  1997 qw/
-rw-------  0 zoid   users  187452  4 Apr  1997 qw/qwprogs.dat
drwx------  0 zoid   users       0  4 Apr  1997 qw/skins/
-rwx------  0 zoid   users     109  4 Apr  1997 qw/skins/fixskins.sh
-rwx------  0 zoid   users  141828  4 Apr  1997 qwsv
-rw-------  0 zoid   users     631  4 Apr  1997 qwsv.txt
```

Readme:

```text
Linux QWSV Notes (April.03.1997 Release)
----------------------------------------

 Please refer to

 http://qwcentral.stomped.com

 for documentation.

 Server operators wishing to link to our master server at id, please use;

 qwsv +setmaster 192.246.40.12.

Skins Note
----------

After you get the skin files from ftp.idsoftware.com (currently,
qw_skins.zip, qws_9652.zip and qws_9706.zip) and install them in
qw/skins, you should run the shell script 'fixskins.sh' that you can find in
the qw/skins directly distributed with this archive.

Linux qwsv will always look for lowercase file names first.
```
-- qwsv.txt





